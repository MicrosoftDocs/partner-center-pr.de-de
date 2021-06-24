---
title: Installieren Partner Center Analytics für Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Führen Sie die Schritte in diesem Artikel aus, um die Partner Center Analytics-App für Power BI (für direkte Partner in CSP) zu installieren und eine Vorschau anzuzeigen.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ff95f989ac847bd2c17558d062c86a52110b2ddf
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565038"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI


**Geeignete Rollen**: Globaler Administrator | Benutzerverwaltungsadministrator | Vertriebsbeauftragter | Administrator-Agent

## <a name="before-you-begin"></a>Bevor Sie beginnen

Wählen Sie in der folgenden Liste der verfügbaren Microsoft Power BI-Apps die Anwendung aus, die für Ihr Unternehmen am relevantesten ist:

- [Direkter Anbieter](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Indirekter Anbieter](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Indirekter Wiederverkäufer](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Bevor Sie die Vorschauversion der Partner Center Analytics-App installieren, stellen Sie sicher, dass Sie die folgenden Anforderungen erfüllen.

- Sie haben die richtige Power BI-App für Ihr Unternehmen ausgewählt.

- Sie verfügen über Power BI Pro-Lizenz.

- Sie haben die Berechtigung, Vorlagen-Apps auf Ihrem Mandanten zu installieren.

- Sie können sich bei Power BI anmelden.

- Sie können sich als globaler Administrator, Administrator-Agent oder Abrechnungsadministrator beim [Azure Active Directory-Mandanten (Azure AD)](azure-active-directory-tenants-and-partner-center.md)Ihres Unternehmens anmelden.

## <a name="to-install-the-app"></a>So installieren Sie die App

1. Wählen Sie den Im obigen Abschnitt angegebenen Link für die App-Quelle (Direkter Anbieter/indirekter Anbieter/indirekter Wiederverkäufer) aus.

2. Wählen Sie **Jetzt herunterladen** aus. 

3. Stimmen Sie den Geschäftsbedingungen zu, indem Sie **Weiter auswählen.**

4. Wählen Sie unter Sie haben bereits ein Konto?**Anmelden** aus.

5. Geben Sie auf der nächsten Seite den Benutzernamen und das Kennwort für Power BI und wählen Sie dann **Anmelden** aus.

6. Installieren Sie den Arbeitsbereich, indem Sie den Namen des Arbeitsbereichs angeben.

7. Sie finden die installierten Vorlagen-Apps im Abschnitt Apps.

8. Wählen **Sie Apps** und dann die installierten Apps aus.

9. Los geht's mit dem Neuen App-Bildschirm wird geöffnet.

10. Wählen Sie Verbinden aus, um eine Verbindung mit den **Daten herzustellen.**

11. Überprüfen Sie **im Popupfenster** Mit Partner Center Analytics verbinden, ob die **Authentifizierungsmethode** auf **oAuth2** festgelegt ist, oder wählen Sie **oAuth2** aus der Liste aus, falls dies nicht der Reihe ist. 

> [!NOTE]  
>  Dieses Fenster erscheint möglicherweise erst nach einigen Minuten.

12. Melden Sie **sich auf der Partner Center Analytics Connector-Seite** mit den Anmeldeinformationen des globalen Administrators, Administrator-Agents oder Abrechnungsadministrators für den Azure AD-Mandanten Ihres Unternehmens an, und wählen Sie dann Anmelden **aus.**
 
13. Wählen Sie zum Zugriff aufgefordert werden, wählen Sie **Annehmen** aus. 

Sobald der Partner Center Analytics-Dienst mit Power BI verbunden ist, werden Daten geladen. Abhängig von der Datenmenge kann dies bis zu 10 Minuten in Anspruch nehmen. 

Nachdem die Daten geladen wurde, können Sie damit beginnen, das Partner Center Analytics-App-Dashboard und Berichte in Power BI zu nutzen.

## <a name="next-steps"></a>Nächste Schritte

[Anzeigen Ihrer Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
