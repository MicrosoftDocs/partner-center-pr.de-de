---
title: Erstellen eines Partner Center-Kontos | Partner Center
ms.topic: article
ms.date: 10/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Mitglieder im Microsoft Partner Network müssen ein Partner Center-Konto erstellen, um ihre Netzwerkvorteile und Kompetenzen verwalten und ein Geschäftsprofil erstellen zu können.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e1497003ef9ca08b61f0ae752eab654dc40b6997
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653263"
---
# <a name="create-a-partner-center-account"></a><span data-ttu-id="766b9-103">Partner Center-Konto erstellen</span><span class="sxs-lookup"><span data-stu-id="766b9-103">Create a Partner Center account</span></span>

<span data-ttu-id="766b9-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="766b9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="766b9-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="766b9-105">Global admin</span></span>
- <span data-ttu-id="766b9-106">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="766b9-106">Admin agent</span></span>

<span data-ttu-id="766b9-107">Damit Sie ein Konto in Partner Center erstellen oder sich für ein Partnerprogramm registrieren können, muss Ihr Unternehmen Mitglied im Microsoft Partner Network sein.</span><span class="sxs-lookup"><span data-stu-id="766b9-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="766b9-108">Falls Sie noch kein Mitglied des Netzwerks sind, können Sie [jetzt beitreten](https://partners.microsoft.com/PartnerProgram/simplifiedenrollment.aspx).</span><span class="sxs-lookup"><span data-stu-id="766b9-108">If you're not already a member of the network, you can [join now](https://partners.microsoft.com/PartnerProgram/simplifiedenrollment.aspx).</span></span>  <span data-ttu-id="766b9-109">Weitere Informationen zur Mitgliedschaft im Microsoft Partner Network finden Sie [hier](https://partner.microsoft.com/membership).</span><span class="sxs-lookup"><span data-stu-id="766b9-109">[Learn more](https://partner.microsoft.com/membership) about membership in the Microsoft Partner Network.</span></span> <span data-ttu-id="766b9-110">Nachdem Sie ein Partner Center-Konto erstellt haben, schauen Sie sich dieses kurze Video an: [Entdecken Ihres Dashboards](https://vimeo.com/290338211).</span><span class="sxs-lookup"><span data-stu-id="766b9-110">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="766b9-111">Vorbemerkungen</span><span class="sxs-lookup"><span data-stu-id="766b9-111">Before you begin</span></span>

<span data-ttu-id="766b9-112">Zum Erstellen eines Kontos im Partner Center müssen Sie über die folgenden Informationen verfügen.</span><span class="sxs-lookup"><span data-stu-id="766b9-112">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="766b9-113">Es empfiehlt sich unter Umständen, vor Beginn des Vorgangs folgende Angaben zu sammeln:</span><span class="sxs-lookup"><span data-stu-id="766b9-113">You may want to take a few minutes to gather these items before you get started:</span></span>

-   <span data-ttu-id="766b9-114">Geschäftliche E-Mail-Adresse des globalen Administrators.</span><span class="sxs-lookup"><span data-stu-id="766b9-114">Global administrator work email.</span></span>

-   <span data-ttu-id="766b9-115">Wenn Sie nicht sicher sind, wie sich das Geschäftskonto Ihres Unternehmens befindet, finden Sie weitere Informationen [unter Ihrem Unternehmens Konto und Partner Center](azure-active-directory-tenants-and-partner-center.md) , wenn Ihr Unternehmen nicht über ein Geschäftskonto verfügt, das Sie während der Kontoerstellung erstellen können.</span><span class="sxs-lookup"><span data-stu-id="766b9-115">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

-   <span data-ttu-id="766b9-116">Der rechtliche geschäftliche Name und die Adresse Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="766b9-116">Your company's legal business name and address.</span></span>  

-   <span data-ttu-id="766b9-117">Befugnis zum Unterzeichnen von Vereinbarungen.</span><span class="sxs-lookup"><span data-stu-id="766b9-117">Authority to sign legal agreements.</span></span> <span data-ttu-id="766b9-118">Stellen Sie sicher, dass Sie berechtigt sind, gesetzliche Verträge im Auftrag Ihres Unternehmens zu signieren, da Sie dazu während des Registrierungsvorgangs aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="766b9-118">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

-   <span data-ttu-id="766b9-119">Name und geschäftliche E-Mail-Adresse der Person, die als Hauptansprechpartner fungieren soll.</span><span class="sxs-lookup"><span data-stu-id="766b9-119">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="766b9-120">Um die Sicherheit und den Datenschutz Ihres Unternehmens zu gewährleisten, senden wir Ihren primären Kontakt an, um zu überprüfen, ob (1) er sich für ein Partner Center-Konto registriert hat und dass (2) diese e-Mail-Adresse zu Ihrem Unternehmen gehört.</span><span class="sxs-lookup"><span data-stu-id="766b9-120">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="766b9-121">Nachdem der primäre Kontakt seine e-Mail-Adresse überprüft hat, wird die Überprüfung der von Ihnen bereitgestellten Informationen fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="766b9-121">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="766b9-122">Diese Informationen werden während des Konto Erstellungs Vorgangs überprüft.</span><span class="sxs-lookup"><span data-stu-id="766b9-122">We'll verify this information during the account creation process.</span></span> 
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="766b9-123">Partner Center-Konto erstellen</span><span class="sxs-lookup"><span data-stu-id="766b9-123">Create a Partner Center account</span></span>

1.  <span data-ttu-id="766b9-124">Lesen Sie die Informationen auf der Seite **Willkommen**, und wählen Sie **Weiter** aus.</span><span class="sxs-lookup"><span data-stu-id="766b9-124">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="766b9-125">Melden Sie sich beim Geschäftskonto Ihres Unternehmens als globaler Administrator an.</span><span class="sxs-lookup"><span data-stu-id="766b9-125">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="766b9-126">Wenn Sie nicht sicher sind, wie sich das Geschäftskonto Ihres Unternehmens befindet, finden Sie weitere Informationen [unter Geschäftskonto und Partner Center](azure-active-directory-tenants-and-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="766b9-126">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="766b9-127">Wählen Sie **Anmelden** aus, wenn Sie wissen, dass Ihr Unternehmen über ein geschäftliches E-Mail-Konto verfügt.</span><span class="sxs-lookup"><span data-stu-id="766b9-127">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="766b9-128">Geben Sie auf der nächsten Seite die Anmeldeinformationen eines globalen Administrators für das Geschäftskonto ein.</span><span class="sxs-lookup"><span data-stu-id="766b9-128">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="766b9-129">Wenn Ihr Unternehmen nicht über ein Geschäftskonto verfügt, wählen Sie **Erstellen** aus, um ein Konto einzurichten.</span><span class="sxs-lookup"><span data-stu-id="766b9-129">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="766b9-130">Nachdem Sie ein Geschäftskonto erstellt haben, melden Sie sich mit ihren globalen Administrator Anmelde Informationen für das soeben erstellte Geschäftskonto an.</span><span class="sxs-lookup"><span data-stu-id="766b9-130">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="766b9-131">Geben oder aktualisieren Sie das rechtliche Geschäftsprofil und die primären Kontaktinformationen Ihres Unternehmens, und klicken Sie dann auf **jetzt registrieren**.</span><span class="sxs-lookup"><span data-stu-id="766b9-131">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="766b9-132">Der Hauptansprechpartner muss eine Person in Ihrem Unternehmen sein, die wir im Zusammenhang mit Ihrer Bewerbung kontaktieren können (entweder Sie selbst oder eine andere Person in Ihrem Unternehmen).</span><span class="sxs-lookup"><span data-stu-id="766b9-132">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="766b9-133">Wir prüfen anhand dieser Informationen auch, ob diese Person in Ihrem Unternehmen arbeitet und sich für ein Partner Center-Konto registriert hat.</span><span class="sxs-lookup"><span data-stu-id="766b9-133">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="766b9-134">Um die Sicherheit und den Datenschutz Ihres Unternehmens zu gewährleisten, senden wir eine e-Mail an Ihren primären Kontakt, um zu überprüfen, ob (1) er sich für ein Partner Center-Konto registriert hat, und (2) dass diese e-Mail-Adresse zu Ihrem Unternehmen gehört</span><span class="sxs-lookup"><span data-stu-id="766b9-134">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="766b9-135">Nachdem der primäre Kontakt seine e-Mail-Adresse überprüft hat, wird die Überprüfung der von Ihnen bereitgestellten Informationen fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="766b9-135">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="766b9-136">Lesen und akzeptieren Sie die Bestimmungen der Microsoft Partner Network-Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="766b9-136">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="766b9-137">Vergewissern Sie sich, dass Sie der Gruppe "Administrator-Agent" hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="766b9-137">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="766b9-138">Um die Einrichtung Ihres Kontos (einschließlich des Hinzufügens weiterer Benutzer) abzuschließen, müssen Sie über Administrator-Agent-Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="766b9-138">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="766b9-139">Führen Sie zum Anzeigen oder Aktualisieren Ihrer Berechtigungen die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="766b9-139">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="766b9-140">a.</span><span class="sxs-lookup"><span data-stu-id="766b9-140">a.</span></span> <span data-ttu-id="766b9-141">Wählen Sie im Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home**)das Symbol " **Einstellungen** " und dann " **Benutzerverwaltung**" aus.</span><span class="sxs-lookup"><span data-stu-id="766b9-141">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="766b9-142">b.</span><span class="sxs-lookup"><span data-stu-id="766b9-142">b.</span></span> <span data-ttu-id="766b9-143">Wählen Sie in der Liste Benutzer ihren Namen aus, und wählen Sie dann **Administrator-Agent** aus, wenn er nicht bereits ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="766b9-143">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="766b9-144">Wählen Sie **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="766b9-144">Select **Update**.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="766b9-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="766b9-145">Next steps</span></span>

-   [<span data-ttu-id="766b9-146">Erstellen von Benutzerkonten und Zuweisen von Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="766b9-146">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="766b9-147">Erstmaliges Erwerben oder Verlängern eines Microsoft Action Pack-Abonnements</span><span class="sxs-lookup"><span data-stu-id="766b9-147">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="766b9-148">Verwalten der Microsoft Partner Network-Mitgliedschaftsvorteile</span><span class="sxs-lookup"><span data-stu-id="766b9-148">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="766b9-149">Erfahren Sie mehr über die Kompetenzanforderungen für die Silber- und Gold-Mitgliedschaft.</span><span class="sxs-lookup"><span data-stu-id="766b9-149">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="766b9-150">Erstellen Sie ein Unternehmensprofil, um Vertriebsleads von Microsoft zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="766b9-150">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="766b9-151">Erhalten und Verwalten von Vertriebsleads von Microsoft</span><span class="sxs-lookup"><span data-stu-id="766b9-151">Get and manage sales leads from Microsoft</span></span>](responding-to-referrals.md)