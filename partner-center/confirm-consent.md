---
title: Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag | Partner Center
ms.topic: article
ms.date: 04/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahre, wie du bestätigst, dass ein Kunde der Microsoft-Kundenvereinbarung zugestimmt hat. Dies kann erforderlich sein, um Microsoft-Produkte und -Dienste für Kunden zu bestellen.
author: LauraBrenner
ms.author: labrenne
keywords: Kunde, Kunden, Zustimmung, MCA, Microsoft-Kundenvereinbarung, Vorlagen für Kundenvereinbarungen
ms.localizationpriority: high
ms.openlocfilehash: 2223a8e05a9df4c2d6ac377fc6f6b5a06944adc9
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123325"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="3712d-105">Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="3712d-105">Confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="3712d-106">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="3712d-106">**Applies to**</span></span>
-  <span data-ttu-id="3712d-107">Partner Center</span><span class="sxs-lookup"><span data-stu-id="3712d-107">Partner Center</span></span>

<span data-ttu-id="3712d-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="3712d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="3712d-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="3712d-109">Admin agent</span></span>
- <span data-ttu-id="3712d-110">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="3712d-110">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="3712d-111">Die Vertragsressource wird zurzeit von Partner Center nur in der Microsoft Public Cloud unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3712d-111">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="3712d-112">Gilt nicht für:</span><span class="sxs-lookup"><span data-stu-id="3712d-112">It is not applicable to:</span></span>
> * <span data-ttu-id="3712d-113">Partner Center-Betreiber ist 21Vianet</span><span class="sxs-lookup"><span data-stu-id="3712d-113">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="3712d-114">Partner Center für Microsoft-Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="3712d-114">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="3712d-115">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="3712d-115">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="3712d-116">Ab dem 31. Januar 2020 müssen alle Kunden (vorhandene Kunden und Neukunden) die neue Microsoft-Kundenvereinbarung signieren.</span><span class="sxs-lookup"><span data-stu-id="3712d-116">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="3712d-117">Weitere Informationen finden Sie unter [Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="3712d-117">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="3712d-118">Als Partner müssen Sie die Zustimmung Ihres Kunden zur Microsoft-Kundenvereinbarung einholen, bevor Sie Microsoft-Produkte und -Dienste für diesen Kunden bestellen können.</span><span class="sxs-lookup"><span data-stu-id="3712d-118">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="3712d-119">Um Partner bei der Einhaltung von Complianceanforderungen zu unterstützen, bittet Microsoft die Partner, die Zustimmung durch Bereitstellung der folgenden Details zu der Person, die dem Vertrag zugestimmt hat, zu bestätigen:</span><span class="sxs-lookup"><span data-stu-id="3712d-119">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="3712d-120">Vorname</span><span class="sxs-lookup"><span data-stu-id="3712d-120">First name</span></span>

- <span data-ttu-id="3712d-121">Nachname</span><span class="sxs-lookup"><span data-stu-id="3712d-121">Last name</span></span>

- <span data-ttu-id="3712d-122">E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="3712d-122">Email address</span></span>

- <span data-ttu-id="3712d-123">Telefonnummer (optional)</span><span class="sxs-lookup"><span data-stu-id="3712d-123">Phone number (optional)</span></span>

- <span data-ttu-id="3712d-124">Datum der Zustimmung</span><span class="sxs-lookup"><span data-stu-id="3712d-124">Date of acceptance</span></span>

<span data-ttu-id="3712d-125">Direct-Bill-Partner und indirekte Anbieter müssen die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung bestätigen, wenn sie über Partner Center oder die Partner Center-API Transaktionen ausführen.</span><span class="sxs-lookup"><span data-stu-id="3712d-125">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="3712d-126">Die Bestätigung ist *obligatorisch*.</span><span class="sxs-lookup"><span data-stu-id="3712d-126">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="3712d-127">Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:</span><span class="sxs-lookup"><span data-stu-id="3712d-127">If confirmation is not provided for a given customer:</span></span>

-    <span data-ttu-id="3712d-128">Können Sie für diesen Kunden keine neuen Aufträge erstellen.</span><span class="sxs-lookup"><span data-stu-id="3712d-128">You won't be able to create new orders for this customer.</span></span>

-    <span data-ttu-id="3712d-129">Können Sie die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierter Abonnements für diesen Kunden nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="3712d-129">You won't be able to change the seat count of existing seat-based subscriptions for this customer.</span></span>

<span data-ttu-id="3712d-130">Die Bestätigung der Zustimmung des Kunden kann über das Partner Center oder die Partner Center-API erfolgen.</span><span class="sxs-lookup"><span data-stu-id="3712d-130">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="3712d-131">Um dies über die Partner Center-API zu erledigen, lesen Sie die folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="3712d-131">To do this through the Partner Center API, see the following topics:</span></span> 

-   [<span data-ttu-id="3712d-132">Abrufen der Bestätigung der Zustimmung des Kunden</span><span class="sxs-lookup"><span data-stu-id="3712d-132">Get confirmation of customer consent</span></span>](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [<span data-ttu-id="3712d-133">Abrufen von Vertragsmetadaten</span><span class="sxs-lookup"><span data-stu-id="3712d-133">Get agreement metadata</span></span>](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [<span data-ttu-id="3712d-134">Bestätigen der Zustimmung des Kunden</span><span class="sxs-lookup"><span data-stu-id="3712d-134">Confirm customer consent</span></span>](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


<span data-ttu-id="3712d-135">Dies gilt für Produktions- und Sandboxumgebungen.</span><span class="sxs-lookup"><span data-stu-id="3712d-135">This applies to both production and sandbox environments.</span></span>

## <a name="confirming-customer-acceptance-in-partner-center"></a><span data-ttu-id="3712d-136">Bestätigen der Zustimmung des Kunden im Partner Center</span><span class="sxs-lookup"><span data-stu-id="3712d-136">Confirming customer acceptance in Partner Center</span></span>

### <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="3712d-137">Bestätigen der Kundenzustimmung für einen neuen Kunden</span><span class="sxs-lookup"><span data-stu-id="3712d-137">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="3712d-138">Verwenden Sie das folgende Verfahren, um die Zustimmung des Kunden zu bestätigen, während Sie einen neuen Kundenmandanten im Partner Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="3712d-138">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="3712d-139">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="3712d-139">Note that you must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3712d-140">Wählen Sie **Kunden** und dann **Neuer Kunde** aus, und klicken Sie anschließend auf **Kontoinformationen**.</span><span class="sxs-lookup"><span data-stu-id="3712d-140">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>
2. <span data-ttu-id="3712d-141">Geben Sie die Informationen zum **Unternehmen** und zum **Primären Kontakt** ein.</span><span class="sxs-lookup"><span data-stu-id="3712d-141">Enter the information about the **Company** and **Primary contact**.</span></span>

![Unternehmensinformationen](images/mca/mca1.png)

3. <span data-ttu-id="3712d-143">Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Der Kunde hat die neueste Microsoft-Kundenvereinbarung akzeptiert** aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-143">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>
4. <span data-ttu-id="3712d-144">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="3712d-144">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3712d-145">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3712d-145">You cannot set this to a future date.</span></span>
5. <span data-ttu-id="3712d-146">Geben Sie die Details des Benutzers ein, der die Zustimmung bereitgestellt hat.</span><span class="sxs-lookup"><span data-stu-id="3712d-146">Enter the details of the user who provided the acceptance.</span></span>

![Hinzufügen eines Annahmedatums](images/mca/MCA3.png)

<span data-ttu-id="3712d-148">Standardmäßig werden die Informationen des primären Kontakts angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3712d-148">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="3712d-149">Wenn diese nicht richtig sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname**, **Nachname**, **E-Mail-Adresse** und \**Telefonnummer* (optional) der Person ein, die der Vereinbarung zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="3712d-149">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="3712d-150">Wählen Sie **Weiter** aus, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.</span><span class="sxs-lookup"><span data-stu-id="3712d-150">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="3712d-151">Bestätigen der Kundenzustimmung für einen vorhandenen Kunden</span><span class="sxs-lookup"><span data-stu-id="3712d-151">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="3712d-152">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="3712d-152">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3712d-153">Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-153">Select **Customers**, and then find and select the customer you want to see.</span></span>
2. <span data-ttu-id="3712d-154">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-154">Select **Account info**.</span></span>
3. <span data-ttu-id="3712d-155">Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-155">Under **Microsoft customer agreement**, select **Update**.</span></span>

![Update/Aktualisieren](images/mca/mca4.png)

4. <span data-ttu-id="3712d-157">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="3712d-157">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>
5. <span data-ttu-id="3712d-158">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="3712d-158">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3712d-159">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3712d-159">You cannot set this to a future date.</span></span>
6. <span data-ttu-id="3712d-160">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-160">Select **Save and continue**.</span></span>

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="3712d-161">Bestätigen der Kundenzustimmung beim Erstellen eines neuen Auftrags für einen vorhandenen Kunden</span><span class="sxs-lookup"><span data-stu-id="3712d-161">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="3712d-162">Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="3712d-162">If you try to create a new order for an existing customer which you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="3712d-163">Führen Sie dazu die nachfolgend aufgeführten Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-163">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="3712d-164">Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.</span><span class="sxs-lookup"><span data-stu-id="3712d-164">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>
2. <span data-ttu-id="3712d-165">Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein.</span><span class="sxs-lookup"><span data-stu-id="3712d-165">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3712d-166">Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3712d-166">You cannot set this to a future date.</span></span>
3. <span data-ttu-id="3712d-167">Wählen Sie **Speichern und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-167">Select **Save and continue**.</span></span>

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="3712d-168">Abrufen der Bestätigung der Kundenzustimmung für einen vorhandenen Kunden</span><span class="sxs-lookup"><span data-stu-id="3712d-168">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="3712d-169">Sie können die Bestätigung der Zustimmung für einen vorhandenen Kunden abrufen, den Sie zuvor mit dem nachstehenden Verfahren angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="3712d-169">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="3712d-170">Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.</span><span class="sxs-lookup"><span data-stu-id="3712d-170">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3712d-171">Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-171">Select **Customers**, and then find and select the customer you want to see.</span></span>
2. <span data-ttu-id="3712d-172">Wählen Sie **Kontoinformationen** aus.</span><span class="sxs-lookup"><span data-stu-id="3712d-172">Select **Account info**.</span></span>
3. <span data-ttu-id="3712d-173">Unter **Microsoft-Kundenvereinbarung** sehen Sie, ob für diesen Kunden eine Bestätigung bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3712d-173">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>
