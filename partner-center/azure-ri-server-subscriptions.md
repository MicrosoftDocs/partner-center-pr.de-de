---
title: Azure Reserved VM Instances (RI) + Server-Abonnements für Azure | Partner Center
ms.topic: article
ms.date: 12/02/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Möglichkeiten von Cloud Solution Provider zum Abrufen, bereitstellen und Verwalten von Azure-Reservierungen und Server Abonnements für Ihre Kunden.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Abonnements, VM, Reservierung, reservierte Instanz
ms.localizationpriority: medium
ms.openlocfilehash: 22ba6af523bf73d9d7778940ef7495e6581a0730
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722260"
---
<!-- Mike Aasen wrote and owns this topic -->

# <a name="azure-reserved-vm-instances-ri--server-subscriptions-for-azure"></a><span data-ttu-id="4344d-104">Azure Reserved VM Instances (RI) + Server-Abonnements für Azure</span><span class="sxs-lookup"><span data-stu-id="4344d-104">Azure reserved VM instances (RI) + server subscriptions for Azure</span></span>

<span data-ttu-id="4344d-105">Betrifft</span><span class="sxs-lookup"><span data-stu-id="4344d-105">Applies to:</span></span>

- <span data-ttu-id="4344d-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="4344d-106">Partner Center</span></span>

<span data-ttu-id="4344d-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="4344d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4344d-108">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="4344d-108">Admin agent</span></span>
- <span data-ttu-id="4344d-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="4344d-109">Global admin</span></span>
- <span data-ttu-id="4344d-110">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="4344d-110">Helpdesk agent</span></span>
- <span data-ttu-id="4344d-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="4344d-111">Sales agent</span></span>
- <span data-ttu-id="4344d-112">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="4344d-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="4344d-113">Was sind Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="4344d-113">What are Azure Reservations?</span></span>

<span data-ttu-id="4344d-114">Mit Azure Reservations können Sie Geld sparen, indem Sie für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Azure-Ressourcen ein oder drei Jahre im Voraus bezahlen.</span><span class="sxs-lookup"><span data-stu-id="4344d-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="4344d-115">Bei Vorauszahlung können Sie einen Rabatt auf die Ressourcen erhalten.</span><span class="sxs-lookup"><span data-stu-id="4344d-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="4344d-116">Reservations ermöglicht Ihnen eine deutliche Reduzierung Ihrer Kosten für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Ressourcen um bis zu 72 % im Vergleich zu nutzungsbasierten Preisen (Pay-As-You-Go).</span><span class="sxs-lookup"><span data-stu-id="4344d-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="4344d-117">Reservations gewähren einen Abrechnungsrabatt und haben keinen Einfluss auf den Laufzeitstatus Ihrer Ressourcen. Weitere Informationen finden Sie unter [Was sind Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations).</span><span class="sxs-lookup"><span data-stu-id="4344d-117">Reservations provide a billing discount and don't affect the runtime state of your resources.For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="4344d-118">Warum sollten Kunden eine Reservierung kaufen?</span><span class="sxs-lookup"><span data-stu-id="4344d-118">Why should customers buy a reservation?</span></span>

<span data-ttu-id="4344d-119">Wenn Kunden über virtuelle Computer, Azure Cosmos DB oder SQL-Datenbanken verfügen, die über längere Zeiträume betrieben werden, stellt der Erwerb einer Reservierung für sie die kostengünstigste Option dar.</span><span class="sxs-lookup"><span data-stu-id="4344d-119">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="4344d-120">Wenn ein Kunde z. B. kontinuierlich vier Instanzen eines Diensts ohne Reservierung ausführt, erfolgt eine nutzungsbasierte Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="4344d-120">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="4344d-121">Wenn sie eine Reservierung für diese Ressourcen kaufen, erhalten sie sofort den Reservierungsrabatt.</span><span class="sxs-lookup"><span data-stu-id="4344d-121">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="4344d-122">Die Ressourcen werden nicht mehr zu den nutzungsbasierten Tarifen abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="4344d-122">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="4344d-123">Faszinierende neue Azure-Angebote in CSP</span><span class="sxs-lookup"><span data-stu-id="4344d-123">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="4344d-124">Durch das Hinzufügen von Azure Reservations und Server-Abonnements in das CSP-Programm, unterstützt Microsoft unsere Partner mit der schnell wachsenden Kundennachfrage für kostengünstigere Lösungen zur Unterstützung von verlässlichen, permanenten Cloud-Workloads.</span><span class="sxs-lookup"><span data-stu-id="4344d-124">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="4344d-125">Mit dem CSP-Programm können Partner Azure Reservations und Server-Abonnements für kommerzielle Kunden über das Microsoft-Partner Center und das Azure-Portal bereitstellen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="4344d-125">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure Portal.</span></span>

<span data-ttu-id="4344d-126">Azure Reservations bieten Kunden die Flexibilität der Virtualisierung für eine Vielzahl von Computing-Lösungen, einschließlich der Entwicklung und dem Ausführen von Testanwendungen und dem erweitern des Rechenzentrums.</span><span class="sxs-lookup"><span data-stu-id="4344d-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="4344d-127">Beispielsweise können gewerbliche Kunden jetzt bis zu 72% im Vergleich zu Preisen für Azure-VMS [Azure reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) mit Nutzungs basierter Bezahlung sparen, indem Sie den virtuellen Computer für einen Zeitraum von 1 bis 3 Jahren erwerben oder "Reservieren".</span><span class="sxs-lookup"><span data-stu-id="4344d-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or “reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="4344d-128">Windows Server-Kunden mit Azure-Hybridvorteil und Software Assurance können bis zu 80 % im Vergleich zu nutzungsbasierten Preisen sparen.</span><span class="sxs-lookup"><span data-stu-id="4344d-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="4344d-129">Mit einer unglaublichen Kombination aus einem überzeugenden Preis und beispielloser Bereitstellungsflexibilität erhalten Kunden den besten Gesamtwert, wenn sie Azure Reservations zusammen mit Server-Abonnements auswählen.</span><span class="sxs-lookup"><span data-stu-id="4344d-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="4344d-130">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="4344d-130">Azure reservations</span></span>

- <span data-ttu-id="4344d-131">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="4344d-131">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="4344d-132">SQL-DB-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="4344d-132">SQL DB Reservations</span></span>
- <span data-ttu-id="4344d-133">SQL-verwaltete Instanz</span><span class="sxs-lookup"><span data-stu-id="4344d-133">SQL Managed Instance</span></span>
- <span data-ttu-id="4344d-134">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4344d-134">Azure Cosmos DB</span></span>
- <span data-ttu-id="4344d-135">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="4344d-135">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="4344d-136">App Services</span><span class="sxs-lookup"><span data-stu-id="4344d-136">App Services</span></span>
- <span data-ttu-id="4344d-137">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="4344d-137">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="4344d-138">Verwalteter Datenträger</span><span class="sxs-lookup"><span data-stu-id="4344d-138">Managed Disk</span></span>
- <span data-ttu-id="4344d-139">Blockblob</span><span class="sxs-lookup"><span data-stu-id="4344d-139">Blockblob</span></span>
- <span data-ttu-id="4344d-140">MySQL</span><span class="sxs-lookup"><span data-stu-id="4344d-140">MySQL</span></span>
- <span data-ttu-id="4344d-141">Azure-Daten-Explorer</span><span class="sxs-lookup"><span data-stu-id="4344d-141">Azure Data explorer</span></span>
- <span data-ttu-id="4344d-142">MariaDB</span><span class="sxs-lookup"><span data-stu-id="4344d-142">MariaDB</span></span>
- <span data-ttu-id="4344d-143">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="4344d-143">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="4344d-144">Serverabonnements</span><span class="sxs-lookup"><span data-stu-id="4344d-144">Server subscriptions</span></span>

- <span data-ttu-id="4344d-145">Windows Server</span><span class="sxs-lookup"><span data-stu-id="4344d-145">Windows Server</span></span>
- <span data-ttu-id="4344d-146">Remotedesktopdienste-CALs (RDS)</span><span class="sxs-lookup"><span data-stu-id="4344d-146">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="4344d-147">SQL Server</span><span class="sxs-lookup"><span data-stu-id="4344d-147">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="4344d-148">Jährliche Linux-ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="4344d-148">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="4344d-149">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="4344d-149">SUSE Linux</span></span>
- <span data-ttu-id="4344d-150">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="4344d-150">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="4344d-151">Azure red hat openshift</span><span class="sxs-lookup"><span data-stu-id="4344d-151">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="4344d-152">Jährliche ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="4344d-152">ISV annual subscriptions</span></span>

- <span data-ttu-id="4344d-153">Azure VMware-Lösung durch cloudsimple</span><span class="sxs-lookup"><span data-stu-id="4344d-153">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="4344d-154">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="4344d-154">Getting started</span></span>

<span data-ttu-id="4344d-155">Um zu verstehen, wie Sie Azure Reservations bei Ihren Kunden positionieren und es so schnell wie möglich einrichten, anzeigen und ausführen, empfehlen wir die folgende Methode zum Überprüfen der Bereitschaft aller Materialien:</span><span class="sxs-lookup"><span data-stu-id="4344d-155">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible we recommend the following approach for reviewing the readiness materials:</span></span>

1. <span data-ttu-id="4344d-156">Schauen Sie sich die Überblickspräsentationen und die zugehörigen Webinare für die Kundennutzung und Positionierung an.</span><span class="sxs-lookup"><span data-stu-id="4344d-156">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="4344d-157">Lesen Sie das Handbuch für modernes E-Commerce.</span><span class="sxs-lookup"><span data-stu-id="4344d-157">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="4344d-158">Schauen Sie sich die häufig gestellten Fragen zu Azure RI und Server-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="4344d-158">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="4344d-159">Verstehen Sie die Updates für Azure Reservations und Server-Abonnements im [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="4344d-159">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="4344d-160">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="4344d-160">Resources</span></span>

<span data-ttu-id="4344d-161">Im Folgenden finden Sie eine umfassende Liste der Ressourcen, die Ihnen helfen, Azure Reservations über Partner Center-Partner schnell zu integrieren:</span><span class="sxs-lookup"><span data-stu-id="4344d-161">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="4344d-162">Verkaufsbereitschaft</span><span class="sxs-lookup"><span data-stu-id="4344d-162">Sales readiness</span></span>

- [<span data-ttu-id="4344d-163">Azure Reservations und Server Abonnements mit Azure-Hybridvorteil Übersicht</span><span class="sxs-lookup"><span data-stu-id="4344d-163">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="4344d-164">Verkaufsblatt</span><span class="sxs-lookup"><span data-stu-id="4344d-164">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="4344d-165">FAQ zu Partnern für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="4344d-165">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="4344d-166">Häufig gestellte Fragen für Azure Reservations- und SQL DB-Partner</span><span class="sxs-lookup"><span data-stu-id="4344d-166">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="4344d-167">Remotedesktopdienste (RDS) CALs (Ankündigung)</span><span class="sxs-lookup"><span data-stu-id="4344d-167">Remote Desktop Services (RDS) CALs (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="4344d-168">Azure reserved VM Instances (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4344d-168">Azure Reserved VM Instances (Azure Portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="4344d-169">Server-Abonnements</span><span class="sxs-lookup"><span data-stu-id="4344d-169">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="4344d-170">Übersicht über SQL DB in Azure</span><span class="sxs-lookup"><span data-stu-id="4344d-170">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="4344d-171">SQL-DB-Reservierungen (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4344d-171">SQL DB Reservations (Azure Portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="4344d-172">Azure Cosmos DB (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4344d-172">Azure Cosmos DB (Azure Portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="4344d-173">SQL verwaltete Instanz (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4344d-173">SQL Managed Instance (Azure Portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="4344d-174">SuSE und Red Hat Enterprise Linux (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4344d-174">SUSE and Red Hat Enterprise Linux (Azure Portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="4344d-175">Red hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="4344d-175">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="4344d-176">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="4344d-176">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="4344d-177">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="4344d-177">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="4344d-178">Übersicht über Azure-Preise</span><span class="sxs-lookup"><span data-stu-id="4344d-178">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="4344d-179">Preisrechner für Azure</span><span class="sxs-lookup"><span data-stu-id="4344d-179">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="4344d-180">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="4344d-180">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="4344d-181">CSP-Preislisten: die Preislisten für **Microsoft Azure reservierten Instanzen** und **Software Abonnements** befinden sich beide auf der Seite Partner Center-Preis [& Angebote](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="4344d-181">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="4344d-182">Schulung</span><span class="sxs-lookup"><span data-stu-id="4344d-182">Training</span></span>

- <span data-ttu-id="4344d-183">[November 2018 – Webinare zur kommerziellen Lizenzierung – Readiness](https://na01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcommercial-licensing.eventbuilder.com%2F%3Flandingpageid%3DV0Bx6L&data=02%7C01%7Cv-oumaki%40microsoft.com%7C96e24687952242e1ff0c08d62ada13f3%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636743513471330495&sdata=DjPAKnW%2BpVekRS3Zngy2uwAkTpU4z1O%2Fh56NuTOmCzM%3D&reserved=0) behandeln CSP Online Services, CSP Azure und ein allgemeines Lizenzierungsupdate (einschließlich Azure).</span><span class="sxs-lookup"><span data-stu-id="4344d-183">[November 2018 Commercial Licensing Readiness Webinars](https://na01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcommercial-licensing.eventbuilder.com%2F%3Flandingpageid%3DV0Bx6L&data=02%7C01%7Cv-oumaki%40microsoft.com%7C96e24687952242e1ff0c08d62ada13f3%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636743513471330495&sdata=DjPAKnW%2BpVekRS3Zngy2uwAkTpU4z1O%2Fh56NuTOmCzM%3D&reserved=0) covering CSP Online Services, CSP Azure and a general licensing update (including Azure)</span></span>
- [<span data-ttu-id="4344d-184">August – Reservierte SQL DB-Kapazität und Flexibilität bei der Instanzgröße – Webinar zur Lizenzierung</span><span class="sxs-lookup"><span data-stu-id="4344d-184">August SQL DB Reserved Capacity & Instance Size Flexibility - Licensing Webinar</span></span>](https://commercial-licensing.eventbuilder.com/view?eventid=d0t9g4)
- [<span data-ttu-id="4344d-185">Juli 2018 – Webinar zu Server-Abonnements im CSP</span><span class="sxs-lookup"><span data-stu-id="4344d-185">July 2018 Server Subscriptions in CSP Webinar</span></span>](https://commercial-licensing.eventbuilder.com/Server_Subscriptions_in_CSP_P2_July)
- [<span data-ttu-id="4344d-186">Mai 2018 – Webinar zur Übersicht über Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="4344d-186">May 2018 Azure Reservations Overview Webinar</span></span>](https://commercial-licensing.eventbuilder.com/Reserved_Instances_in_CSP_May_Option_1)
- [<span data-ttu-id="4344d-187">Azure-Lizenzmodul auf Partner University</span><span class="sxs-lookup"><span data-stu-id="4344d-187">Azure Licensing Module on Partner University</span></span>](https://aka.ms/azure_partner_licensing)

### <a name="operations"></a><span data-ttu-id="4344d-188">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="4344d-188">Operations</span></span>

- <span data-ttu-id="4344d-189">[Betriebshandbuch für den modernen Handel](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aktualisiert): ein umfassendes Handbuch, das wichtige Richtlinien und betriebliche Aspekte behandelt, wie z. b. Verträge, die Bestellung über Partner Center, Rechnungen, Preislisten Details, Anreize, Abstimmungs Dateien, API/SDK, Sandbox und Gemeinsame Dienste von Azure-Partnern.</span><span class="sxs-lookup"><span data-stu-id="4344d-189">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="4344d-190">Länderverfügbarkeit für moderne Angebote und Kundenwährungsmatrix</span><span class="sxs-lookup"><span data-stu-id="4344d-190">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="4344d-191">Verkaufen von Microsoft Azure Reserved Instances</span><span class="sxs-lookup"><span data-stu-id="4344d-191">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="4344d-192">Erwerben von Microsoft Azure Reservations im Auftrag Ihrer Kunden</span><span class="sxs-lookup"><span data-stu-id="4344d-192">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="4344d-193">Azure Reservations im Auftrag Ihrer Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="4344d-193">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="4344d-194">Abrechnung für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="4344d-194">Billing for Azure reservations</span></span>](https://go.microsoft.com/fwlink/?linkid=872809)
- [<span data-ttu-id="4344d-195">VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="4344d-195">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="4344d-196">Partner Center API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="4344d-196">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="4344d-197">Remotedesktopdienste (RDS)</span><span class="sxs-lookup"><span data-stu-id="4344d-197">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="4344d-198">Azure-Hybridvorteil</span><span class="sxs-lookup"><span data-stu-id="4344d-198">Azure Hybrid Benefit</span></span>

<span data-ttu-id="4344d-199">Der [Azure-Hybridvorteil](https://azure.microsoft.com/pricing/hybrid-benefit) hilft Ihnen, mehr Nutzen aus Ihren Windows Server-Lizenzen zu ziehen und bei virtuellen Computern bis zu \*47 % zu sparen.</span><span class="sxs-lookup"><span data-stu-id="4344d-199">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="4344d-200">Sie können mit Windows Server Datacenter und Standard Edition-Lizenzen mit Software Assurance in den Genuss des Vorteils kommen.</span><span class="sxs-lookup"><span data-stu-id="4344d-200">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="4344d-201">Je nach Edition können Sie Ihre Lizenzen zum Ausführen von Windows Server-VMs in Azure konvertieren oder erneut verwenden und einen niedrigeren Computetarif (Tarife für Linux-VMs) zahlen.</span><span class="sxs-lookup"><span data-stu-id="4344d-201">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="4344d-202">Siehe auch [Azure-Hybridvorteil – häufig gestellte Fragen](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="4344d-202">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="4344d-203">\*Aktuelle Einsparungen variieren basierend auf der Region, Instanztyp oder Nutzung</span><span class="sxs-lookup"><span data-stu-id="4344d-203">\*Actual savings may vary based on region, instance type, or usage.</span></span>
