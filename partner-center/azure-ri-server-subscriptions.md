---
title: Azure-Reservierungen und Server Abonnements | Partner Center
ms.topic: article
ms.date: 04/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Möglichkeiten von Cloud Solution Provider zum Abrufen, bereitstellen und Verwalten von Azure-Reservierungen und Server Abonnements für Ihre Kunden.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Abonnements, VM, Reservierung, reservierte Instanz
ms.localizationpriority: medium
ms.openlocfilehash: d0a3fde651db86f8aeed160764fc330a25c0df04
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123278"
---
<!-- Mike Aasen wrote and owns this topic -->

# <a name="azure-reserved-vm-instances-ri--server-subscriptions-for-azure"></a><span data-ttu-id="0a061-104">Azure Reserved VM Instances (RI) + Server-Abonnements für Azure</span><span class="sxs-lookup"><span data-stu-id="0a061-104">Azure reserved VM instances (RI) + server subscriptions for Azure</span></span>

<span data-ttu-id="0a061-105">Betrifft:</span><span class="sxs-lookup"><span data-stu-id="0a061-105">Applies to:</span></span>

- <span data-ttu-id="0a061-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="0a061-106">Partner Center</span></span>

<span data-ttu-id="0a061-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="0a061-107">**Appropriate roles**</span></span>

- <span data-ttu-id="0a061-108">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="0a061-108">Admin agent</span></span>
- <span data-ttu-id="0a061-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="0a061-109">Global admin</span></span>
- <span data-ttu-id="0a061-110">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="0a061-110">Helpdesk agent</span></span>
- <span data-ttu-id="0a061-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="0a061-111">Sales agent</span></span>
- <span data-ttu-id="0a061-112">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="0a061-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="0a061-113">Was sind Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="0a061-113">What are Azure Reservations?</span></span>

<span data-ttu-id="0a061-114">Mit Azure Reservations können Sie Geld sparen, indem Sie für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Azure-Ressourcen ein oder drei Jahre im Voraus bezahlen.</span><span class="sxs-lookup"><span data-stu-id="0a061-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="0a061-115">Bei Vorauszahlung können Sie einen Rabatt auf die Ressourcen erhalten.</span><span class="sxs-lookup"><span data-stu-id="0a061-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="0a061-116">Reservations ermöglicht Ihnen eine deutliche Reduzierung Ihrer Kosten für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Ressourcen um bis zu 72 % im Vergleich zu nutzungsbasierten Preisen (Pay-As-You-Go).</span><span class="sxs-lookup"><span data-stu-id="0a061-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="0a061-117">Reservierungen bieten einen Abrechnungs Rabatt und wirken sich nicht auf den Lauf Zeit Status Ihrer Ressourcen aus.</span><span class="sxs-lookup"><span data-stu-id="0a061-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="0a061-118">Weitere Informationen finden Sie unter [Was ist Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="0a061-118">For more information, see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="0a061-119">Warum sollten Kunden eine Reservierung kaufen?</span><span class="sxs-lookup"><span data-stu-id="0a061-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="0a061-120">Wenn Kunden über virtuelle Computer, Azure Cosmos DB oder SQL-Datenbanken verfügen, die über längere Zeiträume betrieben werden, stellt der Erwerb einer Reservierung für sie die kostengünstigste Option dar.</span><span class="sxs-lookup"><span data-stu-id="0a061-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="0a061-121">Wenn ein Kunde z. B. kontinuierlich vier Instanzen eines Diensts ohne Reservierung ausführt, erfolgt eine nutzungsbasierte Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="0a061-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="0a061-122">Wenn sie eine Reservierung für diese Ressourcen kaufen, erhalten sie sofort den Reservierungsrabatt.</span><span class="sxs-lookup"><span data-stu-id="0a061-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="0a061-123">Die Ressourcen werden nicht mehr zu den nutzungsbasierten Tarifen abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="0a061-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="0a061-124">Faszinierende neue Azure-Angebote in CSP</span><span class="sxs-lookup"><span data-stu-id="0a061-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="0a061-125">Durch das Einbringen von Azure Reservations-und Server Abonnements für das CSP-Programm ermöglicht Microsoft den Partnern, die fast wachsende Kundennachfrage besser zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="0a061-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft allows partners to better address fast-growing customer demand.</span></span> <span data-ttu-id="0a061-126">Dies beinhaltet einen verbesserten Kundenbedarf für kostengünstigere Lösungen zur Unterstützung hochgradig vorhersag barer, persistenter cloudworkloads.</span><span class="sxs-lookup"><span data-stu-id="0a061-126">This includes increased customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="0a061-127">Das CSP-Programm ermöglicht Partnern das Abrufen, bereitstellen und Verwalten von Azure Reservations-und Server Abonnements im Auftrag von kommerziellen Kunden.</span><span class="sxs-lookup"><span data-stu-id="0a061-127">The CSP program enables partners to acquire, provision, and manage Azure Reservations and Server Subscriptions on behalf of commercial customers.</span></span> <span data-ttu-id="0a061-128">Partner können diese Aufgaben über das Microsoft Partner Center und die Azure-Portal durchführen.</span><span class="sxs-lookup"><span data-stu-id="0a061-128">Partners can perform these tasks via Microsoft Partner Center and the Azure portal.</span></span>

<span data-ttu-id="0a061-129">Azure Reservations bieten Kunden die Flexibilität der Virtualisierung für eine Vielzahl von Computinglösungen.</span><span class="sxs-lookup"><span data-stu-id="0a061-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions.</span></span> <span data-ttu-id="0a061-130">Solche Lösungen können das entwickeln und testen, das Ausführen von Anwendungen und das Erweitern des Rechenzentrums umfassen.</span><span class="sxs-lookup"><span data-stu-id="0a061-130">Such solutions can include development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="0a061-131">Beispielsweise können gewerbliche Kunden jetzt bis zu 72% im Vergleich zu Preisen der Azure-VM Azure reserved VM Instances mit Nutzungs basierter Bezahlung sparen, indem Sie den virtuellen Computer für einen Zeitraum von 1 bis 3 Jahren erwerben oder "Reservieren".</span><span class="sxs-lookup"><span data-stu-id="0a061-131">With Azure Reserved VM Instances, for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="0a061-132">Windows Server-Kunden mit Azure-Hybridvorteil, die im Lieferumfang von Software Assurance enthalten sind, können bis zu 80% im Vergleich zu den Tarifen für die Preisgestaltung für die Bezahlung sparen.</span><span class="sxs-lookup"><span data-stu-id="0a061-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, can save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="0a061-133">Mit einer unglaublichen Kombination aus einem überzeugenden Preis und beispielloser Bereitstellungsflexibilität erhalten Kunden den besten Gesamtwert, wenn sie Azure Reservations zusammen mit Server-Abonnements auswählen.</span><span class="sxs-lookup"><span data-stu-id="0a061-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="0a061-134">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="0a061-134">Azure reservations</span></span>

- <span data-ttu-id="0a061-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="0a061-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="0a061-136">SQL-DB-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="0a061-136">SQL DB Reservations</span></span>
- <span data-ttu-id="0a061-137">SQL-verwaltete Instanz</span><span class="sxs-lookup"><span data-stu-id="0a061-137">SQL Managed Instance</span></span>
- <span data-ttu-id="0a061-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0a061-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="0a061-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="0a061-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="0a061-140">App Services</span><span class="sxs-lookup"><span data-stu-id="0a061-140">App Services</span></span>
- <span data-ttu-id="0a061-141">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="0a061-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="0a061-142">Verwalteter Datenträger</span><span class="sxs-lookup"><span data-stu-id="0a061-142">Managed Disk</span></span>
- <span data-ttu-id="0a061-143">Blockblob</span><span class="sxs-lookup"><span data-stu-id="0a061-143">Blockblob</span></span>
- <span data-ttu-id="0a061-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="0a061-144">MySQL</span></span>
- <span data-ttu-id="0a061-145">Azure-Daten-Explorer</span><span class="sxs-lookup"><span data-stu-id="0a061-145">Azure Data explorer</span></span>
- <span data-ttu-id="0a061-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="0a061-146">MariaDB</span></span>
- <span data-ttu-id="0a061-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="0a061-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="0a061-148">Serverabonnements</span><span class="sxs-lookup"><span data-stu-id="0a061-148">Server subscriptions</span></span>

- <span data-ttu-id="0a061-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="0a061-149">Windows Server</span></span>
- <span data-ttu-id="0a061-150">Remotedesktopdienste-CALs (RDS)</span><span class="sxs-lookup"><span data-stu-id="0a061-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="0a061-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="0a061-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="0a061-152">Jährliche Linux-ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="0a061-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="0a061-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="0a061-153">SUSE Linux</span></span>
- <span data-ttu-id="0a061-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="0a061-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="0a061-155">Azure red hat openshift</span><span class="sxs-lookup"><span data-stu-id="0a061-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="0a061-156">Jährliche ISV-Abonnements</span><span class="sxs-lookup"><span data-stu-id="0a061-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="0a061-157">Azure VMware-Lösung durch cloudsimple</span><span class="sxs-lookup"><span data-stu-id="0a061-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="0a061-158">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="0a061-158">Getting started</span></span>

<span data-ttu-id="0a061-159">Um zu verstehen, wie Sie Azure Reservations mit ihren Kunden positionieren und so schnell wie möglich in Betrieb nehmen können, wird der folgende Ansatz empfohlen, um die Bereitschafts Materialien zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="0a061-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="0a061-160">Schauen Sie sich die Überblickspräsentationen und die zugehörigen Webinare für die Kundennutzung und Positionierung an.</span><span class="sxs-lookup"><span data-stu-id="0a061-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="0a061-161">Lesen Sie das Handbuch für modernes E-Commerce.</span><span class="sxs-lookup"><span data-stu-id="0a061-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="0a061-162">Schauen Sie sich die häufig gestellten Fragen zu Azure RI und Server-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="0a061-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="0a061-163">Verstehen Sie die Updates für Azure Reservations und Server-Abonnements im [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="0a061-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="0a061-164">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="0a061-164">Resources</span></span>

<span data-ttu-id="0a061-165">Im Folgenden finden Sie eine umfassende Liste der Ressourcen, die Ihnen helfen, Azure Reservations über Partner Center-Partner schnell zu integrieren:</span><span class="sxs-lookup"><span data-stu-id="0a061-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="0a061-166">Verkaufsbereitschaft</span><span class="sxs-lookup"><span data-stu-id="0a061-166">Sales readiness</span></span>

- [<span data-ttu-id="0a061-167">Azure Reservations und Server Abonnements mit Azure-Hybridvorteil Übersicht</span><span class="sxs-lookup"><span data-stu-id="0a061-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="0a061-168">Verkaufsblatt</span><span class="sxs-lookup"><span data-stu-id="0a061-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="0a061-169">FAQ zu Partnern für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="0a061-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="0a061-170">Häufig gestellte Fragen für Azure Reservations- und SQL DB-Partner</span><span class="sxs-lookup"><span data-stu-id="0a061-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="0a061-171">Remotedesktopdienste (RDS) CALs (Ankündigung)</span><span class="sxs-lookup"><span data-stu-id="0a061-171">Remote Desktop Services (RDS) CALs (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="0a061-172">Azure reserved VM Instances (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="0a061-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="0a061-173">Server-Abonnements</span><span class="sxs-lookup"><span data-stu-id="0a061-173">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="0a061-174">Übersicht über SQL DB in Azure</span><span class="sxs-lookup"><span data-stu-id="0a061-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="0a061-175">SQL-DB-Reservierungen (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="0a061-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="0a061-176">Azure Cosmos DB (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="0a061-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="0a061-177">SQL-verwaltete Instanz (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="0a061-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="0a061-178">SuSE und Red Hat Enterprise Linux (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="0a061-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="0a061-179">Red hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="0a061-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="0a061-180">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="0a061-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="0a061-181">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="0a061-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="0a061-182">Übersicht über Azure-Preise</span><span class="sxs-lookup"><span data-stu-id="0a061-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="0a061-183">Preisrechner für Azure</span><span class="sxs-lookup"><span data-stu-id="0a061-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="0a061-184">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="0a061-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="0a061-185">CSP-Preislisten: die Preislisten für **Microsoft Azure reservierten Instanzen** und **Software Abonnements** befinden sich beide auf der Seite Partner Center-Preis [& Angebote](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="0a061-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="0a061-186">Training</span><span class="sxs-lookup"><span data-stu-id="0a061-186">Training</span></span>

<span data-ttu-id="0a061-187">Registrieren Sie sich, um [kommerzielle Lizenzierungs Bereitschaft](https://commercial-licensing.eventbuilder.com/FY2019_ALL) und on-Demand-Veranstaltungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="0a061-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="0a061-188">Bei on-Demand-Ereignissen für die Lizenzierung sind folgende Themen enthalten:</span><span class="sxs-lookup"><span data-stu-id="0a061-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="0a061-189">CSP-Online Dienste, CSP-Azure und allgemeine Lizenzierungs Updates, einschließlich Azure (November 2018)</span><span class="sxs-lookup"><span data-stu-id="0a061-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="0a061-190">Reservierte Kapazität der SQL DB-Kapazität & instanzgröße (August 2018)</span><span class="sxs-lookup"><span data-stu-id="0a061-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="0a061-191">Server Abonnements in CSP (Juli 2018)</span><span class="sxs-lookup"><span data-stu-id="0a061-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="0a061-192">Azure Reservations Übersicht in CSP (Mai 2018)</span><span class="sxs-lookup"><span data-stu-id="0a061-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="0a061-193">Weitere nützliche Schulungen umfassen das [Azure-Lizenzierungs Modul auf der Partner Universität](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="0a061-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="0a061-194">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="0a061-194">Operations</span></span>

- <span data-ttu-id="0a061-195">[Betriebshandbuch für den modernen Handel](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aktualisiert): ein umfassendes Handbuch, das wichtige Richtlinien und betriebliche Aspekte behandelt, wie z. b. Verträge, die Bestellung über Partner Center, Rechnungen, Preislisten Details, Anreize, Abstimmungs Datei, API/SDK, Sandbox und gemeinsame Azure-Partner Dienste.</span><span class="sxs-lookup"><span data-stu-id="0a061-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="0a061-196">Länderverfügbarkeit für moderne Angebote und Kundenwährungsmatrix</span><span class="sxs-lookup"><span data-stu-id="0a061-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="0a061-197">Verkaufen von Microsoft Azure Reserved Instances</span><span class="sxs-lookup"><span data-stu-id="0a061-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="0a061-198">Erwerben von Microsoft Azure Reservations im Auftrag Ihrer Kunden</span><span class="sxs-lookup"><span data-stu-id="0a061-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="0a061-199">Azure Reservations im Auftrag Ihrer Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="0a061-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="0a061-200">Abrechnung für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="0a061-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="0a061-201">VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="0a061-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="0a061-202">Partner Center API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="0a061-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="0a061-203">Remotedesktopdienste</span><span class="sxs-lookup"><span data-stu-id="0a061-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="0a061-204">Azure-Hybridvorteil</span><span class="sxs-lookup"><span data-stu-id="0a061-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="0a061-205">Der [Azure-Hybridvorteil](https://azure.microsoft.com/pricing/hybrid-benefit) hilft Ihnen, mehr Nutzen aus Ihren Windows Server-Lizenzen zu ziehen und bei virtuellen Computern bis zu \*47 % zu sparen.</span><span class="sxs-lookup"><span data-stu-id="0a061-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="0a061-206">Sie können mit Windows Server Datacenter und Standard Edition-Lizenzen mit Software Assurance in den Genuss des Vorteils kommen.</span><span class="sxs-lookup"><span data-stu-id="0a061-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="0a061-207">Abhängig von der Edition können Sie Ihre Lizenzen konvertieren oder wieder verwenden, um virtuelle Windows Server-Computer in Azure auszuführen und eine niedrigere basiscomputerate zu bezahlen (die Preise für virtuelle Linux-Computer).</span><span class="sxs-lookup"><span data-stu-id="0a061-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="0a061-208">Siehe auch [Azure-Hybridvorteil – häufig gestellte Fragen](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="0a061-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="0a061-209">\*Aktuelle Einsparungen variieren basierend auf der Region, Instanztyp oder Nutzung</span><span class="sxs-lookup"><span data-stu-id="0a061-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
