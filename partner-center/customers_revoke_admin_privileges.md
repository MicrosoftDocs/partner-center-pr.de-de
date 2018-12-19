---
title: Kunden delegieren Administratorrechte an Partner | Partner Center
ms.topic: article
ms.date: 12/18/2018
description: Als Händlerpartner kann Ihre Kunden Sie ihren Administrator delegieren Sie können außerdem Berechtigungen entfernen.
author: labrenne
ms.author: labrenne
keywords: Rechte als stellvertretender Administrator entfernen, Administrator im Namen von, Berechtigungen, DAP AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 92b23c15285db651abab326c18f5b25feaffdb6c
ms.sourcegitcommit: 90d656ed3a4d056a0506f7b5e2b1b8c728f58c46
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2018
ms.locfileid: "8976817"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Kunden delegieren Administratorrechte an Partner

**Betrifft**

-  Partner Center

Um den Dienst oder das Abonnement im Namen eines Kunden zu verwalten, muss der Kunde Ihnen Administratorberechtigungen für diesen Dienst gewähren. Um Administratorberechtigungen von einem Kunden zu erhalten, senden Sie ihm per E-Mail einen Vertriebspartnerschaftsantrag. Nachdem der Kunde den Antrag genehmigt hat, können Sie sich beim Verwaltungsportal des Diensts anmelden und den Dienst im Namen des Kunden verwalten. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Laden Sie einen Kunden ein, eine Vertriebspartnerschaft mit Ihnen einzugehen.

1.  Wählen Sie **Kunden** aus, und wählen Sie dann **beantragen einer vertriebspartnerschaft**.

2.  Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht. Sie können den Nachrichtenentwurf in Ihrer standardmäßigen E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen. 

    >[!IMPORTANT]
    >Sie können den Text in der E-Mail bearbeiten. Nehmen Sie jedoch unbedingt den Link mit auf, da er personalisiert ist und den Kunden direkt mit Ihrem Konto verknüpft. 
    
3.  Wählen Sie **Fertig**, wenn Sie diesen Schrittabgeschlossen haben.

4.  Senden Sie die E-Mail an den Kunden.

5.  Nachdem der Kunde die Einladung angenommen hat, wird er auf der Seite **Kunden** angezeigt, und Sie können den Dienst für den Kunden von dort aus bereitstellen und verwalten.

6.  Um das Konto, Services, Benutzern und Lizenzen des Kunden zu verwalten, erweitern Sie den Kundendatensatz durch Auswählen des Abwärtspfeils neben seinem Namen aus, und wählen Sie dann das Verwaltungsportal für den Dienst, die, den Sie verwalten möchten.

>[!IMPORTANT]  
>Kunden können neu zuweisen oder Entfernen von Administratorberechtigungen im Verwaltungsportal eines Diensts. Erst wenn Sie Ihre Vereinbarung mit dem Kunden erneut verhandeln, sind Sie jedoch weiterhin für die Bereitstellung des Supports und die Einhaltung der Bedingungen des Cloud Reseller Agreement verantwortlich, auch nachdem ein Kunde die Administratorberechtigungen neu zugewiesen oder entfernt hat. In diesem Fall wenn der Kunde Hilfe benötigt, wenden Sie sich an Microsoft Support, um eine Serviceanfrage im Auftrag des Kunden zu öffnen.

Ihre Kunden können ermitteln, welche ihrer Partner über Administratorrechte für ihren Mandanten aus in Office 365 Admin-Portal haben. Gehen Sie dazu folgendermaßen vor:

1. Der Kunde muss für die Anmeldung bei Office 365 Admin-Portal als ein globaler Administrator an.

2. Wählen Sie **Einstellungen** → **Partnerbeziehungen** aus.

3. Auf der Seite **Partnerbeziehungen** wird der Kunde eine Liste der Partner angezeigt, mit denen sie arbeiten und gewährt wurden stellvertretende Administratorrechte für ihren Mandanten.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Kunden können die stellvertretenden Administratorrechte eines Partners verwalten 

Ihr Kunde entscheidet möglicherweise Ihre delegierten Administratorrechte aus ihrem Mandanten zu entfernen, aber die Beziehung mit Ihnen für Abonnement- und lizenzverlängerungszwecke beizubehalten. Kunden verwalten Rechte und Berechtigungen für ihre Office365-Konten auf der Seite **Partnerbeziehungen** im Office365 Admin Center. Auf dieser Seite können Kunden Folgendes durchführen:

- Anzeigen, mit welchen Partnern sie eine Beziehung haben und welche Partner über stellvertretende Administratorrechte verfügen

- Entfernen der stellvertretenden Administratorrechte eines Partners aus dem Mandanten

So entfernen Sie die stellvertretenden Administratorrechte eines Partners:

1. Wählen auf der Seite **Partnerbeziehungen** den entsprechenden Partner aus.
2. Wählen Sie im Detailbereich **Stellvertretenden Administrator entfernen** aus.
3. Wählen Sie im Bestätigungsbereich **Entfernen** aus.

>[!IMPORTANT]  
>Die Azure AD-Rollenzuweisungen für den Partner sind implizit. Wenn Sie versuchen, die Mitglieder der Azure AD-Rollen mithilfe des Azure AD-Portals bzw. PowerShell oder Graph aufzulisten, wird der Partner nicht zurückgegeben. Um festzustellen, ob den Partnern Azure AD-Rollen zugewiesen sind, müssen Sie sich auf die Seite mit den Partnerbeziehungen im Office365 Admin-Portal beziehen, um herauszufinden, ob dem Partner Rechte als stellvertretender Administrator gewährt wurden oder nicht.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Rechte als stellvertretender Administrator in Azure AD 

Im Azure AD-Mandanten des Partners gibt es zwei Sicherheitsgruppen, Administrator-Agenten und Helpdesk-Agenten, die für stellvertretende Administratoren verwendet werden. Wenn ein Kunde einem Partner Rechte als stellvertretender Administrator gewährt, geschieht Folgendes:

- Die Gruppe der Administrator-Agenten wird der globalen Administratorrolle im Azure AD-Mandanten des Kunden zugewiesen.

- Die Gruppe der Helpdesk-Agenten wird der Helpdesk-Administratorrolle im Azure AD-Mandanten des Kunden zugewiesen.

Basierend auf den zugewiesenen Verzeichnisrollen können sich Mitglieder beider Gruppen mithilfe ihrer Partneranmeldedaten und Administratorrechte im Namen des Kunden beim Azure AD-Mandanten und den O365-Diensten des Kunden anmelden.

Wenn Ihr Kunde die Rechte als stellvertretender Administrator entfernt, werden die Azure AD-Rollenzuweisungen entfernt, und Sie können den Azure AD-Mandanten des Kunden nicht mehr verwalten.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-Abonnements und Ressourcenverwaltung

Jedes Azure-Abonnement verfügt über einen eigenen Satz von Ressourcenverwaltungsrollen. Bevor ein CSP-Partner das Azure-Abonnement eines Kunden verwalten kann, muss dem Partner eine oder mehrere Rollen unter dem Azure-Abonnement zugewiesen werden. Zum Beispiel:

- Wenn ein Kunde eine Händlereinladung annimmt und einem Partner stellvertretende Administratorrechte gewährt, erhält der Partner nicht automatisch Zugriff auf vorhandene Azure-Abonnements unter dem Kundenmandanten.

- Wenn der CSP-Partner ein neues Azure-Abonnement für den Kunden bereitstellt, wird der Gruppe der Administrator-Agenten unter dem CSP-Partnermandanten automatisch die Rolle des Besitzers im Rahmen des Abonnements zugewiesen. Basierend auf dieser Rollenzuweisung können Mitglieder der Gruppe auf Ressourcen unter dem Abonnement zugreifen und diese verwalten.

- Wenn ein Kunde über das Office 365-Portal die Rechte als stellvertretender Administrator von einem Partner entfernt, kann der Partner das Azure-Abonnement des Kunden weiterhin verwalten, solange der Partner immer noch einer oder mehreren Rollen unter dem Abonnement zugewiesen ist. Um die Verwaltung des Azure-Abonnements durch den Partner zu beenden, muss der Kunde die Rollenzuweisung entfernen.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

CSP-Partner können Autopilot Profile für ihre Kunden unter diesen Umständen ohne Rechte als stellvertretender Administrator verwalten, von Partner Center: 

- Wenn ein Kunde behält eine vertriebspartnerschaft mit Ihnen delegierte Administratorrechte entfernt, können Sie weiterhin zum Verwalten von Autopilot Profile für sie.

- Sie können Geräte von Kunden, die Sie oder einen anderen Partner hinzugefügt wurden, verwalten. 

- Sie können keine Geräte verwalten, die Ihre Kunden über den Microsoft Store für Unternehmen, Microsoft Store für Bildungseinrichtungen oder Microsoft Intune-Portal hinzugefügt hat.

Weitere Informationen zu Autopilot finden Sie unter [Vereinfachen der Geräteinstallation mit Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>Die aktuelle Autopilot-Management-Erfahrung im Partner Center möglicherweise weiterhin ändern. Zum Zeitpunkt der Veröffentlichung dieses Artikels, werden die folgenden Änderungen in Betracht gezogen:

- Dem Partner muss die Berechtigung als stellvertretender Administrator vom Kunden gewährt werden, bevor der Partner Profile hinzufügen/aktualisieren/entfernen und ein Profil anwenden oder von Geräten im Kundenmandanten entfernen kann.

- Partner muss gewährt werden stellvertretender Administrator vom Kunden die Partner Geräte hinzugefügt, von anderen Partnern oder dem Kunden in den kundenmandanten entfernen kann. Andernfalls kann der Partner nur Geräte, die zuvor vom selben Partner hinzugefügt wurden entfernen.
