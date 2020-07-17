---
title: Azure-Reservierungen & Server-Abonnements
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Möglichkeiten von Cloud Solution Provider zum Abrufen, bereitstellen und Verwalten von Azure-Reservierungen und Server Abonnements für Kunden.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b804c76428b0d1f699874b48f7a884161aebcdd
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435709"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="06292-103">Erwerben, bereitstellen und & Verwalten von reservierten Azure-VM-Instanzen (RI) und Server Abonnements für Kunden</span><span class="sxs-lookup"><span data-stu-id="06292-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="06292-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="06292-104">Applies to:</span></span>

- <span data-ttu-id="06292-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="06292-105">Partner Center</span></span>

<span data-ttu-id="06292-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="06292-106">**Appropriate roles**</span></span>

- <span data-ttu-id="06292-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="06292-107">Admin agent</span></span>
- <span data-ttu-id="06292-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="06292-108">Global admin</span></span>
- <span data-ttu-id="06292-109">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="06292-109">Helpdesk agent</span></span>
- <span data-ttu-id="06292-110">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="06292-110">Sales agent</span></span>
- <span data-ttu-id="06292-111">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="06292-111">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="06292-112">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="06292-112">What are Azure Reservations?</span></span>

<span data-ttu-id="06292-113">Mit Azure Reservations können Sie Geld sparen, indem Sie für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Azure-Ressourcen ein oder drei Jahre im Voraus bezahlen.</span><span class="sxs-lookup"><span data-stu-id="06292-113">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="06292-114">Durch die Vorabzahlung können Sie einen Rabatt für die Ressourcen, die Sie nutzen, in Anspruch nehmen.</span><span class="sxs-lookup"><span data-stu-id="06292-114">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="06292-115">Reservations ermöglicht Ihnen eine deutliche Reduzierung Ihrer Kosten für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Ressourcen um bis zu 72 % im Vergleich zu nutzungsbasierten Preisen (Pay-As-You-Go).</span><span class="sxs-lookup"><span data-stu-id="06292-115">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="06292-116">Reservierungen bieten einen Abrechnungsrabatt und wirken sich nicht auf den Laufzeitstatus Ihrer Ressourcen aus.</span><span class="sxs-lookup"><span data-stu-id="06292-116">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="06292-117">Weitere Informationen finden Sie [unter Was ist Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="06292-117">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="06292-118">Warum sollten Kunden eine Reservierung kaufen?</span><span class="sxs-lookup"><span data-stu-id="06292-118">Why should customers buy a reservation?</span></span>

<span data-ttu-id="06292-119">Wenn Kunden über virtuelle Computer, Azure Cosmos DB oder SQL-Datenbanken verfügen, die über längere Zeiträume betrieben werden, stellt der Erwerb einer Reservierung für sie die kostengünstigste Option dar.</span><span class="sxs-lookup"><span data-stu-id="06292-119">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="06292-120">Wenn ein Kunde z. B. kontinuierlich vier Instanzen eines Diensts ohne Reservierung ausführt, erfolgt eine nutzungsbasierte Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="06292-120">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="06292-121">Wenn sie eine Reservierung für diese Ressourcen kaufen, erhalten sie sofort den Reservierungsrabatt.</span><span class="sxs-lookup"><span data-stu-id="06292-121">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="06292-122">Die Ressourcen werden nicht mehr mit den Gebühren für die nutzungsbasierte Bezahlung in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="06292-122">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="06292-123">Faszinierende neue Azure-Angebote in CSP</span><span class="sxs-lookup"><span data-stu-id="06292-123">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="06292-124">Durch das Hinzufügen von Azure Reservations und Server-Abonnements in das CSP-Programm, unterstützt Microsoft unsere Partner mit der schnell wachsenden Kundennachfrage für kostengünstigere Lösungen zur Unterstützung von verlässlichen, permanenten Cloud-Workloads.</span><span class="sxs-lookup"><span data-stu-id="06292-124">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="06292-125">Mit dem CSP-Programm können Partner Azure Reservations-und Server Abonnements im Auftrag von kommerziellen Kunden über das Microsoft Partner Center und Azure-Portal erwerben, bereitstellen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="06292-125">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="06292-126">Wir haben unseren Partner im CSP-Programm sogar die Wahl, wie Azure-Reservierungen erworben werden können.</span><span class="sxs-lookup"><span data-stu-id="06292-126">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="06292-127">CSP-Partner können [Azure-Reservierungen im Auftrag eines Kunden erwerben](azure-reservations-buying.md) oder [dem Kunden ermöglichen, seine eigenen Reservierungen](give-customers-permission.md) von einem früheren Azure-Abonnement zu erwerben, das der Partner für Sie erworben hat.</span><span class="sxs-lookup"><span data-stu-id="06292-127">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="06292-128">Azure Reservations bieten Kunden die Flexibilität der Virtualisierung für eine Vielzahl von Computing-Lösungen, einschließlich der Entwicklung und dem Ausführen von Testanwendungen und dem erweitern des Rechenzentrums.</span><span class="sxs-lookup"><span data-stu-id="06292-128">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="06292-129">Beispielsweise können gewerbliche Kunden jetzt bis zu 72% im Vergleich zu Preisen für Azure-VMS [Azure reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) mit Nutzungs basierter Bezahlung sparen, indem Sie den virtuellen Computer für einen Zeitraum von 1 bis 3 Jahren erwerben oder "Reservieren".</span><span class="sxs-lookup"><span data-stu-id="06292-129">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="06292-130">Windows Server-Kunden mit Azure-Hybridvorteil und Software Assurance können bis zu 80 % im Vergleich zu nutzungsbasierten Preisen sparen.</span><span class="sxs-lookup"><span data-stu-id="06292-130">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="06292-131">Mit einer unglaublichen Kombination aus einem überzeugenden Preis und beispielloser Bereitstellungsflexibilität erhalten Kunden den besten Gesamtwert, wenn sie Azure Reservations zusammen mit Server-Abonnements auswählen.</span><span class="sxs-lookup"><span data-stu-id="06292-131">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="06292-132">Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="06292-132">Azure reservations</span></span>

- <span data-ttu-id="06292-133">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="06292-133">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="06292-134">SQL DB Reservations</span><span class="sxs-lookup"><span data-stu-id="06292-134">SQL DB Reservations</span></span>
- <span data-ttu-id="06292-135">Verwaltete SQL-Instanz</span><span class="sxs-lookup"><span data-stu-id="06292-135">SQL Managed Instance</span></span>
- <span data-ttu-id="06292-136">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="06292-136">Azure Cosmos DB</span></span>
- <span data-ttu-id="06292-137">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="06292-137">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="06292-138">App-Dienste</span><span class="sxs-lookup"><span data-stu-id="06292-138">App Services</span></span>
- <span data-ttu-id="06292-139">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="06292-139">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="06292-140">Verwalteter Datenträger</span><span class="sxs-lookup"><span data-stu-id="06292-140">Managed Disk</span></span>
- <span data-ttu-id="06292-141">Blockblob</span><span class="sxs-lookup"><span data-stu-id="06292-141">Block blob</span></span>
- <span data-ttu-id="06292-142">MySQL</span><span class="sxs-lookup"><span data-stu-id="06292-142">MySQL</span></span>
- <span data-ttu-id="06292-143">Azure-Daten-Explorer</span><span class="sxs-lookup"><span data-stu-id="06292-143">Azure Data explorer</span></span>
- <span data-ttu-id="06292-144">MariaDB</span><span class="sxs-lookup"><span data-stu-id="06292-144">MariaDB</span></span>
- <span data-ttu-id="06292-145">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="06292-145">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="06292-146">Server Abonnements</span><span class="sxs-lookup"><span data-stu-id="06292-146">Server subscriptions</span></span>

- <span data-ttu-id="06292-147">Windows Server</span><span class="sxs-lookup"><span data-stu-id="06292-147">Windows Server</span></span>
- <span data-ttu-id="06292-148">Remotedesktopdienste-CALs (RDS)</span><span class="sxs-lookup"><span data-stu-id="06292-148">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="06292-149">SQL Server</span><span class="sxs-lookup"><span data-stu-id="06292-149">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="06292-150">Jährliche Linux-ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="06292-150">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="06292-151">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="06292-151">SUSE Linux</span></span>
- <span data-ttu-id="06292-152">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="06292-152">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="06292-153">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="06292-153">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="06292-154">Jährliche ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="06292-154">ISV annual subscriptions</span></span>

- <span data-ttu-id="06292-155">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="06292-155">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="06292-156">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="06292-156">Getting started</span></span>

<span data-ttu-id="06292-157">Um zu verstehen, wie Sie Azure Reservations mit ihren Kunden positionieren und so schnell wie möglich in Betrieb nehmen können, wird der folgende Ansatz empfohlen, um die Bereitschafts Materialien zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="06292-157">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="06292-158">Schauen Sie sich die Überblickspräsentationen und die zugehörigen Webinare für die Kundennutzung und Positionierung an.</span><span class="sxs-lookup"><span data-stu-id="06292-158">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="06292-159">Lesen Sie das Handbuch für modernes E-Commerce.</span><span class="sxs-lookup"><span data-stu-id="06292-159">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="06292-160">Schauen Sie sich die häufig gestellten Fragen zu Azure RI und Server-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="06292-160">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="06292-161">Verstehen Sie die Updates für Azure Reservations und Server-Abonnements im [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="06292-161">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="06292-162">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="06292-162">Resources</span></span>

<span data-ttu-id="06292-163">Im Folgenden finden Sie eine umfassende Liste der Ressourcen, die Ihnen helfen, Azure Reservations über Partner Center-Partner schnell zu integrieren:</span><span class="sxs-lookup"><span data-stu-id="06292-163">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="06292-164">Vertriebsbereitschaft</span><span class="sxs-lookup"><span data-stu-id="06292-164">Sales readiness</span></span>

- [<span data-ttu-id="06292-165">Azure Reservations und Server Abonnements mit Azure-Hybridvorteil Übersicht</span><span class="sxs-lookup"><span data-stu-id="06292-165">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="06292-166">Verkaufsblatt</span><span class="sxs-lookup"><span data-stu-id="06292-166">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="06292-167">FAQ zu Partnern für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="06292-167">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="06292-168">Häufig gestellte Fragen für Azure Reservations- und SQL DB-Partner</span><span class="sxs-lookup"><span data-stu-id="06292-168">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="06292-169">Remotedesktopdienste (RDS)-Client Zugriffslizenz (CAL) (Ankündigung)</span><span class="sxs-lookup"><span data-stu-id="06292-169">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="06292-170">Azure reserved VM Instances (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="06292-170">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="06292-171">Server-Abonnements</span><span class="sxs-lookup"><span data-stu-id="06292-171">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="06292-172">Übersicht über SQL DB in Azure</span><span class="sxs-lookup"><span data-stu-id="06292-172">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="06292-173">SQL-DB-Reservierungen (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="06292-173">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="06292-174">Azure Cosmos DB (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="06292-174">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="06292-175">SQL-verwaltete Instanz (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="06292-175">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="06292-176">SuSE und Red Hat Enterprise Linux (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="06292-176">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="06292-177">Red hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="06292-177">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="06292-178">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="06292-178">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="06292-179">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="06292-179">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="06292-180">Übersicht über Azure-Preise</span><span class="sxs-lookup"><span data-stu-id="06292-180">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="06292-181">Azure-Preisrechner</span><span class="sxs-lookup"><span data-stu-id="06292-181">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="06292-182">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="06292-182">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="06292-183">CSP-Preislisten: die Preislisten für **Microsoft Azure reservierten Instanzen** und **Software Abonnements** befinden sich beide auf der Seite Partner Center-Preis [& Angebote](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="06292-183">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="06292-184">Training</span><span class="sxs-lookup"><span data-stu-id="06292-184">Training</span></span>

<span data-ttu-id="06292-185">Registrieren Sie sich, um [kommerzielle Lizenzierungs Bereitschaft](https://commercial-licensing.eventbuilder.com/FY2019_ALL) und on-Demand-Veranstaltungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="06292-185">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="06292-186">Bei on-Demand-Ereignissen für die Lizenzierung sind folgende Themen enthalten:</span><span class="sxs-lookup"><span data-stu-id="06292-186">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="06292-187">CSP-Online Dienste, CSP-Azure und allgemeine Lizenzierungs Updates, einschließlich Azure (November 2018)</span><span class="sxs-lookup"><span data-stu-id="06292-187">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="06292-188">Reservierte Kapazität der SQL DB-Kapazität & instanzgröße (August 2018)</span><span class="sxs-lookup"><span data-stu-id="06292-188">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="06292-189">Server Abonnements in CSP (Juli 2018)</span><span class="sxs-lookup"><span data-stu-id="06292-189">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="06292-190">Azure Reservations Übersicht in CSP (Mai 2018)</span><span class="sxs-lookup"><span data-stu-id="06292-190">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="06292-191">Weitere nützliche Schulungen umfassen das [Azure-Lizenzierungs Modul auf der Partner Universität](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="06292-191">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="06292-192">Operationen (Operations)</span><span class="sxs-lookup"><span data-stu-id="06292-192">Operations</span></span>

- <span data-ttu-id="06292-193">[Betriebshandbuch für den modernen Handel](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aktualisiert): ein umfassendes Handbuch, das wichtige Richtlinien und betriebliche Aspekte behandelt, wie z. b. Verträge, die Bestellung über Partner Center, Rechnungen, Preislisten Details, Anreize, Abstimmungs Datei, API/SDK, Sandbox und gemeinsame Azure-Partner Dienste.</span><span class="sxs-lookup"><span data-stu-id="06292-193">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="06292-194">Länderverfügbarkeit für moderne Angebote und Kundenwährungsmatrix</span><span class="sxs-lookup"><span data-stu-id="06292-194">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="06292-195">Verkaufen von Microsoft Azure Reserved Instances</span><span class="sxs-lookup"><span data-stu-id="06292-195">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="06292-196">Erwerben von Microsoft Azure Reservations im Auftrag Ihrer Kunden</span><span class="sxs-lookup"><span data-stu-id="06292-196">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="06292-197">Azure Reservations im Auftrag Ihrer Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="06292-197">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="06292-198">Abrechnung für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="06292-198">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="06292-199">VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="06292-199">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="06292-200">Partner Center API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="06292-200">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="06292-201">Remotedesktopdienste</span><span class="sxs-lookup"><span data-stu-id="06292-201">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="06292-202">Azure-Hybridvorteil</span><span class="sxs-lookup"><span data-stu-id="06292-202">Azure Hybrid Benefit</span></span>

<span data-ttu-id="06292-203">Der [Azure-Hybridvorteil](https://azure.microsoft.com/pricing/hybrid-benefit) hilft Ihnen, mehr Nutzen aus Ihren Windows Server-Lizenzen zu ziehen und bei virtuellen Computern bis zu \*47 % zu sparen.</span><span class="sxs-lookup"><span data-stu-id="06292-203">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="06292-204">Sie können mit Windows Server Datacenter und Standard Edition-Lizenzen mit Software Assurance in den Genuss des Vorteils kommen.</span><span class="sxs-lookup"><span data-stu-id="06292-204">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="06292-205">Abhängig von der Edition können Sie Ihre Lizenzen konvertieren oder wieder verwenden, um virtuelle Windows Server-Computer in Azure auszuführen und eine niedrigere basiscomputerate zu bezahlen (die Preise für virtuelle Linux-Computer).</span><span class="sxs-lookup"><span data-stu-id="06292-205">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="06292-206">Siehe auch [Azure-Hybridvorteil – häufig gestellte Fragen](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="06292-206">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="06292-207">\*Aktuelle Einsparungen variieren basierend auf der Region, Instanztyp oder Nutzung</span><span class="sxs-lookup"><span data-stu-id="06292-207">\*Actual savings may vary based on region, instance type, or usage.</span></span>
