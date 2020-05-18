---
title: Azure-Plan-Preisliste für CSP-Partner
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Partner im CSP-Programm im Partner Center die Preisliste für Abonnements unter dem Azure-Plan anzeigen können.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f17dc4cb7e3f52984ce9a1fb7c19d048bb74c47b
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908322"
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

3. Wählen Sie neben **Exporttyp** die Option **Preise für Azure-Plannutzung**, **Preise für Azure-Planreservierungen** oder **Wechselkurse** aus. Hinweis: Die Option **Wechselkurse** ist nicht länderspezifisch.

3. Wählen Sie neben **Preise für Datum** das gewünschte Datum aus, beispielsweise **Aktuell**. 


![Landesspezifisch](images/azure/pricingnew.png)

Hinweis: Sie können zwei verschiedene Preislisten exportieren: Preise für Azure-Pläne und Drittanbieter-Preise für Marketplace. 

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

Preislisten für den Azure-Plan können auf der Seite [Azure-Planpreise und Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any) exportiert werden.

## <a name="pricing-api-for-azure-plan"></a>Preis-API für den Azure-Plan

Mithilfe der [Preis-API](https://docs.microsoft.com/partner/develop/pricing) können Nutzungs- und Reservierungspreise für den Azure-Plan programmgesteuert abgerufen werden. Darüber hinaus können auch Wechselkurse abgerufen werden. 

Die Preis-API befindet sich auf einem anderen Endpunkt als die anderen Partner Center-APIs. Die Preisinformationen umfassen Verbrauchseinheitspreise für Azure-Planressourcen und Reservierungspreise, die für Azure-Planabonnements gelten, in USD.

Mit dieser API können Partner auch monatliche Wechselkurse abrufen, da die Preise für den Azure-Plan nur in USD angegeben sind. Mit den APIs können Preise und Wechselkurse sowohl für den aktuellen Monat als auch für vergangenen Monate abgerufen werden.

>[!NOTE]
> Die Preis-API bezieht sich speziell auf Preise für den Azure-Plan. Für Azure-Ressourcen oder -Reservierungen, die für Nicht-Azure-Planabonnements bereitgestellt werden, sollten weiterhin die bestehende RateCard-API und die Preislisten verwendet werden, die auf der Seite „Preise und Angebote“ im Partner Center veröffentlicht werden. Die Preis-API für den Azure-Plan unterstützt keine Software-, Marketplace- oder arbeitsplatzbasierten Preise wie Microsoft 365 oder Dynamics 365.

Weitere Informationen zu Preisen für den Azure-Plan und zu Wechselkurs-APIs findest du in der vollständigen [Dokumentation zur Preis-API](https://docs.microsoft.com/partner/develop/pricing).
