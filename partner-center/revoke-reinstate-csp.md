---
title: Reaktivieren von Administratorrechten für Azure CSP-Abonnements | Partner Center
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: In diesem Dokument wird erläutert, wie Kunden beim Reaktivieren von Administratorrechten des Partners geholfen werden kann.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 1bcbcf32e3b3f4513ed3e55984b49b090da4a734
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2020
ms.locfileid: "73651704"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>Reaktivieren von Administratorrechten für Azure CSP-Abonnements  

**Zutreffende Rollen**

- Globaler Administrator
- Administrator-Agent

Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und ihre Systeme für sie verwalten. Hierfür ist es erforderlich, dass Sie über Administratorrechte verfügen. Einige Rechte werden Ihnen beim Herstellen der Vertriebspartnerschaft mit dem Kunden gewährt. Andere werden Ihnen vom Kunden erteilt.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratorrechte für Azure in CSP 

Es gibt zwei Ebenen von Administratorrechten für Azure in CSP. 

**Administratorrechte auf Mandantenebene** (**Delegierte Administratorrechte**) – CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden. Dadurch erhalten CSP-Partner Zugriff auf die Mandanten der Kunden, um administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Kennwörtern und das Verwalten von Benutzerlizenzen durchführen zu können. 

**Administratorrechte auf Abonnementebene** – CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden. Dadurch erhalten CSP-Partner den vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können. 


## <a name="reinstate-csp-partners-admin-privileges"></a>Reaktivieren von Administratorrechten für CSP-Partner

Um die delegierten Administratorrechte zu reaktivieren, müssen Sie mit Ihrem Kunden zusammenarbeiten.
 
 1. Melden Sie sich beim Partner Center-Dashboard an, und wählen Sie im Partner Center-Menü **Kunden** aus.

 2. Wählen Sie den Kunden aus, mit dem Sie arbeiten, und **beantragen Sie eine Vertriebspartnerschaft**. Dadurch wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.

 3. Der Benutzer muss den Link auswählen und die Anforderung der Vertriebspartnerschaft genehmigen.
 
![Vertriebspartnerschaft](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Hinzufügen der Gruppe der Administrator-Agents als Besitzer für das Azure CSP-Abonnement

 Ihr Kunde muss Ihre Administrator-Agent-Gruppe als Besitzer des Azure CSP-Abonnements hinzufügen.

1. Verwenden Sie entweder die PowerShell-Konsole oder PowerShell Integrated Scripting Environment (ISE). Stellen Sie sicher, dass die Module AzureRM und AzureAD installiert sind. 

2.  Stellen Sie eine Verbindung mit Ihrem Azure AD-Mandanten her.
PowerShell-Cmdlet: Connect-AzureAD

3.  Abrufen der ObjectId der Gruppe der Administrator-Agents.
PowerShell-Cmdlet: Get-AzureADGroup`1nn

![Administrator-Agent-Gruppe](images/azure/revoke5.png)

Die folgenden Schritte werden vom Benutzer im Unternehmen Ihres Kunden ausgeführt, der über Besitzerzugriff auf das Azure CSP-Abonnement verfügt.

4. Der Benutzer, der über Besitzerzugriff auf das Azure CSP-Abonnement verfügt, meldet sich mit seinen Anmeldeinformationen bei Azure Resource Manager an.

    PowerShell-Cmdlet: Login-AzureRMAccount

5.  Anschließend kann er Ihre Administrator-Agent-Gruppe als Besitzer zum CSP-Azure-Abonnement hinzufügen.

    PowerShell-Cmdlet: New-AzureRMRoleAssignment -ObjectId < In Schritt 3 abgerufene Object-ID> -RoleDefinitionName Owner -Scope „/Abonnements/<SubscriptionId of CSP subscription>“

![Administrator-Agent-Besitzer](images/azure/revoke6.png)    

**Weitere Informationen**

[Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)
