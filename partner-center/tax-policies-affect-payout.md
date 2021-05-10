---
title: Auswirkungen von Steuerrichtlinien auf die Auszahlung für Azure Marketplace
description: Erfahren Sie, wie sich Steuerrichtlinien auf die Auszahlung für Azure Marketplace auswirken.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686312"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Auswirkungen von Steuerrichtlinien auf die Auszahlung für Azure Marketplace

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Administrator-Agent

## <a name="introduction"></a>Einführung

Der kommerzielle Microsoft-Marketplace verfügt über globale Reichweite. Transaktionen erfolgen über Grenzen hinweg. Je nachdem, wo sich der ISV und der Kunde befinden, können die Auswirkungen auf die Steuer variieren. Microsoft AppSource und Azure Marketplace die Partner Center Steuerprofilinformationen verwenden, um das Land des ISV zu bestimmen. Um das Land des Kunden zu bestimmen, verwenden Sie entweder die Abrechnungsinformationen des Kunden, oder wenn sich der Kunde in der EU befindet, verwenden wir zwei verschiedene Informationen.

Um die folgenden Szenarien besser zu verstehen, lesen Sie die Tabelle mit den [Steuerdetails,](tax-details-marketplace.md) in der angezeigt wird, ob Microsoft Steuern im Auftrag des Herausgebers einzieht und bezahlt oder ob diese Verantwortung dem Herausgeber gehört.

> [!NOTE]
> Alle Beispiele für Verkaufswerte und Steuerprozentsätze in diesem Thema dienen nur zur Veranschaulichung, nicht zu genauen Zahlen.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Herausgebertransaktionen in einem von Microsoft verwalteten Steuerland

**Szenario A:** Transaktionen, die zwischen einem Herausgeber und einem Kunden in einem von [Microsoft verwalteten Steuerland](tax-details-marketplace.md#microsoft-managed-countries)stattfinden. Für diese Transaktionen wird zum Zeitpunkt des Verkaufs die entsprechende Steuer hinzugefügt, und Microsoft sendet diese Steuer an das entsprechende Land. Keine Steuern werden aus Auszahlungsberechnungen zurückgehalten, und Auszahlungsberechnungen sind steuerausbesteuert.

Informationen zu Transaktionen zwischen einem Nicht-US-Verleger und einem US-Kunden finden Sie unter [Szenario D.](#foreign-publisher-transacts-with-us-customer)

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario A an.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Herausgebertransaktionen in einem von Microsoft verwalteten Steuerland, in dem die Marketplace-Gebühr steuerbar ist

**Szenario B:** Transaktionen, die zwischen einem US-basierten Herausgeber (wie durch die Partner Center Steuerprofilinformationen definiert) an einen Kunden in einem von Microsoft verwalteten Steuerland stattfinden, in dem das Land eine Steuer auf die Marketplace-Gebühr (einen steuerbaren Dienst) erhebt. In diesem Szenario wird die Gebühr für den Store-Dienst von der Auszahlung des Herausgebers abgezogen.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario B an.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Verlegertransaktionen im vom Herausgeber verwalteten Steuerland

**Szenario C:** Transaktionen zwischen einem Herausgeber und einem Kunden in einem vom Herausgeber verwalteten Steuerland, das keine Quellensteuer für Kunden erzwingt. Kunden zahlen zum Zeitpunkt des Verkaufs keine Steuern, und es ist die Verpflichtung des Herausgebers, alle anwendbaren Steuern zu zahlen.

Weitere Informationen zu landspezifischen Preisen (z. B. zum Ausgleich bevorstehender Angebote) finden Sie unter Pläne und Preise für Angebote [im kommerziellen Marketplace.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher Transacts with US Customer

**Szenario D** : Alle (gemäß ihren Partner Center-Steuerprofilinformationen) in Ländern ohne US-Amerikanischen Verleger (siehe Szenario [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) verkaufen einen Kunden in den USA (gemäß der Kundenkontoadresse). DIE US-Regierung verlangt, dass Microsoft die Steuern im Namen des Herausgebers einbehalten muss. Die Steuer für die Auszahlung an den Herausgeber wird basierend auf dem Angebotspreis berechnet.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Fremder Herausgeber mit einer Transaktionstransaktivierung mit US-Kunden

**Szenario E:** Alle herausgeber (gemäß ihren Partner Center-Steuerprofilinformationen) in Ländern mit einem US-Amerikanischen Kunden, der einen Verkauf an einen Kunden in den USA macht (gemäß der Kundenkontoadresse). Die US-Regierung verlangt nicht, dass Microsoft die Steuern im Auftrag des Herausgebers einbehalten muss.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Ein fremder Herausgeber verkauft an einen Kunden mit EU-Umsatzsteuer-Registrierung in einem von Microsoft verwalteten Land (außerhalb von Irland).

**Szenario F:** Alle Transaktionen zwischen externen Herausgebern und kunden mit EU-Umsatzsteuer (außerhalb von Irland) in einem Microsoft-Managed Land. Der Kunde zahlt keine Steuern für den Verkauf.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario F an.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Ein fremder Herausgeber verkauft an einen bei der EU-Steuer registrierten Kunden in einem von Microsoft verwalteten Land (in Irland)

**Szenario G:** Alle Transaktionen zwischen fremden Herausgebern und Eu-Kunden mit Eu-Umsatzsteuer-Registrierung (innerhalb von Irland) in einem Microsoft-Managed Land. Der Kunde zahlt die gesetzliche Steuer, und Microsoft überzahlt diese Steuer an die Regierung.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario G an.":::

## <a name="next-steps"></a>Nächste Schritte

- [Häufig gestellte Fragen zum Herausgeber](/azure/marketplace/marketplace-faq-publisher-guide)
- [Anweisungen zum Erstellen von Zahlungs- und Steuerprofilen](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)