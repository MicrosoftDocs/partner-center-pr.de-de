---
title: Rechnungs Dateien | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Machen Sie sich mit den Feldern in der Rechnungs Datei für die Partner Center-Abrechnung vertraut.
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
keywords: Abrechnung, Rechnung
ms.localizationpriority: medium
ms.openlocfilehash: 1307a9a2f95cedde5eda7deefb61cb202597f804
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390909"
---
# <a name="invoice-files"></a>Rechnungs Dateien

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Abrechnungsadministrator
-   Helpdesk-Agent

Anhand der folgenden Tabellen können Sie die Felder in den Partner Center-Rechnungs Dateien verstehen.

## <a name="invoice-file-fields"></a>Felder der Rechnungs Datei

Die folgenden Felder werden in den Rechnungs Dateien angezeigt.

| Field | Definition |
| ----- | ---------- |
| US FEIN | Ihre Federal Employer Identification Number (fein). Dies ist Ihre USA Federal Tax Identifier-Nummer. |
| Kundennummer | Ihre Kundennummer. |
| Rechnungsempfänger | Die Adresse, an die wir Ihre Rechnung senden. Sie können Ihren Firmennamen und/oder Ihre Adresse in Ihrem Partner Center-Abrechnungs Profil ändern. |
| Lizenzbasierte Gebühren | Die pauschalen monatlichen oder jährlichen Gebühren für Ihre erworbenen nutzungsbasierten Lizenzen, die im Voraus in Rechnung gestellt werden. Diese Zahl ist die Summe aller Gebühren in der **Teil** Ergebnisspalte (Spalte **T**) in der lizenzbasierten Abstimmungs Datei. |
| Nutzungsbasierte Gebühren | Ihre Azure-Nutzung. Dies schließt neue Dienste oder Anwendungen ein, die während des Abrechnungszeitraums aktiviert und verwendet werden. Diese Zahl ist die Summe aller Gebühren in der Spalte **pretaxcharges** (Spalte **Z**) in der nutzungsbasierten Abstimmungs Datei. |
| Rabatte | Der Rabatt, den der Kunde vom normalen Preis des Abonnements erhält. Diese Zahl wird als *Pauschalbetrag*, nicht als Preis pro Einheit oder Lizenz angezeigt. |
| Guthaben | Gutschriften oder Anpassungen für Änderungen an Abonnements (z. b. erhöhen oder verringern des Arbeitsplatzes). |
| Zwischensumme | Gesamtbetrag vor Steuern und Gebühren und Guthaben exklusive Steuern |
| Tax | Die Gesamt steuersumme für Ihre aktuellen Gebühren, wie im Abschnitt " **Details** " beginnend mit Seite 2 Ihrer Rechnung. Dabei handelt es sich um die Summe aller Gebühren in der Spalte " **taxAmount** " (Spalte **AA**) in der nutzungsbasierten Abstimmungs Datei und die Spalte " **Tax** " (Spalte **U**) in der lizenzbasierten Abstimmungs Datei. |
| Andere Guthaben | Guthaben exklusive Steuern |
| Gesamtsumme der aktuellen Gebühren | Der Betrag, der in ihrer Abrechnungswährung für den Abrechnungszeitraum fällig ist. Diese Gebühren sind auf das Fälligkeitsdatum der Zahlung zurückzuführen. |
| Zahlungsanweisungen | Beschreibung der Zahlung Ihrer Rechnung basierend auf Ihrer Region. *Stellen Sie bei einer Zahlung immer sicher, dass Sie Ihre Rechnungsnummer einschließen.* |
| Rechnungsnummer | Die Nummer Ihrer Rechnung. |
| Abrechnungszeitraum | Der monatliche Zeitraum bis zum Rechnungsdatum. Dies ist der Zeitraum, in dem nutzungsbasierte Dienste verbraucht und lizenzbasierte Dienste auf Guthabenanpassungen oder Änderungen in der Lizenzanzahl abgestimmt werden. |
| Rechnungsdatum | Das Abrechnungsdatum oder das Enddatum, an dem Ihre Rechnung monatlich generiert wird. |
| Zahlungsbedingungen | Der Zahlungs Begriff. Für einmalige Einkäufe wird dies immer 60 Tage sein. |
| Fälligkeitsdatum der Zahlung | Das Datum, an dem Ihre Zahlung empfangen werden muss. |
| Name des Kunden | Ihre Bestellnummer. |
| Kundendienst | Die Adresse der Website, auf die Sie auf den Kundendienst zugreifen können. |
| Dienstempfänger | Die Adresse, unter der der Dienst verwendet wird. (Dies ist die rechtlich gültige Unternehmensadresse. Sie ist mit der Unternehmensprüfung verknüpft.) |

## <a name="one-time-charges-fields"></a>Felder mit einer einmaligen Gebühr

Die folgenden Felder gelten nur für **einmalige Gebühren** in Partner Center:

| Field | Definition |
| ----- | ---------- |
| Date | Kaufdatum. |
| Beschreibung | Produktname. |
| Menge | Die Anzahl erworbener Produkte (z. b. Reservierungen). |
| Preis pro Einheit | Preis pro Produkt (z. b. eine Reservierung). |
| Rabatte | Alle anwendbaren Rabatte. |
| Vorsteuerbetrag | Zwischensumme vor Steuern. |
| Mehrwertsteuer | Steuerbetrag |
| Gesamt | Der Gesamtbetrag, der bezahlt werden soll. |
