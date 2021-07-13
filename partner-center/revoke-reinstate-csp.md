---
title: Wiederherstellen von Administratorrechten für Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Kunden dabei helfen können, die Administratorrechte eines Partners wiederherzustellen, damit der Partner dabei helfen kann die Azure CSP-Abonnements eines Kunden zu verwalten.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510175"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden  

**Geeignete Rollen**: Globaler Administrator | Administrator-Agent

Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und Systeme für sie verwalten. Dazu benötigen Sie Administratorrechte. Einige Rechte werden Ihnen beim Einrichten der Vertriebspartnerschaft mit dem Kunden gewährt. Andere werden Ihnen vom Kunden erteilt.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratorrechte für Azure in CSP

Es gibt zwei Ebenen von Administratorrechten für Azure in CSP.

- **Administratorrechte auf Mandantenebene (Delegierte Administratorrechte)** : CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden. Delegierte Administratorrechte ermöglichen CSP-Partnern Zugriff auf die Mandanten ihrer Kunden. Mit diesem Zugriff können sie administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Passwörtern und die Verwaltung von Benutzerlizenzen durchführen.
- **Administratorrechte auf Abonnementebene**: CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden. Mit diesen Rechten haben CSP-Partner vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Wiederherstellen der Administratorenrechte von CSP-Partnern

Ihr Kunde kann die CSP-Rollenzuweisung neu erstellen, sofern Sie ihm die `object ID` der Administrator-Agenten-Gruppe bereitstellen. Um die delegierten Administratorrechte wiederzuerlangen, müssen Sie mit Ihrem Kunden die folgenden Schritte durchführen.

1. Melde dich beim Partner Center-Dashboard an.

2. Wählen Sie im Menü „Partner Center” **Kunden** aus.

3. Wählen Sie den Kunden aus, mit dem Sie arbeiten und wählen Sie **Anforderung einer Vertriebspartnerschaft**. Durch diese Aktion wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.

4. Ihr Kunde muss den Link auswählen und die Anforderung auf eine Vertriebspartnerschaft genehmigen.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-Mail-Beispiel für das Erstellen einer Vertriebspartnerschaft.":::

5. Sie als Partner müssen eine Verbindung mit dem Partnermandanten herstellen, um die Objekt-ID der Administrator-Agents-Gruppe zu erhalten.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Ihr Kunde muss dann die folgenden Schritte entweder mithilfe von PowerShell oder mit Azure CLI durchführen. Ihr Kunde muss über Folgendes verfügen:

- Rolle des **Besitzers** oder die des **Benutzerzugriffsadministrators** 
- Berechtigungen zum Erstellen von Rollenzuweisungen auf Abonnementebene

   a. Der Kunde muss nur für PowerShell das Modul `Az.Resources` aktualisieren.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Der Kunde stellt eine Verbindung mit dem Mandanten her, in dem das CSP-Abonnement besteht.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Der Kunde stellt eine Verbindung mit dem Abonnement her. Das ist *nur* anwendbar, wenn der Benutzer über Rollenzuweisungsberechtigungen für mehrere Abonnements im Mandanten verfügt.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Der Kunde erstellt dann die Rollenzuweisung.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Anstatt Besitzerberechtigungen im Abonnementbereich zu erteilen, können Sie auf Ressourcengruppen oder Ressourcenebene erteilen. 

- Auf Ressourcengruppenebene

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Auf Ressourcenebene

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Wenn die oben genannten Schritte nicht funktionieren oder beim Versuch Fehler auftreten, versuchen Sie, die folgenden „Auffangverfahren“ zu verwenden, um Administratorrechte für Ihren Kunden wiederherzustellen.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Problembehandlung

Wenn der Kunde Schritt 6 oben nicht ausführen kann, lassen Sie es den Kunden mit dem folgenden Befehl versuchen:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Stellen Sie die resultierende `newRoleAssignment.log` Datei für Microsoft zur weiteren Analyse zur Verfügung.

Wenn das „Auffangverfahren“ während `Import-Module` fehlschlägt, führen Sie die folgenden Schritte aus:
- Wenn beim Import ein Fehler auftritt, weil das Modul verwendet wird, starten Sie die PowerShell-Sitzung neu, indem Sie alle Fenster schließen und erneut öffnen.
- Überprüfen Sie die Version von `Az.Resources` mit `Get-Module Az.Resources -ListAvailable`.
- Wenn die Version 4.1.1 nicht in der Liste der verfügbaren Versionen enthalten ist, müssen Sie `Update-Module Az.Resources -Force` verwenden.
- Wenn der Fehler besagt, dass `Az.Accounts` eine bestimmte Version benötigt, aktualisieren Sie auch dieses Modul, und ersetzen Sie `Az.Resources` durch `Az.Accounts`. Anschließend müssen Sie die PowerShell-Sitzung neu starten.


## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)
