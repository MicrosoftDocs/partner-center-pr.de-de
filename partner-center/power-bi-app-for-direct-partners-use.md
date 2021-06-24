---
title: Verwenden Partner Center Analytics für Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Ihre Geschäftsdaten mithilfe der Partner Center Analytics-App für Power BI anzeigen (für direkte Partner im Cloud Solution Provider(CSP)-Programm).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564980"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="75e0a-103">Ihre Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI anzeigen</span><span class="sxs-lookup"><span data-stu-id="75e0a-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="75e0a-104">**Geeignete Rollen**: Globaler Administrator | Benutzerverwaltungsadministrator | Vertriebsbeauftragter | Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="75e0a-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="75e0a-105">Anzeigen Ihrer Geschäftsdaten</span><span class="sxs-lookup"><span data-stu-id="75e0a-105">View your business data</span></span>

<span data-ttu-id="75e0a-106">Eine visuelle Darstellung Ihrer Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="75e0a-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="75e0a-107">Wachstum bei Kundenstamm, Abonnements und Lizenzen</span><span class="sxs-lookup"><span data-stu-id="75e0a-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="75e0a-108">Verwendung von Office 365-, Microsoft Dynamics- und Microsoft Azure-Produkten</span><span class="sxs-lookup"><span data-stu-id="75e0a-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="75e0a-109">Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem Azure-Abonnement in den letzten 60 Tagen</span><span class="sxs-lookup"><span data-stu-id="75e0a-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="75e0a-110">Geschätzte Kosten (auf Grundlage der aktuellen Gebührenkarte)</span><span class="sxs-lookup"><span data-stu-id="75e0a-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="75e0a-111">Möglichkeit zum Exportieren von Datasets und Erstellen benutzerdefinierter Berichte, einschließlich pro Kunde.</span><span class="sxs-lookup"><span data-stu-id="75e0a-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="75e0a-112">Informationen zur Vorschauversion der Partner Center Analytics-App</span><span class="sxs-lookup"><span data-stu-id="75e0a-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="75e0a-113">Diese App ist nur für direkte Partner im Cloud Solution Provider-Programm (CSP) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="75e0a-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="75e0a-114">Andere Partner im CSP (z. B. indirekte Wiederverkäufer) können sich nicht anmelden.</span><span class="sxs-lookup"><span data-stu-id="75e0a-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="75e0a-115">Alle geschätzten Kosten werden vor Steuern/Abrechnungsdaten angezeigt und sind nicht rechtlich bindend.</span><span class="sxs-lookup"><span data-stu-id="75e0a-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="75e0a-116">Die geschätzten Kosten dienen nur zu Informationszwecken.</span><span class="sxs-lookup"><span data-stu-id="75e0a-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="75e0a-117">Die Kundeninformationen basieren auf Abonnements.</span><span class="sxs-lookup"><span data-stu-id="75e0a-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="75e0a-118">Alle Kunden, für die Sie vor Kurzem Konten erstellt haben, aber noch keine Abonnements haben, werden nicht in die Anzahl einbezogen.</span><span class="sxs-lookup"><span data-stu-id="75e0a-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="75e0a-119">Die geschätzten Kosten basiert auf der aktuellen Gebührenkarte, die auf den CSP-Preisen basiert.</span><span class="sxs-lookup"><span data-stu-id="75e0a-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="75e0a-120">Die Tage sind Kalendertage.</span><span class="sxs-lookup"><span data-stu-id="75e0a-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="75e0a-121">Geschäftsinformationen-Bericht</span><span class="sxs-lookup"><span data-stu-id="75e0a-121">Business Insights report</span></span>

- <span data-ttu-id="75e0a-122">**Kunden-Mandanten:** Anzahl unterschiedlicher Azure Active Directory (Azure AD) Von Kunden, die Abonnements erworben haben</span><span class="sxs-lookup"><span data-stu-id="75e0a-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="75e0a-123">**Neu (letzte 30 Tage):** Neue Kunden, die in den letzten 30 Tagen mindestens ein Abonnement erwerben</span><span class="sxs-lookup"><span data-stu-id="75e0a-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="75e0a-124">**Änderungsabwanderung (letzte 30 Tage):** Kunden ohne "aktive", "in Grace"- oder "disabled"-Abonnements</span><span class="sxs-lookup"><span data-stu-id="75e0a-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="75e0a-125">**Neu (letzte 24 Stunden):** Neue Kunden, die in den letzten 24 Stunden mindestens ein Abonnement erwerben</span><span class="sxs-lookup"><span data-stu-id="75e0a-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="75e0a-126">Geschätzte monatliche Kosten in den letzten **12** Monaten: Trend von Monat zu Monat des geschätzten Rechnungsbetrags vor Steuern, der monatlich über den Zeitraum der letzten 12 Monate aggregiert wurde</span><span class="sxs-lookup"><span data-stu-id="75e0a-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="75e0a-127">Geschätzte Kosten nach Produkt in den letzten **12** Monaten: Verkaufte Produkte sortiert nach geschätztem Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 12 Monate.</span><span class="sxs-lookup"><span data-stu-id="75e0a-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="75e0a-128">Dieser Status gibt die wichtigsten Produkte mit dem größten Umsatz an.</span><span class="sxs-lookup"><span data-stu-id="75e0a-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="75e0a-129">**Kunden in den letzten 12** Monaten: Monatlicher Trend von Neukunden und Kunden mit Kundenabwanderung im Zeitraum der letzten 12 Monate aggregiert</span><span class="sxs-lookup"><span data-stu-id="75e0a-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="75e0a-130">Geschätzte Kosten nach Kunde in den letzten **12** Monaten: Kunden sortiert nach dem geschätzten Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 12 Monate.</span><span class="sxs-lookup"><span data-stu-id="75e0a-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="75e0a-131">Dieser Status gibt die wichtigsten Kunden an, die den größten Umsatz erzielen.</span><span class="sxs-lookup"><span data-stu-id="75e0a-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="75e0a-132">**Kundenanzahl nach Produkt:** Verkaufte Produkte sortiert nach zugeordneten Kunden.</span><span class="sxs-lookup"><span data-stu-id="75e0a-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="75e0a-133">Dieser Status gibt die wichtigsten Produkte an, die an die meisten Kunden verkauft werden.</span><span class="sxs-lookup"><span data-stu-id="75e0a-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="75e0a-134">Abonnement-Bericht</span><span class="sxs-lookup"><span data-stu-id="75e0a-134">Subscription Insights report</span></span>

- <span data-ttu-id="75e0a-135">**Abonnementstatus:**</span><span class="sxs-lookup"><span data-stu-id="75e0a-135">**Subscription status**:</span></span>

- <span data-ttu-id="75e0a-136">Aktiv: Abonnements, die entweder zum Zustand "Aktiv" oder "In Grace" gehören</span><span class="sxs-lookup"><span data-stu-id="75e0a-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="75e0a-137">Angehalten: Abonnements, die zum Status "Deaktiviert" gehören</span><span class="sxs-lookup"><span data-stu-id="75e0a-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="75e0a-138">Nicht mehr bereitgestellt: Abonnements, die zum Status "Bereitstellungslöschung" oder "Abgelaufen" gehören</span><span class="sxs-lookup"><span data-stu-id="75e0a-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="75e0a-139">**Ablaufstatus**:</span><span class="sxs-lookup"><span data-stu-id="75e0a-139">**Expiry status**:</span></span>

  - <span data-ttu-id="75e0a-140">Abgelaufen: Abonnements, die bereits abgelaufen sind (wobei das Enddatum des Abonnements in der Vergangenheit liegt)</span><span class="sxs-lookup"><span data-stu-id="75e0a-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="75e0a-141">Ablauf nach 30 Tagen: Abonnements, die nach 30 Tagen ablaufen (wobei das Enddatum des Abonnements nach den nächsten 30 Tagen liegt)</span><span class="sxs-lookup"><span data-stu-id="75e0a-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="75e0a-142">Ablauf in 30 Tagen: Abonnements, die innerhalb der nächsten 30 Tage ablaufen (wobei das Enddatum des Abonnements zwischen heute und den nächsten 30 Tagen liegt)</span><span class="sxs-lookup"><span data-stu-id="75e0a-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="75e0a-143">**Abonnements gesamt:** Abonnements im Status "Aktiv", "In Grace" oder "Deaktiviert"</span><span class="sxs-lookup"><span data-stu-id="75e0a-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="75e0a-144">**Neu (letzte 30 Tage):** Neue Abonnements, die von Kunden innerhalb der letzten 30 Tage erworben wurden</span><span class="sxs-lookup"><span data-stu-id="75e0a-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="75e0a-145">**Neu (letzte 24 Stunden):** Neue Abonnements, die von Kunden innerhalb der letzten 24 Stunden erworben wurden</span><span class="sxs-lookup"><span data-stu-id="75e0a-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="75e0a-146">**Ablauf in 30 Tagen:** Abonnements, die innerhalb der nächsten 30 Tage ablaufen</span><span class="sxs-lookup"><span data-stu-id="75e0a-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="75e0a-147">**Änderungsabwanderung (letzte 30 Tage):** Abonnements, deren Bereitstellung innerhalb der letzten 30 Tage aufgehoben oder angehalten (deaktiviert) wurde</span><span class="sxs-lookup"><span data-stu-id="75e0a-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="75e0a-148">**Verteilung nach Abonnementtypen:**% Verteilung der Gesamtabonnements nach lizenzbasiertem und nutzungsbasiertem Abonnementtyp</span><span class="sxs-lookup"><span data-stu-id="75e0a-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="75e0a-149">**Anzahl aktiver Abonnements nach Produkt:** Verkaufte Produkte sortiert nach anzahl aktiver Abonnements</span><span class="sxs-lookup"><span data-stu-id="75e0a-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="75e0a-150">**Abonnements in den letzten 12 Monaten:** Monatlicher Trend für neue Abonnements und Abwanderungsabonnements, aggregiert über den Zeitraum der letzten 12 Monate</span><span class="sxs-lookup"><span data-stu-id="75e0a-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="75e0a-151">**Details zum Kundenabonnement:** Detaillierte Ansicht der Kunden, Abonnements und Angebote</span><span class="sxs-lookup"><span data-stu-id="75e0a-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="75e0a-152">Lizenzbericht:</span><span class="sxs-lookup"><span data-stu-id="75e0a-152">License Insights report:</span></span>

- <span data-ttu-id="75e0a-153">**Gesamtanzahl der** Lizenzen: Gesamtzahl der Lizenzen, die für alle lizenzbasierten Abonnements aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="75e0a-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="75e0a-154">**Neu (letzte 30 Tage):** Lizenzer zusätzlich innerhalb der letzten 30 Tage</span><span class="sxs-lookup"><span data-stu-id="75e0a-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="75e0a-155">**Änderungsabwanderung (letzte 30 Tage):** Lizenzreduzierung innerhalb der letzten 30 Tage</span><span class="sxs-lookup"><span data-stu-id="75e0a-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="75e0a-156">**Neu (letzte 24 Stunden):** Lizenzer zusätzlich innerhalb der letzten 24 Stunden</span><span class="sxs-lookup"><span data-stu-id="75e0a-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="75e0a-157">**Lizenzen in den letzten 90 Tagen:** Monatlicher Trend von Lizenzermäßigungen und -reduzierungen, die monatlich über den Zeitraum der letzten 90 Tage aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="75e0a-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="75e0a-158">**Anzahl aktiver Lizenzen nach Produkt:** Verkaufte Produkte sortiert nach aktiver Lizenzanzahl</span><span class="sxs-lookup"><span data-stu-id="75e0a-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="75e0a-159">**Anzahl aktiver Lizenzen nach Kunde:** Kunden sortiert nach aktiver Lizenzanzahl</span><span class="sxs-lookup"><span data-stu-id="75e0a-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="75e0a-160">Details zu Kundenlizenzereignissen der letzten **90** Tage: Detaillierte Ansicht der Kunden-, Abonnement- und Abonnementereignisse, einschließlich Ereignisdatum, Ereignisname, Menge und Änderung der Menge.</span><span class="sxs-lookup"><span data-stu-id="75e0a-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="75e0a-161">Lizenznutzungsbericht:</span><span class="sxs-lookup"><span data-stu-id="75e0a-161">Licenses Usage report:</span></span>

- <span data-ttu-id="75e0a-162">**Nach Produkt zugewiesene Lizenzen:** Verkaufte Produkte sortiert nach Anzahl der Lizenzzuweisungen</span><span class="sxs-lookup"><span data-stu-id="75e0a-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="75e0a-163">**Nach Produkt verwendete Lizenzen:** Verkaufte Produkte sortiert nach Anzahl der Lizenznutzungen</span><span class="sxs-lookup"><span data-stu-id="75e0a-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="75e0a-164">**Kundenverteilung für zugewiesene Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenzzuweisung in Prozent</span><span class="sxs-lookup"><span data-stu-id="75e0a-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="75e0a-165">**Kundenverteilung für genutzte Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenznutzung in Prozent</span><span class="sxs-lookup"><span data-stu-id="75e0a-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="75e0a-166">**Vom Kunden zugewiesene Lizenzen:** Detaillierte Ansicht der verkauften lizenzen und von Kunden und Produkten zugewiesenen Lizenzen</span><span class="sxs-lookup"><span data-stu-id="75e0a-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="75e0a-167">**Vom Kunden verwendete Lizenzen:** Detaillierte Ansicht der verkauften Lizenzen und lizenzen, die von Kunden und Produkten verwendet werden</span><span class="sxs-lookup"><span data-stu-id="75e0a-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="75e0a-168">Azure-Bericht:</span><span class="sxs-lookup"><span data-stu-id="75e0a-168">Azure Insights report:</span></span>

- <span data-ttu-id="75e0a-169">**Nutzungsbasierte Kunden** in den letzten 12 Monaten: Monatlicher Trend von neuen nutzungsbasierten Kunden und kunden, die auf der nutzungsbasierten Kundenabwanderung basieren, die monatlich über den Zeitraum der letzten 12 Monate aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="75e0a-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="75e0a-170">**Nutzungsbasierte Abonnements** in den letzten 12 Monaten: Monatlicher Trend für neue nutzungsbasierte Abonnements und abwanderungsbasierte Abonnements, die monatlich über den Zeitraum der letzten 12 Monate aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="75e0a-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="75e0a-171">Geschätzte Nutzungskosten nach Kunde in den letzten **60** Tagen: Nutzungsbasierte Kunden, sortiert nach dem geschätzten Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="75e0a-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="75e0a-172">Dieser Status gibt die nutzungsbasierten Kunden an, die den meisten Umsatz erzielen.</span><span class="sxs-lookup"><span data-stu-id="75e0a-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="75e0a-173">Geschätzte Nutzungskosten nach Kategorie in den letzten **60** Tagen: Verbrauchsklassen nutzungsbasierter Abonnements, sortiert nach dem geschätzten Rechnungs-Dollarbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="75e0a-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="75e0a-174">Geschätzte Nutzungskosten nach Abonnement in den letzten **60** Tagen: Nutzungsbasierte Abonnements nach geschätztem Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="75e0a-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="75e0a-175">**Geschätzte Nutzungskosten des Kunden nach Ausgabenbudget:** Kunden werden nach Dem Prozentsatz ihres aktuellen Ausgabenbudgets sortiert, das den Schwellenwert überschreitet (100 %).</span><span class="sxs-lookup"><span data-stu-id="75e0a-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="75e0a-176">Azure-Ressourcennutzungsbericht:</span><span class="sxs-lookup"><span data-stu-id="75e0a-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="75e0a-177">**Nutzung von Azure-Ressourcen** nach Tag für den ausgewählten Zeitraum: Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="75e0a-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="75e0a-178">**Geschätzte Nutzungskosten** von Azure-Ressourcen für den ausgewählten Zeitraum: Geschätzte Kosten basierend auf der karte der neuesten Rate für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="75e0a-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="75e0a-179">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="75e0a-179">Next steps</span></span>

- [<span data-ttu-id="75e0a-180">Partner Center Analytics-App für Power BI – Übersicht</span><span class="sxs-lookup"><span data-stu-id="75e0a-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="75e0a-181">Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="75e0a-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
