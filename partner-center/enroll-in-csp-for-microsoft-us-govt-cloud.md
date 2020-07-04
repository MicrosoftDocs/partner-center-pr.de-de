---
title: Registrieren für das CSP-Programm
ms.topic: article
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.date: 06/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Anforderungen an das CSP-Programm für Partner, die sich für das Cloud Solution Provider-Programm für Microsoft Cloud für die US-Regierung registrieren möchten.
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 67dd4823e5167fb0e0ece692e873cd8cde7013ea
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947533"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Registrieren für das Cloud Solution Provider-Programm für Microsoft Cloud for US Government

**Zielgruppe**

- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Globaler Administrator

Microsoft-Partner können jetzt Cloudlösungen und -dienste von Microsoft an Bundesbehörden, staatliche und kommunale Einrichtungen sowie an Stammeseinrichtungen in den USA über das CSP-Programm (Cloud Solution Provider, Cloud-Lösungsanbieter) für Microsoft Cloud for US Government verkaufen. 

Microsoft Cloud for US Government bietet eine private, dedizierte und isolierte Instanz von Microsoft Azure, die die Anforderungen von US-Behörden an Datensicherheit, Datenschutz und Compliance erfüllt. Ihr Unternehmen muss die Qualifizierungskriterien von Microsoft zur Teilnahme am CSP-Programm für Microsoft Cloud for US Government erfüllen. Weitere Informationen finden Sie unter [Partner Center für Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md).

## <a name="before-you-begin"></a>Vorbereitung

Damit Sie sich für das CSP-Programm für Microsoft Cloud for US Government registrieren können, müssen wir uns zunächst vergewissern, dass Ihr Unternehmen die Anforderungen für den Verkauf an US-Behörden erfüllt. Füllen Sie vor Beginn des Registrierungsprozesses das [Formular zur Microsoft Government Cloud-Überprüfung](https://azuregov.microsoft.com/csp) aus, damit die Qualifikation Ihres Unternehmens überprüft werden kann. Nachdem wir die Qualifikation Ihres Unternehmens überprüft haben, stellen wir einen speziellen Azure AD-Mandanten (Azure Active Directory) für Microsoft Cloud for US Government bereit.  

Um ein Partner Center-Konto für CSP für Microsoft Cloud for US Government erstellen und sich registrieren zu können, sind folgende Informationen erforderlich. (Diese Informationen sollten vor dem Registrierungsprozess gesammelt werden.)

-  Anmeldeinformationen eines globalen Administrators für den neuen Azure AD-Mandanten Ihrer Organisation für Microsoft Cloud for US Government
-  Die MPN-ID (Microsoft Partner Network) Ihrer Organisation 
-  Eine geschäftliche Anschrift in den USA

> [!IMPORTANT]  
> Wenn Sie bereits über ein Konto in Partner Center verfügen und sich bei CSP für Microsoft Cloud for US Government registrieren möchten, müssen Sie ein neues, separates Konto speziell für US-Behörden erstellen.

## <a name="how-to-enroll"></a>Registrierung 

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Schritt 1: Erstellen eines Partner Center-Kontos für Microsoft Cloud for US Government

1.  Starten Sie den Registrierungsprozess [hier](https://partnercenter.microsoft.com/register/resellerusgjoinnow). 

2.  Melden Sie sich mit den Anmeldeinformationen eines globalen Administrators für den Azure AD-Mandanten Ihrer Organisation für Microsoft Cloud for US Government an. Falls Ihre Organisation über kein Konto für dieses Portal verfügt, können Sie eines anfordern, indem Sie das [Formular zur Microsoft Government Cloud-Überprüfung](https://azuregov.microsoft.com/csp) ausfüllen.


### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Schritt 2: Beantragen der Teilnahme am Cloud Solution Provider-Programm für Microsoft Cloud for US Government

1.  Füllen Sie die fehlenden Informationen im Registrierungsformular aus, einschließlich Ihrer Microsoft Partner Network-ID und der Kundensupportinformationen Ihrer Organisation. 

2.  Wählen Sie **Zustimmen und fortfahren** aus. Das Überprüfen Ihrer Bewerbung kann mehrere Tage dauern. Wir werden Sie per E-Mail informieren, wenn unsere Überprüfung abgeschlossen ist.

    > [!IMPORTANT]  
    > Durch Auswählen von **Zustimmen und fortfahren** bestätigen Sie, dass Sie berechtigt sind, im Namen Ihrer Organisation zu handeln, und dass Sie Microsoft erlauben, vor der Prüfung der Cloud Solution Provider-Bewerbung Ihrer Organisation eine Bonitätsprüfung vorzunehmen.


### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Schritt 3: Unterschreiben der Vereinbarung für Reseller für Microsoft Cloud for US Government

1. Melden Sie sich über den Link in der Bewerbungsbestätigungs-E-Mail bei Partner Center für Microsoft Cloud for US Government an. 

2. Lesen Sie sich die rechtlichen Hinweise auf der Seite **Vereinbarung** durch. Wenn Sie einverstanden sind, wählen Sie **Zustimmen und fortfahren** aus, um den [Händlervertrag für Microsoft Cloud for US Government](https://go.microsoft.com/fwlink/p/?linkid=843364) digital zu unterzeichnen. Das Erstellen Ihres Kontos kann mehrere Stunden dauern. Melden Sie sich bei Partner Center für Microsoft Cloud for US Government ab und später wieder an.


### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Schritt 4: Zuweisen von Benutzern zur Administrator-Agent-Rolle im Microsoft Azure-Verwaltungsportal für Microsoft Cloud for US Government

Microsoft Cloud for US Government bietet eine separate Instanz von Microsoft Azure, die die Compliance-, Sicherheits- und Datenschutzanforderungen von Behörden erfüllt. Um Administratoren die Verwaltung von Benutzern und Lizenzen im Microsoft Azure-Portal zu ermöglichen, müssen Sie ihnen manuell die Administrator-Agent-Rolle zuweisen.

> [!NOTE]  
> Nachdem Sie Benutzer der Administrator-Agent-Rolle zugewiesen haben, können sie auf der Seite **Kunden** auf Ihre Kundenliste zugreifen und [neue Kunden hinzufügen](add-a-new-customer.md).   

1.  Melden Sie sich unter https://portal.azure.us/ beim Microsoft Azure-Verwaltungsportal an.

2.  Weisen Sie die Administrator-Agent-Rolle den entsprechenden Benutzern in Ihrer Organisation zu. Hierzu müssen die Benutzer der integrierten Gruppe **AdminAgent** hinzugefügt werden. Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Gruppenmitgliedern mithilfe von Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-groups-members-azure-portal).
 
## <a name="connect-with-us"></a>Neuigkeiten abonnieren

- Noch Fragen? Senden Sie uns eine E-Mail: azgovcsp@microsoft.com.

- Folgen Sie uns auf [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777&view=all). 

## <a name="related-topics"></a>Zugehörige Themen

-  [Partner Center für Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md)

-  [Benutzer- und Lizenzverwaltung im Partner Center für Microsoft Cloud for US Government](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)


