---
title: Erstellen eines Partner Center-Kontos | Partner Center
ms.topic: article
ms.date: 10/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Mitglieder im Microsoft Partner Network müssen ein Partner Center-Konto erstellen, um ihre Netzwerkvorteile und Kompetenzen verwalten und ein Geschäftsprofil erstellen zu können.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: high
ms.openlocfilehash: 46a299f8e882f6f55d4f674c989446250c0c26d6
ms.sourcegitcommit: f95cd3e5650451a45c7fe6906202420dd80c5a88
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/14/2019
ms.locfileid: "74096476"
---
# <a name="create-a-partner-center-account"></a><span data-ttu-id="0a481-103">Erstellen eines Partner Center-Kontos</span><span class="sxs-lookup"><span data-stu-id="0a481-103">Create a Partner Center account</span></span>

<span data-ttu-id="0a481-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="0a481-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0a481-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="0a481-105">Global admin</span></span>
- <span data-ttu-id="0a481-106">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="0a481-106">Admin agent</span></span>

<span data-ttu-id="0a481-107">Damit Sie ein Konto in Partner Center erstellen oder sich für ein Partnerprogramm registrieren können, muss Ihr Unternehmen Mitglied im Microsoft Partner Network sein.</span><span class="sxs-lookup"><span data-stu-id="0a481-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="0a481-108">Falls Sie noch kein Mitglied des Netzwerks sind, können Sie [jetzt beitreten](https://partners.microsoft.com/PartnerProgram/simplifiedenrollment.aspx).</span><span class="sxs-lookup"><span data-stu-id="0a481-108">If you're not already a member of the network, you can [join now](https://partners.microsoft.com/PartnerProgram/simplifiedenrollment.aspx).</span></span>  <span data-ttu-id="0a481-109">Weitere Informationen zur Mitgliedschaft im Microsoft Partner Network finden Sie [hier](https://partner.microsoft.com/membership).</span><span class="sxs-lookup"><span data-stu-id="0a481-109">[Learn more](https://partner.microsoft.com/membership) about membership in the Microsoft Partner Network.</span></span> <span data-ttu-id="0a481-110">Nachdem Sie ein Partner Center-Konto erstellt haben, schauen Sie sich dieses kurze Video an: [Entdecken Ihres Dashboards](https://vimeo.com/290338211).</span><span class="sxs-lookup"><span data-stu-id="0a481-110">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="0a481-111">Vorbemerkungen</span><span class="sxs-lookup"><span data-stu-id="0a481-111">Before you begin</span></span>

<span data-ttu-id="0a481-112">Zum Erstellen eines Kontos in Partner Center müssen Sie die folgenden Informationen zur Hand haben.</span><span class="sxs-lookup"><span data-stu-id="0a481-112">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="0a481-113">Es empfiehlt sich unter Umständen, vor Beginn des Vorgangs folgende Angaben zu sammeln:</span><span class="sxs-lookup"><span data-stu-id="0a481-113">You may want to take a few minutes to gather these items before you get started:</span></span>

-   <span data-ttu-id="0a481-114">Geschäftliche E-Mail-Adresse des globalen Administrators.</span><span class="sxs-lookup"><span data-stu-id="0a481-114">Global administrator work email.</span></span>

-   <span data-ttu-id="0a481-115">Wenn Sie nicht genau wissen, was das Geschäftskonto Ihres Unternehmens ist, lesen Sie [Das Geschäftskonto Ihrer Firma und Partner Center](azure-active-directory-tenants-and-partner-center.md). Falls Ihr Unternehmen kein Geschäftskonto hat, können Sie während des Kontoerstellungsprozesses eines erstellen.</span><span class="sxs-lookup"><span data-stu-id="0a481-115">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

-   <span data-ttu-id="0a481-116">Offizieller geschäftlicher Name und geschäftliche Anschrift Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="0a481-116">Your company's legal business name and address.</span></span>  

-   <span data-ttu-id="0a481-117">Befugnis zum Unterzeichnen von Vereinbarungen.</span><span class="sxs-lookup"><span data-stu-id="0a481-117">Authority to sign legal agreements.</span></span> <span data-ttu-id="0a481-118">Stellen Sie sicher, dass Sie berechtigt sind, Vereinbarungen im Auftrag Ihres Unternehmens zu unterzeichnen, weil Sie während des Registrierungsprozesses dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="0a481-118">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

-   <span data-ttu-id="0a481-119">Name und geschäftliche E-Mail-Adresse der Person, die als Hauptansprechpartner fungieren soll.</span><span class="sxs-lookup"><span data-stu-id="0a481-119">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="0a481-120">Aus Sicherheits- und Datenschutzgründen werden wir Ihren Hauptansprechpartner per E-Mail kontaktieren, um uns zu vergewissern, dass (1) er/sie sich für ein Partner Center-Konto registriert hat und dass (2) die E-Mail-Adresse zu Ihrem Unternehmen gehört.</span><span class="sxs-lookup"><span data-stu-id="0a481-120">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="0a481-121">Nachdem der Hauptansprechpartner die E-Mail-Adresse bestätigt hat, fahren wir mit der Prüfung deiner Angaben fort.</span><span class="sxs-lookup"><span data-stu-id="0a481-121">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="0a481-122">Wir überprüfen diese Informationen im Rahmen des Kontoerstellungsprozesses.</span><span class="sxs-lookup"><span data-stu-id="0a481-122">We'll verify this information during the account creation process.</span></span> 
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="0a481-123">Erstellen eines Partner Center-Kontos</span><span class="sxs-lookup"><span data-stu-id="0a481-123">Create a Partner Center account</span></span>

1.  <span data-ttu-id="0a481-124">Lesen Sie die Informationen auf der Seite **Willkommen**, und wählen Sie **Weiter** aus.</span><span class="sxs-lookup"><span data-stu-id="0a481-124">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="0a481-125">Melden Sie sich beim Geschäftskonto Ihres Unternehmens als globaler Administrator an.</span><span class="sxs-lookup"><span data-stu-id="0a481-125">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="0a481-126">Wenn Sie nicht genau wissen, was das Geschäftskonto Ihres Unternehmens ist, lesen Sie [Das Geschäftskonto Ihrer Firma und Partner Center](azure-active-directory-tenants-and-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="0a481-126">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="0a481-127">Wählen Sie **Anmelden** aus, wenn Sie wissen, dass Ihr Unternehmen über ein geschäftliches E-Mail-Konto verfügt.</span><span class="sxs-lookup"><span data-stu-id="0a481-127">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="0a481-128">Geben Sie auf der nächsten Seite die Anmeldeinformationen eines globalen Administrators für das Geschäftskonto ein.</span><span class="sxs-lookup"><span data-stu-id="0a481-128">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="0a481-129">Falls Ihr Unternehmen kein Geschäftskonto besitzt, wählen Sie **Konto erstellen** aus, um eines einzurichten.</span><span class="sxs-lookup"><span data-stu-id="0a481-129">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="0a481-130">Melden Sie sich nach der Erstellung eines Geschäftskontos mit Ihren Anmeldeinformationen eines globalen Administrators für das soeben erstellte Konto an.</span><span class="sxs-lookup"><span data-stu-id="0a481-130">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="0a481-131">Geben Sie das offizielle Geschäftsprofil Ihres Unternehmens und Informationen zum Hauptansprechpartner an, oder aktualisieren Sie die entsprechenden Informationen, und wählen Sie **Jetzt registrieren** aus.</span><span class="sxs-lookup"><span data-stu-id="0a481-131">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="0a481-132">Der Hauptansprechpartner muss eine Person in Ihrem Unternehmen sein, die wir im Zusammenhang mit Ihrer Bewerbung kontaktieren können (entweder Sie selbst oder eine andere Person in Ihrem Unternehmen).</span><span class="sxs-lookup"><span data-stu-id="0a481-132">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="0a481-133">Wir prüfen anhand dieser Informationen auch, ob diese Person in Ihrem Unternehmen arbeitet und sich für ein Partner Center-Konto registriert hat.</span><span class="sxs-lookup"><span data-stu-id="0a481-133">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="0a481-134">Aus Sicherheits- und Datenschutzgründen werden wir Ihren Hauptansprechpartner per E-Mail kontaktieren, um uns zu vergewissern, dass (1) er/sie sich für ein Partner Center-Konto registriert hat und dass (2) die E-Mail-Adresse zu Ihrem Unternehmen gehört.</span><span class="sxs-lookup"><span data-stu-id="0a481-134">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="0a481-135">Nachdem der Hauptansprechpartner die E-Mail-Adresse bestätigt hat, fahren wir mit der Prüfung deiner Angaben fort.</span><span class="sxs-lookup"><span data-stu-id="0a481-135">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="0a481-136">Lesen und akzeptieren Sie die Bestimmungen der Microsoft Partner Network-Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="0a481-136">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="0a481-137">Vergewissern Sie sich, dass Sie der Administrator-Agent-Gruppe hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="0a481-137">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="0a481-138">Um die Einrichtung Ihres Kontos (einschließlich des Hinzufügens weiterer Benutzer) abzuschließen, müssen Sie über Administrator-Agent-Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="0a481-138">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="0a481-139">Führen Sie zum Anzeigen oder Aktualisieren Ihrer Berechtigungen die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="0a481-139">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="0a481-140">a.</span><span class="sxs-lookup"><span data-stu-id="0a481-140">a.</span></span> <span data-ttu-id="0a481-141">Wählen Sie im Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home**) das Symbol **Einstellungen** und anschließend **Benutzerverwaltung** aus.</span><span class="sxs-lookup"><span data-stu-id="0a481-141">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="0a481-142">b.</span><span class="sxs-lookup"><span data-stu-id="0a481-142">b.</span></span> <span data-ttu-id="0a481-143">Wähle deinen Namen aus der Benutzerliste und dann **Administrator-Agent** aus, sofern diese Option nicht bereits ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="0a481-143">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="0a481-144">Wählen Sie **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="0a481-144">Select **Update**.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="0a481-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0a481-145">Next steps</span></span>

-   [<span data-ttu-id="0a481-146">Erstellen von Benutzerkonten und Zuweisen von Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a481-146">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="0a481-147">Erstmaliges Erwerben oder Verlängern eines Microsoft Action Pack-Abonnements</span><span class="sxs-lookup"><span data-stu-id="0a481-147">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="0a481-148">Verwalten der Microsoft Partner Network-Mitgliedschaftsvorteile</span><span class="sxs-lookup"><span data-stu-id="0a481-148">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="0a481-149">Erfahren Sie mehr über die Kompetenzanforderungen für die Silber- und Gold-Mitgliedschaft.</span><span class="sxs-lookup"><span data-stu-id="0a481-149">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="0a481-150">Erstellen Sie ein Unternehmensprofil, um Vertriebsleads von Microsoft zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="0a481-150">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="0a481-151">Erhalten und Verwalten von Vertriebsleads von Microsoft</span><span class="sxs-lookup"><span data-stu-id="0a481-151">Get and manage sales leads from Microsoft</span></span>](responding-to-referrals.md)