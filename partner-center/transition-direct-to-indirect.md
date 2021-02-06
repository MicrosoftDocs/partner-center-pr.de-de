---
title: Direkt Abrechnungspartner auf indirekten Händler umstellen
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie ein CSP-Programmpartner Partner Center für den Übergang von einem Direct-Bill-Partner zum indirekten Händler verwenden kann.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ceaf3fd0819937177648814a02df4a2a266ee06f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624305"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="861cd-103">Übergang vom CSP-Direktabrechnungspartner (Cloud Solution Provider) zum indirekten CSP-Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="861cd-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="861cd-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="861cd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="861cd-105">Globale Administratoren</span><span class="sxs-lookup"><span data-stu-id="861cd-105">Global admins</span></span>

>[!Note]
><span data-ttu-id="861cd-106">Dieser Artikel richtet sich an Direktabrechnungspartner, die indirekte Wiederverkäufer werden möchten.</span><span class="sxs-lookup"><span data-stu-id="861cd-106">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="861cd-107">Auch wenn Sie noch keine explizite Entscheidung getroffen haben, sich als indirekter Reseller anzumelden, werden direkt Rechnungs Partner, die die neuen [Anforderungen](direct-partner-new-requirements.md) für das CSP Direct Bill Partner Program nicht erfüllen, von Microsoft informiert, wenn Ihre [direkten Rechnungs Funktionen eingeschränkt](restricted-direct-bill-capabilities.md)werden.</span><span class="sxs-lookup"><span data-stu-id="861cd-107">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="861cd-108">Ab Januar 2021 wird eine neue Umsatz Anforderung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="861cd-108">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="861cd-109">Partner, die als direkter Rechnungs Partner angemeldet sind, müssen in den letzten 12 Monaten mindestens USD $300 KB in den Einnahmen eines Cloud Solution Provider-Programms auf der globalen Kontoebene eines Partners durchlaufen haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-109">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="861cd-110">Sie können sich unter Verwendung Ihres vorhandenen Direktabrechnungsmandanten beim Programm für indirekte Wiederverkäufer registrieren.</span><span class="sxs-lookup"><span data-stu-id="861cd-110">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="861cd-111">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="861cd-111">Get started</span></span>

1. <span data-ttu-id="861cd-112">Vergewissern Sie sich, dass Ihr Partnerprofil in Partner Center und Ihre MPN-ID aktuell sind.</span><span class="sxs-lookup"><span data-stu-id="861cd-112">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="861cd-113">Melden Sie sich bei Partner Center als globaler Administrator für den Direktabrechnungsmandanten an, den Sie auf einen indirekten Wiederverkäufer umstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="861cd-113">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Übersicht":::

3. <span data-ttu-id="861cd-115">Überprüfen Sie Ihre Partnerdetails im Registrierungsformular.</span><span class="sxs-lookup"><span data-stu-id="861cd-115">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Jetzt registrieren":::

4. <span data-ttu-id="861cd-117">Wählen Sie „Jetzt registrieren“ aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-117">Select Enroll now.</span></span> <span data-ttu-id="861cd-118">Für Ihre Tätigkeit als indirekter Wiederverkäufer wird der gleiche AAD-Mandant verwendet wie für Ihre direkte Tätigkeit.</span><span class="sxs-lookup"><span data-stu-id="861cd-118">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="861cd-119">Diese neue Übergangsfunktion steht anfänglich nur für Partner mit Onboarding-Jahrestagen zwischen September und Dezember zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="861cd-119">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="861cd-120">Wenn Ihr Jahrestag nicht zwischen September und Dezember liegt, wird die Funktion momentan nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-120">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="861cd-121">Partner mit Jahrestagen nach Dezember 2018 werden benachrichtigt, sobald die Funktion für sie aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="861cd-121">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="861cd-122">Melden Sie sich nach der Genehmigung Ihrer Registrierung erneut bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="861cd-122">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="861cd-123">Die Genehmigung erfolgt in der Regel sofort, kann aber bis zu fünf Werktage dauern.</span><span class="sxs-lookup"><span data-stu-id="861cd-123">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="861cd-124">Nach der Genehmigung wird eine entsprechende Benachrichtigung an die E-Mail-Adresse gesendet, die Sie im Registrierungsformular als primären Kontakt angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-124">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="861cd-125">Sie können den Registrierungsstatus auch unter **Einstellungen**  >  **Kontoeinstellungen**  >  **Partner Profil** > Programm Info überprüfen.</span><span class="sxs-lookup"><span data-stu-id="861cd-125">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="861cd-126">Auf der Seite **Übersicht** wird die Vereinbarung für indirekte Wiederverkäufer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-126">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="861cd-127">Wählen Sie **Zustimmen und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-127">Select **Accept and continue**.</span></span> <span data-ttu-id="861cd-128">Diese Aktion ermöglicht die indirekten Reseller-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="861cd-128">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="861cd-129">Wenn Sie die Vereinbarung für indirekte Wiederverkäufer akzeptiert haben, weist Sie Ihr Partnerprofil als Direktabrechnungspartner **und** als indirekter Wiederverkäufer aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-129">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Vereinbarung für indirekte Wiederverkäufer":::

> [!IMPORTANT]
> <span data-ttu-id="861cd-131">Nachdem Sie sich mit der neuen Funktion als indirekter Wiederverkäufer registriert haben, steht keine Option für ein Rollback zu einem reinen Direktabrechnungsmandanten zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="861cd-131">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="861cd-132">Registrieren Sie sich daher erst nach sorgfältiger Prüfung Ihrer geschäftlichen Anforderungen als indirekter Wiederverkäufer.</span><span class="sxs-lookup"><span data-stu-id="861cd-132">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="861cd-133">Übergangsphase vom Direktabrechnungspartner zum indirekten Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="861cd-133">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="861cd-134">In dieser Phase verwalten Sie weiterhin die Abonnement Anforderungen ihrer direkten Kunden, einschließlich des Abrechnungs Prozesses.</span><span class="sxs-lookup"><span data-stu-id="861cd-134">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="861cd-135">Außerdem beginnen Sie damit, Kunden von Ihrem indirekten Anbieter zu akzeptieren und als indirekter Wiederverkäufer zu agieren.</span><span class="sxs-lookup"><span data-stu-id="861cd-135">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Sie sind sowohl Direktabrechnungspartner als auch indirekter Wiederverkäufer.":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="861cd-137">Suchen eines indirekten Anbieters</span><span class="sxs-lookup"><span data-stu-id="861cd-137">Find an indirect provider</span></span>

<span data-ttu-id="861cd-138">Nach der Registrierung wird in Ihrem linken Navigationsbereich ein Link zu indirekten Anbietern angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-138">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="861cd-139">Als indirekter Wiederverkäufer bauen Sie eine Beziehung zu einem indirekten Anbieter auf, der sich dann um Ihre Abrechnung, um den Produkteinkauf für Ihre Kunden sowie um die Supportinfrastruktur kümmern kann.</span><span class="sxs-lookup"><span data-stu-id="861cd-139">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="861cd-140">Verschiedene indirekte Anbieter bieten unterschiedliche Unterstützung und Leistungen. Ermitteln Sie daher die Anbieter in Ihrer Umgebung, die Ihre Anforderungen am besten erfüllen.</span><span class="sxs-lookup"><span data-stu-id="861cd-140">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="861cd-141">Die meisten Anbieter bieten Folgendes:</span><span class="sxs-lookup"><span data-stu-id="861cd-141">Generally, most providers will:</span></span>

- <span data-ttu-id="861cd-142">Technische Schulung und Unterstützung</span><span class="sxs-lookup"><span data-stu-id="861cd-142">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="861cd-143">Hilfe bei der Vermarktung Ihrer Produkte und Dienste</span><span class="sxs-lookup"><span data-stu-id="861cd-143">Help you market your products and services</span></span>
- <span data-ttu-id="861cd-144">Verwaltung Ihrer Finanzierung und Kreditbedingungen</span><span class="sxs-lookup"><span data-stu-id="861cd-144">Manage your financing and credit terms</span></span>

<span data-ttu-id="861cd-145">Die Liste mit offiziellen indirekten Microsoft-Anbietern finden Sie [hier](https://partnercenter.microsoft.com/partner/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="861cd-145">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="861cd-146">Weitere Informationen finden Sie unter [Arbeiten mit indirekten Anbietern im Programm für Cloud-Lösungsanbieter](indirect-reseller-tasks-in-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="861cd-146">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="861cd-147">Annehmen einer Partnerschaftseinladung von Ihrem indirekten Anbieter</span><span class="sxs-lookup"><span data-stu-id="861cd-147">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="861cd-148">Wenn Sie einen passenden indirekte Anbieter gefunden haben, gehen Sie mit ihm in Partner Center eine Partnerschaft ein.</span><span class="sxs-lookup"><span data-stu-id="861cd-148">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="861cd-149">Der von Ihnen ausgewählte indirekte Anbieter sendet Ihnen eine E-Mail mit einem Einladungslink für eine Partnerschaft, über den Sie zur entsprechenden Einladung in Partner Center gelangen.</span><span class="sxs-lookup"><span data-stu-id="861cd-149">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="861cd-150">Stellen Sie sicher, dass sich Ihr globaler Administrator bei Partner Center anmeldet und dem Einladungslink folgt.</span><span class="sxs-lookup"><span data-stu-id="861cd-150">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="861cd-151">Wenn Sie die Einladung annehmen, wird der Name des Anbieters in der Liste der indirekten Anbieter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-151">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="861cd-152">Gewinnen neuer Kunden als indirekter Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="861cd-152">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="861cd-153">Sowohl Sie selbst als auch Ihr indirekter Anbieter müssen über Vertriebspartnerschaften mit Kunden verfügen.</span><span class="sxs-lookup"><span data-stu-id="861cd-153">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="861cd-154">Diese Reseller-Beziehungen ermöglichen es Ihnen, die Abonnements und Dienste eines Kunden in Ihrem Namen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="861cd-154">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="861cd-155">Um einen neuen Kunden zu gewinnen, der bereits über einen Azure AD-Mandanten verfügt, können Sie den Kunden gleichzeitig zu einer Vertriebspartnerschaft mit Ihnen und Ihrem Anbieter einladen.</span><span class="sxs-lookup"><span data-stu-id="861cd-155">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="861cd-156">So erstellen Sie eine Einladung als indirekter Wiederverkäufer:</span><span class="sxs-lookup"><span data-stu-id="861cd-156">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="861cd-157">Wählen Sie in Partner Center im linken Navigationsbereich die Option **Indirekte Anbieter** aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-157">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="861cd-158">Wählen Sie **Neue Kunden einladen** aus, um einen Kunden zu einer Vertriebspartnerschaft mit Ihnen und dem indirekten Anbieter einzuladen.</span><span class="sxs-lookup"><span data-stu-id="861cd-158">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="861cd-159">Der Anbieter muss über eine Reseller-Beziehung mit Ihrem Kunden verfügen, damit er Bestellungen im Auftrag Ihres Kunden einreichen kann, wenn der Kunde neue Abonnements erwerben oder vorhandene Abonnements neue Lizenzen hinzufügen möchte.</span><span class="sxs-lookup"><span data-stu-id="861cd-159">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="861cd-160">Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="861cd-160">On the next page, review the draft email message.</span></span> <span data-ttu-id="861cd-161">Sie können den Nachrichtenentwurf in Ihrer E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen.</span><span class="sxs-lookup"><span data-stu-id="861cd-161">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="861cd-162">Bearbeiten Sie den Text in der e-Mail-Nachricht, um zu sagen, was Sie brauchen, aber achten Sie darauf, den Link so zu schließen, dass er den Kunden direkt mit Ihrem Konto und dem Konto Ihres Anbieters verbindet.</span><span class="sxs-lookup"><span data-stu-id="861cd-162">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="861cd-163">Wählen Sie dann **Fertig** aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-163">Then select **Done**.</span></span>

5. <span data-ttu-id="861cd-164">Nachdem der Kunde dich und deinen Anbieter als Vertriebspartner autorisiert hat, verfügst du über die nötigen Administratorberechtigungen zur Verwaltung seiner Abonnements, Lizenzen und Benutzer, und dein indirekter Anbieter kann Aufträge im Namen des Kunden übermitteln.</span><span class="sxs-lookup"><span data-stu-id="861cd-164">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="861cd-165">Erweitere zum Verwalten des Kontos, des Diensts, der Benutzer und der Lizenzen des Kunden den Kundeneintrag, indem du neben seinem Namen auf den nach unten weisenden Pfeil klickst.</span><span class="sxs-lookup"><span data-stu-id="861cd-165">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="861cd-166">Anders als bei direkten Rechnungs Partnern können indirekte Vertriebspartner Azure AD Mandanten nicht für Ihre neuen Kunden im Partner Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="861cd-166">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="861cd-167">Ihr Anbieter erstellt den Mandanten und gibt Sie als den indirekten Wiederverkäufer für diesen Kunden an.</span><span class="sxs-lookup"><span data-stu-id="861cd-167">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="861cd-168">Dadurch wird sichergestellt, dass der Kunde in Partner Center in Ihrer Kundenliste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="861cd-168">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="861cd-169">Sie können nicht Ihre Direktabrechnungsfunktion verwenden, um Käufe für Kunden zu erstellen, die Sie als indirekter Wiederverkäufer gewinnen.</span><span class="sxs-lookup"><span data-stu-id="861cd-169">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="861cd-170">Verwalten Ihrer Direktabrechnungskunden und Ihrer Kunden für den indirekten Wiederverkauf</span><span class="sxs-lookup"><span data-stu-id="861cd-170">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="861cd-171">Direktabrechnungskunden und Kunden für den indirekten Wiederverkauf werden unterschiedlich verwaltet.</span><span class="sxs-lookup"><span data-stu-id="861cd-171">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="861cd-172">Direktkunden der Rechnung (was Sie nicht als indirekter Händler tun werden)</span><span class="sxs-lookup"><span data-stu-id="861cd-172">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="861cd-173">Erstellen von Bestellungen für Produkte</span><span class="sxs-lookup"><span data-stu-id="861cd-173">Create orders for products</span></span>
- <span data-ttu-id="861cd-174">Verwalten von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="861cd-174">Manage Azure reservations</span></span>
- <span data-ttu-id="861cd-175">Verwalten des Bestellverlaufs</span><span class="sxs-lookup"><span data-stu-id="861cd-175">Manage their order history</span></span>
- <span data-ttu-id="861cd-176">Kaufen von Software</span><span class="sxs-lookup"><span data-stu-id="861cd-176">Purchase software</span></span>
- <span data-ttu-id="861cd-177">Direktes Abrechnen mit Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-177">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="861cd-178">Kunden indirekter Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="861cd-178">Indirect reseller customers</span></span>

- <span data-ttu-id="861cd-179">Indirekter Anbieter bestellt Produkte für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-179">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="861cd-180">Verwalten von Lizenzen und Benutzern von Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-180">Manage customers' licenses and users</span></span>
- <span data-ttu-id="861cd-181">Abwickeln von Abonnementverlängerungen</span><span class="sxs-lookup"><span data-stu-id="861cd-181">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="861cd-182">So erkennen Sie Kunden, die Sie als Direktabrechnungspartner gewonnen haben:</span><span class="sxs-lookup"><span data-stu-id="861cd-182">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="861cd-183">**Kunden** auswählen</span><span class="sxs-lookup"><span data-stu-id="861cd-183">Select **Customers**</span></span>

2. <span data-ttu-id="861cd-184">Wählen Sie einen Kunden aus, um dessen Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="861cd-184">Select a customer to view their details</span></span>

3. <span data-ttu-id="861cd-185">Wenn Sie diesen Kunden als Direktabrechnungspartner gewonnen haben, werden Optionen zum **Hinzufügen** oder **Anzeigen von Produkten** sowie die Abonnements des Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-185">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="861cd-186">Wenn zwischen Ihnen und dem Kunden eine indirekte Vertriebspartnerschaft besteht, sind diese Optionen nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="861cd-186">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="861cd-187">Migrieren Ihrer Direktabrechnungskunden zu Ihrem indirekten Anbieter</span><span class="sxs-lookup"><span data-stu-id="861cd-187">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="861cd-188">Ihr indirekter Anbieter kann keine Bestellungen oder vorhandenen Abonnement Übertragungen für Ihre bestehenden Kunden der direkten Abrechnung übermitteln, bis Sie über eine Reseller-Beziehung verfügen.</span><span class="sxs-lookup"><span data-stu-id="861cd-188">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="861cd-189">Sie können eine der folgenden Methoden verwenden, um die Reseller-Beziehung zwischen Ihrem indirekten Anbieter und Ihrem bestehenden Kunden der direkt Rechnung herzustellen:</span><span class="sxs-lookup"><span data-stu-id="861cd-189">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="861cd-190">Reseller Relationship-Erweiterung</span><span class="sxs-lookup"><span data-stu-id="861cd-190">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="861cd-191">Sendet eine indirekte Reseller-Einladung an den Kunden.</span><span class="sxs-lookup"><span data-stu-id="861cd-191">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="861cd-192">Eine ausführliche Übersicht über den Schritt-für-Schritt-Prozess finden Sie im [Dokument direkt zum indirekten Übergang](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) .</span><span class="sxs-lookup"><span data-stu-id="861cd-192">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="861cd-193">Reseller Relationship-Erweiterung</span><span class="sxs-lookup"><span data-stu-id="861cd-193">Reseller relationship extension</span></span>

<span data-ttu-id="861cd-194">Mit dem Feature für die Reseller-Beziehungs Erweiterung können Sie eine Reseller-Beziehung zwischen Ihren vorhandenen Kunden der direkt Rechnung und Ihrem indirekten Anbieter über das Partner Center-Dashboard herstellen.</span><span class="sxs-lookup"><span data-stu-id="861cd-194">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="861cd-195">Beachten Sie vor der Verwendung des Features Folgendes:</span><span class="sxs-lookup"><span data-stu-id="861cd-195">Before using the feature, note the following:</span></span>

- <span data-ttu-id="861cd-196">Diese Funktion ist nur für direkte Rechnungs Partner verfügbar, die sich im Übergang zu einem indirekten Händler befinden und die [indirekte Reseller](#get-started)-Registrierung abgeschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-196">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="861cd-197">Sie können diese Funktion nur auf vorhandene Kunden der direkt Rechnung anwenden.</span><span class="sxs-lookup"><span data-stu-id="861cd-197">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="861cd-198">Dies gilt nicht für [indirekte Reseller-Kunden](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="861cd-198">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="861cd-199">Sie können nur einen indirekten Anbieter auswählen, für den Sie [eine Partner Einladung Ihres indirekten Anbieters angenommen](#accept-a-partnership-invitation-from-your-indirect-provider)haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-199">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="861cd-200">Eine Kopie der Rechnung-zu-Informationen, die Sie für diesen Kunden haben, wird dem indirekten Anbieter zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="861cd-200">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="861cd-201">Sie können auf die Informationen zu den Rechnungen zugreifen, indem Sie im Partner Center-Dashboard auf die Kontoseite für diesen Kunden zugreifen.</span><span class="sxs-lookup"><span data-stu-id="861cd-201">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="861cd-202">Mit dem Feature für die Reseller-Beziehungs Erweiterung Stimmen Sie der Freigabe der von Ihnen für diesen Kunden über den indirekten Anbieter vorhandenen Rechnung zu.</span><span class="sxs-lookup"><span data-stu-id="861cd-202">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="861cd-203">Ihr indirekter Anbieter wird nicht mit [Delegierten Administratorrechten](customers-revoke-admin-privileges.md) für den Kunden Mandanten bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="861cd-203">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="861cd-204">Wenn Ihr indirekter Anbieter Delegierte Administratorrechte erfordert, müssen Sie stattdessen eine indirekte Reseller-Einladung an den Kunden senden.</span><span class="sxs-lookup"><span data-stu-id="861cd-204">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="861cd-205">Sobald die Reseller-Beziehung eingerichtet ist, wird der indirekte Anbieter als CSP-Partner für den Kunden auf der Seite Partnerbeziehungen in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) und [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business)angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-205">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="861cd-206">Um Verwirrung und Missverständnisse zu vermeiden, werden Sie von Ihrem Partnervertrag vertraglich dazu verpflichtet, die Zustimmung des Kunden Vertrags zu übermitteln, bevor Sie mit dem Relationship-Erweiterungs Feature eine Reseller-Beziehung zwischen einem bestehenden Kunden der direkt Rechnung und einem indirekten Anbieter herstellen.</span><span class="sxs-lookup"><span data-stu-id="861cd-206">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="861cd-207">So verwenden Sie dieses Feature für einen vorhandenen Kunden Mandanten:</span><span class="sxs-lookup"><span data-stu-id="861cd-207">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="861cd-208">Melden Sie sich als **Administrator-Agent** beim Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="861cd-208">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="861cd-209">Wählen Sie auf der **Seite "Kunden**" einen vorhandenen Kunden aus, und klicken Sie auf das Symbol " **Quick Links** ", um die Zusammenfassungs Ansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="861cd-209">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="861cd-210">Klicken Sie unter **indirekte Anbieter** **auf Kunden an einem indirekten Anbieter übertragen**.</span><span class="sxs-lookup"><span data-stu-id="861cd-210">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Kunden an einen indirekten Anbieter übertragen":::

4. <span data-ttu-id="861cd-212">Wählen Sie im Popup Dialogfeld den **indirekten Anbieter** aus, dem die Wiederverkäufer Beziehung zum Kunden hinzugekommen sein soll.</span><span class="sxs-lookup"><span data-stu-id="861cd-212">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="861cd-213">Klicken Sie auf **Speichern und fortfahren**.</span><span class="sxs-lookup"><span data-stu-id="861cd-213">Click **Save and continue**.</span></span>

6. <span data-ttu-id="861cd-214">Überprüfen Sie, ob der ausgewählte indirekte Anbieter unter **indirekte Anbieter** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="861cd-214">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Indirekter Anbieter aufgelistet":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="861cd-216">Sendet eine indirekte Reseller-Einladung an den Kunden.</span><span class="sxs-lookup"><span data-stu-id="861cd-216">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="861cd-217">Ihr indirekter Anbieter kann keine Bestellungen für Ihre bestehenden Kunden der direkt Rechnung übermitteln, bis Sie über eine Reseller-Beziehung verfügen.</span><span class="sxs-lookup"><span data-stu-id="861cd-217">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="861cd-218">Um die Vertriebspartnerschaft zwischen Ihren Bestandskunden und Ihrem indirekten Anbieter aufzubauen, müssen die entsprechenden Kunden jeweils mithilfe einer Einladung für indirekte Wiederverkäufer eingeladen werden.</span><span class="sxs-lookup"><span data-stu-id="861cd-218">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="861cd-219">Wählen Sie in Partner Center im linken Navigationsbereich die Option **Indirekte Anbieter** aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-219">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="861cd-220">Wählen Sie **Neue Kunden einladen** aus, um einen Kunden zu einer Vertriebspartnerschaft mit Ihnen und dem indirekten Anbieter einzuladen.</span><span class="sxs-lookup"><span data-stu-id="861cd-220">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="861cd-221">Der Anbieter muss über eine Reseller-Beziehung mit Ihrem Kunden verfügen, damit er Bestellungen im Auftrag Ihres Kunden einreichen kann, wenn der Kunde neue Abonnements erwerben oder vorhandene Abonnements neue Lizenzen hinzufügen möchte.</span><span class="sxs-lookup"><span data-stu-id="861cd-221">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Neue Kunden einladen":::

3. <span data-ttu-id="861cd-223">Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="861cd-223">On the next page, review the draft email message.</span></span> <span data-ttu-id="861cd-224">Sie können den Nachrichtenentwurf in Ihrer E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen.</span><span class="sxs-lookup"><span data-stu-id="861cd-224">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="861cd-225">Bearbeiten Sie den Text in der e-Mail-Nachricht, um zu sagen, was Sie brauchen, aber achten Sie darauf, den Link so zu schließen, dass er den Kunden direkt mit Ihrem Konto und dem Konto Ihres Anbieters verbindet.</span><span class="sxs-lookup"><span data-stu-id="861cd-225">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="861cd-226">Wählen Sie dann **Fertig** aus.</span><span class="sxs-lookup"><span data-stu-id="861cd-226">Then select **Done**.</span></span>

5. <span data-ttu-id="861cd-227">Nachdem der Kunde dich und deinen Anbieter als Vertriebspartner autorisiert hat, verfügst du über die nötigen Administratorberechtigungen zur Verwaltung seiner Abonnements, Lizenzen und Benutzer, und dein indirekter Anbieter kann Aufträge im Namen des Kunden übermitteln.</span><span class="sxs-lookup"><span data-stu-id="861cd-227">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="861cd-228">Erweitere zum Verwalten des Kontos, des Diensts, der Benutzer und der Lizenzen des Kunden den Kundeneintrag, indem du neben seinem Namen auf den nach unten weisenden Pfeil klickst.</span><span class="sxs-lookup"><span data-stu-id="861cd-228">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="861cd-229">Zustimmung des Microsoft-Kunden Vertrags</span><span class="sxs-lookup"><span data-stu-id="861cd-229">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="861cd-230">Microsoft Cloud Vereinbarung ist bis zum 31. Januar 2020 gültig.</span><span class="sxs-lookup"><span data-stu-id="861cd-230">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="861cd-231">Nach diesem Datum müssen alle Kunden, vorhandene und neue, den neuen Microsoft- [Kundenvertrag](confirm-customer-agreement.md)signieren.</span><span class="sxs-lookup"><span data-stu-id="861cd-231">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="861cd-232">Für den Übergang von Kunden:</span><span class="sxs-lookup"><span data-stu-id="861cd-232">For transitioning customers, if:</span></span>

- <span data-ttu-id="861cd-233">**Der Kunde hat den Microsoft-Kundenvertrag noch nicht akzeptiert.**</span><span class="sxs-lookup"><span data-stu-id="861cd-233">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="861cd-234">Arbeiten Sie mit dem indirekten Anbieter zusammen, damit [der Kunde den Microsoft-Kundenvertrag akzeptiert](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="861cd-234">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="861cd-235">**Der Kunde hat den Microsoft-Kundenvertrag über das Microsoft 365 Admin Center akzeptiert.**</span><span class="sxs-lookup"><span data-stu-id="861cd-235">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="861cd-236">Die Annahme wird beibehalten, sobald die Reseller-Beziehung mit dem indirekten Anbieter hergestellt wird.</span><span class="sxs-lookup"><span data-stu-id="861cd-236">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="861cd-237">Es gibt nichts, was Sie tun müssen.</span><span class="sxs-lookup"><span data-stu-id="861cd-237">There is nothing you need to do.</span></span>

- <span data-ttu-id="861cd-238">**Der Kunde hat den Microsoft-Kundenvertrag über den Partner Nachweis akzeptiert.**</span><span class="sxs-lookup"><span data-stu-id="861cd-238">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="861cd-239">Die Annahme wird nicht beibehalten.</span><span class="sxs-lookup"><span data-stu-id="861cd-239">The acceptance will not be retained.</span></span> <span data-ttu-id="861cd-240">Arbeiten Sie mit dem indirekten Anbieter zusammen, um [die Zustimmung des Kunden in Partner Center zu aktualisieren](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="861cd-240">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="861cd-241">Vorhandene direkte Abrechnungs Abonnements an indirekten Anbieter übertragen</span><span class="sxs-lookup"><span data-stu-id="861cd-241">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="861cd-242">Beim indirekten CSP-Modell haben indirekte Reseller keine Abrechnungs Beziehungen mit Microsoft.</span><span class="sxs-lookup"><span data-stu-id="861cd-242">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="861cd-243">Stattdessen erhalten indirekte Vertriebspartner Abonnements für Ihre Kunden über ihre indirekten Anbieter.</span><span class="sxs-lookup"><span data-stu-id="861cd-243">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="861cd-244">Bei der Umstellung von Direct Bill Partner auf indirekte Reseller müssen Sie die vorhandenen Abonnements, die Sie als direkten Rechnungs Partner haben, an Ihren indirekten Anbieter übertragen.</span><span class="sxs-lookup"><span data-stu-id="861cd-244">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="861cd-245">Sie können das Feature für die Self-served-Abonnement Übertragung im Partner Center-Dashboard verwenden, um dies zu tun.</span><span class="sxs-lookup"><span data-stu-id="861cd-245">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="861cd-246">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="861cd-246">Pre-requisites</span></span>

- <span data-ttu-id="861cd-247">Diese Funktion steht nur für den Übergang von Partnern zur Verfügung, die die indirekte Registrierung des Wiederverkäufers mithilfe Ihrer vorhandenen direkt Rechnungs Partner Mandanten abgeschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-247">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="861cd-248">Vor der Übertragung von Abonnements, die einem bestimmten Kunden zugeordnet sind, muss der Übergangs Partner den Kunden zu einem indirekten Anbieter verschieben.</span><span class="sxs-lookup"><span data-stu-id="861cd-248">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="861cd-249">Der Kunde muss [den Microsoft-Kundenvertrag über den indirekten Anbieter akzeptiert](#microsoft-customer-agreement-acceptance)haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-249">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="861cd-250">Übergang zum indirekten Reseller-Status</span><span class="sxs-lookup"><span data-stu-id="861cd-250">How to transition to indirect reseller status</span></span>

<span data-ttu-id="861cd-251">Die Funktion ist ein 4-stufiger Prozess, bei dem Folgendes gilt:</span><span class="sxs-lookup"><span data-stu-id="861cd-251">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="861cd-252">Der Übergangs Partner erstellt eine Anforderung zum Übertragen von Abonnements.</span><span class="sxs-lookup"><span data-stu-id="861cd-252">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="861cd-253">Die Anforderung enthält mindestens ein vorhandenes Abonnement, das demselben Kunden zugeordnet ist und an einen indirekten Anbieter adressiert ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-253">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="861cd-254">Der indirekte Anbieter prüft die Übertragungs Anforderung und akzeptiert Sie (oder lehnt sie ab).</span><span class="sxs-lookup"><span data-stu-id="861cd-254">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="861cd-255">Der indirekte Anbieter überprüft, ob die Übertragungs Anforderung beendet ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-255">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="861cd-256">Der Übergangs Partner überprüft, ob die Übertragungs Anforderung beendet ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-256">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="861cd-257">Übergangs Partner</span><span class="sxs-lookup"><span data-stu-id="861cd-257">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="861cd-258">Sie können auch die [Partner Center-API/das SDK](/partner-center/develop/manage-customers) verwenden, um die vorhandenen Abonnements an Ihren indirekten Anbieter zu übertragen.</span><span class="sxs-lookup"><span data-stu-id="861cd-258">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="861cd-259">Abrufen der Berechtigung eines Kunden zum Übertragen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="861cd-259">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="861cd-260">Erstellen der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-260">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="861cd-261">Zurückziehen der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-261">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="861cd-262">Akzeptieren der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-262">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="861cd-263">Ablehnen der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-263">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="861cd-264">Abrufen der Übertragungen eines Kunden</span><span class="sxs-lookup"><span data-stu-id="861cd-264">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="861cd-265">Übertragungs Details nach ID erhalten</span><span class="sxs-lookup"><span data-stu-id="861cd-265">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="861cd-266">Übergang von Partner-Create Transfer Request</span><span class="sxs-lookup"><span data-stu-id="861cd-266">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="861cd-267">So erstellen Sie eine Übertragungs Anforderung als Übergangs Partner:</span><span class="sxs-lookup"><span data-stu-id="861cd-267">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="861cd-268">Melden Sie sich als **Administrator-Agent** beim Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="861cd-268">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="861cd-269">Wählen Sie auf der Seite **Customers** den gewünschten Kunden aus, und klicken Sie auf das Symbol Quick Links, um die Zusammenfassungs Ansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="861cd-269">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="861cd-270">Vergewissern Sie sich, dass unter **indirekte Anbieter** der gewünschte indirekte Anbieter aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-270">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="861cd-271">Klicken Sie auf **Abonnements anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="861cd-271">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="861cd-272">Suchen Sie auf der Seite **Abonnements** nach **Abonnement Übertragung**.</span><span class="sxs-lookup"><span data-stu-id="861cd-272">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="861cd-273">Klicken Sie unter **Abonnement Übertragung** auf **Abonnement Übertragung anfordern**.</span><span class="sxs-lookup"><span data-stu-id="861cd-273">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Übertragung von Abonnements anfordern":::

7. <span data-ttu-id="861cd-275">Wählen Sie im Dialogfeld "Übertragungs Anforderung" mindestens ein Abonnement aus, das übertragen werden soll.</span><span class="sxs-lookup"><span data-stu-id="861cd-275">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Übertragungs Anforderung erstellen":::

8. <span data-ttu-id="861cd-277">Klicken Sie auf **Erstellen**.</span><span class="sxs-lookup"><span data-stu-id="861cd-277">Click **Create**.</span></span>

9. <span data-ttu-id="861cd-278">Eine aktive Abonnement Übertragungs Anforderung wird unter **Abonnement Übertragung** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-278">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Liste der Übertragungsanforderungen":::

10. <span data-ttu-id="861cd-280">Informieren Sie Ihren indirekten Anbieter darüber, dass Sie eine Abonnement Übertragungs Anforderung für Sie erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="861cd-280">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="861cd-281">Indirekter Anbieter: Übertragungs Anforderung annehmen</span><span class="sxs-lookup"><span data-stu-id="861cd-281">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="861cd-282">So überprüfen und akzeptieren Sie eine Übertragungs Anforderung als indirekten Anbieter:</span><span class="sxs-lookup"><span data-stu-id="861cd-282">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="861cd-283">Melden Sie sich bei Partner Center als **Administrator** -Agent oder **Vertriebs-Agent** an.</span><span class="sxs-lookup"><span data-stu-id="861cd-283">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="861cd-284">Wählen Sie auf der Seite " **Kunden** " den gewünschten Kunden aus, und klicken Sie auf das Symbol "Quick Links", um die Zusammenfassungs Ansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="861cd-284">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="861cd-285">Vergewissern Sie sich unter **indirekte Händler**, dass der Übergangs Partner aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-285">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="861cd-286">Klicken Sie auf **Abonnements anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="861cd-286">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="861cd-287">Suchen Sie auf der Seite **Abonnements** nach **Abonnement Übertragung**.</span><span class="sxs-lookup"><span data-stu-id="861cd-287">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Übertragungs Anforderung anzeigen":::

6. <span data-ttu-id="861cd-289">Klicken Sie unter **Abonnement Übertragung** auf die zu überprüfende Übertragungs Anforderung.</span><span class="sxs-lookup"><span data-stu-id="861cd-289">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="861cd-290">Klicken Sie nach Bedarf auf **annehmen** (oder **ablehnen**).</span><span class="sxs-lookup"><span data-stu-id="861cd-290">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Übertragungs Anforderung akzeptieren":::

8. <span data-ttu-id="861cd-292">Warten Sie, bis die Übertragungs Anforderung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="861cd-292">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="861cd-293">Indirekte Anbieter-Überprüfen der Übertragungs Anforderung ist beendet</span><span class="sxs-lookup"><span data-stu-id="861cd-293">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="861cd-294">Nachdem die Übertragungs Anforderung erfolgreich abgeschlossen wurde, überprüfen Sie, ob die Abonnements unter **Abonnements** angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="861cd-294">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="861cd-295">Informieren Sie den Übergangs Partner.</span><span class="sxs-lookup"><span data-stu-id="861cd-295">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="861cd-296">Übergangs Partner-Überprüfen der Übertragungs Anforderung ist fertiggestellt.</span><span class="sxs-lookup"><span data-stu-id="861cd-296">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="861cd-297">Der Übergangs Partner sollte folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="861cd-297">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="861cd-298">Melden Sie sich bei Partner Center als **Administrator-Agent** oder Vertriebs- **Agent** an.</span><span class="sxs-lookup"><span data-stu-id="861cd-298">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="861cd-299">Wählen Sie auf der Seite **Customers** den gewünschten Kunden aus, und klicken Sie auf das Symbol **Quick Links** , um die Zusammenfassungs Ansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="861cd-299">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="861cd-300">Klicken Sie auf **Abonnements anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="861cd-300">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="861cd-301">Suchen Sie auf der Seite **Abonnements** nach **Abonnement Übertragung**.</span><span class="sxs-lookup"><span data-stu-id="861cd-301">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="861cd-302">Stellen Sie sicher, dass die Übertragungs Anforderung als " **Fertig**" gekennzeichnet ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-302">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="861cd-303">Überprüfen Sie, ob die Abonnements auf der Seite " **Abonnements** " nicht mehr als aktiv angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="861cd-303">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="861cd-304">Wenn es sich um ein Azure-Abonnement (MS-AZR-0145p) handelt, wird es nicht mehr aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="861cd-304">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="861cd-305">Wenn dies ein Lizenz basiertes Abonnement (Office 365, Dynamics, InTune) ist, wird es mit dem Status angehalten aufgeführt **.**</span><span class="sxs-lookup"><span data-stu-id="861cd-305">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Abonnement angehalten":::

### <a name="considerations"></a><span data-ttu-id="861cd-307">Überlegungen</span><span class="sxs-lookup"><span data-stu-id="861cd-307">Considerations</span></span>

- <span data-ttu-id="861cd-308">**Die Abonnement-ID wird nach der Übertragung anders sein.**</span><span class="sxs-lookup"><span data-stu-id="861cd-308">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="861cd-309">Wenn es sich um ein Azure-Abonnement (MS-AZR-0145p) handelt, wird zusätzlich eine Azure-Abonnement-ID verwendet, die vom vorherigen Besitzer aufbewahrt wird und im Azure-Verwaltungs Portal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="861cd-309">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="861cd-310">**Auf dasselbe Abonnement kann nicht von mehreren Übertragungsanforderungen verwiesen werden.**</span><span class="sxs-lookup"><span data-stu-id="861cd-310">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="861cd-311">Nachdem Sie eine Übertragungs Anforderung erstellt haben, die ein vorhandenes Abonnement enthält, können Sie keine zusätzlichen Übertragungsanforderungen einschließlich desselben Abonnements erstellen, bis die erste Übertragungs Anforderung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="861cd-311">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="861cd-312">**Add-ons für Lizenz basierte Abonnements müssen zusammen mit dem Basis Abonnement übertragen werden.**</span><span class="sxs-lookup"><span data-stu-id="861cd-312">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="861cd-313">Wenn Sie beim Erstellen einer Übertragungs Anforderung ein vorhandenes Abonnement mit einem oder mehreren Add-ons auswählen, werden die Add-ons automatisch in die Übertragungs Anforderung eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="861cd-313">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="861cd-314">**Die Lizenz Anzahl Änderungen an einem Abonnement werden in der vorhandenen Übertragungs Anforderung nicht widergespiegelt.**</span><span class="sxs-lookup"><span data-stu-id="861cd-314">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="861cd-315">Nachdem Sie eine Übertragungs Anforderung erstellt haben, die ein vorhandenes Abonnement enthält, sollten Sie die Lizenz Menge des Abonnements (oder der zugehörigen Addons) nicht mehr aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="861cd-315">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="861cd-316">Wenn Sie dies tun, wird die neue Menge in der Übertragungs Anforderung nicht berücksichtigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-316">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="861cd-317">Nachdem der indirekte Anbieter die Übertragungs Anforderung akzeptiert hat, weist das resultierende Abonnement die alte Menge auf.</span><span class="sxs-lookup"><span data-stu-id="861cd-317">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="861cd-318">Wenn Sie möchten, dass die neue Menge an den indirekten Anbieter übertragen wird, müssen Sie die vorhandene Übertragungs Anforderung abbrechen und eine neue erstellen.</span><span class="sxs-lookup"><span data-stu-id="861cd-318">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="861cd-319">**Nicht alle Käufe können mithilfe der Self-served-Abonnement Übertragung übertragen werden.**</span><span class="sxs-lookup"><span data-stu-id="861cd-319">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="861cd-320">Derzeit können Sie mit diesem Feature nur O365-Abonnements und Azure PAYG-Abonnements (MS-AZR-0145p) übertragen.</span><span class="sxs-lookup"><span data-stu-id="861cd-320">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="861cd-321">Weitere Käufe einschließlich Azure-Pläne, reservierte Azure-Instanzen, Begriffs basierte Abonnements und Saas-Abonnements für Azure Marketplace werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="861cd-321">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="861cd-322">Der Grund für das übertragen eines Abonnements auf der Seite "Übertragungs Anforderung senden" wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="861cd-322">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="861cd-323">Um diese Abonnements zu übertragen, müssen Sie [das vorhandene Abonnement Abbrechen](create-a-new-subscription.md#suspend-or-cancel-a-subscription) und ein neues Angebot für Kunden über den indirekten Anbieter erwerben.</span><span class="sxs-lookup"><span data-stu-id="861cd-323">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="861cd-324">**Kann nicht über die Sandbox Umgebung getestet werden.**</span><span class="sxs-lookup"><span data-stu-id="861cd-324">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="861cd-325">Registrieren für Incentives für indirekte Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="861cd-325">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="861cd-326">Nachdem Sie sich unter Ihrem vorhandenen Direktabrechnungspartner-Mandanten erfolgreich als indirekter Wiederverkäufer registriert haben, erhalten Sie innerhalb von 30 Tagen eine Einladung zur Registrierung für Incentives für indirekte Wiederverkäufer.</span><span class="sxs-lookup"><span data-stu-id="861cd-326">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="861cd-327">Die Einladung basiert auf dem MPN-Partnerkonto, das aktuell Ihrem CSP-Partnermandanten zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="861cd-327">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="861cd-328">Die Einladung wird an die dem MPN-Partnerkonto zugeordnete E-Mail-Adresse gesendet.</span><span class="sxs-lookup"><span data-stu-id="861cd-328">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="861cd-329">Mit dem gleichen Partnermandanten können Sie sich auch für Incentive-Programme für die Direktabrechnung registrieren.</span><span class="sxs-lookup"><span data-stu-id="861cd-329">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="861cd-330">Die Programme müssen separat verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="861cd-330">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="861cd-331">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="861cd-331">Next steps</span></span>

- [<span data-ttu-id="861cd-332">Weitere Informationen zu den Anforderungen an indirekte Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="861cd-332">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="861cd-333">Neue Anforderungen für direkte CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="861cd-333">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="861cd-334">Eingeschränkte Direktabrechnungsfunktionen</span><span class="sxs-lookup"><span data-stu-id="861cd-334">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
