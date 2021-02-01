---
title: Verwalten von Standorten im Partnerkonto
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098889"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts


**Geeignete Rollen**

- Globaler Administrator
- Kontoadministrator

Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet. Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).

## <a name="the-following-is-a-typical-scenario"></a>Ein typisches Szenario:

Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich. Dies ist das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet. Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen. In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt. Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet. Auszahlungen sind an spezifische Standorte gebunden. 

>[!NOTE]
>Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Voraussetzungen für das Hinzufügen eines neuen Kontos für ein CSP-Geschäft

Zum Hinzufügen eines neuen CSP-Geschäftskontos müssen Sie zunächst sicherstellen, dass die Voraussetzungen erfüllt sind.

1. Sie müssen über eine Standort-MPN-ID in dem Land verfügen, in dem Sie CSP-Geschäfte tätigen möchten. Wenn Sie einen neuen MPN-Standort erstellen möchten, lesen Sie „Hinzufügen eines MPN-Standorts“ weiter unten.
  
1. Wenn Sie eine neue CSP Indirect Reseller-Registrierung erstellen möchten, lesen Sie [Arbeiten mit indirekten Anbietern](indirect-reseller-tasks-in-partner-center.md#get-started). 

>[!NOTE] 
 >Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für das **neue** CSP-Konto anzumelden. Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.

2. Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.

## <a name="view-your-mpn-locations"></a>Anzeigen Ihrer MPN-Standorte

1. Melden Sie sich mit den Anmeldeinformationen für Ihr MPN-Konto beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home) an. (Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.) 
 
1. Wählen Sie über das Symbol **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Rechtliche Hinweise** aus. 

1. Vergewissern Sie sich, dass auf der Registerkarte **Partner** keine Fehlermeldung im Banner angezeigt wird, in der Sie dazu aufgefordert werden, von PMC migrierte Standorte zu korrigieren. Wenn dies der Fall ist, befolgen Sie die Anweisungen, und korrigieren Sie diese Standorte. 

3. Wird keine Fehlermeldung angezeigt, wählen Sie unter **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Bezeichner** aus.

4. Suchen Sie nach der MPN-ID mit dem Typ „Standort“, der dem Land dieses CSP-Kontos entspricht, und verwenden Sie sie für die folgende Suche und um die Zuordnung abzuschließen.

5. Wenn Sie die Standort-MPN-ID, die dem zu verwendenden CSP-Konto entspricht, nicht finden, können Sie einen neuen Standort hinzufügen, um eine neue MPN-ID zu erstellen. Weitere Informationen finden Sie im folgenden Abschnitt **Hinzufügen eines MPN-Standorts**.

## <a name="add-an-mpn-location"></a>Hinzufügen eines MPN-Standorts

1. Melden Sie sich mit dem MPN-Konto im Partner Center an. (Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.) Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen. 

1. Wählen Sie über das Symbol **Einstellungen** die **Kontoeinstellungen** und dann **Organisationsprofil** aus.

2. Wählen Sie **Rechtliche Hinweise** und dann auf der Registerkarte **Partner** die Option **Geschäftsstandorte** aus. Klicken Sie anschließend auf **Standort hinzufügen**.

3. Geben Sie die erforderlichen Details einschließlich Firmenname, Adresse und Ansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.
 
1. Klicken Sie auf **Standort hinzufügen**. Dadurch wird eine neue MPN-ID für den neuen Standort erstellt, die Sie für CSP-Transaktionen und -Incentives verwenden können.

:::image type="content" source="images/legal-biz.png" alt-text="Hinzufügen eines neuen Rechtsgeschäfts":::

> [!NOTE]
> In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden. Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.

## <a name="change-country-of-partner-global-account"></a>Ändern des Lands für das globale Partnerkonto 

1. Melden Sie sich mit dem MPN-Konto im Partner Center an. (Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.) Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen. 

2. Wechseln Sie auf der Registerkarte **Partner** zu **Geschäftsstandorte**, und prüfen Sie die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist. 
 
1. Zum Hinzufügen eines Standorts klicken Sie auf **Standort hinzufügen**, und geben Sie im Flyout die erforderlichen Details einschließlich Firmenname, Adresse und Hauptansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten. 
 
1. Wählen Sie neben der Dropdownliste **Land/Region** die Option **Land ändern** aus, und folgen Sie den angegebenen Schritten. 

:::image type="content" source="images/lbp.png" alt-text="Flyout mit Daten des Rechtsgeschäftsprofils":::

5. Klicken Sie auf **Speichern**.

6. Das Land des globalen MPN-Kontos wird in das neue rechtsgültige Land geändert.
  
## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).
