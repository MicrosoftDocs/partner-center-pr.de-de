---
title: Kunden delegieren Administratorrechte an Partner | Partner Center
description: Als Händlerpartner können Ihre Kunden Sie als stellvertretenden Administrator festlegen. Sie können außerdem Berechtigungen entfernen.
author: labrenne
keywords: Rechte als stellvertretender Administrator, Administrator im Namen von, Berechtigungen entfernen
ms.localizationpriority: medium
ms.openlocfilehash: 7209917a92eb2cd9ae86c31f3126bdbac402a04e
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877170"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Kunden delegieren Administratorrechte an Partner

**Betrifft**

-  Partner Center

Als CSP-Partner und vertrauenswürdiger Ratgeber für Ihre Kunden können diese Sie als stellvertretenden Administrator für ihren Azure AD-Mandanten und Office365 festlegen. Sie können diese Beziehung über das Partner-Dashboard initiieren, indem Sie Ihren Kunden eine Einladung senden. 

1. Wählen Sie im Menü **Dashboard** die Option **Kunden** und anschließend **Beantragen einer Vertriebspartnerschaft** aus.
2. Eine Formular-E-Mail mit Ihrer URL wird eingeblendet. Sie können das Formular kopieren und in eine E-Mail einfügen, die Sie an den Kunden senden. Sie können beliebige weitere Informationen hinzufügen, aber achten Sie darauf, dass Sie die URL einfügen. Der Kunde wird diese URL verwenden, um auf Ihre Anfrage zu antworten.  
3. Wenn Ihr Kunde die Einladung annimmt, werden Sie zum Administrator für seine Dienste.

Ihre Kunden können über das Office 365-Dienstportal ermitteln, welche ihrer Partner über Administratorrechte für ihren Mandanten verfügen. Gehen Sie dazu folgendermaßen vor:

1. Melden Sie sich als globaler Administrator beim [Office 365 Admin-Portal](https://portal.office.com/adminportal) an.
2. Wählen Sie **Einstellungen** → **Partnerbeziehungen** aus.
3. Auf der Seite **Partnerbeziehungen** wird eine Liste der Partner angezeigt, mit denen Kunden zusammenarbeiten, sowie der Partner, denen stellvertretende Administratorrechte für ihren Mandanten gewährt wurden.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Kunden können die stellvertretenden Administratorrechte eines Partners verwalten 

Ihr Kunde entscheidet möglicherweise, Ihre Administratorrechte aus ihrem Mandanten zu entfernen, aber die Beziehung mit Ihnen für Abonnement- und Lizenzverlängerungszwecke beizubehalten. Kunden verwalten Rechte und Berechtigungen für ihre Office365-Konten auf der Seite **Partnerbeziehungen** im Office365 Admin Center. Auf dieser Seite können Kunden Folgendes durchführen:

- Anzeigen, mit welchen Partnern sie eine Beziehung haben und welche Partner über stellvertretende Administratorrechte verfügen

- Entfernen der stellvertretenden Administratorrechte eines Partners aus dem Mandanten

So entfernen Sie die stellvertretenden Administratorrechte eines Partners:

1. Wählen auf der Seite **Partnerbeziehungen** den entsprechenden Partner aus.
2. Wählen Sie im Detailbereich **Stellvertretenden Administrator entfernen** aus.
3. Wählen Sie im Bestätigungsbereich **Entfernen** aus.

>**Wichtig**<br>
Die Azure AD-Rollenzuweisungen für den Partner sind implizit. Wenn Sie versuchen, die Mitglieder der Azure AD-Rollen mithilfe des Azure AD-Portals bzw. PowerShell oder Graph aufzulisten, wird der Partner nicht zurückgegeben. Um festzustellen, ob den Partnern Azure AD-Rollen zugewiesen sind, müssen Sie sich auf die Seite mit den Partnerbeziehungen im Office365 Admin-Portal beziehen, um herauszufinden, ob dem Partner Rechte als stellvertretender Administrator gewährt wurden oder nicht.

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

CSP-Partner können über das Partner-Dashboard die Autopilot-Konfiguration für ihre Kunden auch ohne Rechte als stellvertretender Administrator verwalten. Wie das geht, erfahren Sie unter [Vereinfachte Geräteeinrichtung mit Windows Autopilot.](https://docs.microsoft.com/partner-center/autopilot)

Welche Möglichkeiten Sie haben, richtet sich danach, ob Sie ein direkter oder indirekter Händler sind.

|**Vorgang**   |**Direkter Händler oder indirekter Händler**   |**Indirekter Händler**   |
|-----------------|-----------------------------------| -----------------------------|
|Hinzufügen von Geräten (mithilfe einer CSV-Datei)  |Ja      |Nein|
|Entfernen von Geräten   |Ja   |Nein|
|Hinzufügen eines Profils   |Ja   | Ja   |
|Aktualisieren eines Profils   |Ja    |Ja   |
|Entfernen eines Profils   |Ja   |Ja   |
|Anwenden eines Profils auf Geräte   |Ja   |Ja   |
|Entfernen eines Profils von Geräten   |Ja   |Ja   | 

- CSP-Partner können weiterhin die Autopilot-Konfiguration für vorhandene Kunden mit Vertriebspartnerschaft verwalten, auch wenn die Kunden das Recht als stellvertretender Administrator für ihre Partner entfernt haben.

- Sie können vorhandene Geräte für Ihre Kunden verwalten, die entweder von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.

- Sie können keine Geräte verwalten, die Ihr Kunde hochgeladen hat (über Microsoft Store für Unternehmen oder das Microsoft Intune-Portal).

>**Wichtig** Die aktuelle Autopilot-Verwaltungserfahrung im Microsoft Partner Center ist nicht endgültig und unterliegt zukünftigen Änderungen. Zum Zeitpunkt der Zusammenstellung dieses Artikels werden die folgenden Änderungen in Betracht gezogen:

  - Dem Partner muss die Berechtigung als stellvertretender Administrator vom Kunden gewährt werden, bevor der Partner Profile hinzufügen/aktualisieren/entfernen und ein Profil anwenden oder von Geräten im Kundenmandanten entfernen kann.

- Dem Partner muss die Berechtigung als stellvertretender Administrator vom Kunden gewährt werden, bevor der Partner Geräte entfernen kann, die von Geräten anderen Partnern oder dem Kunden in den Kundenmandanten hochgeladen wurden. Andernfalls kann der Partner nur Geräte entfernen, die zuvor vom selben Partner hinzugefügt wurden.
