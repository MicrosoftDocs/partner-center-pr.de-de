---
title: Erstellen einer Kundenzuordnung
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Erstellen Sie Kunden Zuordnungen mit dem Anspruchs enden Partner of Record (cpor)-Modell. Hilft bei der Verwaltung von Verkäufen, Nutzung und Anreizen für Microsoft 365 & Dynamics 365-Kunden.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7a7e3ed40dcc6b1248f008201bff667a9eb9a0f8
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028314"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="ea3ac-104">Kunden Zuordnungen über das beanspruchte cpor-Modell (Partner of Record) für Microsoft 365 und Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ea3ac-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="ea3ac-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="ea3ac-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ea3ac-106">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="ea3ac-106">Incentives admin</span></span>

<span data-ttu-id="ea3ac-107">Am 1. Oktober 2019 begann Microsoft, das Claim Partner of Record-Modell (cpor) zu verwenden, um die Zuordnungen zu verwalten, die Sie mit Ihren Microsoft 365-und Dynamics 365-Kunden in Bezug auf die Online Services Advisory (OSA) Selling, die Nutzung der Onlinedienste (OSU) Microsoft 365 und OSU-Business Anwendungs Incentives haben.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="ea3ac-108">Kunden Zuordnungs Ansprüche (Customer Association, cpor) gelten nur für die Online Services Advisory (OSA) Selling-Microsoft 365 und OSU-Business Application Incentive-Programme.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-108">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="ea3ac-109">Wenn Sie einen Co-op-Anspruch für ein anderes Programm, z. b. cloudlösungsanbieter, verwalteten Händler, Hosting oder Oberfläche, übermitteln, lesen Sie den hier beschriebenen Co-op-Anspruchs Prozess.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-109">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="ea3ac-110">Wenn Sie Ihren Anspruch einreichen, wird er von Microsoft überprüft.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-110">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="ea3ac-111">Wir werden möglicherweise an dieser Stelle Weitere Informationen anfordern.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-111">We may ask you for more information at this point.</span></span> <span data-ttu-id="ea3ac-112">Wir benachrichtigen den Kunden auch über Ihre Zuordnungs Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-112">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="ea3ac-113">Kunden haben fünf Werktage, um sich abzumelden. Wenn Sie sich nicht entscheiden, ist die Zuordnung zu diesem spezifischen Mandanten und der Arbeitsauslastung offiziell.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-113">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="ea3ac-114">An diesem Punkt haben Sie Zugriff auf die Nutzungsdaten des Kunden.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-114">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="ea3ac-115">Zum Vervollständigen eines Anspruchs benötigen Sie die folgenden Informationen:</span><span class="sxs-lookup"><span data-stu-id="ea3ac-115">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="ea3ac-116">Die **MPN-ID** für die Entität, die den Anspruch macht.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-116">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="ea3ac-117">**Domänen Name** des Kunden [Suchen](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="ea3ac-117">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="ea3ac-118">Verzeichnis- **ID** oder Mandanten- **ID** des Kunden [Suchen](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="ea3ac-118">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="ea3ac-119">Der **Lösungs Bereich**, z. b. Business Applications oder Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ea3ac-119">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="ea3ac-120">Die **Aktivität** , die Sie ausgeführt haben, und der Anspruchstyp, den Sie erstellen möchten, z. b. vor der Verkäufe, Verwendung oder Umsatz Zuordnung</span><span class="sxs-lookup"><span data-stu-id="ea3ac-120">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="ea3ac-121">**Kontakt Name**, Titel und e-Mail-Adresse Ihres Kunden</span><span class="sxs-lookup"><span data-stu-id="ea3ac-121">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="ea3ac-122">Für Dynamics 365 müssen Sie auch den **technischen Kontakt** Namen, den Titel und die e-Mail-Adresse Ihres Kunden angeben.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-122">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="ea3ac-123">**Kontakt Name** und e-Mail-Adresse Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="ea3ac-123">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="ea3ac-124">Sie erstellen einen **Namen** für diesen Anspruch.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-124">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="ea3ac-125">Die von Ihnen beanspruchten **Produkte** oder Arbeits Auslastungen</span><span class="sxs-lookup"><span data-stu-id="ea3ac-125">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="ea3ac-126">Der **Ausführungs Nachweis (PoE)**, z. b. eine vom Kunden signierte Anweisung.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-126">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="ea3ac-127">Sie können auch eine zu verwendende Poe-Vorlage herunterladen.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-127">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="ea3ac-128">Für Partner, die nur die Umsatz Zuordnung beanspruchen: **Name des Dynamics-Lösungs Verkäufers**, **Kunden Name** und **Name von ISV-Produkt/-Lösung**.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-128">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="ea3ac-129">Außerdem sollten Sie die folgenden Punkte kennen:</span><span class="sxs-lookup"><span data-stu-id="ea3ac-129">You should also understand the following points:</span></span>

- <span data-ttu-id="ea3ac-130">Wenn Sie über Microsoft 365 Kunden verfügen, müssen Sie Sie erneut zuordnen, um die OSU-Anreize mithilfe dieses Prozesses zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-130">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="ea3ac-131">Wenn Sie über vorhandene Zuordnungen mit Dynamics 365 oder Power BI Kunden verfügen, bleiben diese Zuordnungen bis zum Ablauf Ihrer Abonnements gültig.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-131">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="ea3ac-132">Ein Kunde kann über mehrere Partner verfügen, aber die einzelnen Arbeits Auslastungen (für OSU-Microsoft 365) oder das Abonnement (für OSA-Sell-und OSU-Business Anwendungen) können nur einem Partner zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-132">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="ea3ac-133">Erstellen einer Kundenzuordnung</span><span class="sxs-lookup"><span data-stu-id="ea3ac-133">Create a customer association</span></span>

1. <span data-ttu-id="ea3ac-134">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ea3ac-135">Wählen Sie die Registerkarte " **Incentives** " aus, wählen Sie **Übersicht** und dann **Kunden Zuordnungen** aus.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-135">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="ea3ac-136">Wählen Sie am oberen Rand der Seite Kunden Zuordnungen die Option **+ Customer Association** aus.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-136">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="ea3ac-137">Wählen Sie die **MPN-ID** des Partnerstandorts aus, der dem Kunden zugeordnet werden soll, und fügen Sie dann den Domänennamen und die Verzeichnis-ID des Kunden hinzu.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-137">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="ea3ac-138">Suchen Sie nach diesem</span><span class="sxs-lookup"><span data-stu-id="ea3ac-138">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="ea3ac-139">Wählen Sie **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-139">Select **Continue**.</span></span>

6. <span data-ttu-id="ea3ac-140">Wählen Sie den projektmappenbereich und die **Aktivität** aus. </span><span class="sxs-lookup"><span data-stu-id="ea3ac-140">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="ea3ac-141">Wenn Sie Business Applications auswählen, wählen Sie entweder **Nutzung und/oder vorab Verkäufe** oder **Umsatz** Zuordnung aus, und klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-141">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="ea3ac-142">Wenn Sie die „Umsatzzuordnung“ auswählen, werden Sie aufgefordert, etwas andere Informationen als die unten aufgeführten Informationen anzugeben.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-142">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="ea3ac-143">Geben Sie die entsprechenden Informationen auf der Seite **Customer zuordnen** ein, und wählen Sie dann **Anspruch erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-143">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="ea3ac-144">Wählen Sie die mit dieser Kunden Zuordnung verknüpften Produkte aus, und klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-144">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="ea3ac-145">Vervollständigen Sie die Kundenkontaktinformationen und die Kontaktinformationen Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-145">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="ea3ac-146">Alle Felder sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-146">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="ea3ac-147">Wenn Ihr Produkt Dynamics 365 ist und das ausgewählte Produkt mehrere Abonnements für diesen bestimmten Kunden enthält, müssen Sie auch die Abonnement-ID eingeben.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-147">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="ea3ac-148">Stellen Sie Ihre Ausführungs Prüfung (PoE) bereit.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-148">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="ea3ac-149">Sie können ihn in das Feld ziehen, zur Ihrer eigenen zugehörigen Dokumentation navigieren oder eine Vorlage verwenden, indem Sie **Vorlage herunterladen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-149">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="ea3ac-150">Fügen Sie ggf. Kommentare hinzu und speichern sie, und wählen Sie dann **Anspruch senden** aus.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-150">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="ea3ac-151">Wir senden eine E-Mail an den Kunden, in der die Genehmigung ihrer Kundenzuordnung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-151">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="ea3ac-152">Nachdem Sie Ihre Kunden Zuordnung eingereicht haben, können Sie Sie nicht mehr bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-152">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="ea3ac-153">Der Status der Kundenzuordnung wird im Feld **Status** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-153">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="ea3ac-154">Wählen Sie **Verlauf**  aus, um den Verlauf einer Kundenzuordnung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="ea3ac-154">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ea3ac-155">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ea3ac-155">Next steps</span></span>

- [<span data-ttu-id="ea3ac-156">Verwalten von Kundenzuordnungen</span><span class="sxs-lookup"><span data-stu-id="ea3ac-156">Manage customer associations</span></span>](incentives-manage-customer-associations.md)