---
title: Verstehen der Abrechnungs Rechnungen von Partner Center
ms.topic: article
ms.date: 05/18/2020
description: Machen Sie sich mit den Feldern in der Rechnungs Datei für die Partner Center-Abrechnung vertraut. Enthaltene Felder und Definitionen für alle Rechnungs Felder und die Felder für die einmalige Abrechnung.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44bda5256b14722f143a5bf937e73b2533b8c9f5
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178900"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Informationen zu den Feldern der Partner Center-abrechnungsrechnung

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Abrechnungsadministrator
- Helpdesk-Agent

Anhand der folgenden Tabellen können Sie die Felder in den Partner Center-Rechnungs Dateien verstehen.

## <a name="invoice-file-fields"></a>Felder der Rechnungs Datei

Die folgenden Felder werden in den Rechnungs Dateien angezeigt.

| Feld | Definition |
| ----- | ---------- |
| US FEIN | Ihre Federal Employer Identification Number (fein). Dies ist Ihre USA Federal Tax Identifier-Nummer. |
| Kundennummer | Ihre Kundennummer |
| Bill to | Die Adresse, an die wir Ihre Rechnung senden. Sie können den Namen und die Adresse Ihres Unternehmens in Ihrem Partner Center-Abrechnungs Profil ändern. |
| Lizenzbasierte Gebühren | Die pauschalen monatlichen oder jährlichen Gebühren für Ihre erworbenen nutzungsbasierten Lizenzen, die im Voraus in Rechnung gestellt werden. Diese Zahl ist die Summe aller Gebühren in der **Teil** Ergebnisspalte (Spalte **T**) in der lizenzbasierten Abstimmungs Datei. |
| Nutzungsbasierte Gebühren | Ihre Azure-Nutzung. Dies schließt neue Dienste oder Anwendungen ein, die während des Abrechnungszeitraums aktiviert und verwendet werden. Diese Zahl ist die Summe aller Gebühren in der Spalte **pretaxcharges** (Spalte **Z**) in der nutzungsbasierten Abstimmungs Datei. |
| Discounts | Der Rabatt, den der Kunde vom normalen Preis des Abonnements erhält. Diese Zahl wird als *Pauschalbetrag*, nicht als Preis pro Einheit oder Lizenz angezeigt. |
| Mitwirkende | Gutschriften oder Anpassungen für Änderungen an Abonnements (z. b. zum erhöhen oder verringern der Lizenz). |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern und Gebühren und Guthaben exklusive Steuern |
| Tax (Steuern) | Die Gesamt steuersumme für Ihre aktuellen Gebühren, wie im Abschnitt " **Details** " beginnend mit Seite 2 Ihrer Rechnung. Dabei handelt es sich um die Summe aller Gebühren in der Spalte " **taxAmount** " (Spalte **AA**) in der nutzungsbasierten Abstimmungs Datei und die Spalte " **Tax** " (Spalte **U**) in der lizenzbasierten Abstimmungs Datei. |
| Andere Guthaben | Guthaben exklusive Steuern |
| Aktuelle Gebühren insgesamt | Der Betrag, der in ihrer Abrechnungswährung für den Abrechnungszeitraum fällig ist. Diese Gebühren sind auf das Fälligkeitsdatum der Zahlung zurückzuführen. |
| Payment Instructions | Beschreibung der Zahlung Ihrer Rechnung basierend auf Ihrer Region. *Stellen Sie bei einer Zahlung immer sicher, dass Sie Ihre Rechnungsnummer einschließen.* |
| Rechnungsnummer | Die Nummer Ihrer Rechnung. |
| Abrechnungszeitraum | Der monatliche Zeitraum bis zum Rechnungsdatum. Dies ist der Zeitraum, in dem nutzungsbasierte Dienste verbraucht und lizenzbasierte Dienste auf Guthabenanpassungen oder Änderungen in der Lizenzanzahl abgestimmt werden. |
| Invoice Date | Das Abrechnungsdatum oder das Enddatum, an dem Ihre Rechnung monatlich generiert wird. |
| Zahlungsbedingungen | Der Zahlungs Begriff. Für einmalige Einkäufe wird dies immer 60 Tage sein. |
| Fälligkeitsdatum der Zahlung | Das Datum, an dem Ihre Zahlung empfangen werden muss. |
| Bestellnr. des Kunden | Ihre Bestellnummer. |
| Kundendienst | Die Adresse der Website, auf die Sie auf den Kundendienst zugreifen können. |
| Dienstempfänger | Die Adresse, unter der der Dienst verwendet wird. (Dies ist die rechtlich gültige Unternehmensadresse. Sie ist mit der Unternehmensprüfung verknüpft.) |

## <a name="one-time-charges-fields"></a>Felder mit einer einmaligen Gebühr

Die folgenden Felder gelten nur für **einmalige Gebühren** in Partner Center:

| Feld | Definition |
| ----- | ---------- |
| Date | Kaufdatum. |
| BESCHREIBUNG | Produktname |
| Menge | Die Anzahl erworbener Produkte (z. b. Reservierungen). |
| Unit price | Preis pro Produkt (z. b. eine Reservierung). |
| Discounts | Alle anwendbaren Rabatte. |
| Vorsteuerbetrag | Teil Summe der Käufe vor Steuern. |
| Mehrwertsteuer | Steuerbetrag. |
| Gesamt | Der Gesamtbetrag, der bezahlt werden soll. |
