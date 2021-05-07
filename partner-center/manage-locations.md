---
title: Verwalten von Standorten im Partnerkonto
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702891"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Verwalten von MPN-Kontostandorten und Hinzufügen (Löschen) eines Standorts


**Geeignete Rollen**

- Globaler Administrator
- Kontoadministrator

Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet. Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).

## <a name="the-following-scenario-is-typical"></a>Hier ein typisches Szenario:

Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich. Bei dem PGA handelt es sich um das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet. Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen. In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt. Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet. Auszahlungen sind an spezifische Standorte gebunden. 

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

1. Wenn Sie sich als Partner mit direkter Abrechnung registrieren möchten, lesen Sie die [Anforderungen für Partner mit direkter Abrechnung](direct-partner-new-requirements.md).

## <a name="view-and-update-your-mpn-locations"></a>Anzeigen und Aktualisieren Ihrer MPN-Standorte

1. Melden Sie sich mit den Anmeldeinformationen für Ihr MPN-Konto beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home) an. (Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.) 
 
1. Wählen Sie über das Symbol **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Rechtliche Hinweise** aus. 

1. Vergewissern Sie sich, dass auf der Registerkarte **Partner** keine Fehlermeldung im Banner angezeigt wird, in der Sie dazu aufgefordert werden, von PMC migrierte Standorte zu korrigieren.  Wenn Ihre Standorte in PMC nicht ordnungsgemäß eingerichtet wurden und noch nicht in PC übergegangen sind, müssen Sie diese Standorte aktualisieren.

:::image type="content" source="images/locations/location-two.png" alt-text="Screenshot zum Aktualisieren des Standorts":::
 
4.  Wählen Sie im Bildschirm **PMC-Standorte überprüfen** die Option **Aktualisieren** aus.
Aktualisieren Sie die folgenden Felder:

- **Feld „Name“** : Stellen Sie sicher, dass der Name des Unternehmensstandorts korrekt ist. Wenn ein Duplikatfehler angezeigt wird, versuchen Sie, den Wert z. B. von „Contoso“ in „Contoso, Inc“ zu ändern.

- **Feld „Juristische Entität“** : Stellen Sie sicher, dass Sie die juristische Entität ausgewählt haben, an die der Standort gebunden ist.

- **Felder „Adresszeile 1“ und „Adresszeile 2“** : Vergewissern Sie sich, dass die Adresse richtig ist.

- **Felder „Stadt“ und „Bundesland/Kanton“** : Stellen Sie sicher, dass die Kombination von Stadt und Bundesland/Kanton richtig ist. Es gibt Länder, bei denen das Dropdownmenü zur Auswahl des Bundeslands/Kantons verwendet wird. Bei anderen Ländern muss der Eintrag in das Feld manuell erfolgen.

- **Feld „Postleitzahl“** : Stellen Sie sicher, dass das Feld für die Postleitzahl mit dem jeweiligen Land, der Region, der Stadt oder der Adresse übereinstimmt.

- **Felder für Informationen zum Hauptansprechpartner**: Stellen Sie sicher, dass die Felder für den Vor- und Nachnamen ausgefüllt sind und dass es sich bei der geschäftlichen E-Mail-Adresse nicht um eine private Adresse handelt (z. B. @outlook.com, @live.com usw.).

- **Feld „Telefonnummer“** : Vergewissern Sie sich, dass die Telefonnummer keine Sonderzeichen, Leerzeichen oder die Landeskennzahl enthält. Der im Feld „Telefonnummer“ eingegebene Wert umfasst immer maximal zehn Zeichen.

5. Wird keine Fehlermeldung angezeigt, wählen Sie unter **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Bezeichner** aus.

6. Suchen Sie nach der MPN-ID mit dem Typ „Standort“, der dem Land dieses CSP-Kontos entspricht, und verwenden Sie diese, um die Zuordnung abzuschließen.

7. Wenn Sie die Standort-MPN-ID, die dem zu verwendenden CSP-Konto entspricht, nicht finden, können Sie einen neuen Standort hinzufügen, um eine neue MPN-ID zu erstellen. Weitere Informationen finden Sie im folgenden Abschnitt **Hinzufügen eines MPN-Standorts**.

## <a name="add-an-mpn-location"></a>Hinzufügen eines MPN-Standorts

1. Melden Sie sich mit dem MPN-Konto im Partner Center an. (Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.) Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen. 

1. Wählen Sie über das Symbol **Einstellungen** die **Kontoeinstellungen** und dann **Organisationsprofil** aus.

2. Wählen Sie **Rechtliche Hinweise** und dann auf der Registerkarte **Partner** die Option **Geschäftsstandorte** aus. Klicken Sie anschließend auf **Standort hinzufügen**.

3. Geben Sie die erforderlichen Details einschließlich Firmenname, Adresse und Ansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.
 
1. Klicken Sie auf **Standort hinzufügen**. Dadurch wird eine neue MPN-ID für den neuen Standort erstellt, die Sie für CSP-Transaktionen und -Incentives verwenden können.

:::image type="content" source="images/legal-biz.png" alt-text="Hinzufügen eines neuen Rechtsgeschäfts":::

> [!NOTE]
> In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden. Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.

## <a name="add-the-registration-number-id"></a>Hinzufügen der Registrierungs-ID

Wenn Sie ein indirekter Anbieter, Partner mit direkter Abrechnung oder indirekter Wiederverkäufer sind und Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern tätigen, müssen Sie Registrierungs-IDs für Ihr Unternehmen bereitstellen. Ist das Land, in dem Sie geschäftlich tätig sind, nachfolgend nicht aufgelistet, ist die Angabe der Registrierungs-ID optional.

- Armenien 
- Aserbaidschan 
- Belarus 
- Brasilien 
- Ungarn 
- Indien 
- Irak 
- Kasachstan 
- Kirgisistan 
- Moldawien 
- Myanmar 
- Polen 
- Russland 
- Saudi-Arabien 
- Südafrika 
- Südsudan  
- Tadschikistan 
- Thailand
- Türkei 
- Ukraine 
- Vereinigte Arabische Emirate 
- Usbekistan 
- Venezuela
- Vietnam 


Weitere Informationen finden Sie unter [Informationen zur Registrierungs-ID](reg-number-id.md).

## <a name="delete-a-location"></a>Löschen eines Standorts

Um einen Standort aus Ihrem Konto zu löschen, müssen Sie sich an den [Partner-Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) wenden. Vergewissern Sie sich, dass Ihnen die Auswirkungen dieser Aktion bekannt sind. Gelöschte Standorte können nicht abgerufen werden, und alle Elemente, die mit dieser bestimmten MPN-ID verknüpft sind, werden nicht mehr erkannt oder sind für Ihr Unternehmen nicht mehr aktiv.

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
