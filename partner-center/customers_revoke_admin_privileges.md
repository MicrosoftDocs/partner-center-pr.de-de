---
title: Kunden delegieren Administratorrechte an Partner | Partner Center
ms.topic: article
ms.date: 12/18/2018
description: Als Partner Reseller kann Ihre Kunden Sie ihren Administrator delegieren Sie können auch Berechtigungen entfernen.
author: LauraBrenner
ms.author: labrenne
keywords: delegierte Administratorrechte, Administrator im Auftrag von, entfernen Sie Berechtigungen, DAP AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 9253bcca2d93d9f0d62d6d7241132f0c0c9bf5ec
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586153"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Kunden delegieren Administratorrechte an Partner

**Gilt für**

-  Partner Center

Um den Dienst oder das Abonnement im Namen eines Kunden zu verwalten, muss der Kunde Ihnen Administratorberechtigungen für diesen Dienst gewähren. Um Administratorberechtigungen von einem Kunden zu erhalten, senden Sie ihm per E-Mail einen Vertriebspartnerschaftsantrag. Nachdem der Kunde den Antrag genehmigt hat, können Sie sich beim Verwaltungsportal des Diensts anmelden und den Dienst im Namen des Kunden verwalten. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Einladen eines Kunden zur Einrichtung einer Reseller-Partnerschaft mit Ihnen

1.  Wählen Sie **Kunden** und wählen Sie dann **vertriebspartnerbeziehung anfordern**.

2.  Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht. Sie können den Nachrichtenentwurf in Ihrer standardmäßigen E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen. 

    >[!IMPORTANT]
    >Sie können den Text in der E-Mail bearbeiten. Nehmen Sie jedoch unbedingt den Link mit auf, da er personalisiert ist und den Kunden direkt mit Ihrem Konto verknüpft. 
    
3.  Wählen Sie **Fertig**, wenn Sie diesen Schritt abgeschlossen haben.

4.  Senden Sie die E-Mail an den Kunden.

5.  Nachdem der Kunde die Einladung angenommen hat, wird er auf der Seite **Kunden** angezeigt, und Sie können den Dienst für den Kunden von dort aus bereitstellen und verwalten.

6.  Um des Kunden-Konto, Dienste, Benutzer und Lizenzen verwalten zu können, erweitern Sie den Eintrag des Kunden durch den Pfeil nach unten neben ihren Namen auswählen, und wählen Sie dann auf das Verwaltungsportal für den Dienst, die, den Sie verwalten möchten.

>[!IMPORTANT]  
>Kunden können neu zuweisen oder Entfernen von Administratorrechten im Administratorportal des Diensts. Erst wenn Sie Ihre Vereinbarung mit dem Kunden erneut verhandeln, sind Sie jedoch weiterhin für die Bereitstellung des Supports und die Einhaltung der Bedingungen des Cloud Reseller Agreement verantwortlich, auch nachdem ein Kunde die Administratorberechtigungen neu zugewiesen oder entfernt hat. In diesem Fall wenn der Kunde Hilfe erforderlich ist, wenden Sie sich an Microsoft Support, um eine Serviceanfrage im Auftrag des Kunden zu öffnen.

Ihre Kunden finde heraus, welche der ihre Partner Administratorberechtigungen, um ihren Mandanten aus in das Office 365-Verwaltungsportal haben. Gehen Sie dazu wie folgt vor:

1. Der Kunde muss für die Anmeldung beim Office 365-Verwaltungsportal als globalen Administrator.

2. Wählen Sie **Einstellungen** → **Partnerbeziehungen** aus.

3. Auf der **Partner Beziehungen** angezeigt, auf der Kunden wird eine Liste mit den Partnern, mit denen sie funktionieren, und diejenigen, die erteilt wurde ihrem Mandanten Administratorrechte zugewiesen werden.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Kunden können die stellvertretenden Administratorrechte eines Partners verwalten 

Kunden können Ihnen delegierte Administratorrechte aus ihrem Mandanten entfernen, aber die Beziehung mit der Sie für das Abonnement und die Lizenz erneuerungszwecken beibehalten. Kunden verwalten Rechte und Berechtigungen für ihre Office 365-Konten auf der Seite **Partnerbeziehungen** im Office 365 Admin Center. Auf dieser Seite können Kunden Folgendes durchführen:

- Anzeigen, mit welchen Partnern sie eine Beziehung haben und welche Partner über stellvertretende Administratorrechte verfügen

- Entfernen der stellvertretenden Administratorrechte eines Partners aus dem Mandanten

So entfernen Sie die stellvertretenden Administratorrechte eines Partners:

1. Wählen auf der Seite **Partnerbeziehungen** den entsprechenden Partner aus.
2. Wählen Sie im Detailbereich **Stellvertretenden Administrator entfernen** aus.
3. Wählen Sie im Bestätigungsbereich **Entfernen** aus.

>[!IMPORTANT]  
>Die Azure AD-Rollenzuweisungen für den Partner sind implizit. Wenn Sie versuchen, die Mitglieder der Azure AD-Rollen mithilfe des Azure AD-Portals bzw. PowerShell oder Graph aufzulisten, wird der Partner nicht zurückgegeben. Um festzustellen, ob den Partnern Azure AD-Rollen zugewiesen sind, müssen Sie sich auf die Seite mit den Partnerbeziehungen im Office 365 Admin-Portal beziehen, um herauszufinden, ob dem Partner Rechte als stellvertretender Administrator gewährt wurden oder nicht.

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

Partner Center können CSP-Partner Autopilot-Profile für ihre Kunden ohne delegierte Administratorrechte unter diesen Umständen verwalten: 

- Wenn ein Kunde delegierte Administratorrechte entfernt, aber eine vertriebspartnerbeziehung mit Ihnen behält, können Sie weiterhin zum Verwalten von Autopilot-Profile für sie.

- Sie können Kundengeräte, die Sie oder ein anderer Partner hinzugefügt haben, verwalten. 

- Sie können keine Geräte verwalten, die Ihre Kunden über den Microsoft Store für Unternehmen, Microsoft Store für Bildungseinrichtungen oder Microsoft Intune-Portal hinzugefügt hat.

Weitere Informationen zu den Autopilot, finden Sie unter [vereinfachen der Geräteinstallation mit Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>Die aktuelle Autopilot-Verwaltungsoberfläche im Partner Center kann weiterhin ändern. Zum Zeitpunkt der Veröffentlichung dieses Artikels wurde, werden die folgenden Änderungen in Betracht gezogen:

- Dem Partner muss die Berechtigung als stellvertretender Administrator vom Kunden gewährt werden, bevor der Partner Profile hinzufügen/aktualisieren/entfernen und ein Profil anwenden oder von Geräten im Kundenmandanten entfernen kann.

- Partner muss gewährt werden Berechtigungen für delegierte Administration vom Kunden vor dem Entfernen des Partners Geräte, die vom anderen Partner oder vom Kunden im kundenmandanten hinzugefügt. Andernfalls kann der Partner nur Geräte, die zuvor vom gleichen Partner hinzugefügt entfernen.
