---
title: Verkaufen von Angeboten an Education-Kunden
description: Erfahren Sie, wie Sie einen Education-Kunden erstellen und angebotene Angebote in Partner Center. Umfasst die Bestätigung des Überprüfungsstatus für Ihren Education-Kunden.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b1b89841faf77a78c8cc268357daaaf95307223
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855402"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Verkaufen von Angeboten an Education-Kunden und Erstellen eines Education-Kunden in Partner Center

**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent| Vertriebs-Agent

## <a name="create-an-education-customer"></a>Erstellen eines Education-Kunden

In diesem Artikel wird erläutert, wie Sie einen Education-Kunden in Partner Center und ihnen Education-Produkte verkaufen. Außerdem erfahren Sie, wie Sie den Überprüfungsstatus anzeigen und die Überprüfungsanforderung bei Bedarf erneut senden. Education-Angebote sind **derzeit nur für lizenzbasierte** Dienste wie Microsoft 365, Dynamics, Intune usw. verfügbar. Es ist nicht für andere Typen (Softwareabonnements, unbefristete Software oder Azure-Produkte) verfügbar.

> [!IMPORTANT]
> Microsoft überprüft jeden neu erstellten Education-Kunden-Mandanten, um sicherzustellen, dass er für Education-Angebote qualifiziert ist.  Stellen Sie sicher, dass Sie die erforderlichen Informationen so genau und vollständig wie möglich eingeben, um Verzögerungen beim Überprüfungsprozess zu vermeiden.

1. Melden Sie sich bei Partner Center an.

2. Wählen **Sie Kunden** und dann Kunden hinzufügen **aus.** Wählen **Sie in der** **Dropdownliste Spezielle Qualifikationen die Option** Bildung aus.  Geben Sie die restlichen Kontoinformationen nach Bedarf ein.  Zu den wichtigsten Feldern, die den Überprüfungsprozess unterstützen, gehören:

   - **Firmenname:** GEBEN SIE LEGAL ENTITY NAME ein – Erforderlich für die Überprüfung.
   - **Land/Region und Adresszeilen:** GEBEN SIE FULL ENTITY MAILING ADDRESS ein – für die Überprüfung erforderlich.
   - **E-Mail-Adresse:** Geben Sie die E-Mail-Adresse im Besitz der Entität ein ( keine kostenlose oder on.microsoft.com-E-Mail), die für die Überprüfung erforderlich ist.
   - **Kundenkontaktinformationen:** Diese Details werden im Rahmen des Überprüfungsprozesses verwendet.
   - **Primärer Domänenname:** Wird zum Erstellen des Kontos und der E-Mail-Adressen des Kunden verwendet.  Wählen Sie einen Namen aus, der dem Firmennamen ohne Leerzeichen oder Sonderzeichen ähnelt.  Dieser Name kann später nicht mehr geändert werden.

3. Wenn Sie fertig sind, wählen Sie **Überprüfen** aus.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Education-Kundenkonto":::

4. Nach dem Bestätigen von **Überprüfen** erhalten Sie den **Status InReview,** wenn die übermittelten Informationen gültig sind. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Kundenkonto für Bildungseinrichtungen in Überprüfung"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Bestätigen des Überprüfungsstatus Ihres Education-Kunden

Auf der Seite **Konto** des Kunden finden Sie weitere Informationen unter **Spezieller Qualifizierungsstatus.**
Statusbeispiele:

- Wenn der Kunde die Überprüfung bestanden hat: Education

   :::image type="content" source="images/edupassedvetting.png" alt-text="Überprüfung des Bildungsbereichs war erfolgreich":::

- Wenn der Kunde die Überprüfung nicht bestanden hat: Kein Bildungskunde

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Überprüfung der Bildungseinrichtungen war nicht erfolgreich" lightbox="images/edu/fail-reason-expanded.png":::

- Wenn der Kunde nicht als Education-Kunde gekennzeichnet wurde: Keine

   :::image type="content" source="images/edu/account-one.png" alt-text="Education-Kunde ist nicht als solche gekennzeichnet" lightbox="images/edu/account-one-expanded.png":::

- Wenn der Kunde als Education-Kunde überprüft wird: In Review

    :::image type="content" source="images/edu/in-review.png" alt-text="Education-Kunde wird überprüft" lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Korrigieren Sie die Kundenkontoinformationen, und senden Sie sie zur Überprüfung erneut.

Wenn Ihr Kunde bei der ersten Überprüfung fehlschlägt, können Sie die Informationen jetzt korrigieren und erneut übermitteln.

### <a name="correct-the-customer-account-information"></a>Korrigieren von Kundenkontoinformationen

Sie benötigen globale Administratorrechte, um die Informationen des Kunden zu aktualisieren. Sie aktualisieren die Informationen im Office 365-Portal, da diese Daten nicht über das Partner Center-Portal aktualisiert werden können.

1. Auf der **Seite** Konto werden Informationen angezeigt, die angeben, dass die Qualifikation des Kunden als "Kein Bildungskunde" betrachtet wird.

2. Aktualisieren Sie Ihren Browser, um die Seite zurückzusetzen. Es wird eine Schaltfläche **Aktualisieren angezeigt,** und **der Status der speziellen** Qualifikation ist auf **Keine festgelegt.**

3. Wählen Sie **Aktualisieren** aus. Wählen Sie **auf der Seite Dienstverwaltung** die Option **Office 365 aus.**

4. Sie werden auf einer neuen Registerkarte Ihres Browsers zum Office 365 Admin Center umgeleitet. Möglicherweise werden Sie aufgefordert, sich mit Ihren Anmeldeinformationen anzumelden.

5. Wählen Sie **Einstellungen** aus.

6. Wählen Sie **oben auf dem** Bildschirm die Registerkarte Organisationsprofil und dann **Organisationsinformationen aus.** Sie können jetzt die Kundendetails aktualisieren.

7. Wählen **Sie unten auf** der Randleiste Save changes (Änderungen speichern) aus.  

### <a name="resubmit-for-verification"></a>Erneutes Senden zur Überprüfung

1. Navigieren Sie zur Registerkarte Partner Center Und  zur Seite Kundenkonto. Aktualisieren Sie den Browser, und vergewissern Sie sich, dass die Unternehmensseite auf die neuen Informationen aktualisiert wurde. Wählen Sie **die Schaltfläche** Aktualisieren aus, um eine erneute Überprüfung des Bildungsbereichs an fordern.

2. Wenn die aktualisierten Kundendetails für Education-Angebote geeignet sind, werden die **speziellen Qualifikationen** in **Education aktualisiert.** Wenn "Kein Education-Kunde" **weiterhin zu sehen ist,** wenden Sie sich zur manuellen Überprüfung an den Support.

## <a name="next-steps"></a>Nächste Schritte

- [Verkaufen an spezielle Branchen](get-special-pricing-for-offers.md)

- [Hinzufügen neuer Kunden](add-a-new-customer.md)

- [Verkaufen Minecraft: Education Edition Abonnements an Education-Kunden](minecraft-subscriptions.md)
