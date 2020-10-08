---
title: Verwalten von Standorten im Partnerkonto
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663895"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator
- Kontoadministrator

Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet. Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).

## <a name="the-following-is-a-typical-scenario"></a>Ein typisches Szenario:

Contoso hat seinen globalen Partnerkontostandort (Partner Global Account, PGA) im Vereinigten Königreich. Dies ist das registrierte Unternehmen, das über eine einzelne MPN-ID verfügt, die für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet wird. Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen. In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt. Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet. Auszahlungen sind an spezifische Standorte gebunden. 

>[!NOTE]
>Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Voraussetzungen für das Hinzufügen eines neuen Standorts für ein CSP-Geschäft

Zum Hinzufügen eines neuen CSP-Geschäftsstandorts müssen mehrere Voraussetzungen erfüllt sein:

1. Sie müssen über eine Standort-MPN-ID in dem Land verfügen, in dem Sie geschäftlich tätig sein möchten.

1. Sie benötigen einen neuen Azure AD-Mandanten in der Geschäftsregion, der nicht bereits in CSP registriert ist. Erstellen Sie diesen bei der Registrierung in CSP.
 
3. Verwenden Sie den neuen AAD-Mandanten, um sich beim CSP-Programm in der Region zu registrieren.
Geben Sie rechtliche Firmendetails an, einschließlich des rechtsgültigen Firmennamens, der Adresse sowie Angaben zum primären Kontakt. Dieses Konto wird überprüft. Stellen Sie daher sicher, dass Sie gültige Informationen hinzufügen.

>[!NOTE] 
 >Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für den **neuen** Azure AD-Mandanten anzumelden. Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.

4. Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.

## <a name="add-a-location"></a>Hinzufügen eines Standorts

1. Wählen Sie das **Einstellungssymbol** und anschließend die **Partnereinstellungen** aus.

2. Wählen Sie **Standorte** aus.

3. Wählen Sie **Standort hinzufügen** aus.  

4. Fügen Sie auf der Seite **Standort hinzufügen** die Adressdetails des Standorts ein, den Sie Ihrem Unternehmen hinzufügen möchten, und geben Sie auch einen Hauptansprechpartner für den Standort an.

> [!NOTE]
> In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden.

## <a name="change-global-partner-account-location"></a>Ändern des globalen Partnerkontostandorts

1. Überprüfen Sie auf der Seite **Standorte** die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist. Wenn dies nicht der Fall ist, fügen Sie ihn hinzu.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Struktur von MPN-Standorten":::

2. Wählen Sie **Partnerprofil** aus, und wählen Sie dann **Firmenprofil aktualisieren** aus.

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Struktur von MPN-Standorten":::

3. Wählen Sie die Region und die juristische Entität aus, und klicken Sie auf **Senden**.

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Struktur von MPN-Standorten":::

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).
