---
title: Auswirkungen von Steuer Richtlinien auf die Auszahlung der Azure Marketplace
description: Erfahren Sie, wie sich Steuer Richtlinien auf die Auszahlung der Azure Marketplace auswirken.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712952"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Auswirkungen von Steuer Richtlinien auf die Auszahlung der Azure Marketplace

**Geeignete Rollen**
-    Globaler Administrator
-    Benutzeradministrator
-    Administrator-Agent

## <a name="introduction"></a>Einführung

Der kommerzielle Marketplace von Microsoft bietet globale Reichweite. Transaktionen werden grenzübergreifend durchlaufen, und abhängig davon, wo sich der ISV und der Kunde befinden, können die Auswirkungen auf die Steuereffekte variieren. Microsoft AppSource und Azure Marketplace die Partner Center-Steuer Profilinformationen verwenden, um das ISV-Land zu bestimmen. Um das Land des Kunden zu ermitteln, verwenden Sie entweder die Abrechnungsinformationen des Kunden, oder wenn sich der Kunde in der EU befindet, verwenden wir zwei verschiedene Informationen.

Um die folgenden Szenarien besser zu verstehen, sehen Sie sich die Tabelle " [Tax Details](tax-details-marketplace.md) " an, die anzeigt, ob Microsoft Steuern im Auftrag des Verlegers erfasst und bezahlt oder ob diese Verantwortung zum Verleger gehört.

> [!NOTE]
> Alle Beispiele Verkaufs Werte und Steuer Prozentsätze in diesem Thema dienen nur zu Veranschaulichung, nicht zu exakten Abbildungen.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Verleger transagiert in von Microsoft verwalteten Steuer Ländern

**Szenario A** – Transaktionen, die zwischen einem Verleger und einem Kunden in einem von [Microsoft verwalteten steuerland](tax-details-marketplace.md#microsoft-managed-countries)stattfinden. Diese Transaktionen werden zum Zeitpunkt des Verkaufs der anwendbaren Steuern hinzugefügt, und Microsoft sendet diese Steuern an das anwendbare Land. Keine Steuern von Auszahlungs-und Auszahlungs Berechnungen sind Steuer exklusiv.

Weitere Informationen finden Sie unter [Szenario D](#foreign-publisher-transacts-with-us-customer) für Transaktionen zwischen einem nicht-US-Verleger und einem US-Kunden.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Verleger transagiert in von Microsoft verwalteten Steuer Ländern, in denen die Marketplace-Gebühr gebührenpflichtig ist

**Szenario B** – Transaktionen, die zwischen einem US-basierten Verleger (gemäß der Definition in den Steuer Profilinformationen Ihres Partner Centers) für einen Kunden in einem von Microsoft verwalteten steuerland gelten, in dem das Land eine Steuern der Marketplace-Gebühr auferlegt (ein kostenpflichtiger Dienst). In diesem Szenario wird die Steuern der Kosten für den Store-Dienst von der Auszahlung des Herausgebers subtrahiert.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario B an.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Verleger transaagiert in vom Herausgeber verwalteten Steuer Ländern

**Szenario C** – Transaktionen, die zwischen einem Verleger und einem Kunden in einem von einem Herausgeber verwalteten steuerland stattfinden, das keine der Kunden zurückgibt. Kunden bezahlen zum Point of Sale keine Steuern, und es ist die Verpflichtung des Herausgebers, sämtliche anwendbaren Steuern zu bezahlen.

Weitere Informationen zu Land spezifischen Preisen (z. b. zum versetzen bevorstehender Steuern) finden Sie unter [Pläne und Preise für kommerzielle Marketplace-Angebote](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher transagiert mit US-Kunde

**Szenario D** – alle fremden Verleger (gemäß Definition in Ihren Partner Center-Steuer Profilinformationen) in Ländern ohne einen US-Vertrag (siehe [Szenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) Erstellen eines Verkaufs an einen US-basierten Kunden (gemäß seiner Kundenkonto Adresse). Die US-Regierung verlangt, dass Microsoft Steuern im Auftrag des Verlegers zurückgibt. Die von der Auszahlung an den Verleger zurückgehaltenen Steuererklärungen werden basierend auf dem Angebotspreis berechnet.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Der fremd Verleger mit einem Vertrag wird mit dem US-Kunden abgearbeitet.

**Szenario E** – alle fremden Verleger (gemäß Definition in Ihren Partner Center-Steuer Profilinformationen) in Ländern mit einem US-Vertrag, der einen US-basierten Kunden verkauft (wie von seiner Kundenkonto Adresse definiert). Die US-Regierung verlangt nicht, dass Microsoft Steuern im Auftrag des Verlegers zurückgibt.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Der fremd Verleger wird an einen Kunden in einem von Microsoft verwalteten Land (außerhalb von Irland) in einem von Microsoft verwalteten Land verkauft.

**Szenario F** – alle Transaktionen zwischen fremden Verlegern und EU-Kunden in der EU (außerhalb von Irland) in einem Microsoft-Managed Land. Der Kunde zahlt keine Steuern für den Verkauf.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario F an.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Der fremd Verleger verkauft sich in einem von Microsoft verwalteten Land in einem von Microsoft verwalteten Land (in Irland) an einen Kunden in der EU

**Szenario G** – alle Transaktionen zwischen fremden Verlegern und EU-Kunden in der EU (in Irland) in einem Microsoft-Managed Land. Der Kunde zahlt die irische Umsatzsteuer, und Microsoft zahlt diese Steuern an die irische Regierung.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario G.":::

## <a name="next-steps"></a>Nächste Schritte

- [FAQ zu Verlegern](/azure/marketplace/marketplace-faq-publisher-guide)
- [Anweisungen zum Erstellen von Zahlungs-und Steuer Profilen](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)