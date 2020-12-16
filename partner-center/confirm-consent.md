---
title: Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung
description: Erfahre, wie du bestätigst, dass ein Kunde der Microsoft-Kundenvereinbarung zugestimmt hat. Dies kann erforderlich sein, um Microsoft-Produkte und -Dienste für Kunden zu bestellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354609"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="633d7-104">Aktualisierte Methode zur Bestätigung der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="633d7-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="633d7-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="633d7-105">**Appropriate roles**</span></span>

- <span data-ttu-id="633d7-106">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="633d7-106">Admin agent</span></span>
- <span data-ttu-id="633d7-107">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="633d7-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="633d7-108">Die Vertragsressource wird zurzeit von Partner Center nur in der Microsoft Public Cloud unterstützt.</span><span class="sxs-lookup"><span data-stu-id="633d7-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="633d7-109">Gilt nicht für:</span><span class="sxs-lookup"><span data-stu-id="633d7-109">It is not applicable to:</span></span>
> * <span data-ttu-id="633d7-110">Partner Center-Betreiber ist 21Vianet</span><span class="sxs-lookup"><span data-stu-id="633d7-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="633d7-111">Partner Center für Microsoft-Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="633d7-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="633d7-112">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="633d7-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="633d7-113">Ab dem 31. Januar 2020 müssen alle Kunden (vorhandene Kunden und Neukunden) die neue Microsoft-Kundenvereinbarung signieren.</span><span class="sxs-lookup"><span data-stu-id="633d7-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="633d7-114">Weitere Informationen finden Sie unter [Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="633d7-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="633d7-115">Als Partner müssen Sie die Zustimmung Ihres Kunden zur Microsoft-Kundenvereinbarung einholen, bevor Sie Microsoft-Produkte und -Dienste für diesen Kunden bestellen können.</span><span class="sxs-lookup"><span data-stu-id="633d7-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="633d7-116">Um Partner bei der Einhaltung von Complianceanforderungen zu unterstützen, bittet Microsoft die Partner, die Zustimmung durch Bereitstellung der folgenden Details zu der Person, die dem Vertrag zugestimmt hat, zu bestätigen:</span><span class="sxs-lookup"><span data-stu-id="633d7-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="633d7-117">Vorname</span><span class="sxs-lookup"><span data-stu-id="633d7-117">First name</span></span>

- <span data-ttu-id="633d7-118">Nachname</span><span class="sxs-lookup"><span data-stu-id="633d7-118">Last name</span></span>

- <span data-ttu-id="633d7-119">E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="633d7-119">Email address</span></span>

- <span data-ttu-id="633d7-120">Telefonnummer (optional)</span><span class="sxs-lookup"><span data-stu-id="633d7-120">Phone number (optional)</span></span>

- <span data-ttu-id="633d7-121">Datum der Zustimmung</span><span class="sxs-lookup"><span data-stu-id="633d7-121">Date of acceptance</span></span>

<span data-ttu-id="633d7-122">Direct-Bill-Partner und indirekte Anbieter müssen die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung bestätigen, wenn sie über Partner Center oder die Partner Center-API Transaktionen ausführen.</span><span class="sxs-lookup"><span data-stu-id="633d7-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="633d7-123">Die Bestätigung ist *obligatorisch*.</span><span class="sxs-lookup"><span data-stu-id="633d7-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="633d7-124">Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:</span><span class="sxs-lookup"><span data-stu-id="633d7-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="633d7-125">Können Sie für diesen Kunden keine neuen Aufträge erstellen.</span><span class="sxs-lookup"><span data-stu-id="633d7-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="633d7-126">Können Sie die Anzahl der Lizenzen vorhandener lizenzbasierter Abonnements für diesen Kunden nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="633d7-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="633d7-127">Die Bestätigung der Zustimmung des Kunden kann über das Partner Center oder die Partner Center-API erfolgen.</span><span class="sxs-lookup"><span data-stu-id="633d7-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="633d7-128">Um dies über die Partner Center-API zu erledigen, lesen Sie die folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="633d7-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="633d7-129">Abrufen der Bestätigung der Zustimmung des Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="633d7-130">Abrufen von Vertragsmetadaten</span><span class="sxs-lookup"><span data-stu-id="633d7-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="633d7-131">Bestätigen der Zustimmung des Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="633d7-132">Dies gilt für Produktions- und Sandboxumgebungen.</span><span class="sxs-lookup"><span data-stu-id="633d7-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="633d7-133">Bestätigen der Kundenzustimmung für einen neuen Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="633d7-134">Verwenden Sie das folgende Verfahren, um die Zustimmung des Kunden zu bestätigen, während Sie einen neuen Kundenmandanten im Partner Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="633d7-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="633d7-135">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="633d7-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="633d7-136">Wählen Sie **Kunden** und dann **Neuer Kunde** aus, und klicken Sie anschließend auf **Kontoinformationen**.</span><span class="sxs-lookup"><span data-stu-id="633d7-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="633d7-137">Geben Sie die Informationen zum **Unternehmen** und zum **Primären Kontakt** ein.</span><span class="sxs-lookup"><span data-stu-id="633d7-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Unternehmensinformationen":::

3. <span data-ttu-id="633d7-139">Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Der Kunde hat die neueste Microsoft-Kundenvereinbarung akzeptiert** aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="633d7-140">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="633d7-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="633d7-141">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="633d7-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="633d7-142">Geben Sie die Details des Benutzers ein, der die Zustimmung bereitgestellt hat.</span><span class="sxs-lookup"><span data-stu-id="633d7-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Hinzufügen eines Annahmedatums":::

   <span data-ttu-id="633d7-144">Standardmäßig werden die Informationen des primären Kontakts angezeigt.</span><span class="sxs-lookup"><span data-stu-id="633d7-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="633d7-145">Wenn diese nicht richtig sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname**, **Nachname**, **E-Mail-Adresse** und \**Telefonnummer* (optional) der Person ein, die der Vereinbarung zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="633d7-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="633d7-146">Wählen Sie **Weiter** aus, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.</span><span class="sxs-lookup"><span data-stu-id="633d7-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="633d7-147">Bestätigen der Kundenzustimmung für einen vorhandenen Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="633d7-148">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="633d7-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="633d7-149">Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="633d7-150">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-150">Select **Account info**.</span></span>

3. <span data-ttu-id="633d7-151">Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Aktualisieren":::

4. <span data-ttu-id="633d7-153">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="633d7-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="633d7-154">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="633d7-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="633d7-155">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="633d7-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="633d7-156">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="633d7-157">Bestätigen der Kundenzustimmung beim Erstellen eines neuen Auftrags für einen vorhandenen Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="633d7-158">Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="633d7-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="633d7-159">Führen Sie dazu die nachfolgend aufgeführten Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="633d7-160">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="633d7-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="633d7-161">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="633d7-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="633d7-162">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="633d7-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="633d7-163">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="633d7-164">Abrufen der Bestätigung der Kundenzustimmung für einen vorhandenen Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="633d7-165">Sie können die Bestätigung der Zustimmung für einen vorhandenen Kunden abrufen, den Sie zuvor mit dem nachstehenden Verfahren angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="633d7-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="633d7-166">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="633d7-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="633d7-167">Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="633d7-168">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="633d7-168">Select **Account info**.</span></span>

3. <span data-ttu-id="633d7-169">Unter **Microsoft-Kundenvereinbarung** sehen Sie, ob für diesen Kunden eine Bestätigung bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="633d7-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="633d7-170">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="633d7-170">Next steps</span></span>

- [<span data-ttu-id="633d7-171">Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung im CSP-Partnerprogramm</span><span class="sxs-lookup"><span data-stu-id="633d7-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="633d7-172">Bestätigen der Zustimmung zur Microsoft-Kundenvereinbarung im Namen Ihres Kunden</span><span class="sxs-lookup"><span data-stu-id="633d7-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)