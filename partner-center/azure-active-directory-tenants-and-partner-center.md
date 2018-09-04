---
title: Geschäftskonten und PartnerCenter | Partner Center
description: Damit ein Partner Center-Konto erstellt werden kann, muss Ihr Unternehmen ein Geschäftskonto besitzen.
author: labrenne
Keywords: work account, email, tenant, Azure tenant, create account, domain name
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 2ebc5490d724b49836b0051802038c4ba4c86e20
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876080"
---
# <a name="your-company-work-account-and-the-partner-dashboard"></a>Unternehmenskonto Ihrer Firma und des Partner-Dashboards  

**Betrifft:**

-  Partner Center

## <a name="why-you-need-a-work-account"></a>Warum Sie ein Geschäftskonto benötigen

Wir müssen das Geschäftskonto Ihres Unternehmens mit Ihrem neuen Partner-Dashboard-Konto verknüpfen, damit sich Ihre Kontobenutzer im Partner-Dashboard mit dem Benutzernamen und dem Kennwort für ihr Geschäftskonto anmelden können.

Wenn Ihr Unternehmen bereits ein Geschäftskonto besitzt, können Sie es mit Ihrem Partner-Dashboard-Konto verknüpfen. 

>**Hinweis** Bevor Sie sich entschließen, ein vorhandenes Geschäftskonto zu verwenden, bedenken Sie, wie viele Benutzer des Kontos mit dem Partner-Dashboard arbeiten müssen. Wenn das Konto Benutzer enthält, die nicht im Partner-Dashboard arbeiten müssen, ziehen Sie die Erstellung eines neuen Kontos nur für diese Benutzer in Betracht.

Falls Ihr Unternehmen noch nicht über ein Geschäftskonto verfügt, können Sie ein solches während des Registrierungsprozesses erstellen. 

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Sie sind nicht sicher, ob Ihre Firma bereits ein Geschäftskonto besitzt?

Wenn Sie nicht sicher sind, ob Ihr Unternehmen ein Geschäftskonto besitzt, können Sie das folgendermaßen überprüfen. Beachten Sie: Mit einem aktiven Abonnement für Microsoft Azure oder Office365 besitzen Sie bereits ein Geschäftskonto.
1.  Melden Sie sich beim Microsoft Azure-Portal unter https://ms.portal.azure.com an
2.  Wählen Sie „Azure Active Directory” im Menü, und wählen Sie dann „Domänennamen”.
3.  Wenn Sie bereits ein Geschäftskonto besitzen, wird Ihr Domänenname aufgeführt.

## <a name="using-an-existing-work-account"></a>Verwenden eines vorhandenes Geschäftskontos

Wenn Sie ein vorhandenes Geschäftskonto verwenden möchten, aber Probleme beim Anmelden haben, suchen Sie im folgenden Diagramm das Szenario, das Ihrer Situation am ehesten entspricht, und befolgen Sie die empfohlenen Schritte. 

![Besitzen Sie ein Geschäftskonto oder müssen Sie ein solches erstellen?](images/onboardingAADFlow.png)

Weitere Informationen zum Hinzufügen von Domänen in Azure AD finden Sie unter [Hinzufügen oder Zuweisen einer Domäne in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain).

# <a name="about-microsoft-azure"></a>Informationen zu Microsoft Azure

Microsoft Azure ist eine öffentliche Cloudplattform, die Unternehmen zum Erstellen, Bereitstellen und Verwalten von Apps in einem globalen Netzwerk von durch Microsoft verwalteten Rechenzentren verwenden können. Unternehmen nutzen Azure zum Erstellen einer virtuellen IT-Infrastruktur mit virtuellen Funktionen oder Diensten anstelle von physischen Computern. 

Wenn Sie ein Azure-Abonnement erwerben, mieten Sie im Wesentlichen einen dedizierten, sicheren Platz in der öffentlichen Azure-Cloud. Dies unterscheidet sich nicht allzu sehr vom Mieten eines Stockwerks in einem Bürogebäude für die physische Einrichtung Ihres Unternehmens. Für den Eigentümer des Bürogebäudes ist Ihr Unternehmen ein Mandant. 

Ein Azure-Geschäftskonto ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud. Das Konto wird für Sie erstellt, wenn Sie einen der Microsoft Cloud Services wie Azure, Microsoft Intune oder Office365 abonnieren. 

Das Geschäftskonto hostet die Azure AD-Benutzer und die zugehörigen Informationen – Kennwörter, Profildaten, Berechtigungen usw. Zudem enthält das Geschäftskonto Gruppen, Anwendungen und andere Informationen, die ein Unternehmen und seine Sicherheit betreffen. 
