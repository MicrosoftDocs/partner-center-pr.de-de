---
title: Verstehen der Felder in Abrechnungs Rechnungen
ms.topic: article
ms.date: 05/18/2020
description: Machen Sie sich mit den Feldern in der Rechnungs Datei für die Partner Center-Abrechnung vertraut.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 72b8abc1edb4e27b4c9677cc9f374af2aff25986
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434529"
---
# <a name="partner-center-billing-invoices---learn-how-to-read-the-billing-and-one-time-charge-fields"></a>Abrechnungs Rechnungen für Partner Center: erfahren Sie, wie Sie die Abrechnungs-und einzeitangabefelder lesen.

**Geeignete Rollen**

- Globaler Administrator
- Benutzeradministrator
- Abrechnungsadministrator
- Helpdesk-Agent

Anhand der folgenden Tabellen können Sie die Felder in den Partner Center-Rechnungs Dateien verstehen.

## <a name="invoice-file-fields"></a>Felder der Rechnungs Datei

Die folgenden Felder werden in den Rechnungs Dateien angezeigt.

| Feld | Definition |
| ----- | ---------- |
| US FEIN | Ihre Federal Employer Identification Number (fein). Dies ist Ihre USA Federal Tax Identifier-Nummer. |
| Kundennummer | Ihre Kundennummer |
| Bill to | Die Adresse, an die wir Ihre Rechnung senden. Sie können Ihren Firmennamen und/oder Ihre Adresse in Ihrem Partner Center-Abrechnungs Profil ändern. |
| Lizenzbasierte Gebühren | Die pauschalen monatlichen oder jährlichen Gebühren für Ihre erworbenen nutzungsbasierten Lizenzen, die im Voraus in Rechnung gestellt werden. Diese Zahl ist die Summe aller Gebühren in der **Teil** Ergebnisspalte (Spalte **T**) in der lizenzbasierten Abstimmungs Datei. |
| Nutzungsbasierte Gebühren | Ihre Azure-Nutzung. Dies schließt neue Dienste oder Anwendungen ein, die während des Abrechnungszeitraums aktiviert und verwendet werden. Diese Zahl ist die Summe aller Gebühren in der Spalte **pretaxcharges** (Spalte **Z**) in der nutzungsbasierten Abstimmungs Datei. |
| Discounts | Der Rabatt, den der Kunde vom normalen Preis des Abonnements erhält. Diese Zahl wird als *Pauschalbetrag*, nicht als Preis pro Einheit oder Lizenz angezeigt. |
| Guthaben | Gutschriften oder Anpassungen für Änderungen an Abonnements (z. b. erhöhen oder verringern des Arbeitsplatzes). |
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
| Vorsteuerbetrag | Zwischensumme der Einkäufe vor Steuern. |
| Mehrwertsteuer | Steuerbetrag. |
| Gesamt | Der Gesamtbetrag, der bezahlt werden soll. |
