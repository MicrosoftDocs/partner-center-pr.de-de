---
title: Installieren von Partner Center Analytics für Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Führen Sie die Schritte in diesem Artikel aus, um die Partner Center Analytics-APP für Power BI (für direkte Partner in CSP) zu installieren und in der Vorschau anzuzeigen.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795871"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI

**Zielgruppe**

- Partner Center

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Vertriebsbeauftragter
-   Administrator-Agent

## <a name="before-you-begin"></a>Vorbereitung

Wählen Sie in der folgenden Liste verfügbarer Power BI-Apps die Anwendung aus, die für Ihr Unternehmen am relevantesten ist:
- [Direktpartner](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Indirekter Partner](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Indirekter Reseller](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Bevor Sie die Vorschauversion der Partner Center Analytics-App installieren, stellen Sie sicher, dass Sie die folgenden Anforderungen erfüllen.

- Sie haben die richtige Power BI-App für Ihr Unternehmen ausgewählt.

- Sie besitzen ein aktives Abonnement für Microsoft Power BI Professional oder Microsoft Power BI Premium.

- Sie können sich bei Power BI anmelden.

- Sie können sich als globaler Administrator, Administrator-Agent oder Abrechnungs Administrator beim [Azure Active Directory Ihres Unternehmens (Azure AD)](azure-active-directory-tenants-and-partner-center.md)anmelden.

## <a name="to-install-the-app"></a>So installieren Sie die App

1. Starten Sie den [Installationsprozess](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. Wählen Sie unter **Sie haben bereits ein Konto?****Anmelden** aus. 

3. Geben Sie auf der nächsten Seite den Benutzernamen und das Kennwort für Power BI und wählen Sie dann **Anmelden** aus. 

4. Überprüfen Sie im Popup Fenster **Verbindung mit Partner Center-Analyse herstellen** , ob die **Authentifizierungsmethode** auf **oAuth2** festgelegt ist, oder wählen Sie **oAuth2** in der Liste aus, wenn dies nicht der Fall ist. 

> [!NOTE]  
>  Dieses Fenster erscheint möglicherweise erst nach einigen Minuten.

5. Melden Sie sich auf der Seite **Partner Center Analytics-Connector** mit dem globalen Administrator, dem Administrator-Agent oder den Abrechnungs Administrator-Anmelde Informationen für den Azure AD Mandanten Ihres Unternehmens an, und wählen Sie dann **Anmelden**aus.
 
6. Wählen Sie zum Zugriff aufgefordert werden, wählen Sie **Annehmen** aus. 

Sobald der Partner Center Analytics-Dienst mit Power BI verbunden ist, werden Daten geladen. Abhängig von der Datenmenge kann dies bis zu 10 Minuten in Anspruch nehmen. 

Nachdem die Daten geladen wurde, können Sie damit beginnen, das Partner Center Analytics-App-Dashboard und Berichte in Power BI zu nutzen.

## <a name="next-steps"></a>Nächste Schritte

[Anzeigen Ihrer Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
