---
title: Übertragen eines Azure-Abonnements unter einem Azure-Plan an einen anderen CSP-Partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie den Cloud Solution Provider Programmpartner ändern, der den Azure-Abonnements eines Kunden unter einem Azure-Plan zugeordnet ist.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284501"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="99238-103">Übertragen der Azure-Planabonnements eines Kunden an einen anderen Partner</span><span class="sxs-lookup"><span data-stu-id="99238-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="99238-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="99238-104">**Appropriate roles**</span></span>

- <span data-ttu-id="99238-105">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="99238-105">Account admin</span></span>
- <span data-ttu-id="99238-106">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="99238-106">Sales agent</span></span>
- <span data-ttu-id="99238-107">Abrechnungs-Agent</span><span class="sxs-lookup"><span data-stu-id="99238-107">Billing agent</span></span>

<span data-ttu-id="99238-108">In diesem Artikel wird beschrieben, wie ein Kunde seine Azure-Abonnements unter einem Azure-Plan von einem Cloud Solution Provider (CSP) zu einem anderen wechseln kann.</span><span class="sxs-lookup"><span data-stu-id="99238-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="99238-109">Führen Sie die folgenden Schritte aus, um die Azure-Abonnements eines Kunden von einem anderen Partner zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="99238-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="99238-110">Sowohl der Partner als auch der Kunde müssen schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="99238-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="99238-111">Nur Partner mit einer direkten Abrechnungsbeziehung mit Microsoft können auf die Übergangstools zugreifen.</span><span class="sxs-lookup"><span data-stu-id="99238-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="99238-112">Indirekte Vertriebspartner müssen mit ihren indirekten Anbietern zusammenarbeiten, um dieses Übergangstool nutzen zu können.</span><span class="sxs-lookup"><span data-stu-id="99238-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="99238-113">Der Kunde muss sich mit beiden Partnern (aktuell und zukünftig) in Verbindung setzen, bevor dieses Tool genutzt wird.</span><span class="sxs-lookup"><span data-stu-id="99238-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="99238-114">Eine Offlinekonversation muss erforderlich sein, um Verwirrung und Abwanderung zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="99238-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="99238-115">Darüber hinaus sollten Partner und Kunden diese Überlegungen und Voraussetzungen verstehen, bevor sie einen Übergang initiieren:</span><span class="sxs-lookup"><span data-stu-id="99238-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="99238-116">**Wichtige Überlegungen:**</span><span class="sxs-lookup"><span data-stu-id="99238-116">**Key considerations:**</span></span>

- <span data-ttu-id="99238-117">Azure-Reservierungen werden nicht mit dem Abonnement zu einem zukünftigen Partner verschoben</span><span class="sxs-lookup"><span data-stu-id="99238-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="99238-118">CSP-Preise für Azure-Dienste unter dem aktuellen Partner werden nicht umgestellt</span><span class="sxs-lookup"><span data-stu-id="99238-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="99238-119">Supportaufgaben für Kunden werden an zukünftige Partner übertragen</span><span class="sxs-lookup"><span data-stu-id="99238-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="99238-120">Abrechnung und Rechnungsstellung werden zum Zeitpunkt der Übertragung an den zukünftigen Partner umsteigen.</span><span class="sxs-lookup"><span data-stu-id="99238-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="99238-121">Azure Role-Based Access Control (RBAC) ist von der Übertragung nicht betroffen</span><span class="sxs-lookup"><span data-stu-id="99238-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="99238-122">Administrator im Auftrag von (Admin on Behalf Of, AOBO) wird dem zukünftigen Partner nicht standardmäßig gewährt.</span><span class="sxs-lookup"><span data-stu-id="99238-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="99238-123">Marketplace-Produkte von Drittanbietern werden übertragen, solange die Produkte die Überprüfung der Marketplace-Berechtigung bestehen.</span><span class="sxs-lookup"><span data-stu-id="99238-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="99238-124">Es gibt keine besonderen Rabatte oder regionalen Einschränkungen.</span><span class="sxs-lookup"><span data-stu-id="99238-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="99238-125">Die Produkte sind nicht abonnementbasierte Produkte.</span><span class="sxs-lookup"><span data-stu-id="99238-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="99238-126">Der zukünftige Partner sollte mit dem Herausgeber zusammenarbeiten, um sicherzustellen, dass er in der Allowlist für die Bereitstellung des Produkts ist.</span><span class="sxs-lookup"><span data-stu-id="99238-126">The future partner should work with the publisher to make sure they are on the allowlist for deployment of the product</span></span>
    - <span data-ttu-id="99238-127">Wenn nicht alle diese Bedingungen erfüllt sind, um die Marketplace-Produkte zu übertragen, sollten sie storniert, die Azure-Abonnements übertragen und dann Marketplace-Produkte mit dem neuen Partner neu erwerben.</span><span class="sxs-lookup"><span data-stu-id="99238-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="99238-128">**Voraussetzungen:**</span><span class="sxs-lookup"><span data-stu-id="99238-128">**Prerequisites:**</span></span>

- <span data-ttu-id="99238-129">Der Kunde bespricht den aktuellen CSP-Partner in seiner Absicht, den Übergang zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="99238-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="99238-130">Zukünftige CSP-Partner arbeiten mit Kunden zusammen, um sicherzustellen, dass die Kundenanforderungen erfüllt werden können.</span><span class="sxs-lookup"><span data-stu-id="99238-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="99238-131">Zukünftiger CSP-Partner richtet eine Beziehung mit dem Kunden ein und erwirbt einen Azure-Plan, bevor der Übergang beginnt.</span><span class="sxs-lookup"><span data-stu-id="99238-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="99238-132">Der Kunde muss sich Microsoft-Kundenvereinbarung zukünftigen CSP-Partner anmelden.</span><span class="sxs-lookup"><span data-stu-id="99238-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="99238-133">ZukünftigeR CSP-Partner muss die Microsoft Partner-Vereinbarung für die Verwendung dieses Tools signiert haben.</span><span class="sxs-lookup"><span data-stu-id="99238-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="99238-134">Auszuführende Kundenaufgaben</span><span class="sxs-lookup"><span data-stu-id="99238-134">Customer tasks to be completed</span></span>

<span data-ttu-id="99238-135">Um ein Azure-Abonnement unter einem Azure-Plan zu übertragen, muss der Kunde den Prozess starten, indem er sich an seinen aktuellen Partner wenden kann.</span><span class="sxs-lookup"><span data-stu-id="99238-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="99238-136">Sie sollten den Unternehmensnamen und die Domäne ihres aktuellen Partners erfassen, damit der zukünftige Partner das Formular für die Übertragungsanforderung in ihrem Namen ausfüllen kann.</span><span class="sxs-lookup"><span data-stu-id="99238-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="99238-137">Der Kunde muss auch die Abonnements identifizieren, die er vom aktuellen Partner übertragen möchte.</span><span class="sxs-lookup"><span data-stu-id="99238-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="99238-138">Partner für Office 365-, Enterprise Mobility Suite- oder Microsoft Dynamics CRM-Abonnements können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="99238-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="99238-139">Es liegt in der Verantwortung des zukünftigen Partners, das Übertragungsanforderungsformular zu ausfüllen, das den Übertragungsprozess initiiert.</span><span class="sxs-lookup"><span data-stu-id="99238-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="99238-140">Microsoft kann nicht im Auftrag des Kunden oder des aktuellen Partners eingreifen.</span><span class="sxs-lookup"><span data-stu-id="99238-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="99238-141">Der Kunde sollte eine enge Zusammenarbeit mit seinem zukünftigen und aktuellen Partner planen, um den Übergang reibungslos zu gestalten.</span><span class="sxs-lookup"><span data-stu-id="99238-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="99238-142">Zukünftige Partneraufgaben, die abgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="99238-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="99238-143">Der zukünftige Partner des Abonnements muss ein Übertragungsanforderungsformular von Partner Center um eine Abonnementübertragung an fordern zu können:</span><span class="sxs-lookup"><span data-stu-id="99238-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="99238-144">Wählen Sie Partner Center Menü Kunden aus, und wählen Sie dann den Kunden aus, für den Sie ein Übertragungsanforderungsformular ausfüllen möchten.</span><span class="sxs-lookup"><span data-stu-id="99238-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="99238-145">Wählen Sie im Menü Kunde die Option **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="99238-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="99238-146">Wählen Sie den Abschnitt **Übertragungsanforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="99238-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="99238-147">Wählen Sie im **Abschnitt Übertragungsanforderung** die Option **Neue Anforderung hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="99238-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Abschnitt &quot;Übertragungen&quot;":::

5.  <span data-ttu-id="99238-149">Füllen Sie das Formular **Neue Übertragungsanforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="99238-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="99238-150">Wählen Sie Send transfer request Send **(Übertragungsanforderung**  >  **senden) aus.**</span><span class="sxs-lookup"><span data-stu-id="99238-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Ausfüllen des Formulars für Übertragungsanforderung":::

7.  <span data-ttu-id="99238-152">Überprüfen der Bestätigung der Übertragungsanforderung</span><span class="sxs-lookup"><span data-stu-id="99238-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Überprüfen der ausstehenden Übertragung":::

    >[!Note]
    ><span data-ttu-id="99238-154">Der zukünftige Partner kann die Übertragungsanforderung abbrechen, indem er die **Anforderung abbrechen** in der oberen rechten Ecke nur dann auswählt, wenn der Status der Übertragungsanforderung "Ausstehend" lautet.</span><span class="sxs-lookup"><span data-stu-id="99238-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="99238-155">Sobald der Status der Übertragungsanforderung "In Bearbeitung" oder "Abgeschlossen" lautet, sind Keine Abbruchs möglich.</span><span class="sxs-lookup"><span data-stu-id="99238-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="99238-156">Aktuelle Partneraufgaben, die abgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="99238-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="99238-157">Der Administrator-Agent des aktuellen Partners des Kunden erhält eine E-Mail, dass der Kunde eine Übertragung seiner Abonnements anfordert:</span><span class="sxs-lookup"><span data-stu-id="99238-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Überprüfung":::

<span data-ttu-id="99238-159">Überprüfen und akzeptieren Sie das Formular für die Übertragungsanforderung von Partner Center, um die Abonnementübertragung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="99238-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="99238-160">Wenn vom aktuellen Partner innerhalb von 30 Tagen keine Aktion ausgeführt wird, läuft die Anforderung ab, und der zukünftige Partner muss eine neue Übertragungsanforderung erstellen.</span><span class="sxs-lookup"><span data-stu-id="99238-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="99238-161">Wählen Sie **Übertragungsanforderung** überprüfen aus der E-Mail oder aus.</span><span class="sxs-lookup"><span data-stu-id="99238-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="99238-162">**Wählen** Sie im Menü Partner Center kunden und dann den Kunden aus, für den eine Übertragungsanforderung übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="99238-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="99238-163">Wählen Sie im Menü Kunde die Option **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="99238-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="99238-164">Wählen Sie den Abschnitt **Übertragungsanforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="99238-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="99238-165">Erweitern Sie Übertragungsinformationen, indem Sie unter **Empfangene Anforderungen** die ausgewählte **Übertragungsanforderungs-ID** auswählen.</span><span class="sxs-lookup"><span data-stu-id="99238-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Übertragungsanforderung für Quellüberprüfungen":::

5.  <span data-ttu-id="99238-167">Überprüfen Sie die Übertragungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="99238-167">Review transfer request.</span></span> <span data-ttu-id="99238-168">Wählen Sie die angeforderten Azure-Abonnements für die Übertragung aus.</span><span class="sxs-lookup"><span data-stu-id="99238-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="99238-169">Bevor Sie fortfahren, beachten Sie: Sie haben keinen Zugriff mehr auf die ausgewählten Abonnements.</span><span class="sxs-lookup"><span data-stu-id="99238-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="99238-170">Die weitere Nutzung wird Ihnen nicht in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="99238-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="99238-171">Azure-Reservierungen werden nicht mit den Abonnements übertragen.</span><span class="sxs-lookup"><span data-stu-id="99238-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="99238-172">Wählen Sie dann **Akzeptieren und übertragen aus,** um den Übertragungsprozess abschließen zu können.</span><span class="sxs-lookup"><span data-stu-id="99238-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Auswählen von Abonnements, die unter Ihren Azure-Plänen übertragen werden sollen":::

7.  <span data-ttu-id="99238-174">Anzeigen der Bestätigung der Übertragungsakzeptanz.</span><span class="sxs-lookup"><span data-stu-id="99238-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="99238-175">An diesem Punkt werden der zukünftige Partner, der Kunde und der aktuelle Partner per E-Mail über die akzeptierte Übertragungsanforderung benachrichtigt.</span><span class="sxs-lookup"><span data-stu-id="99238-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="99238-176">Nachdem der Übergang akzeptiert wurde, bleibt der Übertragungsstatus möglicherweise bis zu 15 Minuten ausstehend, während das System aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="99238-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="99238-177">Wenn dies länger dauert, versucht das System drei Tage lang weiter.</span><span class="sxs-lookup"><span data-stu-id="99238-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="99238-178">Wenn der Übertragungsstatus weiterhin Ausstehend bleibt, sollte der Partner eine Serviceanfrage senden.</span><span class="sxs-lookup"><span data-stu-id="99238-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="99238-179">Nach Abschluss der Übertragung werden die in der Anforderung enthaltenen Abonnements im Azure-Plan des zukünftigen Partners angezeigt und nicht mehr bei Ihnen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="99238-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="99238-180">Für indirekte Anbieter: Informieren Sie Ihren indirekten Vertriebspartner, dass die Übertragungsanforderung akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="99238-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="99238-181">Verwalten Ihrer übertragenen Kundenabonnements</span><span class="sxs-lookup"><span data-stu-id="99238-181">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="99238-182">Der Zugriff auf vorhandene Benutzer, Gruppen oder Dienstprinzipale, die per rollenbasierter Azure-Zugriffssteuerung (Azure Role-Based Access Control, Azure RBAC) zugewiesen wurden, ist von der Übertragung nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="99238-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="99238-183">Die rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access [Control, Azure RBAC)](/azure/role-based-access-control/overview) hilft Ihrem Kunden, zu verwalten, wer Zugriff auf Azure-Ressourcen hat, was er mit diesen Ressourcen tun kann und auf welche Bereiche er Zugriff hat.</span><span class="sxs-lookup"><span data-stu-id="99238-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="99238-184">Als neuer Partner erhalten Sie nach der Abonnementübertragung keinen RBAC-Zugriff auf die Ressourcen Ihres Kunden.</span><span class="sxs-lookup"><span data-stu-id="99238-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="99238-185">Der vorherige Partner Ihres Kunden behält seinen RBAC-Zugriff bei.</span><span class="sxs-lookup"><span data-stu-id="99238-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="99238-186">Arbeiten Sie mit Ihrem Kunden zusammen, um zu verstehen, wer Einblick in seine Abonnements hat und wie Sie die änderungen vornehmen können.</span><span class="sxs-lookup"><span data-stu-id="99238-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="99238-187">Daher ist es wichtig, dass Ihr Kunde den Azure RBAC-Zugriff für seinen vorherigen Partner entfernt und den Zugriff für den neuen Partner hinzufüge.</span><span class="sxs-lookup"><span data-stu-id="99238-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="99238-188">Weitere Informationen dazu, wie Ihr Kunde neuen Zugriff erteilt, finden Sie unter Was ist die [rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="99238-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="99238-189">Weitere Informationen dazu, wie Ihr Kunde den RBAC-Zugriff Ihres vorherigen Partners entfernt, finden Sie unter [Entfernen einer Rollenzuweisung.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="99238-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="99238-190">Darüber hinaus erhalten Sie nicht automatisch [Zugriff vom Administrator im Auftrag von (Admin on Behalf Of, AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) auf Ihre Abonnements.</span><span class="sxs-lookup"><span data-stu-id="99238-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="99238-191">AOBO ist erforderlich, damit Partner die Azure-Abonnements ihrer Kunden in ihrem Namen verwalten können.</span><span class="sxs-lookup"><span data-stu-id="99238-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="99238-192">Weitere Informationen zu Azure-Berechtigungen finden Sie unter [Abrufen von Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="99238-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="99238-193">Nächste Schritte:</span><span class="sxs-lookup"><span data-stu-id="99238-193">Next steps:</span></span>

- [<span data-ttu-id="99238-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="99238-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="99238-195">Abrufen von Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden.</span><span class="sxs-lookup"><span data-stu-id="99238-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
