---
title: Wiederherstellen von Administratorrechten für Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Kunden dabei helfen können, die Administratorrechte eines Partners wiederherzustellen, damit der Partner die Azure CSP-Abonnements eines Kunden verwalten kann.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855419"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden  

**Geeignete Rollen**: Globaler Administrator | Administrator-Agent

Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und ihre Systeme für sie verwalten. Hierfür müssen Sie über Administratorrechte verfügen. Einige Rechte werden Ihnen beim Einrichten der Vertriebspartnerschaft mit dem Kunden gewährt. Andere werden Ihnen vom Kunden erteilt.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratorrechte für Azure in CSP

Es gibt zwei Ebenen von Administratorrechten für Azure in CSP.

**Administratorrechte auf Mandantenebene** (**Delegierte Administratorrechte**) – CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden. Durch delegierte Administratorrechte erhalten CSP-Partner Zugriff auf die Mandanten der Kunden, um administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Kennwörtern und das Verwalten von Benutzerlizenzen durchführen zu können.

**Administratorrechte auf Abonnementebene** – CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden. Mit diesen Rechten haben CSP-Partner vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können.

## <a name="reinstate-csp-partners-admin-privileges"></a>Reaktivieren von Administratorrechten für CSP-Partner

Ihr Kunde kann die CSP-Rollenzuweisung neu erstellen, sofern Sie ihm die Objekt-ID der Administrator-Agents-Gruppe bereitstellen. Um die delegierten Administratorrechte zu reaktivieren, müssen Sie mit Ihrem Kunden zusammenarbeiten.

1. Melden Sie sich beim Partner Center-Dashboard an, und wählen Sie im Partner Center-Menü **Kunden** aus.

2. Wählen Sie den Kunden aus, mit dem Sie arbeiten, und **beantragen Sie eine Vertriebspartnerschaft**. Durch diese Aktion wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.

3. Dieser Kunde muss den Link auswählen und den Antrag auf Vertriebspartnerschaft genehmigen.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-Mail-Beispiel für das Erstellen einer Vertriebspartnerschaft":::

4. Sie als Partner müssen eine Verbindung mit dem Partnermandanten herstellen, um die Objekt-ID der Administrator-Agents-Gruppe zu erhalten.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Ihr Kunde, der die Rolle **Besitzer oder Benutzerzugriffsadministrator** hat und über die Berechtigung zum Erstellen einer Rollenzuweisung auf Abonnementebene verfügt, führt folgende Schritte aus:


    1. Er stellt eine Verbindung mit dem Mandanten mit dem CSP-Abonnement her.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Er stellt eine Verbindung mit dem Abonnement her (trifft nur zu, wenn der Benutzer über Rollenzuweisungsberechtigungen für mehrere Abonnements im Mandanten verfügt).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"`


    3. Er erstellt die Rollenzuweisung.
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Wenn Sie die Besitzerrollenberechtigung auf Ressourcengruppen- oder Ressourcenebene statt auf Abonnementebene erteilen möchten, können Sie die folgenden Befehle verwenden:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)
