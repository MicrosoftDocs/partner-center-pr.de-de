---
title: 'Angebote entdecken: kommerzieller Marketplace'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie CSP-Partner Partner Center zum Anzeigen oder Durchsuchen des Marketplace für SaaS-Angebote oder Preise von unabhängigen Software Anbietern (ISVs) verwenden können.
author: LauraBrenner
ms.author: labrenne
keywords: Abonnements, Marketplace, kommerzieller Marketplace, Drittanbieter, ISV, SaaS-Angebote, Cloud Solution Provider Program, CSP-Programm, CSP-Partner
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10653e41adee052b43ed092f4fd9bb48b79a1355
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908112"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>Entdecken Sie Angebote und Preise im Partner Center kommerziell Marketplace

**Zielgruppe**

- Partner Center
- Partner im CSP-Programm

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent

Wenn unabhängige Software Anbieter (Independent Software Anbieters, ISVs) ein Angebot im kommerziellen Marketplace veröffentlichen möchten, können Sie auch entscheiden, ob das Angebot im CSP-Programm zur Verfügung gestellt werden soll. Wenn Sie sich entscheiden, das Angebot über das CSP-Programm zu verkaufen, sollte CSP-Partner das Angebot im Partner Center Marketplace-Bereich sehen.

Wenn ein ISV-Angebot im Partner Center nicht erwartungsgemäß angezeigt wird, liegt dies möglicherweise daran, dass Folgendes der Fall ist:

- Der ISV hat beschlossen, das Angebot nicht über das CSP-Programm zu verkaufen. Beispielsweise können einige ISV-Produkte in anderen Bereichen des kommerziellen Marketplace (z. b. in [Microsoft AppSource](https://appsource.microsoft.com/) und [Azure Marketplace](https://azuremarketplace.microsoft.com/)) verfügbar gemacht werden, werden aber möglicherweise nicht für CSPs im Partner Center-Marketplace angezeigt.

- Der ISV beschloss, das Angebot ausschließlich für eine ausgewählte Anzahl von CSP-Partnern exklusiv zu gestalten. Weitere Informationen zu exklusiven Angeboten finden Sie unter weiter unten in diesem Hilfethema.

- Der Angebotstyp kann nicht über das Partner Center oder Azure-Portal (z. b. Container oder einige Verwendungs basierte Angebote) übertragen werden.

- Das Abrechnungs Land der zugeordneten Kunden wird für dieses ISV-Angebot möglicherweise nicht unterstützt.

## <a name="view-marketplace-offers-in-partner-center"></a>Anzeigen von Marketplace-angeboten im Partner Center

Zum Anzeigen der verfügbaren kommerziellen Marketplace-Angebote im CSP-Programm: 

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü **CSP** aus.

2. Wählen Sie **verkaufen**, gefolgt vom **Marketplace**. Standardmäßig werden Produkte aller Typen und Kategorien angezeigt.

3. Wählen Sie einen Filter nach Typ oder Kategorie aus. Sie können auch die **Suche** verwenden, um nach bestimmten Schlüsselwörtern, Angebots Namen oder Namen von ISV-Verlegern zu suchen.

4. Wählen Sie ein bestimmtes Produktangebot aus der Liste aus. Dadurch gelangen Sie zu einer Registerkarte für die Produktübersicht, auf der Sie mehr über das Angebot erfahren können. Die Informationen auf dieser Registerkarte können Folgendes umfassen: 

    - Eine Beschreibung des Produkts oder Angebots

    - Weitere Informationen zum ISV-Verleger

    - Links zu Dokumentations-oder Marketingmaterialien, die vom ISV-Verleger hochgeladen wurden

    - Andere mögliche ISV-Kontakte für den Kundensupport, das Engineering oder einen Kontakt für das CSP-Programm

5. Wenn Sie weitere Informationen zu den verfügbaren Plänen, SKUs oder Preisen eines Angebots anzeigen möchten, wählen Sie die Registerkarte **Pläne + Preise** aus. Diese Registerkarte zeigt Folgendes:

    - Die Märkte, in denen dieses Angebot für Sie verfügbar ist

    - Eine Liste von SKUs oder Plänen, die für das Angebot verfügbar sind

    - Preise für jede verfügbare SKU oder jeden Plan

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Anzeigen von Marketplace-angeboten über Partner Center-APIs

CSP-Programmpartner können auch APIs verwenden, um eine Liste der berechtigten Angebote zurückzugeben. Berechtigte Angebote sind nur die SaaS-ISV-Angebote, die der Partner über den Partner Center Marketplace verkaufen kann. Partner, die APIs verwenden, um Angebote im Katalog zu identifizieren, finden Sie in der Anleitung zum [Abrufen einer Liste mit Angeboten für einen Markt](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Anzeigen der neuesten Preise für Marketplace-Angebote in Partner Center

Führen Sie die folgenden Schritte aus, um die neuesten Preis Details zu einem Angebot anzuzeigen:

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü **CSP** aus.

2. Wählen Sie **verkaufen**aus, gefolgt von den **Preisen und angeboten**.

3. Scrollen Sie nach unten zum Abschnitt **Marketplace** , wählen Sie einen Standort aus, und laden Sie **Marketplace-Preise**herunter. Dadurch wird eine Tabelle mit den neuesten Preisdaten für SaaS und Lizenz basierte Angebote generiert, die von ISV-Verlegern zur Verfügung gestellt werden. Einige Azure-Anwendungs Preise können auch hier angezeigt werden. Diese Informationen werden täglich aktualisiert, sodass Sie die aktuellen Preise beliebig oft überprüfen können.

4. Wenn ein ISV-Produkt einen kostenlosen Testzeitraum enthält, werden in der Kalkulations Tabelle zwei Zeilen für das Produkt angezeigt:

    - Eine Zeile zeigt den kostenlosen Test Preis von 0 (null) an. Dies bedeutet, dass ein kostenloser Testzeitraum verfügbar ist.

    - Die andere Zeile zeigt den Preis und die Nutzungsbedingungen an, die nach Ablauf der kostenlosen Testversion gelten.

Als CSP-Programmpartner können Sie sich möglicherweise für andere Anreize im Zusammenhang mit bestimmten kommerziellen Marketplace-angeboten qualifizieren. Weitere Informationen zu anderen Incentives finden Sie im [CSP-Handbuch](https://aka.ms/partnerincentives) (CSP-Anmeldung erforderlich).

## <a name="learn-about-marketplace-exclusive-offers"></a>Weitere Informationen zu exklusiven Marketplace-angeboten

ISVs haben die Möglichkeit, Ihre Angebote nur für bestimmte Partner im CSP-Programm verfügbar zu machen. Dies wird als exklusives Angebot bezeichnet. Alle Partner im CSP-Programm können weiterhin alle ISV-Angebote im kommerziellen Marketplace von Partner Center anzeigen, einschließlich der als exklusiv markierten Angebote.

Wenn ein Angebot **nicht** als exklusiv gekennzeichnet ist, können alle Partner dieses Angebot erwerben (vorausgesetzt, das Abrechnungs Land des ausgewählten Kunden entspricht der Landes Verfügbarkeit des ISV-Angebots).

Für alle Angebote, die als exklusiv gekennzeichnet sind, können jedoch nur die vom ISV ausgewählten Partner dieses Angebot erwerben.

> [!NOTE]
> Wenn Sie ein als exklusiv markierte Angebot sehen, das Sie an Ihre Kunden verkaufen möchten, wenden Sie sich direkt an den ISV, und bitten Sie um die Berechtigung, das exklusive Angebot zu verkaufen. Wenn Sie die Details eines exklusiven Angebots anzeigen, wird möglicherweise ein **Kontakt-ISV** -Link angezeigt, den Sie auswählen können.

Weitere Informationen zur ISV-Benutzer Darstellung im kommerziellen Marketplace finden Sie unter [cloudlösungsanbieter](https://docs.microsoft.com/azure/marketplace/cloud-solution-providers).

Weitere Informationen zu den CSP-Funktionen im Marketplace finden Sie unter [Übersicht über den kommerziellen Marketplace](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Nächste Schritte

- [Erwerben kommerzieller Marketplace-Angebote](csp-commercial-marketplace-purchase.md)
