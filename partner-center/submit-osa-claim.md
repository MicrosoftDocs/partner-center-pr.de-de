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
ms.openlocfilehash: fec01e6c4554421593de4135ccd1af5c5e7ce13b
ms.sourcegitcommit: 1840767efa4c5de41889bc9245567cf286a084c8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/29/2020
ms.locfileid: "92917251"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="fa9e4-104">Kunden Zuordnungen über das beanspruchte cpor-Modell (Partner of Record) für Microsoft 365 und Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="fa9e4-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="fa9e4-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="fa9e4-105">**Applies to**</span></span>

- <span data-ttu-id="fa9e4-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="fa9e4-106">Partner Center</span></span>

<span data-ttu-id="fa9e4-107">**Geeignete Rollen:**</span><span class="sxs-lookup"><span data-stu-id="fa9e4-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="fa9e4-108">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="fa9e4-108">Incentives admin</span></span>

<span data-ttu-id="fa9e4-109">Am 1. Oktober 2019 begann Microsoft, das Claim Partner of Record-Modell (cpor) zu verwenden, um die Zuordnungen zu verwalten, die Sie mit Ihren Microsoft 365-und Dynamics 365-Kunden in Bezug auf die Online Services Advisory (OSA) Sell, das OSU-Microsoft 365 und OSU-Business Anwendungs Incentives haben.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="fa9e4-110">Kunden Zuordnungs Ansprüche (Customer Association, cpor) gelten nur für die Online Services Advisory (OSA) Selling-Microsoft 365 und OSU-Business Application Incentive-Programme.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="fa9e4-111">Wenn Sie einen Co-op-Anspruch für ein anderes Programm, z. b. cloudlösungsanbieter, verwalteten Händler, Hosting oder Oberfläche, übermitteln, lesen Sie den hier beschriebenen Co-op-Anspruchs Prozess.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="fa9e4-112">Wenn Sie Ihren Anspruch einreichen, wird er von Microsoft überprüft.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="fa9e4-113">Wir werden möglicherweise an dieser Stelle Weitere Informationen anfordern.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="fa9e4-114">Wir benachrichtigen den Kunden auch über Ihre Zuordnungs Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="fa9e4-115">Kunden haben fünf Werktage, um sich abzumelden. Wenn Sie sich nicht entscheiden, ist die Zuordnung zu diesem spezifischen Mandanten und der Arbeitsauslastung offiziell.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="fa9e4-116">An diesem Punkt haben Sie Zugriff auf die Nutzungsdaten des Kunden.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="fa9e4-117">Zum Vervollständigen eines Anspruchs benötigen Sie die folgenden Informationen:</span><span class="sxs-lookup"><span data-stu-id="fa9e4-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="fa9e4-118">Die **MPN-ID** für die Entität, die den Anspruch macht.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="fa9e4-119">**Domänen Name** des Kunden [Suchen](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="fa9e4-119">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="fa9e4-120">Verzeichnis- **ID** oder Mandanten- **ID** des Kunden [Suchen](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="fa9e4-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="fa9e4-121">Der **Lösungs Bereich** , z. b. Business Applications oder Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fa9e4-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="fa9e4-122">Die **Aktivität** , die Sie ausgeführt haben, und der Anspruchstyp, den Sie erstellen möchten, z. b. vor der Verkäufe, Verwendung oder Umsatz Zuordnung</span><span class="sxs-lookup"><span data-stu-id="fa9e4-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="fa9e4-123">**Kontakt Name** , Titel und e-Mail-Adresse Ihres Kunden</span><span class="sxs-lookup"><span data-stu-id="fa9e4-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="fa9e4-124">Für Dynamics 365 müssen Sie auch den **technischen Kontakt** Namen, den Titel und die e-Mail-Adresse Ihres Kunden angeben.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="fa9e4-125">**Kontakt Name** und e-Mail-Adresse Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="fa9e4-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="fa9e4-126">Sie erstellen einen **Namen** für diesen Anspruch.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="fa9e4-127">Die von Ihnen beanspruchten **Produkte** oder Arbeits Auslastungen</span><span class="sxs-lookup"><span data-stu-id="fa9e4-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="fa9e4-128">Der **Ausführungs Nachweis (PoE)** , z. b. eine vom Kunden signierte Anweisung.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="fa9e4-129">Sie können auch eine zu verwendende Poe-Vorlage herunterladen.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="fa9e4-130">Für Partner, die nur die Umsatz Zuordnung beanspruchen: **Name des Dynamics-Lösungs Verkäufers** , **Kunden Name** und **Name von ISV-Produkt/-Lösung** .</span><span class="sxs-lookup"><span data-stu-id="fa9e4-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="fa9e4-131">Außerdem sollten Sie die folgenden Punkte kennen:</span><span class="sxs-lookup"><span data-stu-id="fa9e4-131">You should also understand the following points:</span></span>

- <span data-ttu-id="fa9e4-132">Wenn Sie über Microsoft 365 Kunden verfügen, müssen Sie Sie erneut zuordnen, um die OSU-Anreize mithilfe dieses Prozesses zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="fa9e4-133">Wenn Sie über vorhandene Zuordnungen mit Dynamics 365 oder Power BI Kunden verfügen, bleiben diese Zuordnungen bis zum Ablauf Ihrer Abonnements gültig.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="fa9e4-134">Ein Kunde kann über mehrere Partner verfügen, aber die einzelnen Arbeits Auslastungen (für OSU-Microsoft 365) oder das Abonnement (für OSA-Sell-und OSU-Business Anwendungen) können nur einem Partner zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="fa9e4-135">Erstellen einer Kundenzuordnung</span><span class="sxs-lookup"><span data-stu-id="fa9e4-135">Create a customer association</span></span>

1. <span data-ttu-id="fa9e4-136">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="fa9e4-137">Wählen Sie die Registerkarte " **Incentives** " aus, wählen Sie **Übersicht** und dann **Kunden Zuordnungen** aus.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="fa9e4-138">Wählen Sie am oberen Rand der Seite Kunden Zuordnungen die Option **+ Customer Association** aus.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="fa9e4-139">Wählen Sie die **MPN-ID** des Partnerstandorts aus, der dem Kunden zugeordnet werden soll, und fügen Sie dann den Domänennamen und die Verzeichnis-ID des Kunden hinzu.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="fa9e4-140">Suchen Sie nach diesem</span><span class="sxs-lookup"><span data-stu-id="fa9e4-140">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="fa9e4-141">Wählen Sie **Weiter** .</span><span class="sxs-lookup"><span data-stu-id="fa9e4-141">Select **Continue** .</span></span>

6. <span data-ttu-id="fa9e4-142">Wählen Sie den projektmappenbereich und die **Aktivität** aus. **Solution area**</span><span class="sxs-lookup"><span data-stu-id="fa9e4-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="fa9e4-143">Wenn Sie Business Applications auswählen, wählen Sie entweder **Nutzung und/oder vorab Verkäufe** oder **Umsatz** Zuordnung aus, und klicken Sie dann auf **weiter** .</span><span class="sxs-lookup"><span data-stu-id="fa9e4-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="fa9e4-144">Wenn Sie die „Umsatzzuordnung“ auswählen, werden Sie aufgefordert, etwas andere Informationen als die unten aufgeführten Informationen anzugeben.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="fa9e4-145">Geben Sie die entsprechenden Informationen auf der Seite **Customer zuordnen** ein, und wählen Sie dann **Anspruch erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="fa9e4-146">Wählen Sie die mit dieser Kunden Zuordnung verknüpften Produkte aus, und klicken Sie dann auf **weiter** .</span><span class="sxs-lookup"><span data-stu-id="fa9e4-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="fa9e4-147">Vervollständigen Sie die Kundenkontaktinformationen und die Kontaktinformationen Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="fa9e4-148">Alle Felder sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="fa9e4-149">Wenn Ihr Produkt Dynamics 365 ist und das ausgewählte Produkt mehrere Abonnements für diesen bestimmten Kunden enthält, müssen Sie auch die Abonnement-ID eingeben.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="fa9e4-150">Stellen Sie Ihre Ausführungs Prüfung (PoE) bereit.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="fa9e4-151">Sie können ihn in das Feld ziehen, zur Ihrer eigenen zugehörigen Dokumentation navigieren oder eine Vorlage verwenden, indem Sie **Vorlage herunterladen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="fa9e4-152">Fügen Sie ggf. Kommentare hinzu und speichern sie, und wählen Sie dann **Anspruch senden** aus.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="fa9e4-153">Wir senden eine E-Mail an den Kunden, in der die Genehmigung ihrer Kundenzuordnung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="fa9e4-154">Nachdem Sie Ihre Kunden Zuordnung eingereicht haben, können Sie Sie nicht mehr bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="fa9e4-155">Der Status der Kundenzuordnung wird im Feld **Status** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="fa9e4-156">Wählen Sie **Verlauf**  aus, um den Verlauf einer Kundenzuordnung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="fa9e4-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa9e4-157">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="fa9e4-157">Next steps</span></span>

- [<span data-ttu-id="fa9e4-158">Verwalten von Kundenzuordnungen</span><span class="sxs-lookup"><span data-stu-id="fa9e4-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)