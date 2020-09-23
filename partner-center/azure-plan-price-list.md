---
title: Azure-Plan-Preisliste für CSP-Partner
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Partner im CSP-Programm im Partner Center die Preisliste für Abonnements unter dem Azure-Plan anzeigen können.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 57e976f2968f0bd6b13f36eb04be9f68577d1389
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000324"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP für Azure

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

Die Preisliste für die neue Azure E-Commerce-Benutzeroberfläche in CSP ist im Partner Center veröffentlicht. Die Preisliste wird dynamisch in einer exakten Echtzeitdatei bereitgestellt, und die Preise werden nur in USD angezeigt. Die Abrechnung erfolgt jedoch in der unterstützten Währung, die am Währungsstandort des Kunden gilt. Weitere Informationen zur Abrechnung am Währungsstandort des Kunden finden Sie unter [Azure-Plan: Abrechnung](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Anzeigen der Preisliste für Abonnements im Rahmen eines Azure-Plans

1. Wählen Sie im Menü des Partner Centers auf der linken Seite **Verkaufen** und dann **Marketplace** aus.

2. Wählen Sie unter „Preise für Azure-Plan“ das Land/die Region aus, für das/die Sie Preise aufrufen möchten.

3. Wählen Sie neben **Exporttyp** die Option **Preise für Azure-Plannutzung**, **Preise für Azure-Planreservierungen** oder **Wechselkurse** aus. 

>[!NOTE] 
>Die Option **Wechselkurse** ist nicht länderspezifisch.

4. Wählen Sie neben **Preise für Datum** das gewünschte Datum aus, beispielsweise **Aktuell**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="Landesspezifisch":::

>[!NOTE] 
>Sie können zwei verschiedene Preislisten exportieren: Preise für Azure-Pläne und Drittanbieter-Preise für Marketplace.

## <a name="azure-price-list-specifics"></a>Besonderheiten der Azure-Preisliste

- Die Preise für Azure-Pläne sind auf der Marketplace-Seite im Partner Center unter **Verkaufen** verfügbar.

- Exporte sind für die Azure-Plan-Verbrauchsdienste, Azure-Reservierungen und Wechselkurse verfügbar.

- Zu den Exportoptionen gehören:

  - **Preise heute**: Dies schließt alle Verbrauchseinheiten und Preise vom 1. des Monats bis zum aktuellen Datum des aktuellen Monats ein. Dies schließt neue Preise, geänderte Preise oder entfernte Preise ein. Alle Preise sind mit den Start- und Enddaten ihrer Gültigkeit aufgelistet, um zu erläutern, ob sie neu sind oder entfernt wurden.

  - **Preise des Vormonats**: Die Downloads für jeden Ressourcentyp erfolgen monatsweise. Bei Preisdateien schließt dies alle Verbrauchseinheiten ein, die für den betreffenden Monat zum Zeitpunkt des Downloads verfügbar sind. Wenn in der Monatsmitte eine neue Verbrauchseinheit auftritt, wird sie als Verbrauchseinheit mit einem Gültigkeitsdatum aufgeführt, das ihre Verfügbarkeit angibt. Ähnliches gilt für eingestellte Preise, die mit dem Enddatum ihrer Gültigkeit aufgeführt werden, das angibt, ab wann sie nicht mehr verfügbar sind.

  - **Wechselkurse**: Wechselkurse stehen für den Download am Tag vor dem 1. des Monats um 18:00 Uhr PST zur Verfügung. Wenn Sie beispielsweise die Wechselkurse für November erfahren möchten, laden Sie die Wechselkurse am 31. Oktober herunter. Die Wechselkurse des Vormonats sind ebenfalls verfügbar.

- Die Preise in den Preislisten sind Direktpreise. Einige Partner sind möglicherweise für vom Partner erworbene Guthaben qualifiziert. Informationen zur Berechnung des vom Partner erworbenen Guthabens finden Sie unter [Wie von Partnern erworbene Guthaben berechnet und bezahlt werden](partner-earned-credit-explanation.md).

- **Berechtigte Dienste**: Das vom Partnern erworbene Guthaben kann auf Dienste angerechnet werden, die in den **Preisen für Azure-Plannutzung** aufgelistet sind, die Partner von der Seite [Azure-Plan-Preise](https://partner.microsoft.com/commerce/sales) exportieren können. Es gibt jedoch auch Ausnahmen, beispielsweise Produkte von Drittanbietern, die in der Tags-Spalte der Preisliste für die Azure-Plannutzung und Azure-Planreservierungen als „Drittanbieter“ gekennzeichnet sind.

## <a name="price-list-data"></a>Preislistendaten

|**Feld**   |**Beschreibung**   |
|--------------------------|:---------------------------|
|ProductTitle  |Der Titel oder Name des Produkts|
|ProductID   |Die ID des Produkts|
|SKuId|Die ID der SKU|
|SkuTitle|Der Titel oder Name der SKU|
|Herausgeber|Der Originalanbieter ist immer Microsoft|
|SkuDescription|Beschreibung der SKU|
|UnitOfMeasure|Die Einheiten die in Rechnung gestellt oder abgerechnet werden|
|TermDuration|Bei Produkten mit Laufzeit die Länge der Laufzeit, auf Reservierungen anwendbar|
|Market|Der Markt, für den diese Preise gelten|
|Währung|Die Währung für die Preise|
|UnitPrice|Preis pro Einheit|
|PricingTierRangeMin|Bei mehrstufigen Preisen gilt der Mindestpreis|
|PricingTierRangeMax|Bei mehrstufigen Preisen gilt der Höchstpreis|
|EffectiveStartDate|Startdatum der Preise|
|EffectiveEndDate|Enddatum der Preise|
|MeterIds|Die Verbrauchseinheit-ID der Produkt-SKU|
|MeterType|Typ der Verbrauchseinheit|
|Tags|Eigenschaften des Artikels, bei Azure-Plan-Preisen ist die Azure oder Azure und Reservierungen (speziell für Reservierungen)|

Preislisten für den Azure-Plan können von der Seite [Preise und Angebote](https://partner.microsoft.com/dashboard/sell/pricingandoffers) im Partner Center exportiert werden.

## <a name="tiered-pricing"></a>Mehrstufige Preise

Einige Dienste für die Nutzung von Azure-Plänen unterstützen mehrstufige Preise. Partner finden diese Produkte und SKUs in der Preisliste für Azure-Pläne. Einträge, für die in den PricingTierRange-Spalten Werte angegeben sind, ermöglichen es Partnern, den Preis basierend auf der Nutzung nachzuvollziehen. Im folgenden Beispiel anhand von Beispieldaten verfügt eine Produkt-SKU über drei Tarife.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Wenn in diesem Beispiel 101 Einheiten verwendet werden, würde die Gebühr 100,80 betragen. Die ersten 100 Einheiten werden jeweils als eine Einheit und die nächste Einheit mit 0,80 berechnet.

## <a name="pricing-api-for-azure-plan"></a>Preis-API für den Azure-Plan

Mithilfe der [Preis-API](/partner/develop/pricing) können Nutzungs- und Reservierungspreise für den Azure-Plan programmgesteuert abgerufen werden. Darüber hinaus können auch Wechselkurse abgerufen werden.

Die Preis-API befindet sich auf einem anderen Endpunkt als die anderen Partner Center-APIs. Die Preisinformationen umfassen Verbrauchseinheitspreise für Azure-Planressourcen und Reservierungspreise, die für Azure-Planabonnements gelten, in USD.

Mit dieser API können Partner auch monatliche Wechselkurse abrufen, da die Preise für den Azure-Plan nur in USD angegeben sind. Mit den APIs können Preise und Wechselkurse sowohl für den aktuellen Monat als auch für vergangenen Monate abgerufen werden.

>[!NOTE]
> Die Preis-API bezieht sich speziell auf Preise für den Azure-Plan. Für Azure-Ressourcen oder -Reservierungen, die für Nicht-Azure-Planabonnements bereitgestellt werden, sollten weiterhin die bestehende RateCard-API und die Preislisten verwendet werden, die auf der Seite „Preise und Angebote“ im Partner Center veröffentlicht werden. Die Preis-API für Azure-Pläne unterstützt keine software-, Marketplace- oder lizenzbasierten Preise wie Microsoft 365 oder Dynamics 365.

Weitere Informationen zu Preisen für den Azure-Plan und zu Wechselkurs-APIs findest du in der vollständigen [Dokumentation zur Preis-API](/partner/develop/pricing).