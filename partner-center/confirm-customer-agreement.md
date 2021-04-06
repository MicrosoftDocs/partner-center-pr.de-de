---
title: Bestätigen, dass Ihr Kunde die Microsoft-Kundenvereinbarung für das CSP-Programm akzeptiert hat
description: CSP-Partner (Cloud Solution Provider) müssen vor dem Bestellen von Microsoft-Diensten für Kunden die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung bestätigen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633777"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="12dc5-103">Bestätigen, dass Ihr Kunde die Microsoft-Kundenvereinbarung für das CSP-Programm akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="12dc5-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="12dc5-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="12dc5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="12dc5-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="12dc5-105">Admin agent</span></span>
- <span data-ttu-id="12dc5-106">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="12dc5-106">Sales agent</span></span>


<span data-ttu-id="12dc5-107">Kunden haben zwei Möglichkeiten, die Microsoft-Kundenvereinbarung zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="12dc5-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="12dc5-108">**Option 1**: Der Partner bestätigt die Zustimmung des Kunden – Der Partner kann die Zustimmung des Kunden über die Partner Center-API, das Partner Center SDK oder das Partner Center-Dashboard bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="12dc5-109">**Option 2**: Der Kunde stimmt direkt zu: Der Partner kann den Kunden über eine URL einladen, damit dieser die Vereinbarung in Microsoft 365 Admin Center überprüfen und ihr zustimmen kann.</span><span class="sxs-lookup"><span data-stu-id="12dc5-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="12dc5-110">Zugreifen auf die Vorlage für die Microsoft-Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="12dc5-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="12dc5-111">[Hier](https://aka.ms/customeragreement) kannst du die neueste Version der Vorlage für die Microsoft-Kundenvereinbarung manuell herunterladen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="12dc5-112">Die Microsoft-Kundenvereinbarung ist länderspezifisch.</span><span class="sxs-lookup"><span data-stu-id="12dc5-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="12dc5-113">Achte beim Anfordern der Vorlage für die Microsoft-Kundenvereinbarung darauf, basierend auf dem Standort des Kunden das richtige Land/die richtige Region auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="12dc5-114">Option 1: Bestätigen der Zustimmung des Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="12dc5-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="12dc5-115">Partner mit direkter Abrechnung können die Zustimmung bestehender und neuer Kunden zur Microsoft-Kundenvereinbarung in Partner Center bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="12dc5-116">Indirekte Wiederverkäufer können keine Bestätigung im Namen ihrer Kunden abgeben und müssen mit ihrem indirekten Anbieter zusammenarbeiten, um den Vorgang abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="12dc5-117">Bestätigen der Kundenzustimmung für Neukunden</span><span class="sxs-lookup"><span data-stu-id="12dc5-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="12dc5-118">Wenn Sie in Partner Center einen Mandanten für einen Neukunden erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert hat.</span><span class="sxs-lookup"><span data-stu-id="12dc5-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="12dc5-119">Um diese Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein.</span><span class="sxs-lookup"><span data-stu-id="12dc5-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="12dc5-120">Wählen Sie **Kunden** und dann **Neuer Kunde** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="12dc5-121">Machen Sie unter **Kontoinformationen** Angaben zum Unternehmen und seinem primären Kontakt.</span><span class="sxs-lookup"><span data-stu-id="12dc5-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="12dc5-122">Aktiviere unter der Option für die **Microsoft-Vereinbarung** das entsprechende Kontrollkästchen, um zu bestätigen, dass der Kunde der Microsoft-Kundenvereinbarung zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="12dc5-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="12dc5-123">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="12dc5-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="12dc5-124">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="12dc5-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="12dc5-125">Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind.</span><span class="sxs-lookup"><span data-stu-id="12dc5-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="12dc5-126">Sind sie nicht korrekt, wähle **Aktualisieren** aus, und gib die richtigen Informationen für die Person ein, die die Vereinbarung akzeptiert hat.</span><span class="sxs-lookup"><span data-stu-id="12dc5-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="12dc5-127">Wähle **Weiter** aus, um die Erstellung des Kundenmandanten fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Neukunde":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="12dc5-129">Bestätigen der Kundenzustimmung für einen Bestandskunden</span><span class="sxs-lookup"><span data-stu-id="12dc5-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="12dc5-130">Um die folgenden Schritte ausführen zu können, musst du Administrator-Agent oder Vertriebsbeauftragter sein:</span><span class="sxs-lookup"><span data-stu-id="12dc5-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="12dc5-131">Wählen Sie **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-131">Select **Customers**.</span></span> <span data-ttu-id="12dc5-132">Suchen und wählen Sie den Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-132">Find and select the customer.</span></span>

2. <span data-ttu-id="12dc5-133">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-133">Select **Account info**.</span></span>

3. <span data-ttu-id="12dc5-134">Wählen Sie unter **Microsoft-Kundenvertrag** die Option **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="12dc5-135">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="12dc5-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="12dc5-136">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="12dc5-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="12dc5-137">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="12dc5-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="12dc5-138">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestandskunde":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="12dc5-140">Abrufen der Bestätigung der Kundenzustimmung für einen Bestandskunden</span><span class="sxs-lookup"><span data-stu-id="12dc5-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="12dc5-141">Mithilfe der folgenden Schritte können Sie eine Bestätigung abrufen, dass ein Bestandskunde die Microsoft-Kundenvereinbarung akzeptiert hat.</span><span class="sxs-lookup"><span data-stu-id="12dc5-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="12dc5-142">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="12dc5-143">Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="12dc5-144">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-144">Select **Account info**.</span></span>

3. <span data-ttu-id="12dc5-145">Unter **Microsoft-Kundenvertrag** wird angezeigt, ob die Bestätigung durch diesen Kunden erfolgt ist.</span><span class="sxs-lookup"><span data-stu-id="12dc5-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="12dc5-146">Bestätigen der Zustimmung des Kunden über die Partner Center-API oder das Partner Center SDK</span><span class="sxs-lookup"><span data-stu-id="12dc5-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="12dc5-147">Du kannst die Partner Center-API oder das Partner Center SDK verwenden, um die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="12dc5-148">Ausführliche Informationen zur API bzw. zum SDK findest du unter:</span><span class="sxs-lookup"><span data-stu-id="12dc5-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="12dc5-149">Abrufen von Vertragsmetadaten für den Microsoft-Kundenvertrag</span><span class="sxs-lookup"><span data-stu-id="12dc5-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="12dc5-150">Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag</span><span class="sxs-lookup"><span data-stu-id="12dc5-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="12dc5-151">Abrufen der Bestätigung der Kundenakzeptanz zur Microsoft-Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="12dc5-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="12dc5-152">Abrufen eines Downloadlinks für die Vorlage des Microsoft-Kundenvertrags</span><span class="sxs-lookup"><span data-stu-id="12dc5-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="12dc5-153">Option 2: Zustimmung des Kunden im Microsoft 365 Admin Center</span><span class="sxs-lookup"><span data-stu-id="12dc5-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="12dc5-154">Partner können neue und bestehende Kunden über eine URL einladen, die Vereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="12dc5-155">In den nächsten Abschnitten wird Folgendes erläutert:</span><span class="sxs-lookup"><span data-stu-id="12dc5-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="12dc5-156">Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="12dc5-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="12dc5-157">Einladen eines neuen Kunden, die Handelspartnerbeziehung und -vereinbarung zu überprüfen und diesen zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="12dc5-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="12dc5-158">Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="12dc5-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="12dc5-159">Sie können die [Partner Center-API oder das Partner Center SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) verwenden, um den Status der direkten Zustimmung eines Kunden zur Microsoft-Kundenvereinbarung zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="12dc5-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="12dc5-160">Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="12dc5-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="12dc5-161">Mit den folgenden Schritten kannst du einen neuen Kunden im Partner Center erstellen und dann einladen, die Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="12dc5-162">Wähle im Partner Center auf der Registerkarte **Kunden** die Option **Kunden hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="12dc5-163">Gib unter **Kontoinformationen** in allen Pflichtfeldern die Informationen zum neuen Kunden ein, darunter auch der Firmenname und Hauptkontakt des Kunden.</span><span class="sxs-lookup"><span data-stu-id="12dc5-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="12dc5-164">Wählen Sie unter **Kundenvereinbarung** die Option **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Der Kunde wird aufgefordert, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen) aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="12dc5-165">Fülle alle weiteren Pflichtfelder auf der Seite aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="12dc5-166">Wählen Sie **Weiter: Überprüfung** aus und führen Sie dann die Schritte zum Erstellen des Kundenmandanten aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="12dc5-167">Neue Kunden können erst einen Kauf tätigen, nachdem sie der Microsoft-Kundenvereinbarung zugestimmt haben.</span><span class="sxs-lookup"><span data-stu-id="12dc5-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Erstellen eines neuen Kunden":::

5. <span data-ttu-id="12dc5-169">Sobald im Workflow für neue Kunden der Bildschirm **Bestätigung** angezeigt wird, musst du die Anmeldeinformationen des Kunden speichern.</span><span class="sxs-lookup"><span data-stu-id="12dc5-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="12dc5-170">Diese Anmeldeinformationen musst du später dem Kunden mitteilen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="12dc5-171">Erstelle und sende außerhalb von Partner Center eine E-Mail, um den Kunden einzuladen, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="12dc5-172">Die folgenden Elemente müssen in der E-Mail enthalten sein:</span><span class="sxs-lookup"><span data-stu-id="12dc5-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="12dc5-173">Ein Link zu dieser [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Anmeldung erforderlich)</span><span class="sxs-lookup"><span data-stu-id="12dc5-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="12dc5-174">Die in Schritt 5 gespeicherten Anmeldeinformationen des Kunden.</span><span class="sxs-lookup"><span data-stu-id="12dc5-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="12dc5-175">Der Kunde erhält dann die E-Mail-Einladung vom Partner und wählt die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="12dc5-176">Der Kunde meldet sich mit den von Ihnen erhaltenen Kundenanmeldeinformationen beim Microsoft 365 Admin Center an.</span><span class="sxs-lookup"><span data-stu-id="12dc5-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="12dc5-177">Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="12dc5-178">Einladen eines neuen Kunden, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="12dc5-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="12dc5-179">Mit den folgenden Schritten kannst du einen neuen Kunden einladen, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="12dc5-180">Wähle im Partner Center auf der Registerkarte **Kunden** den Link **Vertriebspartnerschaft beantragen** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="12dc5-181">Dadurch wird eine automatische E-Mail-Vorlage generiert, die Text und eine parametrisierte URL enthält, durch die der Kunde zum Microsoft 365 Admin Center weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="12dc5-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="12dc5-182">Du kannst die automatisch generierte E-Mail-Vorlage anpassen und dann **In Zwischenablage kopieren** oder **In E-Mail öffnen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="12dc5-183">Verwende diese E-Mail-Vorlage, um den Kunden einzuladen, dem Antrag auf eine **Handelspartnerschaft** und der **Microsoft-Kundenvereinbarung** zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="12dc5-184">(Anmerkung: Achte darauf, dass der Partner in der E-Mail-Einladung auch die automatisch bereitgestellte URL und die kürzlich erstellten Kundenanmeldeinformationen angibt.)</span><span class="sxs-lookup"><span data-stu-id="12dc5-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Erstellen einer Beziehung":::

5. <span data-ttu-id="12dc5-186">Der Kunde empfängt die Einladung per E-Mail und klickt auf die parametrisierte URL.</span><span class="sxs-lookup"><span data-stu-id="12dc5-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="12dc5-187">Der Kunde verwendet die von Ihnen in der E-Mail bereitgestellten Anmeldeinformationen, um sich beim Microsoft 365 Admin Center anzumelden.</span><span class="sxs-lookup"><span data-stu-id="12dc5-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="12dc5-188">Der Kunde aktiviert das Kontrollkästchen, um der **Handelspartnerbeziehung** und **Microsoft-Kundenvereinbarung** zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="12dc5-189">Der Kunde kann unter derselben URL eine konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet.</span><span class="sxs-lookup"><span data-stu-id="12dc5-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="12dc5-190">Er kann einen Partner auswählen, um Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zustimmen zur Vereinbarung":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="12dc5-192">Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="12dc5-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="12dc5-193">Mit den folgenden Schritten kannst du einen bestehenden Kunden einladen, die Microsoft-Kundenvereinbarung zu überprüfen und ihr zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="12dc5-194">Erstelle die Kunden-E-Mail mit der eingebetteten URL, um deinen Kunden einzuladen, der Microsoft-Kundenvereinbarung zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="12dc5-195">Der Kunde erhält die Einladung per E-Mail und klickt auf die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="12dc5-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="12dc5-196">Der Kunde gibt seine Anmeldeinformationen in Microsoft 365 Admin Center ein.</span><span class="sxs-lookup"><span data-stu-id="12dc5-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="12dc5-197">Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="12dc5-198">Der Kunde kann unter derselben URL die konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet.</span><span class="sxs-lookup"><span data-stu-id="12dc5-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="12dc5-199">Er kann einen Partner auswählen, um Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Kunde":::

>[!NOTE]
><span data-ttu-id="12dc5-201">In bestimmten Szenarien können Kunden der Microsoft-Kundenvereinbarung u. U. nicht direkt zustimmen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="12dc5-202">Weitere Informationen zu diesen Situationen finden Sie unter „Zwei Szenarien, in denen Sie die Zustimmung im Namen Ihres Kunden bestätigen müssen“.</span><span class="sxs-lookup"><span data-stu-id="12dc5-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="12dc5-203">Zwei Szenarien, in denen du die Zustimmung im Namen deines Kunden bestätigen musst</span><span class="sxs-lookup"><span data-stu-id="12dc5-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="12dc5-204">Es gibt zwei Szenarien, in denen Kunden der Microsoft-Kundenvereinbarung möglicherweise nicht direkt im Microsoft 365 Admin Center zustimmen können.</span><span class="sxs-lookup"><span data-stu-id="12dc5-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="12dc5-205">**Szenario 1:** Ein Bestandskunde hat über eine bestehende Partnerbeziehung eines der folgenden Produkte erworben: Angebote, Software oder Softwareabonnements, reservierte Instanzen oder einen Azure-Plan.</span><span class="sxs-lookup"><span data-stu-id="12dc5-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="12dc5-206">Der Kunde versucht nun, einen neuen Kauf zu tätigen (außer einer automatischen Verlängerung).</span><span class="sxs-lookup"><span data-stu-id="12dc5-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="12dc5-207">Wenn dieser Kunde auf die URL klickt, erhält er die Mitteilung, dass er sich an seinen Partner wenden soll, um die Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="12dc5-208">**Lösung**: Du musst die Zustimmung im Namen des Kunden bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot: Seite im Microsoft 365 Admin Center mit der Bitte, sich an Ihren Partner zu wenden, um Ihre Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen":::

<span data-ttu-id="12dc5-210">**Szenario 2**: Ein bestehender Kunde hat eines der folgenden Produkte erworben: Angebote, Software und Softwareabonnements, reservierte Instanzen und einen Azure-Plan.</span><span class="sxs-lookup"><span data-stu-id="12dc5-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="12dc5-211">Der Kunde versucht nun, einen neuen Kauf bei einem neuen Partner zu tätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="12dc5-212">Wenn der Kunde auf die URL für das Microsoft 365 Admin Center klickt, um der neuen Partnerbeziehung und Vereinbarung zuzustimmen, erhält er die Mitteilung, dass er sich an seinen Partner wenden soll, um die Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="12dc5-213">**Lösung**: Du musst die Zustimmung im Namen des Kunden bestätigen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="12dc5-214">Bestätigen, dass ein Kunde der Vereinbarung zugestimmt hat</span><span class="sxs-lookup"><span data-stu-id="12dc5-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="12dc5-215">Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="12dc5-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="12dc5-216">Führen Sie dazu die nachfolgend aufgeführten Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="12dc5-217">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="12dc5-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="12dc5-218">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="12dc5-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="12dc5-219">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="12dc5-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="12dc5-220">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="12dc5-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="12dc5-221">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="12dc5-221">Next steps</span></span>

- [<span data-ttu-id="12dc5-222">Überprüfen oder Aktualisieren Ihrer Unternehmensprofilinformationen</span><span class="sxs-lookup"><span data-stu-id="12dc5-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="12dc5-223">Microsoft-Kundenvereinbarungen (nach Region, Sprache)</span><span class="sxs-lookup"><span data-stu-id="12dc5-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
