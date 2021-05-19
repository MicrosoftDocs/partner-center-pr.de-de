---
title: Informationen Partner Center Abrechnungsrechnungen
ms.topic: article
ms.date: 05/18/2020
description: Machen Sie sich mit den Feldern in Ihrer Rechnungsdatei für Partner Center Abrechnung aus. Enthalten sind Felder und Definitionen für alle Rechnungsfelder und Felder für einmalige Gebühren.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146611"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Verstehen Partner Center Abrechnungsrechnungsfeldern

**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Abrechnungsadministrator| Helpdesk-Agent

Sie können die folgenden Tabellen verwenden, um die Felder in den Partner Center zu verstehen.

## <a name="invoice-file-fields"></a>Felder der Rechnungsdatei

Die folgenden Felder werden in Ihren Rechnungsdateien angezeigt.

| Feld | Definition |
| ----- | ---------- |
| US FEIN | Ihre Personalidentifikationsnummer (Federal Identification Number, FEIN). Dies ist Ihre USA steuerbezeichnernummer. |
| Kundennummer | Ihre Kundennummer |
| Bill to | Die Adresse, an die wir Ihre Rechnung senden. Sie können den Namen und die Adresse Ihres Unternehmens in Ihrem Partner Center ändern. |
| Lizenzbasierte Gebühren | Die monatlichen oder jährlichen Pauschalgebühren für Ihre erworbenen nutzungsbasierten Lizenzen, die im Voraus abgerechnet werden. Diese Zahl ist die Summe aller Gebühren in der Spalte **Teilsumme** (Spalte **T)** in Ihrer lizenzbasierten Abstimmungsdatei. |
| Nutzungsbasierte Gebühren | Ihre Azure-Nutzung. Dies schließt neue Dienste oder Anwendungen ein, die während des Abrechnungszeitraums aktiviert und verwendet werden. Diese Zahl ist die Summe aller Gebühren in der **Spalte PretaxCharges** (Spalte **Z)** in Ihrer nutzungsbasierten Abstimmungsdatei. |
| Discounts | Der Rabatt, den der Kunde vom Normalpreis des Abonnements erhält. Diese Zahl wird als Pauschalbetrag *und* nicht als Preis pro Einheit oder Lizenz angezeigt. |
| Mitwirkende | Gutschriften oder Anpassungen für Änderungen an Abonnements (z. B. Lizenzerhöhungen oder -verringerungen). |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern und Gebühren und Guthaben exklusive Steuern |
| Tax (Steuern) | Die Gesamtsteuer für Ihre aktuellen Gebühren, die im Abschnitt **Details** ab Seite 2 Ihrer Rechnung enthalten ist. Diese Zahl ist die Summe aller Gebühren in der Spalte **TaxAmount** (Spalte **AA**) in Ihrer nutzungsbasierten Abstimmungsdatei und die **Spalte Tax** (Spalte **U**) in Ihrer lizenzbasierten Abstimmungsdatei. |
| Andere Guthaben | Guthaben exklusive Steuern |
| Aktuelle Gebühren insgesamt | Der in Ihrer Abrechnungswährung für den Abrechnungszeitraum fällige Betrag. Diese Gebühren sind am Fälligkeitsdatum der Zahlung fällig. |
| Payment Instructions | Beschreibung der Zahlung Ihrer Rechnung basierend auf Ihrer Region. *Achten Sie bei einer Zahlung immer darauf, Dass Sie Ihre Rechnungsnummer angeben.* |
| Rechnungsnummer | Die Nummer Ihrer Rechnung. |
| Abrechnungszeitraum | Der monatliche Zeitraum bis zum Rechnungsdatum. Dies ist der Zeitraum, in dem nutzungsbasierte Dienste verbraucht und lizenzbasierte Dienste auf Guthabenanpassungen oder Änderungen in der Lizenzanzahl abgestimmt werden. |
| Invoice Date | Das Abrechnungsdatum oder das Jahrestag, an dem Ihre Rechnung jeden Monat generiert wird. |
| Zahlungsbedingungen | Die Zahlungsfrist. Für einmalige Einkäufe wird dies immer 60 Tage sein. |
| Fälligkeitsdatum der Zahlung | Das Datum, an dem Ihre Zahlung empfangen werden muss. |
| Bestellnr. des Kunden | Ihre Bestellnummer. |
| Kundendienst | Die Websiteadresse, unter der Sie auf den Kundendienst zugreifen können. |
| Dienstempfänger | Die Adresse, an der der Dienst verwendet wird. (Dies ist die rechtlich gültige Unternehmensadresse. Sie ist mit der Unternehmensprüfung verknüpft.) |

## <a name="one-time-charges-fields"></a>Felder für einmalige Gebühren

Die folgenden Felder gelten nur für **einmalige Gebühren** in Partner Center:

| Feld | Definition |
| ----- | ---------- |
| Date | Kaufdatum. |
| Beschreibung | Produktname |
| Menge | Die Anzahl der erworbenen Produkte (z. B. Reservierungen). |
| Unit price | Preis pro Produkt (z. B. eine Reservierung). |
| Discounts | Alle anwendbaren Rabatte. |
| Vorsteuerbetrag | Teilsumme der Käufe vor Steuern. |
| Mehrwertsteuer | Steuerbetrag. |
| Gesamt | Der zu zahlende Gesamtbetrag. |
