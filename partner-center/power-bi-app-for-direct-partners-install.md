---
title: Installieren von Partner Center Analytics für Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Führen Sie die Schritte in diesem Artikel aus, um die Partner Center Analytics-APP für Power BI (für direkte Partner in CSP) zu installieren und in der Vorschau anzuzeigen.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633691"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI


**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Vertriebsbeauftragter
- Administrator-Agent

## <a name="before-you-begin"></a>Voraussetzungen

Wählen Sie in der folgenden Liste verfügbarer Power BI-Apps die Anwendung aus, die für Ihr Unternehmen am relevantesten ist:

- [Direkter Anbieter](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Indirekter Anbieter](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Indirekter Reseller](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Bevor Sie die Vorschauversion der Partner Center Analytics-App installieren, stellen Sie sicher, dass Sie die folgenden Anforderungen erfüllen.

- Sie haben die richtige Power BI-App für Ihr Unternehmen ausgewählt.

- Sie verfügen über eine Power BI pro-Lizenz.

- Sie verfügen über Berechtigungen zum Installieren von Vorlagen-apps in Ihrem Mandanten.

- Sie können sich bei Power BI anmelden.

- Sie können sich als globaler Administrator, Administrator-Agent oder Abrechnungs Administrator beim [Azure Active Directory Ihres Unternehmens (Azure AD)](azure-active-directory-tenants-and-partner-center.md)anmelden.

## <a name="to-install-the-app"></a>So installieren Sie die App

1. Wählen Sie den entsprechenden Link für die APP-Quelle (direkter Anbieter/indirekter Anbieter/indirekter Reseller) im obigen Abschnitt aus.

2. Wählen Sie **Jetzt herunterladen** aus. 

3. Stimmen Sie den Nutzungsbedingungen zu, indem Sie **weiter** auswählen.

4. Wählen Sie unter Sie haben bereits ein Konto?**Anmelden** aus.

5. Geben Sie auf der nächsten Seite den Benutzernamen und das Kennwort für Power BI und wählen Sie dann **Anmelden** aus.

6. Installieren Sie den Arbeitsbereich, indem Sie den Arbeitsbereichs Namen angeben.

7. Sie finden die Vorlagen-apps, die im Abschnitt "Apps" installiert sind.

8. Wählen Sie **apps** aus, und wählen Sie die installierten apps.

9. Die ersten Schritte mit dem Bildschirm "neue App" werden geöffnet.

10. Wählen Sie zum Herstellen einer Verbindung mit den Daten **verbinden** aus.

11. Überprüfen Sie im Popup Fenster **Verbindung mit Partner Center-Analyse herstellen** , ob die **Authentifizierungsmethode** auf **oAuth2** festgelegt ist, oder wählen Sie **oAuth2** in der Liste aus, wenn dies nicht der Fall ist. 

> [!NOTE]  
>  Dieses Fenster erscheint möglicherweise erst nach einigen Minuten.

12. Melden Sie sich auf der Seite **Partner Center Analytics-Connector** mit dem globalen Administrator, dem Administrator-Agent oder den Abrechnungs Administrator-Anmelde Informationen für den Azure AD Mandanten Ihres Unternehmens an, und wählen Sie dann **Anmelden** aus.
 
13. Wählen Sie zum Zugriff aufgefordert werden, wählen Sie **Annehmen** aus. 

Sobald der Partner Center Analytics-Dienst mit Power BI verbunden ist, werden Daten geladen. Abhängig von der Datenmenge kann dies bis zu 10 Minuten in Anspruch nehmen. 

Nachdem die Daten geladen wurde, können Sie damit beginnen, das Partner Center Analytics-App-Dashboard und Berichte in Power BI zu nutzen.

## <a name="next-steps"></a>Nächste Schritte

[Anzeigen Ihrer Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
