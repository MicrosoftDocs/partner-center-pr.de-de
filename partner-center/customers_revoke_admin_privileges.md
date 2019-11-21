---
title: Kunden delegieren Administratorrechte an Partner | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to ask customers to delegate administrator permissions to a reseller or remove the same permissions and how to use the permissions.
author: LauraBrenner
ms.author: labrenne
keywords: delegierte Administratorrechte, Administrator im Auftrag von, Berechtigungen entfernen, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 8f49fa5c4b320d05c6c6a9049b41170457bb394f
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253480"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Kunden delegieren Administratorrechte an Partner

**Zielgruppe**

-  Partner Center

Um den Dienst oder das Abonnement im Auftrag eines Kunden verwalten zu können, muss der Kunde Ihnen Administratorberechtigungen für diesen Dienst gewähren. Um Administratorberechtigungen von einem Kunden zu erhalten, senden Sie ihm per E-Mail einen Vertriebspartnerschaftsantrag. Nachdem der Kunde den Antrag genehmigt hat, können Sie sich beim Verwaltungsportal des Diensts anmelden und den Dienst im Auftrag des Kunden verwalten. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Einladen eines Kunden zur Einrichtung einer Vertriebspartnerschaft mit Ihnen

1.  Wählen Sie **Kunden** aus, und wählen Sie dann **Vertriebspartnerschaft beantragen** aus.

2.  Überprüfen Sie auf der nächsten Seite den E-Mail-Entwurf. Sie können den Nachrichtenentwurf in Ihrer standardmäßigen E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen. 

    >[!IMPORTANT]
    >Sie können den Text in der E-Mail bearbeiten. Nehmen Sie jedoch unbedingt den Link mit auf, da er personalisiert ist und den Kunden direkt mit Ihrem Konto verknüpft. 
    
3.  Select **Done** when you've completed this step.

4.  Senden Sie die E-Mail an den Kunden.

5.  Nachdem der Kunde die Einladung angenommen hat, wird er auf der Seite **Kunden** angezeigt, und Sie können den Dienst für den Kunden von dort aus bereitstellen und verwalten.

6.  To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name and then select the admin portal for the service you want to manage.

>[!IMPORTANT]  
>Kunden können Administratorberechtigungen im Verwaltungsportal eines Diensts neu zuweisen oder entfernen. Erst wenn Sie Ihre Vereinbarung mit dem Kunden erneut verhandeln, sind Sie jedoch weiterhin für die Bereitstellung des Supports und die Einhaltung der Bedingungen der Vereinbarung für Cloud-Vertriebspartner verantwortlich, auch nachdem ein Kunde die Administratorberechtigungen neu zugewiesen oder entfernt hat. In diesem Fall können Sie sich an den Microsoft-Support wenden, wenn der Kunde Hilfe benötigt, um eine Serviceanfrage im Auftrag des Kunden zu öffnen.

Ihre Kunden können über das Office 365-Verwaltungsportal ermitteln, welche ihrer Partner über Administratorrechte für ihren Mandanten verfügen. Gehen Sie dazu wie folgt vor:

1. Der Kunde muss sich als globaler Administrator beim Office 365-Verwaltungsportal anmelden.

2. Select **Settings** > **Partner relationships**.

3. Auf der Seite **Partnerbeziehungen** wird dem Kunden eine Liste der Partner angezeigt, mit denen er zusammenarbeitet, sowie der Partner, denen delegierte Administratorrechte für den Mandanten erteilt wurden.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Customers can manage a partner's delegated admin privileges 

Ihr Kunde kann beispielsweise Ihre delegierten Administratorrechte aus dem Mandanten entfernen, aber die Beziehung mit Ihnen zu Abonnement- und Lizenzverlängerungszwecken beibehalten. Kunden verwalten Rechte und Berechtigungen für ihre Office 365-Konten im Office 365 Admin Center auf der Seite **Partnerbeziehungen**. Auf dieser Seite können Kunden die folgenden Aktionen ausführen:

- Anzeigen, mit welchen Partnern eine Beziehung besteht und welche Partner über delegierte Administratorrechte verfügen

- Remove a partner's delegated administration privileges from the tenant

Gehen Sie wie folgt vor, um die delegierten Administratorrechte eines Partners zu entfernen:

1. Wählen auf der Seite **Partnerbeziehungen** den entsprechenden Partner aus.
2. Wählen Sie im Detailbereich die Option **Delegierten Administrator entfernen** aus.
3. Wählen Sie im Bestätigungsbereich die Option **Entfernen** aus.

>[!IMPORTANT]  
>Die Azure AD-Rollenzuweisungen für den Partner sind implizit. Wenn Sie versuchen, die Mitglieder der Azure AD-Rollen mithilfe des Azure AD-Portals bzw. mithilfe von PowerShell oder Graph aufzulisten, wird der Partner nicht zurückgegeben. Um festzustellen, ob den Partnern Azure AD-Rollen zugewiesen sind, müssen Sie im Office 365-Verwaltungsportal auf der Seite „Partnerbeziehungen“ überprüfen, ob dem Partner delegierte Administratorrechte erteilt wurden oder nicht.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegierte Administratorrechte in Azure AD 

There are two security groups, Admin Agents and Helpdesk Agents, in the partner's Azure AD tenant that are used for delegated administration. Wenn ein Kunde einem Partner delegierte Administratorrechte erteilt, geschieht Folgendes:

- The Admin Agent group is assigned to the Global Administrator role in the customer's Azure AD tenant.

- The Helpdesk Agent group is assigned to the Helpdesk Administrator role in the customer's Azure AD tenant.

Based on the directory roles assigned, members of both groups can sign in to the customer's Azure AD tenant and O365 services using their partner credentials and administrator on behalf of the customer.

If your customer removes delegated admin privileges, the Azure AD role assignments are removed, and you will no longer be able to manage the customer's Azure AD tenant.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-Abonnements und Ressourcenverwaltung

Jedes Azure-Abonnement verfügt über einen eigenen Satz von Ressourcenverwaltungsrollen. Before a CSP partner can manage a customer's Azure subscription, the partner must be assigned to one or more roles under the Azure subscription. Das bedeutet Folgendes:

- Wenn ein Kunde eine Händlereinladung annimmt und einem Partner delegierte Administratorrechte erteilt, erhält der Partner nicht automatisch Zugriff auf vorhandene Azure-Abonnements unter dem Kundenmandanten.

- Wenn der CSP-Partner ein neues Azure-Abonnement für den Kunden bereitstellt, wird der Gruppe der Administrator-Agents unter dem CSP-Partnermandanten automatisch die Rolle „Besitzer“ unter dem Abonnement zugewiesen. Basierend auf dieser Rollenzuweisung können Mitglieder der Gruppe auf Ressourcen unter dem Abonnement zugreifen und diese verwalten.

- When a customer removes delegated administration privileges from a partner using Office 365 Portal, the partner can still manage the customer's Azure subscription as long as the partner is still assigned to one or more roles under the subscription. Um die Verwaltung des Azure-Abonnements durch den Partner zu beenden, muss der Kunde die Rollenzuweisung entfernen.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Im Partner Center können CSP-Partner unter den folgenden Umständen Autopilot-Profile für ihre Kunden ohne delegierte Administratorrechte verwalten: 

- Wenn ein Kunde delegierte Administratorrechte entfernt, aber eine Vertriebspartnerbeziehung mit Ihnen aufrechterhält, können Sie die Autopilot-Profile für diesen Kunden weiterhin verwalten.

- Sie können von Ihnen oder einem anderen Partner hinzugefügte Kundengeräte verwalten. 

- You can't manage devices your customer has added through the Microsoft Store for Business, Microsoft Store for Education, or Microsoft Intune Portal.

Weitere Informationen zu Autopilot finden Sie unter [Vereinfachen der Geräteinstallation mit Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>Die aktuelle Autopilot-Verwaltungsoberfläche im Partner Center kann weiterhin Änderungen unterliegen. Zum Zeitpunkt der Veröffentlichung dieses Artikels werden die folgenden Änderungen in Betracht gezogen:

- Der Kunde muss dem Partner zuerst delegierte Administratorrechte erteilen, damit der Partner Profile hinzufügen/aktualisieren/entfernen und ein Profil anwenden oder von Geräten im Kundenmandanten entfernen kann.

- Der Kunde muss dem Partner zuerst delegierte Administratorrechte erteilen, damit der Partner im Kundenmandanten Geräte entfernen kann, die von anderen Partnern oder dem Kunden hinzugefügt wurden. Andernfalls kann der Partner nur Geräte entfernen, die zuvor vom selben Partner hinzugefügt wurden.
