---
title: Auswirkungen von Steuerrichtlinien auf die Auszahlung Azure Marketplace
description: Erfahren Sie, wie sich Steuerrichtlinien auf die Auszahlung Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856014"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Auswirkungen von Steuerrichtlinien auf die Auszahlung Azure Marketplace

**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Administrator-Agent

## <a name="introduction"></a>Einführung

Der kommerzielle Microsoft-Marketplace hat globale Reichweite. Transaktionen erfolgen über Grenzen hinweg, und je nachdem, wo sich der ISV und der Kunde befinden, können die Steuerauswirkungen variieren. Microsoft AppSource und Azure Marketplace sie Partner Center Steuerprofilinformationen, um das Land des ISV zu bestimmen. Um das Land des Kunden zu ermitteln, verwenden Sie entweder die Abrechnungsinformationen des Kunden, oder wenn der Kunde in der EU ist, verwenden wir zwei verschiedene Informationen.

Um die folgenden Szenarien besser [](tax-details-marketplace.md) zu verstehen, lesen Sie die Tabelle "Steuerdetails", die zeigt, ob Microsoft Steuern im Auftrag des Herausgebers einzieht und abzahlt oder ob diese Verantwortung dem Herausgeber gehört.

> [!NOTE]
> Alle Beispiele für Verkaufswerte und Steuerprozentsätze in diesem Thema dienen nur zur Veranschaulichung, nicht zu genauen Zahlen.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Herausgebertransaktionen in einem von Microsoft verwalteten Steuerland

**Szenario A:** Transaktionen, die zwischen einem Herausgeber und einem Kunden in einem von Microsoft verwalteten [Steuerland stattfinden.](tax-details-marketplace.md#microsoft-managed-countries) Diese Transaktionen werden zum Zeitpunkt des Verkaufs steuerlich hinzugefügt, und Microsoft sendet diese Steuer an das anwendbare Land. Es werden keine Steuern aus Auszahlungs- und Auszahlungsberechnungen abgezogen.

Informationen zu Transaktionen zwischen einem Nicht-US-Herausgeber und einem KUNDEN in den USA finden Sie unter Szenario [D.](#foreign-publisher-transacts-with-us-customer)

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario A an.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Herausgebertransaktionen in einem von Microsoft verwalteten Steuerland, in dem die Marketplace-Gebühr für den Dienst "1" steht

**Szenario B:** Transaktionen zwischen einem Herausgeber in den USA (gemäß definition in den Partner Center-Steuerprofilinformationen) für einen Kunden in einem von Microsoft verwalteten Steuerland, in dem das Land eine Steuer auf die Marketplace-Gebühr (einen Dienstanbieter) erzwingt. In diesem Szenario wird die Steuer für die Store-Dienstgebühr von der Auszahlung des Herausgebers abgezogen.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario B an.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Verlegertransaktionen im vom Herausgeber verwalteten Steuerland

**Szenario C:** Transaktionen zwischen einem Herausgeber und einem Kunden in einem vom Herausgeber verwalteten Steuerland, das keine Quellensteuer für Kunden erzwingt. Kunden zahlen zum Zeitpunkt des Verkaufs keine Steuern, und es ist die Verpflichtung des Herausgebers, alle anwendbaren Steuern zu zahlen.

Weitere Informationen zu landspezifischen Preisen (z. B. zum Ausgleich bevorstehender Angebote) finden Sie unter Pläne und Preise für Angebote [im kommerziellen Marketplace.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher Transacts with US Customer

**Szenario D** : Alle (gemäß ihren Partner Center-Steuerprofilinformationen) in Ländern ohne US-Amerikanischen Verleger (siehe Szenario [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)verkaufen einen Kunden in den USA (gemäß der Kundenkontoadresse). Die US-Regierung verlangt, dass Microsoft die Steuern im Auftrag des Herausgebers einbehalten muss. Die Steuer für die Auszahlung an den Herausgeber wird basierend auf dem Angebotspreis berechnet.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Fremder Herausgeber mit einer Transaktion mit US-Kunden

**Szenario E:** Alle (gemäß ihren Partner Center-Steuerprofilinformationen) in Ländern mit einem US-amerikanischen Kunden, der einen Verkauf an einen Kunden in den USA vorzieht (gemäß der Kundenkontoadresse). Die US-Regierung verlangt nicht, dass Microsoft die Steuern im Auftrag des Herausgebers einbehalten muss.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Ein fremder Herausgeber verkauft an einen Kunden mit EU-Umsatzsteuer-Registrierung in einem von Microsoft verwalteten Land (außerhalb von Irland).

**Szenario F:** Alle Transaktionen zwischen externen Herausgebern und kunden mit EU-Umsatzsteuer (außerhalb von Irland) in einem Microsoft-Managed Land. Der Kunde zahlt keine Steuern für den Verkauf.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario F an.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Ein fremder Herausgeber verkauft an einen kunden mit EU-Umsatzsteuer-Registrierung in einem von Microsoft verwalteten Land (in Irland).

**Szenario G:** Alle Transaktionen zwischen fremden Herausgebern und Eu-Kunden mit Eu-Umsatzsteuer-Registrierung (innerhalb von Irland) in einem Microsoft-Managed Land. Der Kunde zahlt die Gesetzliche Steuer, und Microsoft zahlt diese Steuer an die Regierung.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario G an.":::

## <a name="next-steps"></a>Nächste Schritte

- [Häufig gestellte Fragen zum Herausgeber](/azure/marketplace/marketplace-faq-publisher-guide)
- [Anweisungen zum Erstellen von Zahlungs- und Steuerprofilen](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)