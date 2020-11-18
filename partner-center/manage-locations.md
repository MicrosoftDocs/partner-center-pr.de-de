---
title: Verwalten von Standorten im Partnerkonto
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/15/2020
ms.locfileid: "92100770"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator
- Kontoadministrator

Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet. Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).

## <a name="the-following-is-a-typical-scenario"></a>Ein typisches Szenario:

Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich. Dies ist das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet. Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen. In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt. Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet. Auszahlungen sind an spezifische Standorte gebunden. 

>[!NOTE]
>Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Voraussetzungen für das Hinzufügen eines neuen Standorts für ein CSP-Geschäft

Zum Hinzufügen eines neuen CSP-Geschäftsstandorts müssen mehrere Voraussetzungen erfüllt sein:

1. Sie müssen über eine Standort-MPN-ID in dem Land/der Region verfügen, in dem/der Sie geschäftlich tätig sein möchten.

1. Sie benötigen einen neuen Azure AD-Mandanten in der [Geschäftsregion](regional-authorization-overview.md), der nicht bereits in CSP registriert ist. Erstellen Sie diesen bei der Registrierung in CSP.
 
3. Verwenden Sie den neuen AAD-Mandanten, um sich beim CSP-Programm in der Region zu registrieren.
Geben Sie rechtliche Firmendetails an, einschließlich des rechtsgültigen Firmennamens, der Adresse sowie Angaben zum primären Kontakt. Dieses Konto wird überprüft. Stellen Sie daher sicher, dass Sie gültige Informationen hinzufügen.

>[!NOTE] 
 >Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für den **neuen** Azure AD-Mandanten anzumelden. Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.

4. Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.

## <a name="add-an-mpn-location"></a>Fügen Sie einen Standort für das MPN hinzu.

1. Melden Sie sich mit dem MPN-Konto im Partner Center an. Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen. 

1. Wählen Sie das **Einstellungssymbol** und anschließend die **Partnereinstellungen** aus.

2. Wählen Sie **Standorte** aus.

3. Wählen Sie **Standort hinzufügen** aus, und fügen Sie die Adressdetails des Standorts ein, den Sie Ihrem Unternehmen hinzufügen möchten. Geben Sie auch einen Hauptansprechpartner für den Standort an.

> [!NOTE]
> In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden. Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.

## <a name="change-global-partner-account-location"></a>Ändern des globalen Partnerkontostandorts

1. Überprüfen Sie auf der Seite **[Standorte](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist. Wenn dies nicht der Fall ist, fügen Sie ihn hinzu.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Screenshot: Liste aller aktuellen Standorte auf der Seite mit den Standorten für Partner Center-Konten":::

2. Wählen Sie **Partnerprofil** aus, und wählen Sie dann **Firmenprofil aktualisieren** aus.

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Screenshot: Partner Center-Konto mit Informationen zum Partnerprofil und auswählbarer Aktualisierungsoption":::

3. Wählen Sie die Region und die juristische Entität aus, und klicken Sie auf **Senden**.

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Screenshot zum Aktualisieren des rechtlichen Geschäftsprofils des Partners einschließlich Dropdownlisten, über die das Land oder die Region und die juristische Person aktualisiert werden können":::

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).
