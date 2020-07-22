---
title: Abrufen der Administratorberechtigungen eines Kunden
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Rufen Sie die Berechtigungen ab, die Sie benötigen, um den Dienst oder das Abonnement eines Kunden in seinem Namen zu verwalten. Erfahren Sie, wie Berechtigungen erteilt, widerrufen und verwaltet werden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 22cdcb48df263323ac2862ced3a0f06eff2b0570
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434749"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Abrufen von Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Administrator-Agent
- Vertriebsbeauftragter

Um den Dienst oder das Abonnement im Auftrag eines Kunden verwalten zu können, muss der Kunde Ihnen Administratorberechtigungen für diesen Dienst gewähren. Um Administratorberechtigungen von einem Kunden zu erhalten, senden Sie ihm per E-Mail einen Vertriebspartnerschaftsantrag. Nachdem der Kunde den Antrag genehmigt hat, können Sie sich beim Verwaltungsportal des Diensts anmelden und den Dienst im Auftrag des Kunden verwalten. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Einladen eines Kunden, eine Vertriebspartnerschaft mit Ihnen einzugehen

1.  Wählen Sie **Kunden** aus, und wählen Sie dann **Vertriebspartnerschaft beantragen** aus.

2.  Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht. Sie können den Entwurf der Nachricht in Ihrer Standardanwendung für E-Mails öffnen oder in die Zwischenablage kopieren und in eine E-Mail einfügen. 

    >[!IMPORTANT]
    >Sie können den Text in der E-Mail bearbeiten. Nehmen Sie jedoch unbedingt den Link mit auf, da er personalisiert ist und den Kunden direkt mit Ihrem Konto verknüpft. 
    
3.  Wähle **Fertig** aus, nachdem du diesen Schritt abgeschlossen hast.

4.  Senden Sie die E-Mail an den Kunden.

5.  Nachdem der Kunde die Einladung angenommen hat, wird er auf der Seite **Kunden** angezeigt, und Sie können den Dienst für den Kunden von dort aus bereitstellen und verwalten.

6.  Erweitern Sie zum Verwalten des Kontos, des Diensts, der Benutzer und der Lizenzen des Kunden den Kundendatensatz, indem Sie neben seinem Namen auf den Pfeil nach unten klicken, und wählen Sie dann das Verwaltungsportal für den Dienst aus, den Sie verwalten möchten.

>[!IMPORTANT]  
>Kunden können Administratorberechtigungen im Verwaltungsportal eines Diensts neu zuweisen oder entfernen. Erst wenn Sie Ihre Vereinbarung mit dem Kunden erneut verhandeln, sind Sie jedoch weiterhin für die Bereitstellung des Supports und die Einhaltung der Bedingungen der Vereinbarung für Cloud-Vertriebspartner verantwortlich, auch nachdem ein Kunde die Administratorberechtigungen neu zugewiesen oder entfernt hat. In diesem Fall können Sie sich an den Microsoft-Support wenden, wenn der Kunde Hilfe benötigt, um eine Serviceanfrage im Auftrag des Kunden zu öffnen.

Ihre Kunden können über das Office 365-Verwaltungsportal ermitteln, welche ihrer Partner über Administratorrechte für ihren Mandanten verfügen. Aufgabe:

1. Der Kunde muss sich als globaler Administrator beim Office 365-Verwaltungsportal anmelden.

2. Wählen Sie **Einstellungen** > **Partnerbeziehungen** aus.

3. Auf der Seite **Partnerbeziehungen** wird dem Kunden eine Liste der Partner angezeigt, mit denen er zusammenarbeitet, sowie der Partner, denen delegierte Administratorrechte für den Mandanten erteilt wurden.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Kunden können die delegierten Administratorrechte eines Partners verwalten 

Ihr Kunde kann beispielsweise Ihre delegierten Administratorrechte aus dem Mandanten entfernen, aber die Beziehung mit Ihnen zu Abonnement- und Lizenzverlängerungszwecken beibehalten. Kunden verwalten Rechte und Berechtigungen für ihre Office 365-Konten im Office 365 Admin Center auf der Seite **Partnerbeziehungen**. Auf dieser Seite können Kunden die folgenden Aktionen ausführen:

- Anzeigen, mit welchen Partnern eine Beziehung besteht und welche Partner über delegierte Administratorrechte verfügen

- Entfernen der delegierten Administratorrechte eines Partners aus dem Mandanten

Gehen Sie wie folgt vor, um die delegierten Administratorrechte eines Partners zu entfernen:

1. Wählen auf der Seite **Partnerbeziehungen** den entsprechenden Partner aus.
2. Wählen Sie im Detailbereich die Option **Delegierten Administrator entfernen** aus.
3. Wählen Sie im Bestätigungsbereich die Option **Entfernen** aus.

>[!IMPORTANT]  
>Die Azure AD-Rollenzuweisungen für den Partner sind implizit. Wenn Sie versuchen, die Mitglieder der Azure AD-Rollen mithilfe des Azure AD-Portals bzw. mithilfe von PowerShell oder Graph aufzulisten, wird der Partner nicht zurückgegeben. Um festzustellen, ob den Partnern Azure AD-Rollen zugewiesen sind, müssen Sie im Office 365-Verwaltungsportal auf der Seite „Partnerbeziehungen“ überprüfen, ob dem Partner delegierte Administratorrechte erteilt wurden oder nicht.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegierte Administratorrechte in Azure AD 

Im Azure AD-Mandanten des Partners gibt es zwei Sicherheitsgruppen, Administrator-Agents und Helpdesk-Agents, die für die delegierte Verwaltung verwendet werden. Wenn ein Kunde einem Partner delegierte Administratorrechte erteilt, geschieht Folgendes:

- Der Gruppe der Administrator-Agents wird im Azure AD-Mandanten des Kunden die Rolle „Globaler Administrator“ zugewiesen.

- Der Gruppe der Helpdesk-Agents wird im Azure AD-Mandanten des Kunden die Rolle „Helpdeskadministrator“ zugewiesen.

Basierend auf den zugewiesenen Verzeichnisrollen können sich Mitglieder beider Gruppen mit ihren Partneranmeldeinformationen und als Administrator im Auftrag des Kunden beim Azure AD-Mandanten und den Office 365-Diensten des Kunden anmelden.

Wenn Ihr Kunde delegierte Administratorrechte entfernt, werden die Azure AD-Rollenzuweisungen entfernt, und Sie können den Azure AD-Mandanten des Kunden nicht mehr verwalten.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-Abonnements und Ressourcenverwaltung

Jedes Azure-Abonnement verfügt über einen eigenen Satz von Ressourcenverwaltungsrollen. Bevor ein CSP-Partner das Azure-Abonnement eines Kunden verwalten kann, muss dem Partner mindestens eine Rolle unter dem Azure-Abonnement zugewiesen werden. Das bedeutet Folgendes:

- Wenn ein Kunde eine Händlereinladung annimmt und einem Partner delegierte Administratorrechte erteilt, erhält der Partner nicht automatisch Zugriff auf vorhandene Azure-Abonnements unter dem Kundenmandanten.

- Wenn der CSP-Partner ein neues Azure-Abonnement für den Kunden bereitstellt, wird der Gruppe der Administrator-Agents unter dem CSP-Partnermandanten automatisch die Rolle „Besitzer“ unter dem Abonnement zugewiesen. Basierend auf dieser Rollenzuweisung können Mitglieder der Gruppe auf Ressourcen unter dem Abonnement zugreifen und diese verwalten.

- Wenn ein Kunde über das Office 365-Portal die delegierten Administratorrechte eines Partners entfernt, kann der Partner das Azure-Abonnement des Kunden weiterhin verwalten, solange dem Partner noch mindestens eine Rolle unter dem Abonnement zugewiesen ist. Um die Verwaltung des Azure-Abonnements durch den Partner zu beenden, muss der Kunde die Rollenzuweisung entfernen.

## <a name="windows-autopilot"></a>Windows Autopilot

Im Partner Center können CSP-Partner unter den folgenden Umständen Autopilot-Profile für ihre Kunden ohne delegierte Administratorrechte verwalten: 

- Wenn ein Kunde delegierte Administratorrechte entfernt, aber eine Vertriebspartnerbeziehung mit Ihnen aufrechterhält, können Sie die Autopilot-Profile für diesen Kunden weiterhin verwalten.

- Sie können von Ihnen oder einem anderen Partner hinzugefügte Kundengeräte verwalten. 

- Sie können keine Geräte verwalten, die Ihr Kunde über den Microsoft Store für Unternehmen, den Microsoft Store für Bildungseinrichtungen oder das Microsoft Intune-Portal hinzugefügt hat.

Weitere Informationen zu Autopilot finden Sie unter [Vereinfachen der Geräteinstallation mit Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>Die aktuelle Autopilot-Verwaltungsoberfläche im Partner Center kann weiterhin Änderungen unterliegen. Zum Zeitpunkt der Veröffentlichung dieses Artikels werden die folgenden Änderungen in Betracht gezogen:

- Der Kunde muss dem Partner zuerst delegierte Administratorrechte erteilen, damit der Partner Profile hinzufügen/aktualisieren/entfernen und ein Profil anwenden oder von Geräten im Kundenmandanten entfernen kann.

- Der Kunde muss dem Partner zuerst delegierte Administratorrechte erteilen, damit der Partner im Kundenmandanten Geräte entfernen kann, die von anderen Partnern oder dem Kunden hinzugefügt wurden. Andernfalls kann der Partner nur Geräte entfernen, die zuvor vom selben Partner hinzugefügt wurden.
