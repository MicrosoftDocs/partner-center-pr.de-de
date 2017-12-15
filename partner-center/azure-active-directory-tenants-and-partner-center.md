---
title: "Geschäftskonten und PartnerCenter | Partner Center"
description: "Um ein Partner Center-Konto erstellen zu können, muss Ihr Unternehmen ein Arbeitskonto besitzen."
author: labrenne
robots: 
ms.openlocfilehash: 8885f20d2f5975da8e4585e1bc314697fa04ad6d
ms.sourcegitcommit: d5ce1bf171e535b0236bcd1e6dfbc4ef01ebd209
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2017
---
# <a name="your-company-work-account-and-partner-center"></a>Unternehmenskonto Ihrer Firma und Partner Center  

**Betrifft:**

-  Partner Center

# <a name="why-you-need-a-work-account"></a>Warum Sie ein Arbeitskonto benötigen

Wir müssen das Arbeitskonto Ihres Unternehmens mit Ihrem neuen Partner Center-Konto verknüpfen, damit sich Ihre Kontobenutzer im Partner Center mit dem Benutzernamen und dem Kennwort für ihr Arbeitskonto anmelden können.

Wenn Ihr Unternehmen bereits ein Arbeitskonto besitzt, können Sie es mit Ihrem Partner Center-Konto verknüpfen. 

**Hinweis** Bevor Sie sich entschließen, ein vorhandenes Arbeitskonto zu verwenden, bedenken Sie, wie viele Benutzer des Kontos mit dem Partner Center arbeiten müssen. Wenn das Konto Benutzer enthält, die nicht im Partner Center arbeiten müssen, ziehen Sie die Erstellung eines neuen Kontos nur für diese Benutzer in Betracht.

Falls Ihr Unternehmen noch nicht über ein Arbeitskonto verfügt, können Sie ein solches während des Registrierungsprozesses kostenlos erstellen. Wählen Sie **Neuen Mandanten erstellen** auf der Seite **Bei Azure Active Directory anmelden**. Wenn Sie einen neuen Azure Active Directory-Mandanten erstellen, erstellen Sie ein neues Arbeitskonto. Azure Active Directory ist die Identitätsverwaltungslösung von Microsoft mit Einmalanmeldung.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Sie sind nicht sicher, ob Ihre Firma bereits ein Arbeitskonto besitzt?

Wenn Sie nicht sicher sind, ob Ihr Unternehmen ein Arbeitskonto besitzt, können Sie das folgendermaßen überprüfen. Beachten Sie: Mit einem aktiven Abonnement für Microsoft Azure oder Office365 besitzen Sie bereits ein Arbeitskonto.
1.  Melden Sie sich im Azure-Verwaltungsportal unter https://ms.portal.azure.com an.
2.  Wählen Sie „Azure Active Directory” im Menü, und wählen Sie dann „Domänennamen”.
3.  Wenn Sie bereits ein Arbeitskonto besitzen, wird Ihr Domänenname aufgeführt.

## <a name="using-an-existing-work-account"></a>Verwenden eines vorhandenes Arbeitskontos

Wenn Sie ein vorhandenes Arbeitskonto verwenden möchten, aber Probleme beim Anmelden haben, suchen Sie im folgenden Diagramm das Szenario, das Ihrer Situation am ehesten entspricht, und befolgen Sie die empfohlenen Schritte. 

![Besitzen Sie ein Arbeitskonto oder müssen Sie ein solches erstellen?](images/onboardingAADFlow.png)

Weitere Informationen zum Hinzufügen von Domänen in Azure AD finden Sie unter [Hinzufügen oder Zuweisen einer Domäne in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain).

# <a name="about-microsoft-azure"></a>Informationen zu Microsoft Azure

Microsoft Azure ist eine öffentliche Cloudplattform, die Unternehmen zum Erstellen, Bereitstellen und Verwalten von Apps in einem globalen Netzwerk von durch Microsoft verwalteten Rechenzentren verwenden können. Unternehmen nutzen Azure zum Erstellen einer virtuellen IT-Infrastruktur mit virtuellen Funktionen oder Diensten anstelle von physischen Computern. 

Wenn Sie ein Azure-Abonnement erwerben, mieten Sie im Wesentlichen einen dedizierten, sicheren Platz in der öffentlichen Azure-Cloud. Dies unterscheidet sich nicht allzu sehr vom Mieten eines Stockwerks in einem Bürogebäude für die physische Einrichtung Ihres Unternehmens. Für den Eigentümer des Bürogebäudes ist Ihr Unternehmen ein Mandant. 

Ein Azure-Arbeitskonto ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud. Das Konto wird für Sie erstellt, wenn Sie einen der Microsoft Cloud Services wie Azure, Microsoft Intune oder Office365 abonnieren. 

Das Arbeitskonto hostet die Azure AD-Benutzer und die zugehörigen Informationen – Kennwörter, Profildaten, Berechtigungen usw. Zudem enthält das Arbeitskonto Gruppen, Anwendungen und andere Informationen, die ein Unternehmen und seine Sicherheit betreffen. 
