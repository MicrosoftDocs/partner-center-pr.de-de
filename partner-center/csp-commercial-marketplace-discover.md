---
title: Entdecken von Angeboten – kommerzieller Marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie CSP-Partner Partner Center verwenden können, um den Marketplace nach SaaS-Angeboten oder Preisen von unabhängigen Softwareherstellern (Independent Software Vendors, ISVs) zu suchen.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147971"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Entdecken von Angeboten und Preisen im Partner Center Marketplace

**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent

Wenn unabhängige Softwarehersteller (Independent Software Vendors, ISVs) ein Angebot im kommerziellen Marketplace veröffentlichen, können sie auch entscheiden, ob das Angebot im CSP-Programm verfügbar gemacht werden soll. Wenn sie sich dafür entscheiden, das Angebot über das CSP-Programm zu verkaufen, sollten CSP-Partner das Angebot im marketplace Partner Center bereich sehen.

Wenn ein ISV-Angebot nicht wie erwartet in der Partner Center angezeigt wird, liegt dies möglicherweise daran:

- Der ISV hat sich entschieden, das Angebot nicht über das CSP-Programm zu verkaufen. Beispielsweise wurden einige ISV-Produkte möglicherweise in anderen Bereichen des kommerziellen Marketplace (z. B. in Microsoft AppSource und [Azure Marketplace)](https://azuremarketplace.microsoft.com/)zur Verfügung [gestellt,](https://appsource.microsoft.com/) werden aber möglicherweise nicht für Partner im CSP-Programm im Partner Center-Marketplace angezeigt.

- Der ISV hat sich entschieden, das Angebot nur für eine ausgewählte Anzahl von CSP-Partnern exklusiv zu machen. Weitere Informationen zu exklusiven Angeboten finden Sie weiter unten in diesem Hilfethema.

- Der Angebotstyp kann möglicherweise nicht über Partner Center oder Azure-Portal (z. B. Container oder einige nutzungsbasierte Angebote) durchgeführt werden.

- Das Abrechnungsland Ihrer zugeordneten Kunden wird für dieses ISV-Angebot möglicherweise nicht unterstützt.

## <a name="view-marketplace-offers-in-partner-center"></a>Anzeigen von Marketplace-Angeboten in Partner Center

So zeigen Sie verfügbare Angebote für den kommerziellen Marketplace im CSP-Programm an:

1. Melden Sie sich Partner Center [Dashboard an,](https://partner.microsoft.com/dashboard)und wählen Sie dann im linken Navigationsmenü **CSP** aus.

2. Wählen Sie **Verkaufen** und dann **Marketplace aus.** Standardmäßig werden Produkte aller Typen und Kategorien angezeigt.

3. Wählen Sie einen Filter nach Typ oder Kategorie aus. Sie können die Suche auch **verwenden,** um nach bestimmten Schlüsselwörtern, Angebotsnamen oder Namen von ISV-Herausgebern zu suchen.

4. Wählen Sie in der Liste ein bestimmtes Produktangebot aus. Dadurch gelangen Sie zu einer Produktübersichtsregisterkarte, auf der Sie mehr über das Angebot erfahren können. Informationen auf dieser Registerkarte können Folgendes umfassen: 

    - Eine Beschreibung des Produkts oder Angebots

    - Weitere Informationen zum ISV-Herausgeber

    - Links zu Dokumentations- oder Marketingmaterialien, die vom ISV-Herausgeber hochgeladen wurden

    - Andere mögliche ISV-Kontakte für Kundensupport, Engineering oder einen Kontakt für das CSP-Programm

5. Um weitere Informationen zu den verfügbaren Plänen, SKUs oder Preisen eines Angebots anzuzeigen, wählen Sie die Registerkarte **Pläne + Preise** aus. Auf dieser Registerkarte werden Dies wird angezeigt:

    - Die Märkte, in denen dieses Angebot für Sie verfügbar ist

    - Eine Liste der für das Angebot verfügbaren SKUs oder Pläne

    - Preise für jede verfügbare SKU oder jeden Plan

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Anzeigen von Marketplace-Angeboten über Partner Center-APIs

CSP-Programmpartner können auch APIs verwenden, um eine Liste berechtigter Angebote zurückzugeben. Berechtigte Angebote sind nur die SaaS ISV-Angebote, die der Partner über Partner Center Marketplace verkaufen kann. Partner, die APIs verwenden, um Angebote im Katalog zu identifizieren, finden Sie in der Anleitung zum [Abrufen einer Liste von Angeboten für einen Markt.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Anzeigen der aktuellen Marketplace-Angebotspreise in Partner Center

Führen Sie die folgenden Schritte aus, um die aktuellen Preisdetails für ein Angebot anzuzeigen:

1. Melden Sie sich bei Partner Center [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü **CSP** aus.

2. Wählen Sie **Verkaufen** und dann **Preise und Angebote** aus.

3. Scrollen Sie nach unten zum Abschnitt **Marketplace,** wählen Sie einen Standort aus, und laden Sie **die Marketplace-Preise** herunter. Dadurch wird ein Arbeitsblatt mit den neuesten Preisdaten für SaaS, lizenzbasierte Angebote und gemessene Angebote generiert, die von ISV-Herausgebern verfügbar sind. Einige Preise für Azure-Anwendungen werden möglicherweise auch hier angezeigt. Diese Informationen werden täglich aktualisiert, sodass Sie sie so oft wie möglich auf aktuelle Preise überprüfen können.

4. Wenn ein ISV-Produkt einen kostenlosen Testzeitraum enthält, zeigt das Arbeitsblatt zwei Zeilen für dieses Produkt an:

    - In einer Zeile wird der kostenlose Testpreis 0 (null) gezeigt. Dies bedeutet, dass ein kostenloser Testzeitraum verfügbar ist.

    - Die andere Zeile enthält den Preis und die Bedingungen, die nach Dem Ende des kostenlosen Testzeitraums gelten.

Als CSP-Programmpartner sind Sie möglicherweise für andere Incentives berechtigt, die bestimmten Angeboten im kommerziellen Marketplace zugeordnet sind. Weitere Informationen zu anderen Incentives finden Sie im [Leitfaden für CSP-Incentives](https://aka.ms/partnerincentives) (erfordert CSP-Anmeldung).

## <a name="learn-about-marketplace-exclusive-offers"></a>Informationen zu exklusiven Marketplace-Angeboten

ISVs haben die Möglichkeit, ihre Angebote nur bestimmten Partnern im CSP-Programm zur Verfügung zu stellen. Dies wird als exklusives Angebot bezeichnet. Alle Partner im CSP-Programm können weiterhin alle ISV-Angebote in Partner Center kommerziellen Marketplace anzeigen, einschließlich der Angebote, die als Exklusiv gekennzeichnet sind.

Wenn ein Angebot **nicht** als Exklusiv gekennzeichnet ist, können alle Partner dieses Angebot erwerben (vorausgesetzt, das Abrechnungsland des ausgewählten Kunden entspricht der Länderverfügbarkeit des ISV-Angebots).

Für alle Angebote, die als Exklusiv gekennzeichnet sind, können jedoch nur die vom ISV ausgewählten Partner dieses Angebot erwerben.

> [!NOTE]
> Wenn sie ein Angebot mit der Schilderung Exklusiv sehen, das Sie an Ihre Kunden verkaufen möchten, wenden Sie sich direkt an den ISV, und bitten Sie um die Berechtigung zum Verkauf des exklusiven Angebots. Wenn Sie die Details eines exklusiven Angebots anzeigen, wird möglicherweise ein Link **IsV** kontaktieren angezeigt, den Sie auswählen können.

Weitere Informationen zur ISV-Erfahrung im kommerziellen Marketplace finden Sie unter [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).

Weitere Informationen zur CSP-Erfahrung im Marketplace finden Sie unter Übersicht über den [kommerziellen Marketplace.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Nächste Schritte

- [Erwerben von Angeboten für den kommerziellen Marketplace](csp-commercial-marketplace-purchase.md)