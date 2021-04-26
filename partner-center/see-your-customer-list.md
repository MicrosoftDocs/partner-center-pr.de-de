---
title: Ihre Kundenliste verwalten
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Kundendatensätze gehören zu den wichtigsten Informationsressourcen. Hier erfahren Sie, wie Sie Informationen in Ihrer & anzeigen, Partner Center aktualisieren und exportieren.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1791d415d0004520e8c7dc950decf540c91cf003
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002840"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Verwalten Ihrer Kundenliste– Suchen, Aktualisieren oder Exportieren von Kunden in Partner Center

**Zielgruppe**

- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Administrator-Agent
- Globaler Administrator

Kundendatensätze gehören zu den wichtigsten Informationsressourcen in Partner Center. Sie können Ihre Kundenkontendatenbank durchsuchen oder die gesamte Kundendatenbank bzw. eine Teilmenge in eine Excel-kompatible, durch Trennzeichen getrennte Datei (CSV-Datei) exportieren. Sie können auch Informationen zu Kundenabonnements in eine CSV-Datei exportieren.

Darüber hinaus enthalten die Aktivitätsprotokolle exportierbare Daten zu Transaktionen und Verwaltungsaktionen für Kunden. Weitere Informationen finden Sie unter [Kundenaktivitätsprotokolle anzeigen](activity-logs.md).

## <a name="search-for-a-customer"></a>Suchen nach einem Kunden

1. Wählen Sie **Partner Center** Menü Kunden **aus.**
2. Um nach einem Kunden zu suchen, geben Sie in das Suchfeld den Kundennamen oder den Domänennamen ein.
3. Wählen Sie den **Pfeil nach unten** am Ende einer Kundenzeile aus, um die Microsoft-ID des Kunden sowie die verknüpften Abonnements und Quicklinks zu Diensten anzuzeigen.

## <a name="update-a-customers-company-name"></a>Firmennamen von Kunden aktualisieren

Wählen Sie **Partner Center** Menü Kunden **aus.**
2. Um nach einem Kunden zu suchen, geben Sie in das Suchfeld den Kundennamen oder den Domänennamen ein.
3. Wählen Sie den **Pfeil nach unten** am Ende einer Kundenzeile aus, um die Microsoft-ID des Kunden sowie die verknüpften Abonnements und Quicklinks zu Diensten anzuzeigen.
4. Aktualisieren Sie in den Daten zum **Rechnungsempfänger** den Unternehmensnamen. Wenn Sie den neuen Wert speichern, wird er in die Kundenliste aufgenommen. Dadurch werden nur der Firmenname für die Rechnungsadresse und der Wert in der Kundenliste geändert. Anderswo werden die Änderungen nicht wiedergegeben.

## <a name="export-your-customer-list"></a>Exportieren der Kundenliste

1. Wählen Sie **Partner Center** Menü Kunden **aus.**
2. Wählen Sie **Kunden exportieren** aus.

   Partner Center konvertiert die gesamte Kundenliste in eine CSV-Datei und lädt sie in den Standarddownloadordner auf Ihrem Computer hoch. Sie können auch Teilmengen von Kundendaten exportieren. Zu den Datenspalten gehören u. a.:

   - **Microsoft-ID;**
   - **Firmenname;**
   - **Primärer Domänenname;**
   - **Beziehung** – die Geschäftsbeziehung des Partners zu den einzelnen aufgelisteten Kunden.

    Standardmäßig exportiert Partner Center die gesamte Kundenliste, unabhängig von der Länge. Sie können die Kundenliste auch nach dem Namen des Unternehmens oder der Domäne auflisten und diese Teilmenge von Daten exportieren.

3. Wenn Sie indirekter Anbieter sind, können Sie die Kundenliste nach indirekten Händlern filtern. Wählen Sie die Liste **Nach indirekten Händlern filtern** aus, und wählen Sie einen Händler aus.


## <a name="export-customer-subscription-information"></a>Exportieren von Informationen zum Kundenabonnement

1. Wählen Sie **Partner Center** Menü Kunden **aus.**

2. Wählen Sie den **Unternehmensnamen** eines Kunden aus. Die Seite **Abonnements** des Kunden wird geöffnet und zeigt die vollständige Liste der Produktabonnements an.

3. Wählen Sie **Abonnements exportieren** aus. Partner Center konvertiert die Abonnementdaten des Kunden in eine CSV-Datei und lädt sie in den Standarddownloadordner auf Ihrem Computer hoch. Zu den Datenspalten gehören u. a.:
   - **Abonnement-ID;**
   - **Abonnement** – der Produktname für das Abonnement;
   - **Menge** – die Anzahl der gekauften Lizenzen;
   - **Status**;
   - **Händler** – die ID des Händlers, der das Abonnement besitzt und verwaltet.

> [!NOTE]  
> Weitere Informationen zur Abonnementverwaltung finden Sie unter [Kundenabonnements](customer-subscriptions.md).
