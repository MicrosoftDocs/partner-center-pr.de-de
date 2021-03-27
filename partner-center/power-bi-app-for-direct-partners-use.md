---
title: Verwenden von Partner Center Analytics für Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Ihre Geschäftsdaten mithilfe der Partner Center Analytics-APP für Power BI anzeigen (für direkte Partner in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633861"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="f5037-103">Ihre Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI anzeigen</span><span class="sxs-lookup"><span data-stu-id="f5037-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="f5037-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="f5037-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f5037-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="f5037-105">Global admin</span></span>
- <span data-ttu-id="f5037-106">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="f5037-106">User management admin</span></span>
- <span data-ttu-id="f5037-107">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="f5037-107">Sales agent</span></span>
- <span data-ttu-id="f5037-108">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="f5037-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="f5037-109">Anzeigen Ihrer Geschäftsdaten</span><span class="sxs-lookup"><span data-stu-id="f5037-109">View your business data</span></span>

<span data-ttu-id="f5037-110">Nutzen Sie eine visuelle Darstellung Ihrer Daten mit der Partner Center Analytics-App für Power BI, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="f5037-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="f5037-111">Wachstum bei Kundenstamm, Abonnements und Lizenzen</span><span class="sxs-lookup"><span data-stu-id="f5037-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="f5037-112">Verwendung von Office 365-, Microsoft Dynamics- und Microsoft Azure-Produkten</span><span class="sxs-lookup"><span data-stu-id="f5037-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="f5037-113">Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem Azure-Abonnement in den letzten 60 Tagen</span><span class="sxs-lookup"><span data-stu-id="f5037-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="f5037-114">Geschätzte Kosten (auf Grundlage der aktuellen Gebührenkarte)</span><span class="sxs-lookup"><span data-stu-id="f5037-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="f5037-115">Möglichkeit zum Exportieren von Datasets und Erstellen von benutzerdefinierten Berichten, einschließlich pro Kunde.</span><span class="sxs-lookup"><span data-stu-id="f5037-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="f5037-116">Informationen zur Vorschauversion der Partner Center Analytics-App</span><span class="sxs-lookup"><span data-stu-id="f5037-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="f5037-117">Diese App ist nur für direkte Partner im Cloud Solution Provider-Programm gedacht.</span><span class="sxs-lookup"><span data-stu-id="f5037-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="f5037-118">Andere Partner im CSP (z. B. indirekte Wiederverkäufer) können sich nicht anmelden.</span><span class="sxs-lookup"><span data-stu-id="f5037-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="f5037-119">Alle geschätzten Kosten werden vor Steuern/Abrechnungsdaten angezeigt und sind nicht rechtlich bindend.</span><span class="sxs-lookup"><span data-stu-id="f5037-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="f5037-120">Die geschätzten Kosten dienen nur zu Informationszwecken.</span><span class="sxs-lookup"><span data-stu-id="f5037-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="f5037-121">Die Kundeninformationen basieren auf Abonnements.</span><span class="sxs-lookup"><span data-stu-id="f5037-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="f5037-122">Alle Kunden, für die Sie vor kurzem ein Konto erstellt haben, aber noch keine Abonnements haben, sind nicht in Zählungen enthalten.</span><span class="sxs-lookup"><span data-stu-id="f5037-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="f5037-123">Die geschätzten Kosten basiert auf der aktuellen Gebührenkarte, die auf den CSP-Preisen basiert.</span><span class="sxs-lookup"><span data-stu-id="f5037-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="f5037-124">Die Tage sind Kalendertage.</span><span class="sxs-lookup"><span data-stu-id="f5037-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="f5037-125">Geschäftsinformationen-Bericht</span><span class="sxs-lookup"><span data-stu-id="f5037-125">Business Insights report</span></span>

- <span data-ttu-id="f5037-126">**Kunden** Mandanten: Anzahl der unterschiedlichen Azure AD Mandanten von Kunden, die Abonnements erworben haben</span><span class="sxs-lookup"><span data-stu-id="f5037-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="f5037-127">**Neu (Letzte 30 Tage)**: neue Kunden kaufen mindestens ein Abonnement in den letzten 30 Tagen</span><span class="sxs-lookup"><span data-stu-id="f5037-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="f5037-128">Änderungs Rate **(Letzte 30 Tage)**: Kunden ohne die Abonnements "aktiv", "in der Toleranz" oder "deaktiviert"</span><span class="sxs-lookup"><span data-stu-id="f5037-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="f5037-129">**Neu (Letzte 24 Stunden)**: neue Kunden kaufen mindestens ein Abonnement in den letzten 24 Stunden</span><span class="sxs-lookup"><span data-stu-id="f5037-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="f5037-130">**Geschätzte monatliche Kosten in den letzten 12 Monaten**: Monat im Vergleich zum Monat im Vergleich zu einem monatlichen Betrag der geschätzten vorab Steuerrechnung, aggregiert im Verlauf der letzten 12 Monate</span><span class="sxs-lookup"><span data-stu-id="f5037-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f5037-131">**Geschätzte Kosten nach Produkt in den letzten 12 Monaten**: verkaufte Produkte nach geschätzten Dollarbetrag der vorab Steuerrechnung, aggregiert über den Zeitraum der letzten 12 Monate.</span><span class="sxs-lookup"><span data-stu-id="f5037-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="f5037-132">Dieser Status gibt an, dass die besten Produkte den größten Umsatz bringen.</span><span class="sxs-lookup"><span data-stu-id="f5037-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="f5037-133">Kunden, die sich **in den letzten 12 Monaten im** Vergleich zu einem Monat im Vergleich zu einem Monat im Vergleich zu den letzten 12 Monaten aggregiert haben</span><span class="sxs-lookup"><span data-stu-id="f5037-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f5037-134">**Geschätzte Kosten nach Kunde in den letzten 12 Monaten**: Kunden, die nach dem geschätzten Dollarbetrag der vorab Steuerrechnung sortiert wurden, der über den Zeitraum der letzten 12 Monate aggregiert wurde.</span><span class="sxs-lookup"><span data-stu-id="f5037-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="f5037-135">Dieser Status gibt an, dass Top-Kunden die meisten Umsätze einbringen.</span><span class="sxs-lookup"><span data-stu-id="f5037-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="f5037-136">**Kundenanzahl nach Produkt**: verkaufte Produkte nach zugeordneten Kunden.</span><span class="sxs-lookup"><span data-stu-id="f5037-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="f5037-137">Dieser Status gibt an, dass die meisten Kunden die besten Produkte verkauft haben.</span><span class="sxs-lookup"><span data-stu-id="f5037-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="f5037-138">Abonnement-Bericht</span><span class="sxs-lookup"><span data-stu-id="f5037-138">Subscription Insights report</span></span>

- <span data-ttu-id="f5037-139">**Abonnement Status**:</span><span class="sxs-lookup"><span data-stu-id="f5037-139">**Subscription status**:</span></span>

- <span data-ttu-id="f5037-140">Aktiv: Abonnements, die entweder zum Zustand "aktiv" oder "in der Toleranz" gehören</span><span class="sxs-lookup"><span data-stu-id="f5037-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="f5037-141">Angehalten: Abonnements, die zum Zustand "deaktiviert" gehören</span><span class="sxs-lookup"><span data-stu-id="f5037-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="f5037-142">Aufhebung der Bereitstellung: Abonnements, die zum Status "bereitgestellt" oder "abgelaufen" gehören.</span><span class="sxs-lookup"><span data-stu-id="f5037-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="f5037-143">**Ablaufstatus**:</span><span class="sxs-lookup"><span data-stu-id="f5037-143">**Expiry status**:</span></span>

  - <span data-ttu-id="f5037-144">Abgelaufen: Abonnements, die bereits abgelaufen sind (wobei das Enddatum des Abonnements in der Vergangenheit liegt)</span><span class="sxs-lookup"><span data-stu-id="f5037-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="f5037-145">Läuft nach 30 Tagen ab: Abonnements, die nach 30 Tagen ablaufen (wobei das Enddatum des Abonnements nach den nächsten 30 Tagen liegt)</span><span class="sxs-lookup"><span data-stu-id="f5037-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="f5037-146">Läuft innerhalb von 30 Tagen ab: Abonnements, die innerhalb der nächsten 30 Tage ablaufen (wobei das Enddatum des Abonnements zwischen heute und 30 Tagen liegt)</span><span class="sxs-lookup"><span data-stu-id="f5037-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="f5037-147">**Abonnements Gesamt**: Abonnements im Status "aktiv", "in der Toleranz" oder "deaktiviert"</span><span class="sxs-lookup"><span data-stu-id="f5037-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="f5037-148">**Neu (Letzte 30 Tage)**: neue Abonnements, die innerhalb der letzten 30 Tage von Kunden erworben wurden</span><span class="sxs-lookup"><span data-stu-id="f5037-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="f5037-149">**Neu (Letzte 24 Stunden)**: neue Abonnements, die innerhalb der letzten 24 Stunden von Kunden erworben wurden</span><span class="sxs-lookup"><span data-stu-id="f5037-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="f5037-150">Läuft innerhalb von **30 Tagen** ab: Abonnements, die innerhalb der nächsten 30 Tage ablaufen</span><span class="sxs-lookup"><span data-stu-id="f5037-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="f5037-151">Änderungs Rate **(Letzte 30 Tage)**: Abonnements, die innerhalb der letzten 30 Tage deaktiviert oder angehalten (deaktiviert) wurden.</span><span class="sxs-lookup"><span data-stu-id="f5037-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="f5037-152">**Verteilung nach Abonnementtypen**:% Verteilung der Abonnements Gesamt gemäß Lizenz basiert und Nutzungs basierter Abonnementtyp</span><span class="sxs-lookup"><span data-stu-id="f5037-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="f5037-153">**Anzahl aktiver Abonnements nach Produkt**: verkaufte Produkte sortiert nach Anzahl aktiver Abonnements</span><span class="sxs-lookup"><span data-stu-id="f5037-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="f5037-154">**Abonnements im Vergleich zu den letzten 12 Monaten**: Monat im Vergleich zu einem Monat im Vergleich zu den in den letzten 12 Monaten monatlich aggregierten Abonnements und Änderungs Abonnements</span><span class="sxs-lookup"><span data-stu-id="f5037-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f5037-155">**Kunden Abonnement Details**: detaillierte Ansicht der Kunden, Abonnements und Angebote</span><span class="sxs-lookup"><span data-stu-id="f5037-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="f5037-156">Lizenzbericht:</span><span class="sxs-lookup"><span data-stu-id="f5037-156">License Insights report:</span></span>

- <span data-ttu-id="f5037-157">**Lizenzen Gesamt**: Gesamtzahl der Lizenzen, die über alle lizenzbasierten Abonnements aggregiert werden</span><span class="sxs-lookup"><span data-stu-id="f5037-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="f5037-158">**Neu (Letzte 30 Tage)**: Lizenz Addition innerhalb der letzten 30 Tage</span><span class="sxs-lookup"><span data-stu-id="f5037-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="f5037-159">Änderungs Rate **(Letzte 30 Tage)**: Lizenz Reduzierung innerhalb der letzten 30 Tage</span><span class="sxs-lookup"><span data-stu-id="f5037-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="f5037-160">**Neu (Letzte 24 Stunden)**: Hinzufügen von Lizenzen innerhalb der letzten 24 Stunden</span><span class="sxs-lookup"><span data-stu-id="f5037-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="f5037-161">**Lizenzen im Verlauf der letzten 90 Tage**: Monat im Vergleich zum Monat im Vergleich zum Zeitraum der letzten 90 Tage monatlich aggregiert</span><span class="sxs-lookup"><span data-stu-id="f5037-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="f5037-162">**Anzahl aktiver Lizenzen nach Produkt**: verkaufte Produkte sortiert nach aktiver Lizenz Anzahl</span><span class="sxs-lookup"><span data-stu-id="f5037-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="f5037-163">**Anzahl aktiver Lizenzen nach Kunde**: nach aktiver Lizenz Anzahl sortierte Kunden</span><span class="sxs-lookup"><span data-stu-id="f5037-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="f5037-164">Details zu Kunden Lizenz Ereignissen im Verlauf der **letzten 90 Tage**: ausführliche Ansicht der Kunden, Abonnements und Abonnement Ereignisse einschließlich Ereignis Datum, Ereignis Name, Menge und Änderung der Menge.</span><span class="sxs-lookup"><span data-stu-id="f5037-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="f5037-165">Lizenznutzungsbericht:</span><span class="sxs-lookup"><span data-stu-id="f5037-165">Licenses Usage report:</span></span>

- <span data-ttu-id="f5037-166">**Vom Produkt zugewiesene Lizenzen**: verkaufte Produkte sortiert nach Lizenz Zuweisungs Anzahl</span><span class="sxs-lookup"><span data-stu-id="f5037-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="f5037-167">**Von Produkt verwendete Lizenzen**: verkaufte Produkte nach Lizenz Verwendungs Anzahl</span><span class="sxs-lookup"><span data-stu-id="f5037-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="f5037-168">**Kundenverteilung für zugewiesene Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenzzuweisung in Prozent</span><span class="sxs-lookup"><span data-stu-id="f5037-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="f5037-169">**Kundenverteilung für genutzte Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenznutzung in Prozent</span><span class="sxs-lookup"><span data-stu-id="f5037-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="f5037-170">**Vom Kunden zugewiesene Lizenzen**: ausführliche Ansicht der verkauften Lizenzen und von Kunden und Produkten zugewiesene Lizenzen</span><span class="sxs-lookup"><span data-stu-id="f5037-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="f5037-171">**Von Customer verwendete Lizenzen**: Ausführliche Übersicht über verkaufte Lizenzen und von Kunden und Produkten verwendete Lizenzen</span><span class="sxs-lookup"><span data-stu-id="f5037-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="f5037-172">Azure-Bericht:</span><span class="sxs-lookup"><span data-stu-id="f5037-172">Azure Insights report:</span></span>

- <span data-ttu-id="f5037-173">**Nutzungsbasierte Kunden in den letzten 12 Monaten**: Monat im Vergleich zu einem Monat im Vergleich zu neuen nutzungsbasierten Kunden und nutzungsbasierten nutzungsbasierten Kunden, die monatlich im Zeitraum der letzten 12 Monate aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="f5037-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f5037-174">**Nutzungsbasierte Abonnements in den letzten 12 Monaten**: Monat im Vergleich zu einem Monat im Vergleich zu neuen Verwendungs basierten Abonnements und nutzungsbasierten Abonnements, die monatlich im Zeitraum der letzten 12 Monate aggregiert wurden</span><span class="sxs-lookup"><span data-stu-id="f5037-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f5037-175">**Geschätzte Kosten der Nutzung durch Kunden in den letzten 60 Tagen**: nutzungsbasierte Kunden, sortiert nach geschätzter Dollarbetrag der vorab Steuerrechnung, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="f5037-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="f5037-176">Dieser Status gibt an, dass die besten nutzungsbasierten Kunden die meisten Umsätze einbringen.</span><span class="sxs-lookup"><span data-stu-id="f5037-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="f5037-177">**Geschätzte Kosten der Nutzung nach Kategorie im Verlauf der letzten 60 Tage**: Verbrauchs Kategorien von Verwendungs basierten Abonnements, sortiert nach geschätzten Dollarbetrag der vorab Steuerrechnung, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="f5037-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="f5037-178">**Geschätzte Kosten der Nutzung nach Abonnement im Verlauf der letzten 60 Tage**: nutzungsbasierte Abonnements nach geschätzter Dollarbetrag der vorab Steuerrechnung, aggregiert über den Zeitraum der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="f5037-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="f5037-179">**Geschätzte Nutzung der Kunden nach Ausgabenbudget**: Kunden, geordnet nach Prozentsatz Ihres aktuellen Ausgabenbudgets, das den Schwellenwert überschreitet (100%).</span><span class="sxs-lookup"><span data-stu-id="f5037-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="f5037-180">Azure-Ressourcennutzungsbericht:</span><span class="sxs-lookup"><span data-stu-id="f5037-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="f5037-181">**Nutzung von Azure-Ressourcen nach Tag für den ausgewählten Zeitraum**: tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="f5037-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="f5037-182">**Geschätzte Nutzungskosten der Azure-Ressourcen für den ausgewählten Zeitraum**: geschätzte Kosten basierend auf der aktuellen Preiskarte für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.</span><span class="sxs-lookup"><span data-stu-id="f5037-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f5037-183">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f5037-183">Next steps</span></span>

- [<span data-ttu-id="f5037-184">Partner Center Analytics-App für Power BI – Übersicht</span><span class="sxs-lookup"><span data-stu-id="f5037-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="f5037-185">Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="f5037-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
