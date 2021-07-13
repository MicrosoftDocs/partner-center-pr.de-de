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
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277010"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="8d01d-103">Bestätigen, dass Ihr Kunde die Microsoft-Kundenvereinbarung für das CSP-Programm akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="8d01d-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="8d01d-104">**Geeignete Rollen:** Administrator-Agent | Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="8d01d-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="8d01d-105">Kunden haben zwei Möglichkeiten, die Microsoft-Kundenvereinbarung zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="8d01d-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="8d01d-106">**Option 1**: Der Partner bestätigt die Zustimmung des Kunden – Der Partner kann die Zustimmung des Kunden über die Partner Center-API, das Partner Center SDK oder das Partner Center-Dashboard bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="8d01d-107">**Option 2**: Der Kunde stimmt direkt zu: Der Partner kann den Kunden über eine URL einladen, damit dieser die Vereinbarung in Microsoft 365 Admin Center überprüfen und ihr zustimmen kann.</span><span class="sxs-lookup"><span data-stu-id="8d01d-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="8d01d-108">Zugreifen auf die Vorlage für die Microsoft-Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="8d01d-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="8d01d-109">[Hier](https://aka.ms/customeragreement) kannst du die neueste Version der Vorlage für die Microsoft-Kundenvereinbarung manuell herunterladen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="8d01d-110">Die Microsoft-Kundenvereinbarung ist länderspezifisch.</span><span class="sxs-lookup"><span data-stu-id="8d01d-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="8d01d-111">Achte beim Anfordern der Vorlage für die Microsoft-Kundenvereinbarung darauf, basierend auf dem Standort des Kunden das richtige Land/die richtige Region auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="8d01d-112">Option 1: Bestätigen der Zustimmung des Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="8d01d-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="8d01d-113">Partner mit direkter Abrechnung können die Zustimmung bestehender und neuer Kunden zur Microsoft-Kundenvereinbarung in Partner Center bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="8d01d-114">Indirekte Wiederverkäufer können keine Bestätigung im Namen ihrer Kunden abgeben und müssen mit ihrem indirekten Anbieter zusammenarbeiten, um den Vorgang abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="8d01d-115">Bestätigen der Kundenzustimmung für Neukunden</span><span class="sxs-lookup"><span data-stu-id="8d01d-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="8d01d-116">Wenn Sie in Partner Center einen Mandanten für einen Neukunden erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert hat.</span><span class="sxs-lookup"><span data-stu-id="8d01d-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8d01d-117">Um diese Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein.</span><span class="sxs-lookup"><span data-stu-id="8d01d-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="8d01d-118">Wählen Sie **Kunden** und dann **Neuer Kunde** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="8d01d-119">Machen Sie unter **Kontoinformationen** Angaben zum Unternehmen und seinem primären Kontakt.</span><span class="sxs-lookup"><span data-stu-id="8d01d-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="8d01d-120">Aktiviere unter der Option für die **Microsoft-Vereinbarung** das entsprechende Kontrollkästchen, um zu bestätigen, dass der Kunde der Microsoft-Kundenvereinbarung zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="8d01d-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="8d01d-121">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="8d01d-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="8d01d-122">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8d01d-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="8d01d-123">Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind.</span><span class="sxs-lookup"><span data-stu-id="8d01d-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="8d01d-124">Sind sie nicht korrekt, wähle **Aktualisieren** aus, und gib die richtigen Informationen für die Person ein, die die Vereinbarung akzeptiert hat.</span><span class="sxs-lookup"><span data-stu-id="8d01d-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="8d01d-125">Wähle **Weiter** aus, um die Erstellung des Kundenmandanten fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Neukunde.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="8d01d-127">Bestätigen der Kundenzustimmung für einen Bestandskunden</span><span class="sxs-lookup"><span data-stu-id="8d01d-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="8d01d-128">Um die folgenden Schritte ausführen zu können, musst du Administrator-Agent oder Vertriebsbeauftragter sein:</span><span class="sxs-lookup"><span data-stu-id="8d01d-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="8d01d-129">Wählen Sie **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-129">Select **Customers**.</span></span> <span data-ttu-id="8d01d-130">Suchen und wählen Sie den Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-130">Find and select the customer.</span></span>

2. <span data-ttu-id="8d01d-131">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-131">Select **Account info**.</span></span>

3. <span data-ttu-id="8d01d-132">Wählen Sie unter **Microsoft-Kundenvertrag** die Option **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="8d01d-133">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="8d01d-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="8d01d-134">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="8d01d-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="8d01d-135">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8d01d-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="8d01d-136">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestandskunde.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="8d01d-138">Abrufen der Bestätigung der Kundenzustimmung für einen Bestandskunden</span><span class="sxs-lookup"><span data-stu-id="8d01d-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="8d01d-139">Mithilfe der folgenden Schritte können Sie eine Bestätigung abrufen, dass ein Bestandskunde die Microsoft-Kundenvereinbarung akzeptiert hat.</span><span class="sxs-lookup"><span data-stu-id="8d01d-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="8d01d-140">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="8d01d-141">Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="8d01d-142">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-142">Select **Account info**.</span></span>

3. <span data-ttu-id="8d01d-143">Unter **Microsoft-Kundenvertrag** wird angezeigt, ob die Bestätigung durch diesen Kunden erfolgt ist.</span><span class="sxs-lookup"><span data-stu-id="8d01d-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="8d01d-144">Bestätigen der Zustimmung des Kunden über die Partner Center-API oder das Partner Center SDK</span><span class="sxs-lookup"><span data-stu-id="8d01d-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="8d01d-145">Du kannst die Partner Center-API oder das Partner Center SDK verwenden, um die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8d01d-146">Ausführliche Informationen zur API bzw. zum SDK findest du unter:</span><span class="sxs-lookup"><span data-stu-id="8d01d-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="8d01d-147">Abrufen von Vertragsmetadaten für den Microsoft-Kundenvertrag</span><span class="sxs-lookup"><span data-stu-id="8d01d-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="8d01d-148">Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag</span><span class="sxs-lookup"><span data-stu-id="8d01d-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="8d01d-149">Abrufen der Bestätigung der Kundenakzeptanz zur Microsoft-Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="8d01d-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="8d01d-150">Abrufen eines Downloadlinks für die Vorlage des Microsoft-Kundenvertrags</span><span class="sxs-lookup"><span data-stu-id="8d01d-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="8d01d-151">Option 2: Zustimmung des Kunden im Microsoft 365 Admin Center</span><span class="sxs-lookup"><span data-stu-id="8d01d-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="8d01d-152">Partner können neue und bestehende Kunden über eine URL einladen, die Vereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="8d01d-153">In den nächsten Abschnitten wird Folgendes erläutert:</span><span class="sxs-lookup"><span data-stu-id="8d01d-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="8d01d-154">Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="8d01d-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="8d01d-155">Einladen eines neuen Kunden, die Handelspartnerbeziehung und -vereinbarung zu überprüfen und diesen zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="8d01d-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="8d01d-156">Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="8d01d-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="8d01d-157">Sie können die [Partner Center-API oder das Partner Center SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) verwenden, um den Status der direkten Zustimmung eines Kunden zur Microsoft-Kundenvereinbarung zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="8d01d-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="8d01d-158">Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="8d01d-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="8d01d-159">Mit den folgenden Schritten kannst du einen neuen Kunden im Partner Center erstellen und dann einladen, die Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="8d01d-160">Wähle im Partner Center auf der Registerkarte **Kunden** die Option **Kunden hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="8d01d-161">Gib unter **Kontoinformationen** in allen Pflichtfeldern die Informationen zum neuen Kunden ein, darunter auch der Firmenname und Hauptkontakt des Kunden.</span><span class="sxs-lookup"><span data-stu-id="8d01d-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="8d01d-162">Wählen Sie unter **Kundenvereinbarung** die Option **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Der Kunde wird aufgefordert, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen) aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="8d01d-163">Fülle alle weiteren Pflichtfelder auf der Seite aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="8d01d-164">Wählen Sie **Weiter: Überprüfung** aus und führen Sie dann die Schritte zum Erstellen des Kundenmandanten aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="8d01d-165">Neue Kunden können erst einen Kauf tätigen, nachdem sie der Microsoft-Kundenvereinbarung zugestimmt haben.</span><span class="sxs-lookup"><span data-stu-id="8d01d-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Erstellen eines neuen Kunden.":::

5. <span data-ttu-id="8d01d-167">Sobald im Workflow für neue Kunden der Bildschirm **Bestätigung** angezeigt wird, musst du die Anmeldeinformationen des Kunden speichern.</span><span class="sxs-lookup"><span data-stu-id="8d01d-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="8d01d-168">Diese Anmeldeinformationen musst du später dem Kunden mitteilen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="8d01d-169">Erstelle und sende außerhalb von Partner Center eine E-Mail, um den Kunden einzuladen, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="8d01d-170">Die folgenden Elemente müssen in der E-Mail enthalten sein:</span><span class="sxs-lookup"><span data-stu-id="8d01d-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="8d01d-171">Ein Link zu dieser [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Anmeldung erforderlich)</span><span class="sxs-lookup"><span data-stu-id="8d01d-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="8d01d-172">Die in Schritt 5 gespeicherten Anmeldeinformationen des Kunden.</span><span class="sxs-lookup"><span data-stu-id="8d01d-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="8d01d-173">Der Kunde erhält dann die E-Mail-Einladung vom Partner und wählt die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="8d01d-174">Der Kunde meldet sich mit den von Ihnen erhaltenen Kundenanmeldeinformationen beim Microsoft 365 Admin Center an.</span><span class="sxs-lookup"><span data-stu-id="8d01d-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="8d01d-175">Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="8d01d-176">Einladen eines neuen Kunden, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="8d01d-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="8d01d-177">Mit den folgenden Schritten kannst du einen neuen Kunden einladen, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="8d01d-178">Wähle im Partner Center auf der Registerkarte **Kunden** den Link **Vertriebspartnerschaft beantragen** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="8d01d-179">Dadurch wird eine automatische E-Mail-Vorlage generiert, die Text und eine parametrisierte URL enthält, durch die der Kunde zum Microsoft 365 Admin Center weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="8d01d-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="8d01d-180">Du kannst die automatisch generierte E-Mail-Vorlage anpassen und dann **In Zwischenablage kopieren** oder **In E-Mail öffnen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="8d01d-181">Verwende diese E-Mail-Vorlage, um den Kunden einzuladen, dem Antrag auf eine **Handelspartnerschaft** und der **Microsoft-Kundenvereinbarung** zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="8d01d-182">(Anmerkung: Achte darauf, dass der Partner in der E-Mail-Einladung auch die automatisch bereitgestellte URL und die kürzlich erstellten Kundenanmeldeinformationen angibt.)</span><span class="sxs-lookup"><span data-stu-id="8d01d-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Erstellen einer Beziehung.":::

5. <span data-ttu-id="8d01d-184">Der Kunde empfängt die Einladung per E-Mail und klickt auf die parametrisierte URL.</span><span class="sxs-lookup"><span data-stu-id="8d01d-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="8d01d-185">Der Kunde verwendet die von Ihnen in der E-Mail bereitgestellten Anmeldeinformationen, um sich beim Microsoft 365 Admin Center anzumelden.</span><span class="sxs-lookup"><span data-stu-id="8d01d-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="8d01d-186">Der Kunde aktiviert das Kontrollkästchen, um der **Handelspartnerbeziehung** und **Microsoft-Kundenvereinbarung** zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="8d01d-187">Der Kunde kann unter derselben URL eine konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet.</span><span class="sxs-lookup"><span data-stu-id="8d01d-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="8d01d-188">Er kann einen Partner auswählen, um Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Annehmen einer Vereinbarung.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="8d01d-190">Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen</span><span class="sxs-lookup"><span data-stu-id="8d01d-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="8d01d-191">Mit den folgenden Schritten kannst du einen bestehenden Kunden einladen, die Microsoft-Kundenvereinbarung zu überprüfen und ihr zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="8d01d-192">Erstelle die Kunden-E-Mail mit der eingebetteten URL, um deinen Kunden einzuladen, der Microsoft-Kundenvereinbarung zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="8d01d-193">Der Kunde erhält die Einladung per E-Mail und klickt auf die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="8d01d-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="8d01d-194">Der Kunde gibt seine Anmeldeinformationen in Microsoft 365 Admin Center ein.</span><span class="sxs-lookup"><span data-stu-id="8d01d-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="8d01d-195">Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="8d01d-196">Der Kunde kann unter derselben URL die konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet.</span><span class="sxs-lookup"><span data-stu-id="8d01d-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="8d01d-197">Er kann einen Partner auswählen, um Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Kunde.":::

>[!NOTE]
><span data-ttu-id="8d01d-199">In bestimmten Szenarien können Kunden der Microsoft-Kundenvereinbarung u. U. nicht direkt zustimmen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8d01d-200">Weitere Informationen zu diesen Situationen finden Sie unter „Zwei Szenarien, in denen Sie die Zustimmung im Namen Ihres Kunden bestätigen müssen“.</span><span class="sxs-lookup"><span data-stu-id="8d01d-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="8d01d-201">Zwei Szenarien, in denen du die Zustimmung im Namen deines Kunden bestätigen musst</span><span class="sxs-lookup"><span data-stu-id="8d01d-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="8d01d-202">Es gibt zwei Szenarien, in denen Kunden der Microsoft-Kundenvereinbarung möglicherweise nicht direkt im Microsoft 365 Admin Center zustimmen können.</span><span class="sxs-lookup"><span data-stu-id="8d01d-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="8d01d-203">**Szenario 1:** Ein Bestandskunde hat über eine bestehende Partnerbeziehung eines der folgenden Produkte erworben: Angebote, Software oder Softwareabonnements, reservierte Instanzen oder einen Azure-Plan.</span><span class="sxs-lookup"><span data-stu-id="8d01d-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="8d01d-204">Der Kunde versucht nun, einen neuen Kauf zu tätigen (außer einer automatischen Verlängerung).</span><span class="sxs-lookup"><span data-stu-id="8d01d-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="8d01d-205">Wenn dieser Kunde auf die URL klickt, erhält er die Mitteilung, dass er sich an seinen Partner wenden soll, um die Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="8d01d-206">**Lösung**: Du musst die Zustimmung im Namen des Kunden bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot: Seite im Microsoft 365 Admin Center mit der Bitte, sich an Ihren Partner zu wenden, um Ihre Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen":::

<span data-ttu-id="8d01d-208">**Szenario 2**: Ein bestehender Kunde hat eines der folgenden Produkte erworben: Angebote, Software und Softwareabonnements, reservierte Instanzen und einen Azure-Plan.</span><span class="sxs-lookup"><span data-stu-id="8d01d-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="8d01d-209">Der Kunde versucht nun, einen neuen Kauf bei einem neuen Partner zu tätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="8d01d-210">Wenn der Kunde auf die URL für das Microsoft 365 Admin Center klickt, um der neuen Partnerbeziehung und Vereinbarung zuzustimmen, erhält er die Mitteilung, dass er sich an seinen Partner wenden soll, um die Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="8d01d-211">**Lösung**: Du musst die Zustimmung im Namen des Kunden bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="8d01d-212">Bestätigen, dass ein Kunde der Vereinbarung zugestimmt hat</span><span class="sxs-lookup"><span data-stu-id="8d01d-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="8d01d-213">Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="8d01d-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="8d01d-214">Führen Sie dazu die nachfolgend aufgeführten Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="8d01d-215">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="8d01d-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="8d01d-216">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="8d01d-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="8d01d-217">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8d01d-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="8d01d-218">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="8d01d-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="8d01d-219">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="8d01d-219">Next steps</span></span>

- [<span data-ttu-id="8d01d-220">Überprüfen oder Aktualisieren Ihrer Unternehmensprofilinformationen</span><span class="sxs-lookup"><span data-stu-id="8d01d-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="8d01d-221">Microsoft-Kundenvereinbarungen (nach Region, Sprache)</span><span class="sxs-lookup"><span data-stu-id="8d01d-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
