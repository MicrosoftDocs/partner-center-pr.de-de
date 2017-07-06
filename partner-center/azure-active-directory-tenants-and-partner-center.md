---
title: Azure Active Directory-Mandanten und Partner Center | Partner Center
description: "Um ein Partner Center-Konto zu erstellen, muss Ihr Unternehmen über einen Azure Active Directory-Mandanten (Azure AD) verfügen. Azure AD ist der cloudbasierte Verzeichnis- und Identitätsverwaltungsdienst von Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Azure Active Directory-Mandanten und Partner Center  

**Betrifft:**

-  Partner Center

## <a name="why-you-need-an-azure-ad-tenant"></a>Warum benötigen Sie einen Azure AD-Mandanten?

Wir müssen den Azure AD-Mandanten Ihrer Organisation mit Ihrem neuen Partner Center-Konto verknüpfen, damit sich Ihre Mandantenbenutzer mit ihren AzureAD-Benutzernamen und -Kennwörtern (Microsoft-Konto) bei Partner Center anmelden können.

Wenn Ihr Unternehmen bereits einen Azure AD-Mandanten besitzt, können Sie ihn mit Ihrem Partner Center-Konto verknüpfen. 

>**Hinweis:**<br> Bevor Sie sich entschließen, einen vorhandenen Azure AD-Mandanten zu verwenden, bedenken Sie, wie viele Benutzer im Mandanten Partner Center verwenden müssen. Wenn Benutzer im Mandanten vorhanden sind, die nicht in Partner Center arbeiten müssen, ziehen Sie die Erstellung eines neuen Mandanten nur für die Benutzer in Betracht, die Partner Center verwenden müssen.

Falls Ihr Unternehmen nicht bereits über einen Azure AD-Mandanten verfügt, können Sie während des Registrierungsprozesses kostenlos einen erstellen. Wählen Sie **Neuen Mandanten erstellen** auf der Seite **Bei Azure Active Directory anmelden**. 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Sie sind nicht sicher, ob Ihre Firma bereits einen Azure AD-Mandanten besitzt?

Wenn Sie nicht sicher sind, ob Ihr Unternehmen einen Azure AD-Mandanten hat, gehen Sie folgendermaßen vor, um dies zu überprüfen. Beachten Sie Folgendes: Wenn Sie ein aktives Abonnement für Microsoft Azure oder Office365 haben, besitzen Sie bereits einen Azure AD-Mandanten.
1.  Melden Sie sich im Azure-Verwaltungsportal unter https://ms.portal.azure.com an.
2.  Wählen Sie im Menü Azure Active Directory, und wählen Sie dann die Domänennamen.
3.  Wenn Sie bereits einen Mandanten haben, wird Ihr Domänenname aufgeführt.

### <a name="using-an-existing-tenant"></a>Verwenden Sie einen vorhandenen Mandanten?

Wenn Sie einen vorhandenen Azure AD-Mandanten verwenden möchten, aber Probleme beim Anmelden haben, suchen Sie das Szenario im folgenden Diagramm, das Ihrer Situation am ehesten entspricht, und befolgen Sie die empfohlenen Schritte. 

![Haben Sie einen Azure AD-Mandanten oder müssen Sie einen erstellen?](images/onboardingAADFlow.png)

Weitere Informationen zum Hinzufügen von Domänen in Azure AD finden Sie unter [Hinzufügen oder Zuweisen einer Domäne in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain).

## <a name="about-microsoft-azure"></a>Informationen zu Microsoft Azure

Microsoft Azure ist eine öffentliche Cloudplattform, die Unternehmen zum Erstellen, Bereitstellen und Verwalten von Apps in einem globalen Netzwerk von durch Microsoft verwalteten Rechenzentren verwenden können. Unternehmen nutzen Azure zum Erstellen einer virtuellen IT-Infrastruktur mit virtuellen Funktionen oder Diensten anstelle von physischen Computern. 

Wenn Sie ein Azure-Abonnement erwerben, mieten Sie im Wesentlichen einen dedizierten, sicheren Platz in der öffentlichen Azure-Cloud. Dies unterscheidet sich nicht allzu sehr vom Mieten eines Stockwerks in einem Bürogebäude für die physische Einrichtung Ihres Unternehmens. Für den Eigentümer des Bürogebäudes ihr Ihr Unternehmen ein Mandant. 

Ein Azure AD-Mandant ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud, die für Sie erstellt wird, wenn Sie einen Microsoft-Clouddienst wie Azure, Microsoft Intune oder Office365 abonnieren. 

Der Mandanten hostet die Azure AD-Benutzer und die Informationen zu ihnen – ihre Kennwörter, Profildaten, Berechtigungen usw. Der Mandant enthält darüber hinaus Gruppen, Anwendungen und andere Informationen, die ein Unternehmen und seine Sicherheit betreffen. 

Weitere Informationen zu Azure AD finden Sie in der [Dokumentation zu Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/). 