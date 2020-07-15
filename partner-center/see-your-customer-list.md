---
title: Ihre Kundenliste verwalten
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Kundendaten Sätze gehören zu den wichtigsten Informationsressourcen. Erfahren Sie, wie Sie Informationen in ihrer Partner Center-Kundenliste anzeigen, suchen, aktualisieren und & exportieren.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 865af6a054fc10cddd5422e1ef91ec3df14f69aa
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377744"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Verwalten der Kundenliste: suchen, aktualisieren oder Exportieren von Kunden im Partner Center

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

Kundendatensätze gehören zu den wichtigsten Informationsressourcen in Partner Center. Sie können Ihre Kundenkontendatenbank durchsuchen oder die gesamte Kundendatenbank bzw. eine Teilmenge in eine Excel-kompatible, durch Trennzeichen getrennte Datei (CSV-Datei) exportieren. Sie können auch Informationen zu Kundenabonnements in eine CSV-Datei exportieren.

Darüber hinaus enthalten die Aktivitätsprotokolle exportierbare Daten zu Transaktionen und Verwaltungsaktionen für Kunden. Weitere Informationen finden Sie unter [Kundenaktivitätsprotokolle anzeigen](activity-logs.md).

## <a name="search-for-a-customer"></a>Suchen nach einem Kunden

1.  Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.
2.  Um nach einem Kunden zu suchen, geben Sie in das Suchfeld den Kundennamen oder den Domänennamen ein.
3.  Wählen Sie den **Pfeil nach unten** am Ende einer Kundenzeile aus, um die Microsoft-ID des Kunden sowie die verknüpften Abonnements und Quicklinks zu Diensten anzuzeigen.

## <a name="update-a-customers-company-name"></a>Firmennamen von Kunden aktualisieren

Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.
2.  Um nach einem Kunden zu suchen, geben Sie in das Suchfeld den Kundennamen oder den Domänennamen ein.
3.  Wählen Sie den **Pfeil nach unten** am Ende einer Kundenzeile aus, um die Microsoft-ID des Kunden sowie die verknüpften Abonnements und Quicklinks zu Diensten anzuzeigen.
4.  Aktualisieren Sie in den Daten zum **Rechnungsempfänger** den Unternehmensnamen. Wenn Sie den neuen Wert speichern, wird er in die Kundenliste aufgenommen. Dadurch werden nur der Firmenname für die Rechnungsadresse und der Wert in der Kundenliste geändert. Anderswo werden die Änderungen nicht wiedergegeben.
<sup>1</sup>
## <a name="export-your-customer-list"></a>Exportieren der Kundenliste

1. Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.
2. Wählen Sie **Kunden exportieren** aus.

   Partner Center konvertiert die gesamte Kundenliste in eine CSV-Datei und lädt sie in den Standarddownloadordner auf Ihrem Computer hoch. Sie können auch Teilmengen von Kundendaten exportieren. Zu den Datenspalten gehören u. a.:

   - **Microsoft-ID**;
   - **Firmenname**;
   - **Primärer Domänen Name**;
   - **Beziehung** – die Geschäftsbeziehung des Partners zu den einzelnen aufgelisteten Kunden.

    Standardmäßig exportiert Partner Center die gesamte Kundenliste, unabhängig von der Länge. Sie können die Kundenliste auch nach dem Namen des Unternehmens oder der Domäne auflisten und diese Teilmenge von Daten exportieren.

3. Wenn Sie indirekter Anbieter sind, können Sie die Kundenliste nach indirekten Händlern filtern. Wählen Sie die Liste **Nach indirekten Händlern filtern** aus, und wählen Sie einen Händler aus.
<sup>1</sup>

## <a name="export-customer-subscription-information"></a>Exportieren von Informationen zum Kundenabonnement

1. Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.

2. Wählen Sie den **Unternehmensnamen** eines Kunden aus. Die Seite **Abonnements** des Kunden wird geöffnet und zeigt die vollständige Liste der Produktabonnements an.

3. Wählen Sie **Abonnements exportieren** aus. Partner Center konvertiert die Abonnementdaten des Kunden in eine CSV-Datei und lädt sie in den Standarddownloadordner auf Ihrem Computer hoch. Zu den Datenspalten gehören u. a.:
   - **Abonnement-ID**;
   - **Abonnement** – der Produktname für das Abonnement;
   - **Menge** – die Anzahl der gekauften Lizenzen;
   - **Status**;
   - **Händler** – die ID des Händlers, der das Abonnement besitzt und verwaltet.

> [!NOTE]  
> Weitere Informationen zur Abonnementverwaltung finden Sie unter [Kundenabonnements](customer-subscriptions.md).
