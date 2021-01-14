---
title: Azure-Reservierungen & Server-Abonnements
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Möglichkeiten von Cloud Solution Provider zum Abrufen, bereitstellen und Verwalten von Azure-Reservierungen und Server Abonnements für Kunden.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182493"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="4c11e-103">Erwerben, bereitstellen und & Verwalten von reservierten Azure-VM-Instanzen (RI) und Server Abonnements für Kunden</span><span class="sxs-lookup"><span data-stu-id="4c11e-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="4c11e-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="4c11e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4c11e-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="4c11e-105">Admin agent</span></span>
- <span data-ttu-id="4c11e-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="4c11e-106">Global admin</span></span>
- <span data-ttu-id="4c11e-107">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="4c11e-107">Helpdesk agent</span></span>
- <span data-ttu-id="4c11e-108">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="4c11e-108">Sales agent</span></span>
- <span data-ttu-id="4c11e-109">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="4c11e-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="4c11e-110">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="4c11e-110">What are Azure Reservations?</span></span>

<span data-ttu-id="4c11e-111">Mit Azure Reservations können Sie Geld sparen, indem Sie für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Azure-Ressourcen ein oder drei Jahre im Voraus bezahlen.</span><span class="sxs-lookup"><span data-stu-id="4c11e-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="4c11e-112">Durch die Vorabzahlung können Sie einen Rabatt für die Ressourcen, die Sie nutzen, in Anspruch nehmen.</span><span class="sxs-lookup"><span data-stu-id="4c11e-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="4c11e-113">Reservations ermöglicht Ihnen eine deutliche Reduzierung Ihrer Kosten für virtuelle Computer, Computekapazität für SQL-Datenbanken, Azure Cosmos DB-Durchsatz und andere Ressourcen um bis zu 72 % im Vergleich zu nutzungsbasierten Preisen (Pay-As-You-Go).</span><span class="sxs-lookup"><span data-stu-id="4c11e-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="4c11e-114">Reservierungen bieten einen Abrechnungsrabatt und wirken sich nicht auf den Laufzeitstatus Ihrer Ressourcen aus.</span><span class="sxs-lookup"><span data-stu-id="4c11e-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="4c11e-115">Weitere Informationen finden Sie [unter Was ist Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="4c11e-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="4c11e-116">Warum sollten Kunden eine Reservierung kaufen?</span><span class="sxs-lookup"><span data-stu-id="4c11e-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="4c11e-117">Wenn Kunden über virtuelle Computer, Azure Cosmos DB oder SQL-Datenbanken verfügen, die über längere Zeiträume betrieben werden, stellt der Erwerb einer Reservierung für sie die kostengünstigste Option dar.</span><span class="sxs-lookup"><span data-stu-id="4c11e-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="4c11e-118">Wenn ein Kunde z. B. kontinuierlich vier Instanzen eines Diensts ohne Reservierung ausführt, erfolgt eine nutzungsbasierte Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="4c11e-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="4c11e-119">Wenn sie eine Reservierung für diese Ressourcen kaufen, erhalten sie sofort den Reservierungsrabatt.</span><span class="sxs-lookup"><span data-stu-id="4c11e-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="4c11e-120">Die Ressourcen werden nicht mehr mit den Gebühren für die nutzungsbasierte Bezahlung in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="4c11e-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="4c11e-121">Faszinierende neue Azure-Angebote in CSP</span><span class="sxs-lookup"><span data-stu-id="4c11e-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="4c11e-122">Durch das Hinzufügen von Azure Reservations und Server-Abonnements in das CSP-Programm, unterstützt Microsoft unsere Partner mit der schnell wachsenden Kundennachfrage für kostengünstigere Lösungen zur Unterstützung von verlässlichen, permanenten Cloud-Workloads.</span><span class="sxs-lookup"><span data-stu-id="4c11e-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="4c11e-123">Mit dem CSP-Programm können Partner Azure Reservations-und Server Abonnements im Auftrag von kommerziellen Kunden über das Microsoft Partner Center und Azure-Portal erwerben, bereitstellen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="4c11e-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="4c11e-124">Wir haben unseren Partner im CSP-Programm sogar die Wahl, wie Azure-Reservierungen erworben werden können.</span><span class="sxs-lookup"><span data-stu-id="4c11e-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="4c11e-125">CSP-Partner können [Azure-Reservierungen im Auftrag eines Kunden erwerben](azure-reservations-buying.md) oder [dem Kunden ermöglichen, seine eigenen Reservierungen](give-customers-permission.md) von einem früheren Azure-Abonnement zu erwerben, das der Partner für Sie erworben hat.</span><span class="sxs-lookup"><span data-stu-id="4c11e-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="4c11e-126">Azure Reservations bieten Kunden die Flexibilität der Virtualisierung für eine Vielzahl von Computing-Lösungen, einschließlich der Entwicklung und dem Ausführen von Testanwendungen und dem erweitern des Rechenzentrums.</span><span class="sxs-lookup"><span data-stu-id="4c11e-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="4c11e-127">Beispielsweise können gewerbliche Kunden jetzt bis zu 72% im Vergleich zu Preisen für Azure-VMS [Azure reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) mit Nutzungs basierter Bezahlung sparen, indem Sie den virtuellen Computer für einen Zeitraum von 1 bis 3 Jahren erwerben oder "Reservieren".</span><span class="sxs-lookup"><span data-stu-id="4c11e-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="4c11e-128">Windows Server-Kunden mit Azure-Hybridvorteil und Software Assurance können bis zu 80 % im Vergleich zu nutzungsbasierten Preisen sparen.</span><span class="sxs-lookup"><span data-stu-id="4c11e-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="4c11e-129">Bei einer nicht übereinstimmenden Kombination aus überzeugenden Preisen und nicht übereinstimmender Flexibilität bei der Bereitstellung sehen Kunden bei der Auswahl Azure Reservations den besten Gesamtwert.</span><span class="sxs-lookup"><span data-stu-id="4c11e-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="4c11e-130">Siehe [Kauf Reservierungen](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) im Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="4c11e-130">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="4c11e-131">Weitere Informationen finden Sie in der **Preisliste für den Azure RI CSP-Preis** in der Kategorie " **Microsoft Azure reservierte Instanzen** " auf der Seite " [Preise und Angebote](https://partner.microsoft.com/dashboard/sell/pricingandoffers) " im Partner Center für Software Abonnements und Jahresabonnements für Linux</span><span class="sxs-lookup"><span data-stu-id="4c11e-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="4c11e-132">**Jährliche Linux-ISV-Abonnements**</span><span class="sxs-lookup"><span data-stu-id="4c11e-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="4c11e-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="4c11e-133">SUSE Linux</span></span>
- <span data-ttu-id="4c11e-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="4c11e-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="4c11e-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="4c11e-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="4c11e-136">**Jährliche ISV-Abonnements**</span><span class="sxs-lookup"><span data-stu-id="4c11e-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="4c11e-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="4c11e-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="4c11e-138">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="4c11e-138">Getting started</span></span>

<span data-ttu-id="4c11e-139">Um zu verstehen, wie Sie Azure Reservations mit ihren Kunden positionieren und so schnell wie möglich in Betrieb nehmen können, wird der folgende Ansatz empfohlen, um die Bereitschafts Materialien zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="4c11e-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="4c11e-140">Lesen und verstehen Sie das Handbuch für den [Partner Center New Commerce-Betriebshandbuch](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span><span class="sxs-lookup"><span data-stu-id="4c11e-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="4c11e-141">Informationen zu Updates für Azure Reservations-und Server Abonnements in der [Partner Center-API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="4c11e-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="4c11e-142">Vertriebsbereitschaft</span><span class="sxs-lookup"><span data-stu-id="4c11e-142">Sales readiness</span></span>

- [<span data-ttu-id="4c11e-143">Remotedesktopdienste (RDS)-Client Zugriffslizenz (CAL) (Ankündigung)</span><span class="sxs-lookup"><span data-stu-id="4c11e-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="4c11e-144">Azure reserved VM Instances (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4c11e-144">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="4c11e-145">Server-Abonnements</span><span class="sxs-lookup"><span data-stu-id="4c11e-145">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="4c11e-146">SQL-DB-Reservierungen (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4c11e-146">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="4c11e-147">Azure Cosmos DB (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4c11e-147">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="4c11e-148">SQL-verwaltete Instanz (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4c11e-148">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="4c11e-149">SuSE und Red Hat Enterprise Linux (Azure-Portal)</span><span class="sxs-lookup"><span data-stu-id="4c11e-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="4c11e-150">Red hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="4c11e-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="4c11e-151">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="4c11e-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="4c11e-152">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="4c11e-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="4c11e-153">Übersicht über Azure-Preise</span><span class="sxs-lookup"><span data-stu-id="4c11e-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="4c11e-154">Azure-Preisrechner</span><span class="sxs-lookup"><span data-stu-id="4c11e-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="4c11e-155">Azure Databricks Einheiten Reservierungen</span><span class="sxs-lookup"><span data-stu-id="4c11e-155">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="4c11e-156">Training</span><span class="sxs-lookup"><span data-stu-id="4c11e-156">Training</span></span>

<span data-ttu-id="4c11e-157">Registrieren Sie sich, um [kommerzielle Lizenzierungs Bereitschaft](https://commercial-licensing.eventbuilder.com/FY2019_ALL) und on-Demand-Veranstaltungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="4c11e-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="4c11e-158">Bei on-Demand-Ereignissen in der Vergangenheit aufgezeichnete Lizenz Bereitschaft sind folgende Themen enthalten:</span><span class="sxs-lookup"><span data-stu-id="4c11e-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="4c11e-159">CSP-Online Dienste, CSP-Azure und allgemeine Lizenzierungs Updates, einschließlich Azure (November 2018)</span><span class="sxs-lookup"><span data-stu-id="4c11e-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="4c11e-160">Reservierte Kapazität der SQL DB-Kapazität & instanzgröße (August 2018)</span><span class="sxs-lookup"><span data-stu-id="4c11e-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="4c11e-161">Server Abonnements in CSP (Juli 2018)</span><span class="sxs-lookup"><span data-stu-id="4c11e-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="4c11e-162">Azure Reservations Übersicht in CSP (Mai 2018)</span><span class="sxs-lookup"><span data-stu-id="4c11e-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="4c11e-163">Operationen (Operations)</span><span class="sxs-lookup"><span data-stu-id="4c11e-163">Operations</span></span>

<span data-ttu-id="4c11e-164">[Handbuch zum Service Center New Commerce-Betriebshandbuch](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): umfassendes Handbuch, das wichtige Richtlinien und betriebliche Aspekte behandelt, wie z. b. Verträge, die Bestellung über Partner Center, Rechnungen, Preislisten Details, Anreize, Abstimmungs Dateien, API/SDK, Sandbox und gemeinsame Azure-Partner Dienste.</span><span class="sxs-lookup"><span data-stu-id="4c11e-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="4c11e-165">Azure-Hybridvorteil</span><span class="sxs-lookup"><span data-stu-id="4c11e-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="4c11e-166">Der [Azure-Hybridvorteil](https://azure.microsoft.com/pricing/hybrid-benefit) ist ein Preisangebot für Kunden, die über Lizenzen mit Software Assurance verfügen, die bei der Migration zu Azure den Wert vorhandener lokaler Windows Server-und/oder SQL Server Lizenz Investitionen maximieren.</span><span class="sxs-lookup"><span data-stu-id="4c11e-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="4c11e-167">Berechtigte Kunden können bis zu 40% \* in Azure Virtual Machines (Infrastructure-as-a-Service oder IaaS) sparen und bis zu 55% in Azure SQL-Datenbank (Platform as a Service oder PAS) und SQL Server in Azure Virtual Machines (IaaS) mit Azure-Hybridvorteil sparen, was in Kombination mit reservierten Azure-Instanzen zu bis zu 80% zunimmt.</span><span class="sxs-lookup"><span data-stu-id="4c11e-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4c11e-168">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="4c11e-168">Next steps</span></span>

- [<span data-ttu-id="4c11e-169">Häufig gestellte Fragen zum Azure-Hybridvorteil</span><span class="sxs-lookup"><span data-stu-id="4c11e-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="4c11e-170">\*Aktuelle Einsparungen variieren basierend auf der Region, Instanztyp oder Nutzung</span><span class="sxs-lookup"><span data-stu-id="4c11e-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>