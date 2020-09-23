---
title: Erstellen eines Partner Center-Kontos
ms.topic: article
ms.date: 08/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Mitglieder im Microsoft Partner Network ein Partner Center-Konto erstellen können, um ihre Netzwerkvorteile und Kompetenzen zu verwalten.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f94b11c4feb9cd1bedd97bebc537a504f9c4d127
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999354"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="1cb81-103">Erstellen eines Partner Center-Kontos zum Verwalten von Netzwerkvorteilen und Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="1cb81-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="1cb81-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="1cb81-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1cb81-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="1cb81-105">Global admin</span></span>
- <span data-ttu-id="1cb81-106">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="1cb81-106">Admin agent</span></span>

<span data-ttu-id="1cb81-107">Damit Sie ein Konto in Partner Center erstellen oder sich für ein Partnerprogramm registrieren können, muss Ihr Unternehmen Mitglied im Microsoft Partner Network sein.</span><span class="sxs-lookup"><span data-stu-id="1cb81-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="1cb81-108">Falls Sie noch kein Mitglied des Netzwerks sind, können Sie [jetzt beitreten](https://partner.microsoft.com/commercial#).</span><span class="sxs-lookup"><span data-stu-id="1cb81-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="1cb81-109">Nachdem Sie ein Partner Center-Konto erstellt haben, schauen Sie sich dieses kurze Video an: [Entdecken Ihres Dashboards](https://vimeo.com/290338211).</span><span class="sxs-lookup"><span data-stu-id="1cb81-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1cb81-110">Vorbereitung</span><span class="sxs-lookup"><span data-stu-id="1cb81-110">Before you begin</span></span>

<span data-ttu-id="1cb81-111">Zum Erstellen eines Kontos in Partner Center müssen Sie die folgenden Informationen zur Hand haben.</span><span class="sxs-lookup"><span data-stu-id="1cb81-111">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="1cb81-112">Es empfiehlt sich unter Umständen, vor Beginn des Vorgangs folgende Angaben zu sammeln:</span><span class="sxs-lookup"><span data-stu-id="1cb81-112">You may want to take a few minutes to gather these items before you get started:</span></span>

-   <span data-ttu-id="1cb81-113">Geschäftliche E-Mail-Adresse des globalen Administrators.</span><span class="sxs-lookup"><span data-stu-id="1cb81-113">Global administrator work email.</span></span>

-   <span data-ttu-id="1cb81-114">Wenn Sie nicht genau wissen, was das Geschäftskonto Ihres Unternehmens ist, lesen Sie [Das Geschäftskonto Ihrer Firma und Partner Center](azure-active-directory-tenants-and-partner-center.md). Falls Ihr Unternehmen kein Geschäftskonto hat, können Sie während des Kontoerstellungsprozesses eines erstellen.</span><span class="sxs-lookup"><span data-stu-id="1cb81-114">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

-   <span data-ttu-id="1cb81-115">Offizieller geschäftlicher Name und geschäftliche Anschrift Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="1cb81-115">Your company's legal business name and address.</span></span>  

-   <span data-ttu-id="1cb81-116">Befugnis zum Unterzeichnen von Vereinbarungen.</span><span class="sxs-lookup"><span data-stu-id="1cb81-116">Authority to sign legal agreements.</span></span> <span data-ttu-id="1cb81-117">Stellen Sie sicher, dass Sie berechtigt sind, Vereinbarungen im Auftrag Ihres Unternehmens zu unterzeichnen, weil Sie während des Registrierungsprozesses dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="1cb81-117">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

-   <span data-ttu-id="1cb81-118">Name und geschäftliche E-Mail-Adresse der Person, die als Hauptansprechpartner fungieren soll.</span><span class="sxs-lookup"><span data-stu-id="1cb81-118">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="1cb81-119">Aus Sicherheits- und Datenschutzgründen werden wir Ihren Hauptansprechpartner per E-Mail kontaktieren, um uns zu vergewissern, dass (1) er/sie sich für ein Partner Center-Konto registriert hat und dass (2) die E-Mail-Adresse zu Ihrem Unternehmen gehört.</span><span class="sxs-lookup"><span data-stu-id="1cb81-119">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="1cb81-120">Nachdem der Hauptansprechpartner die E-Mail-Adresse bestätigt hat, fahren wir mit der Prüfung deiner Angaben fort.</span><span class="sxs-lookup"><span data-stu-id="1cb81-120">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="1cb81-121">Wir überprüfen diese Informationen im Rahmen des Kontoerstellungsprozesses.</span><span class="sxs-lookup"><span data-stu-id="1cb81-121">We'll verify this information during the account creation process.</span></span> 
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="1cb81-122">Erstellen eines Partner Center-Kontos</span><span class="sxs-lookup"><span data-stu-id="1cb81-122">Create a Partner Center account</span></span>

1.  <span data-ttu-id="1cb81-123">Lesen Sie die Informationen auf der Seite **Willkommen**, und wählen Sie **Weiter** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb81-123">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="1cb81-124">Melden Sie sich beim Geschäftskonto Ihres Unternehmens als globaler Administrator an.</span><span class="sxs-lookup"><span data-stu-id="1cb81-124">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="1cb81-125">Wenn Sie nicht genau wissen, was das Geschäftskonto Ihres Unternehmens ist, lesen Sie [Das Geschäftskonto Ihrer Firma und Partner Center](azure-active-directory-tenants-and-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="1cb81-125">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="1cb81-126">Wählen Sie **Anmelden** aus, wenn Sie wissen, dass Ihr Unternehmen über ein geschäftliches E-Mail-Konto verfügt.</span><span class="sxs-lookup"><span data-stu-id="1cb81-126">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="1cb81-127">Geben Sie auf der nächsten Seite die Anmeldeinformationen eines globalen Administrators für das Geschäftskonto ein.</span><span class="sxs-lookup"><span data-stu-id="1cb81-127">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="1cb81-128">Falls Ihr Unternehmen kein Geschäftskonto besitzt, wählen Sie **Konto erstellen** aus, um eines einzurichten.</span><span class="sxs-lookup"><span data-stu-id="1cb81-128">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="1cb81-129">Melden Sie sich nach der Erstellung eines Geschäftskontos mit Ihren Anmeldeinformationen eines globalen Administrators für das soeben erstellte Konto an.</span><span class="sxs-lookup"><span data-stu-id="1cb81-129">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="1cb81-130">Geben Sie das offizielle Geschäftsprofil Ihres Unternehmens und Informationen zum Hauptansprechpartner an, oder aktualisieren Sie die entsprechenden Informationen, und wählen Sie **Jetzt registrieren** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb81-130">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="1cb81-131">Der Hauptansprechpartner muss eine Person in Ihrem Unternehmen sein, die wir im Zusammenhang mit Ihrer Bewerbung kontaktieren können (entweder Sie selbst oder eine andere Person in Ihrem Unternehmen).</span><span class="sxs-lookup"><span data-stu-id="1cb81-131">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="1cb81-132">Wir prüfen anhand dieser Informationen auch, ob diese Person in Ihrem Unternehmen arbeitet und sich für ein Partner Center-Konto registriert hat.</span><span class="sxs-lookup"><span data-stu-id="1cb81-132">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="1cb81-133">Aus Sicherheits- und Datenschutzgründen werden wir Ihren Hauptansprechpartner per E-Mail kontaktieren, um uns zu vergewissern, dass (1) er/sie sich für ein Partner Center-Konto registriert hat und dass (2) die E-Mail-Adresse zu Ihrem Unternehmen gehört.</span><span class="sxs-lookup"><span data-stu-id="1cb81-133">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="1cb81-134">Nachdem der Hauptansprechpartner die E-Mail-Adresse bestätigt hat, fahren wir mit der Prüfung deiner Angaben fort.</span><span class="sxs-lookup"><span data-stu-id="1cb81-134">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="1cb81-135">Lesen und akzeptieren Sie die Bestimmungen der Microsoft Partner Network-Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="1cb81-135">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="1cb81-136">Vergewissern Sie sich, dass Sie der Administrator-Agent-Gruppe hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="1cb81-136">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="1cb81-137">Um die Einrichtung Ihres Kontos (einschließlich des Hinzufügens weiterer Benutzer) abzuschließen, müssen Sie über Administrator-Agent-Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="1cb81-137">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="1cb81-138">Führen Sie zum Anzeigen oder Aktualisieren Ihrer Berechtigungen die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="1cb81-138">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="1cb81-139">ein.</span><span class="sxs-lookup"><span data-stu-id="1cb81-139">a.</span></span> <span data-ttu-id="1cb81-140">Wählen Sie im Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home**) das Symbol **Einstellungen** und anschließend **Benutzerverwaltung** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb81-140">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="1cb81-141">b.</span><span class="sxs-lookup"><span data-stu-id="1cb81-141">b.</span></span> <span data-ttu-id="1cb81-142">Wähle deinen Namen aus der Benutzerliste und dann **Administrator-Agent** aus, sofern diese Option nicht bereits ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="1cb81-142">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="1cb81-143">Wählen Sie **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb81-143">Select **Update**.</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="1cb81-144">Anzeigen von MPN-Kontodetails</span><span class="sxs-lookup"><span data-stu-id="1cb81-144">View MPN account details</span></span>

<span data-ttu-id="1cb81-145">Nachdem Sie ein Partner Center-Konto erstellt haben, können Sie zum Partner Center zurückkehren, um verschiedene Kontodetails anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="1cb81-145">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="1cb81-146">Viele dieser Details sind auf der Seite **Partnerprofil** in Ihrem Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) enthalten.</span><span class="sxs-lookup"><span data-stu-id="1cb81-146">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="1cb81-147">Diese Details umfassen Folgendes:</span><span class="sxs-lookup"><span data-stu-id="1cb81-147">Such details include:</span></span>

- <span data-ttu-id="1cb81-148">Offizielles Geschäftsprofil Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="1cb81-148">Your company's legal business profile</span></span>

- <span data-ttu-id="1cb81-149">Informationen zu Ihrer MPN-ID</span><span class="sxs-lookup"><span data-stu-id="1cb81-149">Information about your MPN ID</span></span>

- <span data-ttu-id="1cb81-150">Links zu aktuellen Vereinbarungen im Zusammenhang mit Ihrem registrierten Microsoft-Programm</span><span class="sxs-lookup"><span data-stu-id="1cb81-150">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="1cb81-151">Wenn Sie z. B. für das MPN-Programm registriert sind, wird ein Link zur aktuellen Microsoft Partner Network-Vereinbarung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1cb81-151">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="1cb81-152">Wenn Sie für andere Partnerprogramme wie das CSP-Programm (Cloud Solution Provider) registriert sind, werden möglicherweise auch Links zu anderen Vereinbarungen angezeigt, z. B. der Microsoft Partner-Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="1cb81-152">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="1cb81-153">Diese Art von Links kann nützlich sein, wenn Sie eine Vereinbarung überprüfen, darauf zugreifen oder herunterladen möchten, oder wenn Sie das Datum prüfen möchten, an dem sie unterzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="1cb81-153">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="1cb81-154">Anzeigen von Kontodetails oder Anzeigen und Herunterladen der MPN-Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="1cb81-154">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="1cb81-155">Führen Sie die folgenden Schritte aus, um Kontodetails anzuzeigen oder die MPN-Vereinbarung anzuzeigen und herunterzuladen:</span><span class="sxs-lookup"><span data-stu-id="1cb81-155">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="1cb81-156">Melden Sie sich mit dem Benutzernamen und Kennwort Ihres Geschäftskonto beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="1cb81-156">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1cb81-157">Eine Übersichtsseite wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1cb81-157">An Overview page appears.</span></span> <span data-ttu-id="1cb81-158">(Wenn die Übersichtsseite nicht angezeigt wird, wählen Sie im linken Navigationsmenü die Option **Übersicht** aus.)</span><span class="sxs-lookup"><span data-stu-id="1cb81-158">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="1cb81-159">Wählen Sie das Zahnradsymbol in der oberen rechten Ecke des Dashboards und dann **Partnereinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb81-159">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings**.</span></span> <span data-ttu-id="1cb81-160">Dadurch gelangen Sie zur Seite „Partnerprofil“.</span><span class="sxs-lookup"><span data-stu-id="1cb81-160">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="1cb81-161">Auf der Seite „Partnerprofil“ werden verschiedene Bereiche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1cb81-161">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="1cb81-162">Hierzu gehören ein Bereich **Unternehmensprofil** und ein Bereich **Programminfos**.</span><span class="sxs-lookup"><span data-stu-id="1cb81-162">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="1cb81-163">Suchen Sie unter **Programminfos** nach dem Feld **MPN-Programmstatus**.</span><span class="sxs-lookup"><span data-stu-id="1cb81-163">Under **Program info**, locate the **MPN program status** field.</span></span> <span data-ttu-id="1cb81-164">Dadurch wird ein Link zu Ihrer Microsoft Partner Network-Vereinbarung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1cb81-164">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="1cb81-165">Außerdem wird Ihr aktueller Status im Programm beschrieben.</span><span class="sxs-lookup"><span data-stu-id="1cb81-165">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="Abbildung des Bereichs „Programminfos“ auf der Seite „Partnerprofil“ mit einem roten Kasten zur Hervorhebung des Felds „MPN-Programmstatus“ in diesem Bereich sowie dem zugehörigen Link zur Microsoft Partner Network-Vereinbarung":::

6. <span data-ttu-id="1cb81-167">Wählen Sie **Microsoft Partner Network-Vereinbarung** aus, um diese Vereinbarung anzuzeigen oder herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="1cb81-167">To view or download this agreement, select **Microsoft Partner Network agreement**.</span></span>  

> [!NOTE]
> <span data-ttu-id="1cb81-168">Mithilfe der oben genannten Schritte können Sie auch andere Vereinbarungen für andere registrierte Programme anzeigen oder herunterladen, z. B. die Microsoft Partner-Vereinbarung, wenn Sie für das CSP-Programm (Cloud Solution Provider) registriert sind.</span><span class="sxs-lookup"><span data-stu-id="1cb81-168">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1cb81-169">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="1cb81-169">Next steps</span></span>

-   [<span data-ttu-id="1cb81-170">Erstellen von Benutzerkonten und Zuweisen von Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1cb81-170">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="1cb81-171">Erstmaliges Erwerben oder Verlängern eines Microsoft Action Pack-Abonnements</span><span class="sxs-lookup"><span data-stu-id="1cb81-171">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="1cb81-172">Verwalten der Microsoft Partner Network-Mitgliedschaftsvorteile</span><span class="sxs-lookup"><span data-stu-id="1cb81-172">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="1cb81-173">Erfahren Sie mehr über die Kompetenzanforderungen für die Silber- und Gold-Mitgliedschaft.</span><span class="sxs-lookup"><span data-stu-id="1cb81-173">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="1cb81-174">Erstellen Sie ein Unternehmensprofil, um Vertriebsleads von Microsoft zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="1cb81-174">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="1cb81-175">Erhalten und Verwalten von Vertriebsleads von Microsoft</span><span class="sxs-lookup"><span data-stu-id="1cb81-175">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
