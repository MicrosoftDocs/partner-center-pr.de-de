---
title: Erstellen einer Kundenzuordnung
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Erstellen Sie Kundenzuordnungen mit dem Claiming Partner of Record -Modell (CPOR). Hilft bei der Verwaltung von Vertrieb, Nutzung und Incentives Microsoft 365 & Dynamics 365-Kunden.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489950"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="fe2af-104">Kundenzuordnungen über das CPOR-Modell (Claimed Partner of Record) für Microsoft 365 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="fe2af-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="fe2af-105">**Geeignete Rollen:** Incentives-Administrator</span><span class="sxs-lookup"><span data-stu-id="fe2af-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="fe2af-106">Am 1. Oktober 2019 begann Microsoft mit der Verwendung des Claiming Partner of Record-Modells (CPOR), um die Zuordnungen zu Ihren Microsoft 365- und Dynamics 365-Kunden im Hinblick auf die Incentives für Online services Advisory (OSA) Sell, Online Services Usage (OSU Microsoft 365) und OSU-Business Application zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="fe2af-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="fe2af-107">CPOR-Ansprüche (Customer Association) gelten nur für die Incentiveprogramme Online Services Advisory (OSA) Sell, Online Services Usage (OSU) und Microsoft 365 OSU-Business Application.</span><span class="sxs-lookup"><span data-stu-id="fe2af-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="fe2af-108">Wenn Sie einen Co-Op-Anspruch für ein anderes Programm wie Cloud Solution Provider (CSP), Managed Reseller, Hosting oder Surface übermitteln, lesen Sie den hier beschriebenen Co-Op-Anspruchsprozess.</span><span class="sxs-lookup"><span data-stu-id="fe2af-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="fe2af-109">Wenn Sie Ihren Anspruch übermitteln, überprüft Microsoft ihn.</span><span class="sxs-lookup"><span data-stu-id="fe2af-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="fe2af-110">An dieser Stelle können wir Sie um weitere Informationen bitten.</span><span class="sxs-lookup"><span data-stu-id="fe2af-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="fe2af-111">Wir benachrichtigen den Kunden auch über Ihre Zuordnungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="fe2af-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="fe2af-112">Kunden haben fünf Werktage Zeit, sich zu deaktivieren. Wenn sie sich nicht abmelden, ist Ihre Zuordnung zu diesem spezifischen Mandanten und dieser Workload offiziell.</span><span class="sxs-lookup"><span data-stu-id="fe2af-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="fe2af-113">An diesem Punkt haben Sie Zugriff auf die Nutzungsdaten des Kunden.</span><span class="sxs-lookup"><span data-stu-id="fe2af-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="fe2af-114">Sie benötigen die folgenden Informationen, um einen Anspruch zu vervollständigen:</span><span class="sxs-lookup"><span data-stu-id="fe2af-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="fe2af-115">Die **MPN-ID** (Microsoft Partner Network-ID) für Ihre Entität, die den Anspruch erstellt</span><span class="sxs-lookup"><span data-stu-id="fe2af-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="fe2af-116">Domänenname des **Kunden** (weitere Informationen finden Sie unter Suchen der [Mandanten-ID, des Domänennamens, der Benutzerobjekt-ID)](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="fe2af-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="fe2af-117">Verzeichnis-ID oder **Mandanten-ID** des Kunden (weitere Informationen finden Sie unter Suchen der  [Mandanten-ID, des Domänennamens, der Benutzerobjekt-ID).](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="fe2af-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="fe2af-118">Der **Projektmappenbereich,** z. B. Business Applications oder Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fe2af-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="fe2af-119">Die **aktivität,** die Sie ausgeführt haben, und der Typ des Anspruchs, den Sie machen möchten, z. B. Pre-Sales, Usage oder Revenue association</span><span class="sxs-lookup"><span data-stu-id="fe2af-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="fe2af-120">Kontaktname, Titel **und** E-Mail-Adresse Ihres Kunden</span><span class="sxs-lookup"><span data-stu-id="fe2af-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="fe2af-121">Für Dynamics 365 müssen Sie auch den  Namen des technischen Kontakts, den Titel und die E-Mail-Adresse Ihres Kunden angeben.</span><span class="sxs-lookup"><span data-stu-id="fe2af-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="fe2af-122">Kontaktname und  E-Mail-Adresse Ihres eigenen Unternehmens</span><span class="sxs-lookup"><span data-stu-id="fe2af-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="fe2af-123">Sie erstellen einen Namen **für** diesen Anspruch.</span><span class="sxs-lookup"><span data-stu-id="fe2af-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="fe2af-124">Die **Produkte oder Workloads,** die Sie beanspruchen</span><span class="sxs-lookup"><span data-stu-id="fe2af-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="fe2af-125">**Ausführungsnachweis (Proof of Execution, PoE),** z. B. eine vom Kunden signierte Arbeitserklärung.</span><span class="sxs-lookup"><span data-stu-id="fe2af-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="fe2af-126">Sie können auch eine Zu verwendende PoE-Vorlage herunterladen.</span><span class="sxs-lookup"><span data-stu-id="fe2af-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="fe2af-127">Nur für Partner, die umsatzorientierte Zuordnungen beanspruchen: Name des Dynamics-Lösungsverkäufer, **Kundenname** und **Name des ISV-Produkts/der ISV-Lösung**. </span><span class="sxs-lookup"><span data-stu-id="fe2af-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="fe2af-128">Sie sollten auch die folgenden Punkte verstehen:</span><span class="sxs-lookup"><span data-stu-id="fe2af-128">You should also understand the following points:</span></span>

- <span data-ttu-id="fe2af-129">Wenn Sie bereits über Microsoft 365-Kunden verfügen, müssen Sie sich mit denjenigen neu verknüpfen, die Sie mit diesem Prozess weiterhin OSU-Incentives erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="fe2af-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="fe2af-130">Wenn Sie bereits Zuordnungen mit Dynamics 365- oder Power BI-Kunden haben, bleiben diese Zuordnungen bis zum Ablauf ihrer Abonnements gültig.</span><span class="sxs-lookup"><span data-stu-id="fe2af-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="fe2af-131">Ein Kunde kann mehrere Partner haben, aber jede Workload (für OSU-Microsoft 365) oder jedes Abonnement (für OSA-Sell- und OSU-Business-Anwendungen) kann nur einem Partner zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="fe2af-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="fe2af-132">Erstellen einer Kundenzuordnung</span><span class="sxs-lookup"><span data-stu-id="fe2af-132">Create a customer association</span></span>

1. <span data-ttu-id="fe2af-133">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="fe2af-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="fe2af-134">Wählen Sie die **Registerkarte Incentives** aus, wählen **Sie Übersicht** und dann **Kundenzuordnungen aus.**</span><span class="sxs-lookup"><span data-stu-id="fe2af-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="fe2af-135">Wählen Sie oben auf der Seite Kundenzuordnungen die Option **+ Kundenzuordnung aus.**</span><span class="sxs-lookup"><span data-stu-id="fe2af-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="fe2af-136">Wählen Sie die **MPN-ID** des Partnerstandorts aus, der dem Kunden zugeordnet werden soll, und fügen Sie dann den Domänennamen und die Verzeichnis-ID des Kunden hinzu.</span><span class="sxs-lookup"><span data-stu-id="fe2af-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="fe2af-137">Suchen Sie nach diesem</span><span class="sxs-lookup"><span data-stu-id="fe2af-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="fe2af-138">Wählen Sie **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="fe2af-138">Select **Continue**.</span></span>

6. <span data-ttu-id="fe2af-139">Wählen Sie den **Bereich Projektmappe und** **Aktivität aus.**</span><span class="sxs-lookup"><span data-stu-id="fe2af-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="fe2af-140">Wenn Sie Business Applications auswählen, wählen Sie entweder **Nutzung und/oder Pre-Sales** oder **Revenue association** aus, und wählen Sie dann **Weiter aus.**</span><span class="sxs-lookup"><span data-stu-id="fe2af-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="fe2af-141">Wenn Sie die „Umsatzzuordnung“ auswählen, werden Sie aufgefordert, etwas andere Informationen als die unten aufgeführten Informationen anzugeben.</span><span class="sxs-lookup"><span data-stu-id="fe2af-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="fe2af-142">Geben Sie die entsprechenden Informationen auf der Seite **Kunden zuordnen** ein, und wählen Sie dann Anspruch **erstellen aus.**</span><span class="sxs-lookup"><span data-stu-id="fe2af-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="fe2af-143">Wählen Sie die Produkte aus, die dieser Kundenbindung zugeordnet sind, und wählen Sie dann **Weiter aus.**</span><span class="sxs-lookup"><span data-stu-id="fe2af-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="fe2af-144">Vervollständigen Sie die Kundenkontaktinformationen und die Kontaktinformationen Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="fe2af-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="fe2af-145">Alle Felder sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe2af-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="fe2af-146">Wenn Ihr Produkt Dynamics 365 ist und das von Ihnen auswählen Produkt über mehrere Abonnements für diesen bestimmten Kunden verfügt, müssen Sie auch die Abonnement-ID eingeben.</span><span class="sxs-lookup"><span data-stu-id="fe2af-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="fe2af-147">Geben Sie Ihren PoE an.</span><span class="sxs-lookup"><span data-stu-id="fe2af-147">Supply your PoE.</span></span> <span data-ttu-id="fe2af-148">Sie können ihn in das Feld ziehen, zur Ihrer eigenen zugehörigen Dokumentation navigieren oder eine Vorlage verwenden, indem Sie **Vorlage herunterladen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="fe2af-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="fe2af-149">Fügen Sie ggf. Kommentare hinzu und speichern sie, und wählen Sie dann **Anspruch senden** aus.</span><span class="sxs-lookup"><span data-stu-id="fe2af-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="fe2af-150">Wir senden eine E-Mail an den Kunden, in der die Genehmigung ihrer Kundenzuordnung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="fe2af-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="fe2af-151">Nachdem Sie Ihre Kundenbindung übermittelt haben, können Sie sie nicht mehr bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="fe2af-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="fe2af-152">Der Status der Kundenzuordnung wird im Feld **Status** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fe2af-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="fe2af-153">Wählen Sie **Verlauf**  aus, um den Verlauf einer Kundenzuordnung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="fe2af-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fe2af-154">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="fe2af-154">Next steps</span></span>

- [<span data-ttu-id="fe2af-155">Verwalten von Kundenzuordnungen</span><span class="sxs-lookup"><span data-stu-id="fe2af-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)