---
title: Azure-Reservierungen & Server-Abonnements
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Möglichkeiten von Cloud Solution Provider zum Abrufen, bereitstellen und Verwalten von Azure-Reservierungen und Server Abonnements für Kunden.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b8a9cf07f8dace47346c68ade3707d6b12a1532
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900089"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="e04a1-103">Erwerben, bereitstellen und & Verwalten von reservierten Azure-VM-Instanzen (RI) und Server Abonnements für Kunden</span><span class="sxs-lookup"><span data-stu-id="e04a1-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="e04a1-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="e04a1-104">Applies to:</span></span>

- <span data-ttu-id="e04a1-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e04a1-105">Partner Center</span></span>

<span data-ttu-id="e04a1-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="e04a1-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e04a1-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="e04a1-107">Admin agent</span></span>
- <span data-ttu-id="e04a1-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="e04a1-108">Global admin</span></span>
- <span data-ttu-id="e04a1-109">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="e04a1-109">Helpdesk agent</span></span>
- <span data-ttu-id="e04a1-110">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="e04a1-110">Sales agent</span></span>
- <span data-ttu-id="e04a1-111">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="e04a1-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="e04a1-112">Dieser Artikel gilt nur für Partner im CSP-Programm (Cloud Solution Provider).</span><span class="sxs-lookup"><span data-stu-id="e04a1-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="e04a1-113">Kunden, die andere Abonnementtypen (z. b. Pay-as-you-go, individuelle, Microsoft-Kunden Vereinbarung oder Konzernvertrag Abonnements) verwenden, sollten stattdessen [diese Azure-Reservierungs Dokumentation](https://docs.microsoft.com/azure/cost-management-billing/reservations)lesen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="e04a1-114">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="e04a1-114">What are Azure Reservations?</span></span>

<span data-ttu-id="e04a1-115">Mit Azure Reservations können Sie Geld sparen, indem Sie für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Azure-Ressourcen ein oder drei Jahre im Voraus bezahlen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="e04a1-116">Durch die Vorabzahlung können Sie einen Rabatt für die Ressourcen, die Sie nutzen, in Anspruch nehmen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="e04a1-117">Reservations ermöglicht Ihnen eine deutliche Reduzierung Ihrer Kosten für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Ressourcen um bis zu 72 % im Vergleich zu nutzungsbasierten Preisen (Pay-As-You-Go).</span><span class="sxs-lookup"><span data-stu-id="e04a1-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="e04a1-118">Reservierungen bieten einen Abrechnungsrabatt und wirken sich nicht auf den Laufzeitstatus Ihrer Ressourcen aus.</span><span class="sxs-lookup"><span data-stu-id="e04a1-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="e04a1-119">Weitere Informationen finden Sie [unter Was ist Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="e04a1-119">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="e04a1-120">Warum sollten Kunden eine Reservierung kaufen?</span><span class="sxs-lookup"><span data-stu-id="e04a1-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="e04a1-121">Wenn Kunden über virtuelle Computer, Azure Cosmos DB oder SQL-Datenbanken verfügen, die über längere Zeiträume betrieben werden, stellt der Erwerb einer Reservierung für sie die kostengünstigste Option dar.</span><span class="sxs-lookup"><span data-stu-id="e04a1-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="e04a1-122">Wenn ein Kunde z. B. kontinuierlich vier Instanzen eines Diensts ohne Reservierung ausführt, erfolgt eine nutzungsbasierte Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="e04a1-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="e04a1-123">Wenn sie eine Reservierung für diese Ressourcen kaufen, erhalten sie sofort den Reservierungsrabatt.</span><span class="sxs-lookup"><span data-stu-id="e04a1-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="e04a1-124">Die Ressourcen werden nicht mehr mit den Gebühren für die nutzungsbasierte Bezahlung in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="e04a1-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="e04a1-125">Faszinierende neue Azure-Angebote in CSP</span><span class="sxs-lookup"><span data-stu-id="e04a1-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="e04a1-126">Durch das Hinzufügen von Azure Reservations und Server-Abonnements in das CSP-Programm, unterstützt Microsoft unsere Partner mit der schnell wachsenden Kundennachfrage für kostengünstigere Lösungen zur Unterstützung von verlässlichen, permanenten Cloud-Workloads.</span><span class="sxs-lookup"><span data-stu-id="e04a1-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="e04a1-127">Mit dem CSP-Programm können Partner Azure Reservations-und Server Abonnements im Auftrag von kommerziellen Kunden über das Microsoft Partner Center und Azure-Portal erwerben, bereitstellen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="e04a1-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="e04a1-128">Wir haben unseren Partner im CSP-Programm sogar die Wahl, wie Azure-Reservierungen erworben werden können.</span><span class="sxs-lookup"><span data-stu-id="e04a1-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="e04a1-129">CSP-Partner können [Azure-Reservierungen im Auftrag eines Kunden erwerben](azure-reservations-buying.md) oder [dem Kunden ermöglichen, seine eigenen Reservierungen](give-customers-permission.md) von einem früheren Azure-Abonnement zu erwerben, das der Partner für Sie erworben hat.</span><span class="sxs-lookup"><span data-stu-id="e04a1-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="e04a1-130">Azure Reservations bieten Kunden die Flexibilität der Virtualisierung für eine Vielzahl von Computing-Lösungen, einschließlich der Entwicklung und dem Ausführen von Testanwendungen und dem erweitern des Rechenzentrums.</span><span class="sxs-lookup"><span data-stu-id="e04a1-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="e04a1-131">Beispielsweise können gewerbliche Kunden jetzt bis zu 72% im Vergleich zu Preisen für Azure-VMS [Azure reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) mit Nutzungs basierter Bezahlung sparen, indem Sie den virtuellen Computer für einen Zeitraum von 1 bis 3 Jahren erwerben oder "Reservieren".</span><span class="sxs-lookup"><span data-stu-id="e04a1-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="e04a1-132">Windows Server-Kunden mit Azure-Hybridvorteil und Software Assurance können bis zu 80 % im Vergleich zu nutzungsbasierten Preisen sparen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="e04a1-133">Mit einer unglaublichen Kombination aus einem überzeugenden Preis und beispielloser Bereitstellungsflexibilität erhalten Kunden den besten Gesamtwert, wenn sie Azure Reservations zusammen mit Server-Abonnements auswählen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="e04a1-134">Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="e04a1-134">Azure reservations</span></span>

- <span data-ttu-id="e04a1-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="e04a1-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="e04a1-136">SQL DB Reservations</span><span class="sxs-lookup"><span data-stu-id="e04a1-136">SQL DB Reservations</span></span>
- <span data-ttu-id="e04a1-137">Verwaltete SQL-Instanz</span><span class="sxs-lookup"><span data-stu-id="e04a1-137">SQL Managed Instance</span></span>
- <span data-ttu-id="e04a1-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e04a1-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="e04a1-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="e04a1-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="e04a1-140">App-Dienste</span><span class="sxs-lookup"><span data-stu-id="e04a1-140">App Services</span></span>
- <span data-ttu-id="e04a1-141">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="e04a1-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="e04a1-142">Verwalteter Datenträger</span><span class="sxs-lookup"><span data-stu-id="e04a1-142">Managed Disk</span></span>
- <span data-ttu-id="e04a1-143">Blockblob</span><span class="sxs-lookup"><span data-stu-id="e04a1-143">Block blob</span></span>
- <span data-ttu-id="e04a1-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="e04a1-144">MySQL</span></span>
- <span data-ttu-id="e04a1-145">Azure-Daten-Explorer</span><span class="sxs-lookup"><span data-stu-id="e04a1-145">Azure Data explorer</span></span>
- <span data-ttu-id="e04a1-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="e04a1-146">MariaDB</span></span>
- <span data-ttu-id="e04a1-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="e04a1-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="e04a1-148">Server Abonnements</span><span class="sxs-lookup"><span data-stu-id="e04a1-148">Server subscriptions</span></span>

- <span data-ttu-id="e04a1-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="e04a1-149">Windows Server</span></span>
- <span data-ttu-id="e04a1-150">Remotedesktopdienste-CALs (RDS)</span><span class="sxs-lookup"><span data-stu-id="e04a1-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="e04a1-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="e04a1-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="e04a1-152">Jährliche Linux-ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="e04a1-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="e04a1-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="e04a1-153">SUSE Linux</span></span>
- <span data-ttu-id="e04a1-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="e04a1-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="e04a1-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="e04a1-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="e04a1-156">Jährliche ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="e04a1-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="e04a1-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="e04a1-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="e04a1-158">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="e04a1-158">Getting started</span></span>

<span data-ttu-id="e04a1-159">Um zu verstehen, wie Sie Azure Reservations mit ihren Kunden positionieren und so schnell wie möglich in Betrieb nehmen können, wird der folgende Ansatz empfohlen, um die Bereitschafts Materialien zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="e04a1-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="e04a1-160">Schauen Sie sich die Überblickspräsentationen und die zugehörigen Webinare für die Kundennutzung und Positionierung an.</span><span class="sxs-lookup"><span data-stu-id="e04a1-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="e04a1-161">Lesen Sie das Handbuch für modernes E-Commerce.</span><span class="sxs-lookup"><span data-stu-id="e04a1-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="e04a1-162">Schauen Sie sich die häufig gestellten Fragen zu Azure RI und Server-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="e04a1-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="e04a1-163">Verstehen Sie die Updates für Azure Reservations und Server-Abonnements im [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="e04a1-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="e04a1-164">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="e04a1-164">Resources</span></span>

<span data-ttu-id="e04a1-165">Im Folgenden finden Sie eine umfassende Liste der Ressourcen, die Ihnen helfen, Azure Reservations über Partner Center-Partner schnell zu integrieren:</span><span class="sxs-lookup"><span data-stu-id="e04a1-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="e04a1-166">Vertriebsbereitschaft</span><span class="sxs-lookup"><span data-stu-id="e04a1-166">Sales readiness</span></span>

- [<span data-ttu-id="e04a1-167">Azure Reservations und Server Abonnements mit Azure-Hybridvorteil Übersicht</span><span class="sxs-lookup"><span data-stu-id="e04a1-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="e04a1-168">Verkaufsblatt</span><span class="sxs-lookup"><span data-stu-id="e04a1-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="e04a1-169">FAQ zu Partnern für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="e04a1-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="e04a1-170">Häufig gestellte Fragen für Azure Reservations- und SQL DB-Partner</span><span class="sxs-lookup"><span data-stu-id="e04a1-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="e04a1-171">Remotedesktopdienste (RDS)-Client Zugriffslizenz (CAL) (Ankündigung)</span><span class="sxs-lookup"><span data-stu-id="e04a1-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="e04a1-172">Azure reserved VM Instances (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="e04a1-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="e04a1-173">Server-Abonnements</span><span class="sxs-lookup"><span data-stu-id="e04a1-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="e04a1-174">Übersicht über SQL DB in Azure</span><span class="sxs-lookup"><span data-stu-id="e04a1-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="e04a1-175">SQL-DB-Reservierungen (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="e04a1-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="e04a1-176">Azure Cosmos DB (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="e04a1-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="e04a1-177">SQL-verwaltete Instanz (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="e04a1-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="e04a1-178">SuSE und Red Hat Enterprise Linux (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="e04a1-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="e04a1-179">Red hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="e04a1-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="e04a1-180">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="e04a1-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="e04a1-181">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="e04a1-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="e04a1-182">Übersicht über Azure-Preise</span><span class="sxs-lookup"><span data-stu-id="e04a1-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="e04a1-183">Azure-Preisrechner</span><span class="sxs-lookup"><span data-stu-id="e04a1-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="e04a1-184">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="e04a1-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="e04a1-185">CSP-Preislisten: die Preislisten für **Microsoft Azure reservierten Instanzen** und **Software Abonnements** befinden sich beide auf der Seite Partner Center-Preis [& Angebote](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="e04a1-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="e04a1-186">Training</span><span class="sxs-lookup"><span data-stu-id="e04a1-186">Training</span></span>

<span data-ttu-id="e04a1-187">Registrieren Sie sich, um [kommerzielle Lizenzierungs Bereitschaft](https://commercial-licensing.eventbuilder.com/FY2019_ALL) und on-Demand-Veranstaltungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="e04a1-188">Bei on-Demand-Ereignissen für die Lizenzierung sind folgende Themen enthalten:</span><span class="sxs-lookup"><span data-stu-id="e04a1-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="e04a1-189">CSP-Online Dienste, CSP-Azure und allgemeine Lizenzierungs Updates, einschließlich Azure (November 2018)</span><span class="sxs-lookup"><span data-stu-id="e04a1-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="e04a1-190">Reservierte Kapazität der SQL DB-Kapazität & instanzgröße (August 2018)</span><span class="sxs-lookup"><span data-stu-id="e04a1-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="e04a1-191">Server Abonnements in CSP (Juli 2018)</span><span class="sxs-lookup"><span data-stu-id="e04a1-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="e04a1-192">Azure Reservations Übersicht in CSP (Mai 2018)</span><span class="sxs-lookup"><span data-stu-id="e04a1-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="e04a1-193">Weitere nützliche Schulungen umfassen das [Azure-Lizenzierungs Modul auf der Partner Universität](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="e04a1-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="e04a1-194">Operationen (Operations)</span><span class="sxs-lookup"><span data-stu-id="e04a1-194">Operations</span></span>

- <span data-ttu-id="e04a1-195">[Betriebshandbuch für den modernen Handel](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aktualisiert): ein umfassendes Handbuch, das wichtige Richtlinien und betriebliche Aspekte behandelt, wie z. b. Verträge, die Bestellung über Partner Center, Rechnungen, Preislisten Details, Anreize, Abstimmungs Datei, API/SDK, Sandbox und gemeinsame Azure-Partner Dienste.</span><span class="sxs-lookup"><span data-stu-id="e04a1-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="e04a1-196">Länderverfügbarkeit für moderne Angebote und Kundenwährungsmatrix</span><span class="sxs-lookup"><span data-stu-id="e04a1-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="e04a1-197">Verkaufen von Microsoft Azure Reserved Instances</span><span class="sxs-lookup"><span data-stu-id="e04a1-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="e04a1-198">Erwerben von Microsoft Azure Reservations im Auftrag Ihrer Kunden</span><span class="sxs-lookup"><span data-stu-id="e04a1-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="e04a1-199">Azure Reservations im Auftrag Ihrer Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="e04a1-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="e04a1-200">Abrechnung für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="e04a1-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="e04a1-201">VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="e04a1-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="e04a1-202">Partner Center API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="e04a1-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="e04a1-203">Remotedesktopdienste</span><span class="sxs-lookup"><span data-stu-id="e04a1-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="e04a1-204">Azure-Hybridvorteil</span><span class="sxs-lookup"><span data-stu-id="e04a1-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="e04a1-205">Der [Azure-Hybridvorteil](https://azure.microsoft.com/pricing/hybrid-benefit) hilft Ihnen, mehr Nutzen aus Ihren Windows Server-Lizenzen zu ziehen und bei virtuellen Computern bis zu \*47 % zu sparen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="e04a1-206">Sie können mit Windows Server Datacenter und Standard Edition-Lizenzen mit Software Assurance in den Genuss des Vorteils kommen.</span><span class="sxs-lookup"><span data-stu-id="e04a1-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="e04a1-207">Abhängig von der Edition können Sie Ihre Lizenzen konvertieren oder wieder verwenden, um virtuelle Windows Server-Computer in Azure auszuführen und eine niedrigere basiscomputerate zu bezahlen (die Preise für virtuelle Linux-Computer).</span><span class="sxs-lookup"><span data-stu-id="e04a1-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="e04a1-208">Siehe auch [Azure-Hybridvorteil – häufig gestellte Fragen](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="e04a1-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="e04a1-209">\*Aktuelle Einsparungen variieren basierend auf der Region, Instanztyp oder Nutzung</span><span class="sxs-lookup"><span data-stu-id="e04a1-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
