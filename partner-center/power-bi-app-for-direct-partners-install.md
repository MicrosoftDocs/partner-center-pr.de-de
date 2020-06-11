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
ms.openlocfilehash: 7e2a1d17a7520cca1a6e1da540cc58d2d365d8cb
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679307"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI

**Zielgruppe**

- Partner Center

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Vertriebsbeauftragter
-   Administrator-Agent

## <a name="before-you-begin"></a>Voraussetzungen

Wählen Sie in der folgenden Liste verfügbarer Power BI-Apps die Anwendung aus, die für Ihr Unternehmen am relevantesten ist:
- [Direkter Anbieter](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Indirekter Anbieter](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Indirekter Reseller](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Bevor Sie die Vorschauversion der Partner Center Analytics-App installieren, stellen Sie sicher, dass Sie die folgenden Anforderungen erfüllen.

- Sie haben die richtige Power BI-App für Ihr Unternehmen ausgewählt.

- Sie verfügen über eine Power BI pro-Lizenz.

- Sie verfügen über Berechtigungen zum Installieren von Vorlagen-apps in Ihrem Mandanten.

- Sie können sich bei Power BI anmelden.

- Sie können sich als globaler Administrator, Administrator-Agent oder Abrechnungs Administrator beim [Azure Active Directory Ihres Unternehmens (Azure AD)](azure-active-directory-tenants-and-partner-center.md)anmelden.

## <a name="to-install-the-app"></a>So installieren Sie die App

1. Klicken Sie im obigen Abschnitt auf den entsprechenden Link für die APP-Quelle (direkter Anbieter/indirekter Anbieter/indirekter Reseller).

2. Klicken Sie auf **jetzt starten**. 

3. Stimmen Sie den Bedingungen zu, indem Sie auf **weiter**klicken.

4. Wählen Sie unter Sie haben bereits ein Konto?**Anmelden** aus.

5. Geben Sie auf der nächsten Seite den Benutzernamen und das Kennwort für Power BI und wählen Sie dann Anmelden aus.

6. Installieren Sie den Arbeitsbereich, indem Sie den WorkspaceName angeben.

7. Sie finden die Vorlagen-apps, die im Abschnitt "Apps" installiert sind.

8. Klicken Sie auf apps, und wählen Sie die installierten Apps aus.

9. Die ersten Schritte mit dem Bildschirm "neue App" werden geöffnet.

10. Zum Herstellen einer Verbindung mit den Daten klicken Sie auf **verbinden**.

11. Überprüfen Sie im Popup Fenster **Verbindung mit Partner Center-Analyse herstellen** , ob die **Authentifizierungsmethode** auf **oAuth2** festgelegt ist, oder wählen Sie **oAuth2** in der Liste aus, wenn dies nicht der Fall ist. 

> [!NOTE]  
>  Dieses Fenster erscheint möglicherweise erst nach einigen Minuten.

12. Melden Sie sich auf der Seite **Partner Center Analytics-Connector** mit dem globalen Administrator, dem Administrator-Agent oder den Abrechnungs Administrator-Anmelde Informationen für den Azure AD Mandanten Ihres Unternehmens an, und wählen Sie dann **Anmelden**aus.
 
13. Wählen Sie zum Zugriff aufgefordert werden, wählen Sie **Annehmen** aus. 

Sobald der Partner Center Analytics-Dienst mit Power BI verbunden ist, werden Daten geladen. Abhängig von der Datenmenge kann dies bis zu 10 Minuten in Anspruch nehmen. 

Nachdem die Daten geladen wurde, können Sie damit beginnen, das Partner Center Analytics-App-Dashboard und Berichte in Power BI zu nutzen.

## <a name="next-steps"></a>Nächste Schritte

[Anzeigen Ihrer Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
