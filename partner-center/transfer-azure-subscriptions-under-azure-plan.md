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
ms.openlocfilehash: f0abfdfd2fbb242f7cdbe0ded04d387ea712cce5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702721"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="87ad8-103">Übertragen der Azure-Planabonnements eines Kunden an einen anderen Partner</span><span class="sxs-lookup"><span data-stu-id="87ad8-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="87ad8-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="87ad8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="87ad8-105">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="87ad8-105">Account admin</span></span>
- <span data-ttu-id="87ad8-106">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="87ad8-106">Sales agent</span></span>
- <span data-ttu-id="87ad8-107">Abrechnungs-Agent</span><span class="sxs-lookup"><span data-stu-id="87ad8-107">Billing agent</span></span>

<span data-ttu-id="87ad8-108">In diesem Artikel wird beschrieben, wie ein Kunde seine Azure-Abonnements unter einem Azure-Plan von einem Cloud Solution Provider (CSP) in einen anderen umschalten kann.</span><span class="sxs-lookup"><span data-stu-id="87ad8-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="87ad8-109">Führen Sie die folgenden Schritte aus, um die Azure-Abonnements eines Kunden von einem anderen Partner zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="87ad8-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="87ad8-110">Sowohl der Partner als auch der Kunde müssen schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="87ad8-111">Nur Partner mit direkter Abrechnungsbeziehung mit Microsoft können auf die Umstellungstools zugreifen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="87ad8-112">Indirekte Wiederverkäufer müssen mit ihren indirekten Anbietern zusammenarbeiten, um dieses Übergangstool zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="87ad8-113">Der Kunde muss mit beiden Partnern (aktuell und zukünftig) im Gespräch sein, bevor dieses Tool genutzt wird.</span><span class="sxs-lookup"><span data-stu-id="87ad8-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="87ad8-114">Eine Offline-Konversation muss ausgeführt werden, um Verwirrung und Abwanderung zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="87ad8-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="87ad8-115">Darüber hinaus sollten Partner und Kunden diese Überlegungen und Voraussetzungen kennen, bevor sie einen Übergang initiieren:</span><span class="sxs-lookup"><span data-stu-id="87ad8-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="87ad8-116">**Wichtige Überlegungen:**</span><span class="sxs-lookup"><span data-stu-id="87ad8-116">**Key considerations:**</span></span>

- <span data-ttu-id="87ad8-117">Azure-Reservierungen werden nicht mit dem Abonnement zum zukünftigen Partner umziehen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="87ad8-118">CSP-Preise für Azure-Dienste unter dem aktuellen Partner werden nicht umstiegen</span><span class="sxs-lookup"><span data-stu-id="87ad8-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="87ad8-119">Supportaufgaben für Den Kunden werden zu zukünftigen Partnern wechseln</span><span class="sxs-lookup"><span data-stu-id="87ad8-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="87ad8-120">Abrechnung und Rechnungsstellung werden zum Zeitpunkt der Übertragung an den zukünftigen Partner übertragen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="87ad8-121">Azure Role-Based Access Control (RBAC) ist von der Übertragung nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="87ad8-122">Der Administrator im Auftrag von (AOBO) wird dem zukünftigen Partner nicht standardmäßig gewährt.</span><span class="sxs-lookup"><span data-stu-id="87ad8-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="87ad8-123">Marketplace-Produkte von Drittanbietern werden übertragen, solange die Produkte die Marketplace-Berechtigungsprüfung bestehen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="87ad8-124">Es gibt keine speziellen Rabatte oder regionalen Einschränkungen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="87ad8-125">Die Produkte sind nicht abonnementbasiert.</span><span class="sxs-lookup"><span data-stu-id="87ad8-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="87ad8-126">Der zukünftige Partner sollte mit dem Herausgeber zusammenarbeiten, um sicherzustellen, dass er sich in der Liste mit den Zulässigen für die Bereitstellung des Produkts befindet.</span><span class="sxs-lookup"><span data-stu-id="87ad8-126">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="87ad8-127">Wenn nicht alle diese Bedingungen erfüllt sind, um die Marketplace-Produkte zu übertragen, sollten sie storniert, die Azure-Abonnements übertragen und dann marketplace-Produkte mit dem neuen Partner erneut erworben werden.</span><span class="sxs-lookup"><span data-stu-id="87ad8-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="87ad8-128">**Voraussetzungen:**</span><span class="sxs-lookup"><span data-stu-id="87ad8-128">**Prerequisites:**</span></span>

- <span data-ttu-id="87ad8-129">Der Kunde betreibt den aktuellen CSP-Partner bei seiner Absicht, zu übergehen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="87ad8-130">Zukünftiger CSP-Partner arbeitet mit Kunden zusammen, um sicherzustellen, dass die Kundenanforderungen erfüllt werden können.</span><span class="sxs-lookup"><span data-stu-id="87ad8-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="87ad8-131">Zukünftiger CSP-Partner stellt eine Beziehung mit dem Kunden her und erwirbt einen Azure-Plan, bevor der Übergang beginnt.</span><span class="sxs-lookup"><span data-stu-id="87ad8-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="87ad8-132">Kunde muss Microsoft-Kundenvereinbarung mit zukünftigem CSP-Partner signieren</span><span class="sxs-lookup"><span data-stu-id="87ad8-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="87ad8-133">Der zukünftige CSP-Partner muss die Microsoft Partner-Vereinbarung signiert haben, um dieses Tool verwenden zu können.</span><span class="sxs-lookup"><span data-stu-id="87ad8-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="87ad8-134">Auszuführende Kundenaufgaben</span><span class="sxs-lookup"><span data-stu-id="87ad8-134">Customer tasks to be completed</span></span>

<span data-ttu-id="87ad8-135">Um ein Azure-Abonnement unter einem Azure-Plan zu übertragen, muss der Kunde den Prozess starten, indem er sich an den aktuellen Partner wendet.</span><span class="sxs-lookup"><span data-stu-id="87ad8-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="87ad8-136">Sie sollten den Firmennamen und die Domäne ihres aktuellen Partners erfassen, damit der zukünftige Partner das Formular für die Übertragungsanforderung in ihrem Namen ausfüllen kann.</span><span class="sxs-lookup"><span data-stu-id="87ad8-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="87ad8-137">Der Kunde muss auch die Abonnements identifizieren, die er vom aktuellen Partner übertragen möchte.</span><span class="sxs-lookup"><span data-stu-id="87ad8-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="87ad8-138">Partner für Office 365-, Enterprise Mobility Suite- oder Microsoft Dynamics CRM-Abonnements können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="87ad8-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="87ad8-139">Es liegt in der Verantwortung des zukünftigen Partners, das Formular für die Übertragungsanforderung auszufüllen, das den Übertragungsvorgang initiiert.</span><span class="sxs-lookup"><span data-stu-id="87ad8-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="87ad8-140">Microsoft kann nicht im Auftrag des Kunden oder des aktuellen Partners eingreifen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="87ad8-141">Der Kunde sollte planen, eng mit dem zukünftigen und aktuellen Partner zusammenzuarbeiten, damit der Übergang reibungslos verläuft.</span><span class="sxs-lookup"><span data-stu-id="87ad8-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="87ad8-142">Zukünftige Partneraufgaben, die abgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="87ad8-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="87ad8-143">Der zukünftige Partner des Abonnements muss ein Übertragungsanforderungsformular von Partner Center ausfüllen, um eine Abonnementübertragung anzufordern:</span><span class="sxs-lookup"><span data-stu-id="87ad8-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="87ad8-144">**Wählen** Sie im Menü Partner Center kunden und dann den Kunden aus, für den Sie ein Formular für eine Übertragungsanforderung ausfüllen möchten.</span><span class="sxs-lookup"><span data-stu-id="87ad8-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="87ad8-145">Wählen Sie im Menü Kunde die Option **Abonnements aus.**</span><span class="sxs-lookup"><span data-stu-id="87ad8-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="87ad8-146">Wählen Sie den **Abschnitt Übertragungsanforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="87ad8-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="87ad8-147">Wählen Sie **im Abschnitt Übertragungsanforderung** die Option **Neue Anforderung hinzufügen aus.**</span><span class="sxs-lookup"><span data-stu-id="87ad8-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Abschnitt &quot;Übertragungen&quot;":::

5.  <span data-ttu-id="87ad8-149">Füllen Sie das **Formular Neue Übertragungsanforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="87ad8-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="87ad8-150">Wählen Sie **Übertragungsanforderung**  >  **senden Senden aus.**</span><span class="sxs-lookup"><span data-stu-id="87ad8-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formular &quot;Übertragungsanforderung abschließen&quot;":::

7.  <span data-ttu-id="87ad8-152">Überprüfen der Bestätigung der Übertragungsanforderung</span><span class="sxs-lookup"><span data-stu-id="87ad8-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Überprüfen der ausstehenden Übertragung":::

    >[!Note]
    ><span data-ttu-id="87ad8-154">Der zukünftige Partner kann die Übertragungsanforderung nur dann abbrechen, wenn der Status der Übertragungsanforderung "Ausstehend" ist. </span><span class="sxs-lookup"><span data-stu-id="87ad8-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="87ad8-155">Sobald der Status der Übertragungsanforderung "In Bearbeitung" oder "Abgeschlossen" ist, sind Abbruche nicht mehr möglich.</span><span class="sxs-lookup"><span data-stu-id="87ad8-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="87ad8-156">Aktuelle Partneraufgaben, die abgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="87ad8-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="87ad8-157">Der Administrator-Agent des aktuellen Partners des Kunden erhält eine E-Mail, dass der Kunde eine Übertragung seiner Abonnements an fordert:</span><span class="sxs-lookup"><span data-stu-id="87ad8-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Überprüfung":::

<span data-ttu-id="87ad8-159">Überprüfen und akzeptieren Sie das Formular für die Übertragungsanforderung Partner Center, um die Abonnementübertragung abschließen zu können.</span><span class="sxs-lookup"><span data-stu-id="87ad8-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="87ad8-160">Wenn der aktuelle Partner innerhalb von 30 Tagen keine Aktion ergriffen hat, läuft die Anforderung ab, und der zukünftige Partner hat eine , um eine neue Übertragungsanforderung zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="87ad8-161">Wählen Sie **in der E-Mail die Option** Übertragungsanforderung überprüfen oder aus.</span><span class="sxs-lookup"><span data-stu-id="87ad8-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="87ad8-162">Wählen Sie Partner Center Menü Kunden aus, und wählen Sie dann den Kunden aus, für den eine Übertragungsanforderung übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="87ad8-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="87ad8-163">Wählen Sie im Menü Kunde die Option **Abonnements aus.**</span><span class="sxs-lookup"><span data-stu-id="87ad8-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="87ad8-164">Wählen Sie den **Abschnitt Übertragungsanforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="87ad8-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="87ad8-165">Erweitern Sie Übertragungsinformationen, indem Sie unter Empfangene Anforderungen die ausgewählte **Übertragungsanforderungs-ID** **auswählen.**</span><span class="sxs-lookup"><span data-stu-id="87ad8-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Übertragungsanforderung für Quellüberprüfungen":::

5.  <span data-ttu-id="87ad8-167">Überprüfen Sie die Übertragungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="87ad8-167">Review transfer request.</span></span> <span data-ttu-id="87ad8-168">Wählen Sie die angeforderten Azure-Abonnements aus, die übertragen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="87ad8-169">Bevor Sie fortfahren, beachten Sie Folgendes: Sie haben keinen Zugriff mehr auf die ausgewählten Abonnements.</span><span class="sxs-lookup"><span data-stu-id="87ad8-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="87ad8-170">Die weitere Nutzung wird Ihnen nicht in Rechnung stellen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="87ad8-171">Azure-Reservierungen werden nicht mit den Abonnements übertragen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="87ad8-172">Wählen Sie dann **Akzeptieren und übertragen** aus, um den Übertragungsvorgang abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Auswählen von Abonnements, die unter Ihren Azure-Plänen übertragen werden sollen":::

7.  <span data-ttu-id="87ad8-174">Anzeigen der Bestätigung der Übertragungsakzeptanz.</span><span class="sxs-lookup"><span data-stu-id="87ad8-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="87ad8-175">An diesem Punkt werden der zukünftige Partner, der Kunde und der aktuelle Partner per E-Mail über die akzeptierte Übertragungsanforderung benachrichtigt.</span><span class="sxs-lookup"><span data-stu-id="87ad8-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="87ad8-176">Nachdem der Übergang akzeptiert wurde, kann der Übertragungsstatus bis zu 15 Minuten lang ausstehend bleiben, während das System aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="87ad8-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="87ad8-177">Wenn es länger dauert, versucht das System drei Tage lang weiter.</span><span class="sxs-lookup"><span data-stu-id="87ad8-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="87ad8-178">Wenn der Übertragungsstatus weiterhin Ausstehend bleibt, sollte der Partner eine Serviceanfrage senden.</span><span class="sxs-lookup"><span data-stu-id="87ad8-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="87ad8-179">Sobald die Übertragung abgeschlossen ist, werden die in der Anforderung enthaltenen Abonnements im Azure-Plan des zukünftigen Partners angezeigt und nicht mehr bei Ihnen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="87ad8-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="87ad8-180">Für indirekte Anbieter: Informieren Sie Ihren indirekten Handelspartner, dass die Übertragungsanforderung akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="87ad8-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="87ad8-181">Verwalten Ihrer übertragenen Kundenabonnements</span><span class="sxs-lookup"><span data-stu-id="87ad8-181">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="87ad8-182">Der Zugriff auf vorhandene Benutzer, Gruppen oder Dienstprinzipale, die per rollenbasierter Azure-Zugriffssteuerung (Azure Role-Based Access Control, Azure RBAC) zugewiesen wurden, ist von der Übertragung nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="87ad8-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="87ad8-183">Die rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, [Azure RBAC)](/azure/role-based-access-control/overview) unterstützt Ihren Kunden bei der Verwaltung, wer Zugriff auf Azure-Ressourcen hat, was er mit diesen Ressourcen tun kann und auf welche Bereiche er Zugriff hat.</span><span class="sxs-lookup"><span data-stu-id="87ad8-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="87ad8-184">Als neuer Partner erhalten Sie nach der Abonnementübertragung keinen RBAC-Zugriff auf die Ressourcen Ihres Kunden.</span><span class="sxs-lookup"><span data-stu-id="87ad8-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="87ad8-185">Der vorherige Partner Ihres Kunden behält seinen RBAC-Zugriff.</span><span class="sxs-lookup"><span data-stu-id="87ad8-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="87ad8-186">Arbeiten Sie mit Ihrem Kunden zusammen, um zu verstehen, wer Einblicke in seine Abonnements hat und wie sie gewünschte Änderungen vornehmen können.</span><span class="sxs-lookup"><span data-stu-id="87ad8-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="87ad8-187">Daher ist es wichtig, dass Ihr Kunde den Azure RBAC-Zugriff für seinen vorherigen Partner entfernt und dem neuen Partner Zugriff hinzufüge.</span><span class="sxs-lookup"><span data-stu-id="87ad8-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="87ad8-188">Weitere Informationen dazu, wie Ihr Kunde neuen Zugriff bietet, finden Sie unter Was [ist die rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="87ad8-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="87ad8-189">Weitere Informationen dazu, wie Ihr Kunde den RBAC-Zugriff Ihres vorherigen Partners entfernt, finden Sie unter [Entfernen einer Rollenzuweisung.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="87ad8-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="87ad8-190">Darüber hinaus erhalten Sie nicht automatisch [AOBO-Zugriff (Admin on Behalf Of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) auf Ihre Abonnements.</span><span class="sxs-lookup"><span data-stu-id="87ad8-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="87ad8-191">AOBO ist erforderlich, damit Partner die Azure-Abonnements ihrer Kunden in ihrem Namen verwalten können.</span><span class="sxs-lookup"><span data-stu-id="87ad8-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="87ad8-192">Weitere Informationen zu Azure-Berechtigungen finden Sie unter Abrufen von Berechtigungen zum Verwalten des Diensts [oder Abonnements eines Kunden.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="87ad8-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="87ad8-193">Nächste Schritte:</span><span class="sxs-lookup"><span data-stu-id="87ad8-193">Next steps:</span></span>

- [<span data-ttu-id="87ad8-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="87ad8-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="87ad8-195">Erhalten Sie Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden.</span><span class="sxs-lookup"><span data-stu-id="87ad8-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
