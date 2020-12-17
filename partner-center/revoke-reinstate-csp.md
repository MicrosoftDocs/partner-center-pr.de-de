---
title: Wiederherstellen von Administratorrechten für Azure CSP
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Kunden dabei helfen können, die Administratorrechte eines Partners wiederherzustellen, damit der Partner die Azure CSP-Abonnements eines Kunden verwalten kann.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011501"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden  

**Zutreffende Rollen**

- Globaler Administrator
- Administrator-Agent

Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und ihre Systeme für sie verwalten. Hierfür müssen Sie über Administratorrechte verfügen. Einige Rechte werden Ihnen beim Herstellen der Vertriebspartnerschaft mit dem Kunden gewährt. Andere werden Ihnen vom Kunden erteilt.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratorrechte für Azure in CSP

Es gibt zwei Ebenen von Administratorrechten für Azure in CSP.

**Administratorrechte auf Mandantenebene** (**Delegierte Administratorrechte**) – CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden. Dadurch erhalten CSP-Partner Zugriff auf die Mandanten der Kunden, um administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Kennwörtern und das Verwalten von Benutzerlizenzen durchführen zu können.

**Administratorrechte auf Abonnementebene** – CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden. Mit diesen Rechten haben CSP-Partner vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können.

## <a name="reinstate-csp-partners-admin-privileges"></a>Reaktivieren von Administratorrechten für CSP-Partner

Um die delegierten Administratorrechte zu reaktivieren, müssen Sie mit Ihrem Kunden zusammenarbeiten.

1. Melden Sie sich beim Partner Center-Dashboard an, und wählen Sie im Partner Center-Menü **Kunden** aus.

2. Wählen Sie den Kunden aus, mit dem Sie arbeiten, und **beantragen Sie eine Vertriebspartnerschaft**. Dadurch wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.

3. Der Benutzer muss den Link auswählen und die Anforderung der Vertriebspartnerschaft genehmigen.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Vertriebspartnerschaft":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Hinzufügen der Gruppe der Administrator-Agents als Besitzer für das Azure CSP-Abonnement

Ihr Kunde muss Ihre Administrator-Agent-Gruppe als Besitzer eines Azure CSP-Abonnements, einer Ressourcengruppe oder eine Ressource hinzufügen. 

1. Verwenden Sie entweder die PowerShell-Konsole oder PowerShell Integrated Scripting Environment (ISE). Stellen Sie sicher, dass die AzureAD-Module installiert sind.

2. Stellen Sie eine Verbindung mit Ihrem Azure AD-Mandanten her.

   ```powershell
   Connect-AzureAD
   ```

3. Abrufen der ObjectId der Gruppe der Administrator-Agents.

   ```powershell
   Get-AzureADGroup
   ```
   Die folgenden Schritte werden vom Benutzer im Unternehmen Ihres Kunden ausgeführt, der über Besitzerzugriff auf das Azure CSP-Abonnement verfügt.

4. Der Benutzer, der über Besitzerzugriff für das Azure CSP-Abonnement verfügt, meldet sich mit seinen Anmeldeinformationen bei Azure an.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Dann kann er einen geeigneten Ressourcen-URI im Bereichsparameter anwenden, um Ihre Administrator-Agent-Gruppe als Besitzer dem CSP-Azure-Abonnement, der Ressourcengruppe oder der Ressource hinzuzufügen. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Nächste Schritte

[Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)
