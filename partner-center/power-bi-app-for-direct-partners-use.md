---
title: Verwenden Partner Center Analytics für Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Ihre Geschäftsdaten mithilfe der Partner Center Analytics-App für Power BI (für direkte Partner in CSP) anzeigen.
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855028"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="bb5f9-103">Ihre Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI anzeigen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="bb5f9-104">**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Sales agent | Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="bb5f9-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="bb5f9-105">Anzeigen Ihrer Geschäftsdaten</span><span class="sxs-lookup"><span data-stu-id="bb5f9-105">View your business data</span></span>

<span data-ttu-id="bb5f9-106">Nutzen Sie eine visuelle Darstellung Ihrer Daten mit der Partner Center Analytics-App für Power BI, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="bb5f9-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="bb5f9-107">Wachstum bei Kundenstamm, Abonnements und Lizenzen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="bb5f9-108">Verwendung von Office 365-, Microsoft Dynamics- und Microsoft Azure-Produkten</span><span class="sxs-lookup"><span data-stu-id="bb5f9-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="bb5f9-109">Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem Azure-Abonnement in den letzten 60 Tagen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="bb5f9-110">Geschätzte Kosten (auf Grundlage der aktuellen Gebührenkarte)</span><span class="sxs-lookup"><span data-stu-id="bb5f9-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="bb5f9-111">Möglichkeit zum Exportieren von Datasets und Erstellen benutzerdefinierter Berichte, einschließlich pro Kunde.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="bb5f9-112">Informationen zur Vorschauversion der Partner Center Analytics-App</span><span class="sxs-lookup"><span data-stu-id="bb5f9-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="bb5f9-113">Diese App ist nur für direkte Partner im Cloud Solution Provider-Programm gedacht.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="bb5f9-114">Andere Partner im CSP (z. B. indirekte Wiederverkäufer) können sich nicht anmelden.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="bb5f9-115">Alle geschätzten Kosten werden vor Steuern/Abrechnungsdaten angezeigt und sind nicht rechtlich bindend.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="bb5f9-116">Die geschätzten Kosten dienen nur zu Informationszwecken.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="bb5f9-117">Die Kundeninformationen basieren auf Abonnements.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="bb5f9-118">Alle Kunden, für die Sie vor Kurzem Konten erstellt haben, aber noch keine Abonnements haben, werden nicht in die Anzahl einbezogen.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="bb5f9-119">Die geschätzten Kosten basiert auf der aktuellen Gebührenkarte, die auf den CSP-Preisen basiert.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="bb5f9-120">Die Tage sind Kalendertage.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="bb5f9-121">Geschäftsinformationen-Bericht</span><span class="sxs-lookup"><span data-stu-id="bb5f9-121">Business Insights report</span></span>

- <span data-ttu-id="bb5f9-122">**Kunden-Mandanten:** Anzahl unterschiedlicher Azure AD Mandanten von Kunden, die Abonnements erworben haben</span><span class="sxs-lookup"><span data-stu-id="bb5f9-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="bb5f9-123">**Neu (letzte 30 Tage):** Neue Kunden, die in den letzten 30 Tagen mindestens ein Abonnement erwerben</span><span class="sxs-lookup"><span data-stu-id="bb5f9-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="bb5f9-124">**Änderungsabwanderung (letzte 30 Tage):** Kunden ohne "aktive", "in Grace"- oder "deaktivierte" Abonnements</span><span class="sxs-lookup"><span data-stu-id="bb5f9-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="bb5f9-125">**Neu (letzte 24 Stunden):** Neue Kunden, die in den letzten 24 Stunden mindestens ein Abonnement erwerben</span><span class="sxs-lookup"><span data-stu-id="bb5f9-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="bb5f9-126">Geschätzte monatliche Kosten in den letzten **12** Monaten: Trend von Monat zu Monat des geschätzten Rechnungsbetrags vor Steuern, der monatlich über den Zeitraum der letzten 12 Monate aggregiert wurde</span><span class="sxs-lookup"><span data-stu-id="bb5f9-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bb5f9-127">Geschätzte Kosten nach Produkt in den letzten **12** Monaten: Verkaufte Produkte sortiert nach geschätztem Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 12 Monate.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="bb5f9-128">Dieser Status gibt die wichtigsten Produkte an, die den größten Umsatz bringen.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="bb5f9-129">**Kunden in den letzten 12** Monaten: Monatlicher Trend von Neukunden und Abwanderungskunden im Zeitraum der letzten 12 Monate aggregiert</span><span class="sxs-lookup"><span data-stu-id="bb5f9-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bb5f9-130">Geschätzte Kosten nach Kunde in den letzten **12** Monaten: Kunden sortiert nach dem geschätzten Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 12 Monate.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="bb5f9-131">Dieser Status gibt die wichtigsten Kunden an, die den größten Umsatz erzielen.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="bb5f9-132">**Kundenanzahl nach Produkt:** Verkaufte Produkte sortiert nach zugeordneten Kunden.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="bb5f9-133">Dieser Status gibt die wichtigsten Produkte an, die an die meisten Kunden verkauft werden.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="bb5f9-134">Abonnement-Bericht</span><span class="sxs-lookup"><span data-stu-id="bb5f9-134">Subscription Insights report</span></span>

- <span data-ttu-id="bb5f9-135">**Abonnementstatus:**</span><span class="sxs-lookup"><span data-stu-id="bb5f9-135">**Subscription status**:</span></span>

- <span data-ttu-id="bb5f9-136">Aktiv: Abonnements, die entweder zum Zustand "aktiv" oder "in Grace" gehören</span><span class="sxs-lookup"><span data-stu-id="bb5f9-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="bb5f9-137">Angehalten: Abonnements, die zum Status "Deaktiviert" gehören</span><span class="sxs-lookup"><span data-stu-id="bb5f9-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="bb5f9-138">Bereitstellung aufgehoben: Abonnements, die zum Status "Bereitstellung aufgehoben" oder "Abgelaufen" gehören</span><span class="sxs-lookup"><span data-stu-id="bb5f9-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="bb5f9-139">**Ablaufstatus**:</span><span class="sxs-lookup"><span data-stu-id="bb5f9-139">**Expiry status**:</span></span>

  - <span data-ttu-id="bb5f9-140">Abgelaufen: Abonnements, die bereits abgelaufen sind (das Enddatum des Abonnements liegt in der Vergangenheit)</span><span class="sxs-lookup"><span data-stu-id="bb5f9-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="bb5f9-141">Ablauf nach 30 Tagen: Abonnements, die nach 30 Tagen ablaufen (wobei das Enddatum des Abonnements nach den nächsten 30 Tagen liegt)</span><span class="sxs-lookup"><span data-stu-id="bb5f9-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="bb5f9-142">Ablauf in 30 Tagen: Abonnements, die innerhalb der nächsten 30 Tage ablaufen (wobei das Enddatum des Abonnements zwischen heute und den nächsten 30 Tagen liegt)</span><span class="sxs-lookup"><span data-stu-id="bb5f9-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="bb5f9-143">**Abonnements gesamt:** Abonnements mit dem Status "aktiv", "ordnungsgemäß" oder "deaktiviert"</span><span class="sxs-lookup"><span data-stu-id="bb5f9-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="bb5f9-144">**Neu (letzte 30 Tage):** Neue Abonnements, die von Kunden innerhalb der letzten 30 Tage erworben wurden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="bb5f9-145">**Neu (letzte 24 Stunden):** Neue Abonnements, die von Kunden innerhalb der letzten 24 Stunden erworben wurden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="bb5f9-146">**Ablauf in 30 Tagen:** Abonnements, die innerhalb der nächsten 30 Tage ablaufen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="bb5f9-147">**Änderungsrate (letzte 30 Tage):** Abonnements, die innerhalb der letzten 30 Tage nicht mehr bereitgestellt oder angehalten (deaktiviert) wurden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="bb5f9-148">**Verteilung nach Abonnementtypen:**% Verteilung der Gesamtabonnements nach lizenzbasiertem und nutzungsbasiertem Abonnementtyp</span><span class="sxs-lookup"><span data-stu-id="bb5f9-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="bb5f9-149">**Anzahl aktiver Abonnements nach Produkt:** Verkaufte Produkte sortiert nach Anzahl aktiver Abonnements</span><span class="sxs-lookup"><span data-stu-id="bb5f9-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="bb5f9-150">**Abonnements über die letzten 12 Monate:** Monatlicher Trend neuer Abonnements und Abwanderungsabonnements, die im Zeitraum der letzten 12 Monate monatlich aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bb5f9-151">**Details zum Kundenabonnement:** Detaillierte Ansicht der Kunden, Abonnements und Angebote</span><span class="sxs-lookup"><span data-stu-id="bb5f9-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="bb5f9-152">Lizenzbericht:</span><span class="sxs-lookup"><span data-stu-id="bb5f9-152">License Insights report:</span></span>

- <span data-ttu-id="bb5f9-153">**Lizenzen gesamt:** Gesamtanzahl von Lizenzen, die über alle lizenzbasierten Abonnements aggregiert werden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="bb5f9-154">**Neu (letzte 30 Tage):** Lizenzerweiterung innerhalb der letzten 30 Tage</span><span class="sxs-lookup"><span data-stu-id="bb5f9-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="bb5f9-155">**Änderungsrate (letzte 30 Tage):** Lizenzverringerung innerhalb der letzten 30 Tage</span><span class="sxs-lookup"><span data-stu-id="bb5f9-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="bb5f9-156">**Neu (letzte 24 Stunden):** Lizenzerweiterung innerhalb der letzten 24 Stunden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="bb5f9-157">**Lizenzen über die letzten 90 Tage:** Monatlicher Trend von Lizenzzufügungen und -reduzierungen, der monatlich über den Zeitraum der letzten 90 Tage aggregiert wurde</span><span class="sxs-lookup"><span data-stu-id="bb5f9-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="bb5f9-158">**Anzahl der aktiven Lizenzen nach Produkt:** Verkaufte Produkte sortiert nach Anzahl aktiver Lizenzen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="bb5f9-159">**Anzahl der aktiven Lizenzen nach Kunde:** Kunden sortiert nach anzahl aktiver Lizenzen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="bb5f9-160">Details zu Kundenlizenzereignissen der letzten **90** Tage: Detaillierte Ansicht der Kunden-, Abonnement- und Abonnementereignisse, einschließlich Ereignisdatum, Ereignisname, Menge und Änderung der Menge.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="bb5f9-161">Lizenznutzungsbericht:</span><span class="sxs-lookup"><span data-stu-id="bb5f9-161">Licenses Usage report:</span></span>

- <span data-ttu-id="bb5f9-162">**Nach Produkt zugewiesene Lizenzen:** Verkaufte Produkte sortiert nach Anzahl der Lizenzzuweisungen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="bb5f9-163">**Nach Produkt verwendete Lizenzen:** Verkaufte Produkte sortiert nach Anzahl der Lizenznutzungen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="bb5f9-164">**Kundenverteilung für zugewiesene Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenzzuweisung in Prozent</span><span class="sxs-lookup"><span data-stu-id="bb5f9-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="bb5f9-165">**Kundenverteilung für genutzte Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenznutzung in Prozent</span><span class="sxs-lookup"><span data-stu-id="bb5f9-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="bb5f9-166">**Vom Kunden zugewiesene Lizenzen:** Detaillierte Ansicht der verkauften lizenzen und von Kunden und Produkten zugewiesenen Lizenzen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="bb5f9-167">**Vom Kunden verwendete Lizenzen:** Detaillierte Ansicht der verkauften lizenzen und von Kunden und Produkten verwendeten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="bb5f9-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="bb5f9-168">Azure-Bericht:</span><span class="sxs-lookup"><span data-stu-id="bb5f9-168">Azure Insights report:</span></span>

- <span data-ttu-id="bb5f9-169">**Nutzungsbasierte Kunden** in den letzten 12 Monaten: Monatlicher Trend von neuen nutzungsbasierten Kunden und kunden, die auf der nutzungsbasierten Kundenabwanderung basieren, die monatlich über den Zeitraum der letzten 12 Monate aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bb5f9-170">**Nutzungsbasierte Abonnements** in den letzten 12 Monaten: Monatlicher Trend für neue nutzungsbasierte Abonnements und abwanderungsbasierte Abonnements, die monatlich über den Zeitraum der letzten 12 Monate aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="bb5f9-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bb5f9-171">Geschätzte Nutzungskosten nach Kunde in den letzten **60** Tagen: Nutzungsbasierte Kunden, sortiert nach dem geschätzten Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="bb5f9-172">Dieser Status gibt die nutzungsbasierten Kunden an, die den meisten Umsatz erzielen.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="bb5f9-173">Geschätzte Nutzungskosten nach Kategorie in den letzten **60** Tagen: Verbrauchsklassen nutzungsbasierter Abonnements, sortiert nach dem geschätzten Rechnungs-Dollarbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="bb5f9-174">Geschätzte Nutzungskosten nach Abonnement in den letzten **60** Tagen: Nutzungsbasierte Abonnements nach geschätztem Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="bb5f9-175">**Geschätzte Nutzungskosten des Kunden nach Ausgabenbudget:** Kunden werden nach Dem Prozentsatz ihres aktuellen Ausgabenbudgets sortiert, das den Schwellenwert überschreitet (100 %).</span><span class="sxs-lookup"><span data-stu-id="bb5f9-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="bb5f9-176">Azure-Ressourcennutzungsbericht:</span><span class="sxs-lookup"><span data-stu-id="bb5f9-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="bb5f9-177">**Nutzung von Azure-Ressourcen** nach Tag für den ausgewählten Zeitraum: Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="bb5f9-178">**Geschätzte Nutzungskosten von Azure-Ressourcen für den ausgewählten Zeitraum:** Geschätzte Kosten basierend auf der karte mit der neuesten Rate für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="bb5f9-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bb5f9-179">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="bb5f9-179">Next steps</span></span>

- [<span data-ttu-id="bb5f9-180">Partner Center Analytics-App für Power BI – Übersicht</span><span class="sxs-lookup"><span data-stu-id="bb5f9-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="bb5f9-181">Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="bb5f9-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
