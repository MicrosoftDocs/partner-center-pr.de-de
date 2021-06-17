---
title: Umstellen des Direktabrechnungspartners auf einen indirekten Vertriebspartner
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie ein CSP-Programmpartner Partner Center verwenden kann, um vom Direktabrechnungspartner zum indirekten Handelspartner zu wechseln.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57c4a5d0a02079e887b38fa9754d276062d20cc
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276415"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="203f6-103">Übergang vom CSP-Direktabrechnungspartner (Cloud Solution Provider) zum indirekten CSP-Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="203f6-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="203f6-104">**Geeignete Rollen**: Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="203f6-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="203f6-105">Dieser Artikel richtet sich an Direktabrechnungspartner, die indirekte Wiederverkäufer werden möchten.</span><span class="sxs-lookup"><span data-stu-id="203f6-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="203f6-106">Selbst wenn Sie noch keine explizite Entscheidung getroffen haben, sich als indirekter Vertriebspartner zu registrieren, werden Direktabrechnungspartner, die die neuen [Anforderungen](direct-partner-new-requirements.md) für das CSP Direct Bill Partner-Programm nicht erfüllen, von Microsoft darüber informiert, wenn ihre [Funktionen für direkte Rechnungen eingeschränkt werden.](restricted-direct-bill-capabilities.md)</span><span class="sxs-lookup"><span data-stu-id="203f6-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="203f6-107">Ab Januar 2021 wird eine neue Umsatzanforderung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="203f6-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="203f6-108">Partner, die als Partner mit direkter Abrechnung registriert sind, müssen in den letzten 12 Monaten mindestens 300.000 USD an Cloud Solution Provider Programmumsatz auf ebene eines globalen Partnerkontos abgewickelt haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="203f6-109">Sie können sich unter Verwendung Ihres vorhandenen Direktabrechnungsmandanten beim Programm für indirekte Wiederverkäufer registrieren.</span><span class="sxs-lookup"><span data-stu-id="203f6-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="203f6-110">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="203f6-110">Get started</span></span>

1. <span data-ttu-id="203f6-111">Vergewissern Sie sich, dass Ihr Partnerprofil in Partner Center und Ihre MPN-ID aktuell sind.</span><span class="sxs-lookup"><span data-stu-id="203f6-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="203f6-112">Melden Sie sich bei Partner Center als globaler Administrator für den Direktabrechnungsmandanten an, den Sie auf einen indirekten Wiederverkäufer umstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="203f6-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Übersicht.":::

3. <span data-ttu-id="203f6-114">Überprüfen Sie Ihre Partnerdetails im Registrierungsformular.</span><span class="sxs-lookup"><span data-stu-id="203f6-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Registrieren Sie sich jetzt.":::

4. <span data-ttu-id="203f6-116">Wählen Sie „Jetzt registrieren“ aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-116">Select Enroll now.</span></span> <span data-ttu-id="203f6-117">Für Ihre Tätigkeit als indirekter Wiederverkäufer wird der gleiche AAD-Mandant verwendet wie für Ihre direkte Tätigkeit.</span><span class="sxs-lookup"><span data-stu-id="203f6-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="203f6-118">Diese neue Übergangsfunktion steht anfänglich nur für Partner mit Onboarding-Jahrestagen zwischen September und Dezember zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="203f6-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="203f6-119">Wenn Ihr Jahrestag nicht zwischen September und Dezember liegt, wird die Funktion momentan nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="203f6-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="203f6-120">Partner mit Jahrestagen nach Dezember 2018 werden benachrichtigt, sobald die Funktion für sie aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="203f6-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="203f6-121">Melden Sie sich nach der Genehmigung Ihrer Registrierung erneut bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="203f6-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="203f6-122">Die Genehmigung erfolgt in der Regel sofort, kann aber bis zu fünf Werktage dauern.</span><span class="sxs-lookup"><span data-stu-id="203f6-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="203f6-123">Nach der Genehmigung wird eine entsprechende Benachrichtigung an die E-Mail-Adresse gesendet, die Sie im Registrierungsformular als primären Kontakt angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="203f6-124">Sie können Ihren Registrierungsstatus auch unter **Einstellungen**  >  **Kontoeinstellungen**  >  **Partnerprofil** > Programminformationen überprüfen.</span><span class="sxs-lookup"><span data-stu-id="203f6-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="203f6-125">Auf der Seite **Übersicht** wird die Vereinbarung für indirekte Wiederverkäufer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="203f6-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="203f6-126">Wählen Sie **Zustimmen und fortfahren** aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-126">Select **Accept and continue**.</span></span> <span data-ttu-id="203f6-127">Diese Aktion ermöglicht die Funktionen indirekter Vertriebspartner.</span><span class="sxs-lookup"><span data-stu-id="203f6-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="203f6-128">Wenn Sie die Vereinbarung für indirekte Wiederverkäufer akzeptiert haben, weist Sie Ihr Partnerprofil als Direktabrechnungspartner **und** als indirekter Wiederverkäufer aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Indirekter Handelspartnervertrag.":::

> [!IMPORTANT]
> <span data-ttu-id="203f6-130">Nachdem Sie sich mit der neuen Funktion als indirekter Wiederverkäufer registriert haben, steht keine Option für ein Rollback zu einem reinen Direktabrechnungsmandanten zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="203f6-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="203f6-131">Registrieren Sie sich daher erst nach sorgfältiger Prüfung Ihrer geschäftlichen Anforderungen als indirekter Wiederverkäufer.</span><span class="sxs-lookup"><span data-stu-id="203f6-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="203f6-132">Übergangsphase vom Direktabrechnungspartner zum indirekten Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="203f6-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="203f6-133">Während dieser Phase verwalten Sie weiterhin die Abonnementanforderungen Ihrer direkten Kunden, einschließlich des Abrechnungsprozesses.</span><span class="sxs-lookup"><span data-stu-id="203f6-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="203f6-134">Außerdem beginnen Sie damit, Kunden von Ihrem indirekten Anbieter zu akzeptieren und als indirekter Wiederverkäufer zu agieren.</span><span class="sxs-lookup"><span data-stu-id="203f6-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Sie sind sowohl direkt abgerechnet als auch indirekter Vertriebspartner.":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="203f6-136">Suchen eines indirekten Anbieters</span><span class="sxs-lookup"><span data-stu-id="203f6-136">Find an indirect provider</span></span>

<span data-ttu-id="203f6-137">Nach der Registrierung wird in Ihrem linken Navigationsbereich ein Link zu indirekten Anbietern angezeigt.</span><span class="sxs-lookup"><span data-stu-id="203f6-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="203f6-138">Als indirekter Wiederverkäufer bauen Sie eine Beziehung zu einem indirekten Anbieter auf, der sich dann um Ihre Abrechnung, um den Produkteinkauf für Ihre Kunden sowie um die Supportinfrastruktur kümmern kann.</span><span class="sxs-lookup"><span data-stu-id="203f6-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="203f6-139">Verschiedene indirekte Anbieter bieten unterschiedliche Unterstützung und Leistungen. Ermitteln Sie daher die Anbieter in Ihrer Umgebung, die Ihre Anforderungen am besten erfüllen.</span><span class="sxs-lookup"><span data-stu-id="203f6-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="203f6-140">Die meisten Anbieter bieten Folgendes:</span><span class="sxs-lookup"><span data-stu-id="203f6-140">Generally, most providers will:</span></span>

- <span data-ttu-id="203f6-141">Technische Schulung und Unterstützung</span><span class="sxs-lookup"><span data-stu-id="203f6-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="203f6-142">Hilfe bei der Vermarktung Ihrer Produkte und Dienste</span><span class="sxs-lookup"><span data-stu-id="203f6-142">Help you market your products and services</span></span>
- <span data-ttu-id="203f6-143">Verwaltung Ihrer Finanzierung und Kreditbedingungen</span><span class="sxs-lookup"><span data-stu-id="203f6-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="203f6-144">Die Liste mit offiziellen indirekten Microsoft-Anbietern finden Sie [hier](https://partnercenter.microsoft.com/partner/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="203f6-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="203f6-145">Weitere Informationen finden Sie unter [Arbeiten mit indirekten Anbietern im Programm für Cloud-Lösungsanbieter](indirect-reseller-tasks-in-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="203f6-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="203f6-146">Annehmen einer Partnerschaftseinladung von Ihrem indirekten Anbieter</span><span class="sxs-lookup"><span data-stu-id="203f6-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="203f6-147">Wenn Sie einen passenden indirekte Anbieter gefunden haben, gehen Sie mit ihm in Partner Center eine Partnerschaft ein.</span><span class="sxs-lookup"><span data-stu-id="203f6-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="203f6-148">Der von Ihnen ausgewählte indirekte Anbieter sendet Ihnen eine E-Mail mit einem Einladungslink für eine Partnerschaft, über den Sie zur entsprechenden Einladung in Partner Center gelangen.</span><span class="sxs-lookup"><span data-stu-id="203f6-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="203f6-149">Stellen Sie sicher, dass sich Ihr globaler Administrator bei Partner Center anmeldet und dem Einladungslink folgt.</span><span class="sxs-lookup"><span data-stu-id="203f6-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="203f6-150">Wenn Sie die Einladung annehmen, wird der Name des Anbieters in der Liste Ihrer indirekten Anbieter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="203f6-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="203f6-151">Gewinnen neuer Kunden als indirekter Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="203f6-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="203f6-152">Sowohl Sie selbst als auch Ihr indirekter Anbieter müssen über Vertriebspartnerschaften mit Kunden verfügen.</span><span class="sxs-lookup"><span data-stu-id="203f6-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="203f6-153">Diese Handelspartnerbeziehungen ermöglichen es Ihnen, die Abonnements und Dienste eines Kunden in dessen Namen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="203f6-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="203f6-154">Um einen neuen Kunden zu gewinnen, der bereits über einen Azure AD-Mandanten verfügt, können Sie den Kunden gleichzeitig zu einer Vertriebspartnerschaft mit Ihnen und Ihrem Anbieter einladen.</span><span class="sxs-lookup"><span data-stu-id="203f6-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="203f6-155">So erstellen Sie eine Einladung als indirekter Wiederverkäufer:</span><span class="sxs-lookup"><span data-stu-id="203f6-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="203f6-156">Wählen Sie in Partner Center im linken Navigationsbereich die Option **Indirekte Anbieter** aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="203f6-157">Wählen Sie **Neue Kunden einladen** aus, um einen Kunden zu einer Vertriebspartnerschaft mit Ihnen und dem indirekten Anbieter einzuladen.</span><span class="sxs-lookup"><span data-stu-id="203f6-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="203f6-158">Der Anbieter muss eine Vertriebspartnerschaft mit Ihrem Kunden haben, damit er Bestellungen im Namen Ihres Kunden übermitteln kann, wenn der Kunde neue Abonnements kaufen oder vorhandenen Abonnements neue Lizenzen hinzufügen möchte.</span><span class="sxs-lookup"><span data-stu-id="203f6-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="203f6-159">Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="203f6-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="203f6-160">Sie können den Nachrichtenentwurf in Ihrer E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen.</span><span class="sxs-lookup"><span data-stu-id="203f6-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="203f6-161">Bearbeiten Sie den Text in der E-Mail, um zu sagen, was Sie benötigen. Stellen Sie jedoch sicher, dass Sie den Link einschließen, da er personalisiert ist, um den Kunden direkt mit Ihrem Konto und dem Konto Ihres Anbieters zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="203f6-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="203f6-162">Wählen Sie dann **Fertig** aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-162">Then select **Done**.</span></span>

5. <span data-ttu-id="203f6-163">Nachdem der Kunde dich und deinen Anbieter als Vertriebspartner autorisiert hat, verfügst du über die nötigen Administratorberechtigungen zur Verwaltung seiner Abonnements, Lizenzen und Benutzer, und dein indirekter Anbieter kann Aufträge im Namen des Kunden übermitteln.</span><span class="sxs-lookup"><span data-stu-id="203f6-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="203f6-164">Erweitere zum Verwalten des Kontos, des Diensts, der Benutzer und der Lizenzen des Kunden den Kundeneintrag, indem du neben seinem Namen auf den nach unten weisenden Pfeil klickst.</span><span class="sxs-lookup"><span data-stu-id="203f6-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="203f6-165">Im Gegensatz zu Direktabrechnungspartnern können indirekte Vertriebspartner keine Azure AD Mandanten für ihre neuen Kunden in Partner Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="203f6-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="203f6-166">Ihr Anbieter erstellt den Mandanten und gibt Sie als den indirekten Wiederverkäufer für diesen Kunden an.</span><span class="sxs-lookup"><span data-stu-id="203f6-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="203f6-167">Dadurch wird sichergestellt, dass der Kunde in Partner Center in Ihrer Kundenliste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="203f6-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="203f6-168">Sie können nicht Ihre Direktabrechnungsfunktion verwenden, um Käufe für Kunden zu erstellen, die Sie als indirekter Wiederverkäufer gewinnen.</span><span class="sxs-lookup"><span data-stu-id="203f6-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="203f6-169">Verwalten Ihrer Direktabrechnungskunden und Ihrer Kunden für den indirekten Wiederverkauf</span><span class="sxs-lookup"><span data-stu-id="203f6-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="203f6-170">Direktabrechnungskunden und Kunden für den indirekten Wiederverkauf werden unterschiedlich verwaltet.</span><span class="sxs-lookup"><span data-stu-id="203f6-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="203f6-171">Direktabrechnungskunden (Dinge, die Sie nicht als indirekter Vertriebspartner erledigen)</span><span class="sxs-lookup"><span data-stu-id="203f6-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="203f6-172">Erstellen von Bestellungen für Produkte</span><span class="sxs-lookup"><span data-stu-id="203f6-172">Create orders for products</span></span>
- <span data-ttu-id="203f6-173">Verwalten von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="203f6-173">Manage Azure reservations</span></span>
- <span data-ttu-id="203f6-174">Verwalten des Bestellverlaufs</span><span class="sxs-lookup"><span data-stu-id="203f6-174">Manage their order history</span></span>
- <span data-ttu-id="203f6-175">Kaufen von Software</span><span class="sxs-lookup"><span data-stu-id="203f6-175">Purchase software</span></span>
- <span data-ttu-id="203f6-176">Direktes Abrechnen mit Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="203f6-177">Kunden indirekter Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="203f6-177">Indirect reseller customers</span></span>

- <span data-ttu-id="203f6-178">Indirekter Anbieter bestellt Produkte für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="203f6-179">Verwalten der Lizenzen und Benutzer von Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="203f6-180">Abwickeln von Abonnementverlängerungen</span><span class="sxs-lookup"><span data-stu-id="203f6-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="203f6-181">So erkennen Sie Kunden, die Sie als Direktabrechnungspartner gewonnen haben:</span><span class="sxs-lookup"><span data-stu-id="203f6-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="203f6-182">Wählen Sie **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-182">Select **Customers**.</span></span>

2. <span data-ttu-id="203f6-183">Wählen Sie einen Kunden aus, um seine Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="203f6-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="203f6-184">Wenn Sie diesen Kunden als Direktabrechnungspartner gewonnen haben, werden Optionen zum **Hinzufügen** oder **Anzeigen von Produkten** sowie die Abonnements des Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="203f6-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="203f6-185">Wenn zwischen Ihnen und dem Kunden eine indirekte Vertriebspartnerschaft besteht, sind diese Optionen nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="203f6-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="203f6-186">Migrieren Ihrer Direktabrechnungskunden zu Ihrem indirekten Anbieter</span><span class="sxs-lookup"><span data-stu-id="203f6-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="203f6-187">Ihr indirekter Anbieter kann keine Bestellungen oder vorhandene Abonnementübertragungen für Ihre vorhandenen Kunden mit direkter Abrechnung übermitteln, bis sie über eine Vertriebspartnerschaft mit ihnen verfügen.</span><span class="sxs-lookup"><span data-stu-id="203f6-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="203f6-188">Um die Vertriebspartnerschaft zwischen Ihrem indirekten Anbieter und Ihrem vorhandenen Kunden mit direkter Rechnung herzustellen, können Sie eine der folgenden Methoden verwenden:</span><span class="sxs-lookup"><span data-stu-id="203f6-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="203f6-189">Handelspartnerbeziehungserweiterung</span><span class="sxs-lookup"><span data-stu-id="203f6-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="203f6-190">Senden einer Einladung eines indirekten Handelspartners an den Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="203f6-191">Eine ausführliche Übersicht über den schrittweisen Prozess finden Sie im [Dokument Direkt zu indirektem Übergang.](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="203f6-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="203f6-192">Handelspartnerbeziehungserweiterung</span><span class="sxs-lookup"><span data-stu-id="203f6-192">Reseller relationship extension</span></span>

<span data-ttu-id="203f6-193">Sie können das Feature für die Resellerbeziehungserweiterung verwenden, um mithilfe Partner Center Dashboards eine Vertriebspartnerschaft zwischen Ihren vorhandenen Direktabrechnungskunden und Ihrem indirekten Anbieter herzustellen.</span><span class="sxs-lookup"><span data-stu-id="203f6-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="203f6-194">Beachten Sie vor der Verwendung des Features Folgendes:</span><span class="sxs-lookup"><span data-stu-id="203f6-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="203f6-195">Dieses Feature ist nur für Direktabrechnungspartner verfügbar, die in einen indirekten Vertriebspartner übergehen und die Registrierung für [indirekte Vertriebspartner](#get-started)abgeschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="203f6-196">Sie können dieses Feature nur auf bestehende Direktabrechnungskunden anwenden.</span><span class="sxs-lookup"><span data-stu-id="203f6-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="203f6-197">Sie gilt nicht für [Kunden indirekter Vertriebspartner.](#acquire-new-customers-as-indirect-reseller)</span><span class="sxs-lookup"><span data-stu-id="203f6-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="203f6-198">Sie können nur einen indirekten Anbieter auswählen, für den Sie [eine Partner-Einladung von Ihrem indirekten Anbieter akzeptiert](#accept-a-partnership-invitation-from-your-indirect-provider)haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="203f6-199">Eine Kopie der Rechnungsinformationen, die Sie für diesen Kunden haben, wird dem indirekten Anbieter zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="203f6-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="203f6-200">Sie können auf die Rechnungsinformationen zugreifen, indem Sie in Partner Center Dashboard auf die Seite Konto für diesen Kunden zugreifen.</span><span class="sxs-lookup"><span data-stu-id="203f6-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="203f6-201">Mithilfe des Vertriebspartnerbeziehungserweiterungsfeatures erklären Sie sich damit einverstanden, die Rechnungsinformationen, die Sie für diesen Kunden haben, an den indirekten Anbieter weiterzugeben.</span><span class="sxs-lookup"><span data-stu-id="203f6-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="203f6-202">Ihrem indirekten Anbieter werden keine delegierten Administratorrechte für den [Kundenmandanten](customers-revoke-admin-privileges.md) zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="203f6-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="203f6-203">Wenn Ihr indirekter Anbieter delegierte Administratorrechte erfordert, müssen Sie stattdessen eine Einladung für indirekte Vertriebspartner an den Kunden senden.</span><span class="sxs-lookup"><span data-stu-id="203f6-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="203f6-204">Sobald die Handelspartnerbeziehung eingerichtet wurde, wird der indirekte Anbieter dem Kunden auf der Seite Partnerbeziehungen im [Admin Center Microsoft 365 als](https://admin.microsoft.com/AdminPortal/Home#/partners) CSP-Partner angezeigt und [Microsoft Store für Unternehmen](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="203f6-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="203f6-205">Um Verwechslungen und Verwechslungen zu vermeiden, sind Sie durch Ihre Partnervereinbarung vertraglich verpflichtet, den Kunden der direkten Rechnung zu informieren und seine Zustimmung einzuholen, bevor Sie das Feature für die Beziehungserweiterung verwenden, um eine Vertriebspartnerschaft zwischen einem vorhandenen Direktabrechnungskunden und einem indirekten Anbieter herzustellen.</span><span class="sxs-lookup"><span data-stu-id="203f6-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="203f6-206">So verwenden Sie dieses Feature für einen vorhandenen Kundenmandanten:</span><span class="sxs-lookup"><span data-stu-id="203f6-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="203f6-207">Melden Sie sich bei Partner Center als **Administrator-Agent an.**</span><span class="sxs-lookup"><span data-stu-id="203f6-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="203f6-208">Wählen Sie auf der **Seite Kunden** einen vorhandenen Kunden aus, und klicken Sie auf das Symbol **Quicklinks,** um die Zusammenfassungsansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="203f6-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="203f6-209">Klicken Sie unter **Indirekte Anbieter** auf Kunde auf **einen indirekten Anbieter übertragen.**</span><span class="sxs-lookup"><span data-stu-id="203f6-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Übertragen sie den Kunden an einen indirekten Anbieter.":::

4. <span data-ttu-id="203f6-211">Wählen Sie im Popupdialogfeld den **indirekten Anbieter** aus, für den Sie eine Handelspartnerbeziehung mit dem Kunden einrichten möchten.</span><span class="sxs-lookup"><span data-stu-id="203f6-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="203f6-212">Klicken Sie auf **Speichern und fortfahren**.</span><span class="sxs-lookup"><span data-stu-id="203f6-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="203f6-213">Überprüfen Sie, ob der ausgewählte indirekte Anbieter unter **Indirekte Anbieter** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="203f6-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Indirekter Anbieter aufgeführt.":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="203f6-215">Senden einer Einladung eines indirekten Handelspartners an den Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="203f6-216">Ihr indirekter Anbieter kann keine Bestellungen für Ihre vorhandenen Kunden mit direkter Abrechnung übermitteln, bis sie über eine Vertriebspartnerschaft mit ihnen verfügen.</span><span class="sxs-lookup"><span data-stu-id="203f6-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="203f6-217">Um die Vertriebspartnerschaft zwischen Ihren Bestandskunden und Ihrem indirekten Anbieter aufzubauen, müssen die entsprechenden Kunden jeweils mithilfe einer Einladung für indirekte Wiederverkäufer eingeladen werden.</span><span class="sxs-lookup"><span data-stu-id="203f6-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="203f6-218">Wählen Sie in Partner Center im linken Navigationsbereich die Option **Indirekte Anbieter** aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="203f6-219">Wählen Sie **Neue Kunden einladen** aus, um einen Kunden zu einer Vertriebspartnerschaft mit Ihnen und dem indirekten Anbieter einzuladen.</span><span class="sxs-lookup"><span data-stu-id="203f6-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="203f6-220">Der Anbieter muss über eine Vertriebspartnerschaft mit Ihrem Kunden verfügen, damit er Bestellungen im Namen Ihres Kunden übermitteln kann, wenn der Kunde neue Abonnements kaufen oder vorhandenen Abonnements neue Lizenzen hinzufügen möchte.</span><span class="sxs-lookup"><span data-stu-id="203f6-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Laden Sie neue Kunden ein.":::

3. <span data-ttu-id="203f6-222">Überprüfen Sie auf der nächsten Seite den Entwurf der E-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="203f6-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="203f6-223">Sie können den Nachrichtenentwurf in Ihrer E-Mail-Anwendung öffnen oder die Nachricht in die Zwischenablage kopieren und in eine E-Mail einfügen.</span><span class="sxs-lookup"><span data-stu-id="203f6-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="203f6-224">Bearbeiten Sie den Text in der E-Mail, um zu sagen, was Sie benötigen. Stellen Sie jedoch sicher, dass Sie den Link einschließen, da er personalisiert ist, um den Kunden direkt mit Ihrem Konto und dem Konto Ihres Anbieters zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="203f6-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="203f6-225">Wählen Sie dann **Fertig** aus.</span><span class="sxs-lookup"><span data-stu-id="203f6-225">Then select **Done**.</span></span>

5. <span data-ttu-id="203f6-226">Nachdem der Kunde dich und deinen Anbieter als Vertriebspartner autorisiert hat, verfügst du über die nötigen Administratorberechtigungen zur Verwaltung seiner Abonnements, Lizenzen und Benutzer, und dein indirekter Anbieter kann Aufträge im Namen des Kunden übermitteln.</span><span class="sxs-lookup"><span data-stu-id="203f6-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="203f6-227">Erweitere zum Verwalten des Kontos, des Diensts, der Benutzer und der Lizenzen des Kunden den Kundeneintrag, indem du neben seinem Namen auf den nach unten weisenden Pfeil klickst.</span><span class="sxs-lookup"><span data-stu-id="203f6-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="203f6-228">Microsoft-Kundenvereinbarung Zustimmung</span><span class="sxs-lookup"><span data-stu-id="203f6-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="203f6-229">Microsoft Cloud-Vertrag ist bis zum 31. Januar 2020 gültig.</span><span class="sxs-lookup"><span data-stu-id="203f6-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="203f6-230">Nach diesem Datum müssen alle Vorhandenen und neuen Kunden die neue [Microsoft-Kundenvereinbarung](confirm-customer-agreement.md)signieren.</span><span class="sxs-lookup"><span data-stu-id="203f6-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="203f6-231">Für kundenübergehende Kunden, wenn:</span><span class="sxs-lookup"><span data-stu-id="203f6-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="203f6-232">**Kunde hat Microsoft-Kundenvereinbarung noch nicht akzeptiert**</span><span class="sxs-lookup"><span data-stu-id="203f6-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="203f6-233">Wenden Sie sich an den indirekten Anbieter, damit der Kunde [die Microsoft-Kundenvereinbarung akzeptiert.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="203f6-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="203f6-234">**Der Kunde hat Microsoft-Kundenvereinbarung mit Ihnen über das Microsoft 365 Admin Center akzeptiert.**</span><span class="sxs-lookup"><span data-stu-id="203f6-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="203f6-235">Die Zustimmung wird beibehalten, sobald die Vertriebspartnerschaft mit dem indirekten Anbieter hergestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="203f6-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="203f6-236">Sie müssen nichts tun.</span><span class="sxs-lookup"><span data-stu-id="203f6-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="203f6-237">**Der Kunde hat Microsoft-Kundenvereinbarung mit Ihnen über den Partnernachweis akzeptiert.**</span><span class="sxs-lookup"><span data-stu-id="203f6-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="203f6-238">Die Zustimmung wird nicht beibehalten.</span><span class="sxs-lookup"><span data-stu-id="203f6-238">The acceptance will not be retained.</span></span> <span data-ttu-id="203f6-239">Wenden Sie sich an den indirekten Anbieter, um die Zustimmung des Kunden in Partner Center zu [aktualisieren.](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)</span><span class="sxs-lookup"><span data-stu-id="203f6-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="203f6-240">Übertragen vorhandener Direktabrechnungsabonnements an indirekte Anbieter</span><span class="sxs-lookup"><span data-stu-id="203f6-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="203f6-241">Beim indirekten CSP-Modell verfügen indirekte Vertriebspartner nicht über Abrechnungsbeziehungen mit Microsoft.</span><span class="sxs-lookup"><span data-stu-id="203f6-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="203f6-242">Stattdessen erhalten indirekte Vertriebspartner Abonnements für ihre Kunden über ihre indirekten Anbieter.</span><span class="sxs-lookup"><span data-stu-id="203f6-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="203f6-243">Beim Übergang vom Direktabrechnungspartner zum indirekten Vertriebspartner müssen Sie die vorhandenen Abonnements, über die Sie als Partner für direkte Rechnungen verfügen, an Ihren indirekten Anbieter übertragen.</span><span class="sxs-lookup"><span data-stu-id="203f6-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="203f6-244">Hierzu können Sie das Feature für die self-served-Abonnementübertragung in Partner Center Dashboard verwenden.</span><span class="sxs-lookup"><span data-stu-id="203f6-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="203f6-245">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="203f6-245">Prerequisites</span></span>

- <span data-ttu-id="203f6-246">Dieses Feature ist nur für umgestellte Partner verfügbar, die die Registrierung indirekter Vertriebspartner mithilfe ihrer vorhandenen Partnermandanten mit direkter Abrechnung abgeschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="203f6-247">Vor der Übertragung von Abonnements, die einem bestimmten Kunden zugeordnet sind, muss der übergehende Partner den Kunden zu einem indirekten Anbieter verschieben.</span><span class="sxs-lookup"><span data-stu-id="203f6-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="203f6-248">Der Kunde muss [Microsoft-Kundenvereinbarung über den indirekten Anbieter akzeptiert](#microsoft-customer-agreement-acceptance)haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="203f6-249">Umstieg auf den Status "Indirekter Handelspartner"</span><span class="sxs-lookup"><span data-stu-id="203f6-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="203f6-250">Das Feature ist ein vierstufiger Prozess, bei dem Folgendes gilt:</span><span class="sxs-lookup"><span data-stu-id="203f6-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="203f6-251">Der übergehende Partner erstellt eine Abonnementübertragungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="203f6-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="203f6-252">Die Anforderung enthält mindestens ein vorhandenes Abonnement, das demselben Kunden zugeordnet ist, und wird an einen indirekten Anbieter adressiert.</span><span class="sxs-lookup"><span data-stu-id="203f6-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="203f6-253">Der indirekte Anbieter überprüft die Übertragungsanforderung und akzeptiert sie (oder lehnt sie ab).</span><span class="sxs-lookup"><span data-stu-id="203f6-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="203f6-254">Der indirekte Anbieter überprüft, ob die Übertragungsanforderung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="203f6-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="203f6-255">Der übergangende Partner überprüft, ob die Übertragungsanforderung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="203f6-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="203f6-256">Übergangspartner</span><span class="sxs-lookup"><span data-stu-id="203f6-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="203f6-257">Sie können auch [Partner Center API/SDK](/partner-center/develop/manage-customers) verwenden, um die vorhandenen Abonnements an Ihren indirekten Anbieter zu übertragen.</span><span class="sxs-lookup"><span data-stu-id="203f6-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="203f6-258">Abrufen der Berechtigung eines Kunden zum Übertragen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="203f6-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="203f6-259">Erstellen der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="203f6-260">Zurückziehen der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="203f6-261">Akzeptieren der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="203f6-262">Ablehnen der Übertragung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="203f6-263">Abrufen der Übertragungen eines Kunden</span><span class="sxs-lookup"><span data-stu-id="203f6-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="203f6-264">Abrufen von Übertragungsdetails nach ID</span><span class="sxs-lookup"><span data-stu-id="203f6-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="203f6-265">Übergangspartner : Erstellen einer Übertragungsanforderung</span><span class="sxs-lookup"><span data-stu-id="203f6-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="203f6-266">So erstellen Sie eine Übertragungsanforderung als Übergangspartner:</span><span class="sxs-lookup"><span data-stu-id="203f6-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="203f6-267">Melden Sie sich bei Partner Center als **Administrator-Agent an.**</span><span class="sxs-lookup"><span data-stu-id="203f6-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="203f6-268">Wählen Sie auf der Seite **Kunden** den gewünschten Kunden aus, und klicken Sie auf das Symbol Schnelllinks, um die Zusammenfassungsansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="203f6-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="203f6-269">Vergewissern Sie sich unter **Indirekte Anbieter,** dass der beabsichtigte indirekte Anbieter aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="203f6-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="203f6-270">Klicken Sie auf **Abonnements anzeigen.**</span><span class="sxs-lookup"><span data-stu-id="203f6-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="203f6-271">Suchen Sie auf der Seite **Abonnements** nach **Abonnementübertragung.**</span><span class="sxs-lookup"><span data-stu-id="203f6-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="203f6-272">Klicken Sie unter **Abonnementübertragung** auf **Abonnementübertragung anfordern.**</span><span class="sxs-lookup"><span data-stu-id="203f6-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Anfordern der Abonnementübertragung.":::

7. <span data-ttu-id="203f6-274">Wählen Sie im Dialogfeld "Übertragungsanforderung" ein oder mehrere Abonnements aus, die übertragen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="203f6-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Erstellen sie die Übertragungsanforderung.":::

8. <span data-ttu-id="203f6-276">Klicken Sie auf **Erstellen**.</span><span class="sxs-lookup"><span data-stu-id="203f6-276">Click **Create**.</span></span>

9. <span data-ttu-id="203f6-277">Eine aktive Abonnementübertragungsanforderung wird unter **Abonnementübertragung** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="203f6-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Übertragungsanforderungsliste.":::

10. <span data-ttu-id="203f6-279">Informieren Sie Ihren indirekten Anbieter darüber, dass Sie eine Abonnementübertragungsanforderung an diesen erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="203f6-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="203f6-280">Indirekter Anbieter: Übertragungsanforderung akzeptieren</span><span class="sxs-lookup"><span data-stu-id="203f6-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="203f6-281">So überprüfen und akzeptieren Sie eine Übertragungsanforderung als indirekter Anbieter:</span><span class="sxs-lookup"><span data-stu-id="203f6-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="203f6-282">Melden Sie sich bei Partner Center als **Administrator-Agent** oder **Vertriebs-Agent an.**</span><span class="sxs-lookup"><span data-stu-id="203f6-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="203f6-283">Wählen Sie auf der Seite **Kunden** den gewünschten Kunden aus, und klicken Sie auf das Symbol Quicklinks , um die Zusammenfassungsansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="203f6-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="203f6-284">Vergewissern Sie sich unter **Indirekte Vertriebspartner,** dass der übergehende Partner aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="203f6-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="203f6-285">Klicken Sie auf **Abonnements anzeigen.**</span><span class="sxs-lookup"><span data-stu-id="203f6-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="203f6-286">Suchen Sie auf der Seite **Abonnements** nach **Abonnementübertragung.**</span><span class="sxs-lookup"><span data-stu-id="203f6-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Anzeigen der Übertragungsanforderung.":::

6. <span data-ttu-id="203f6-288">Klicken Sie unter **Abonnementübertragung** auf die zu überprüfende Übertragungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="203f6-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="203f6-289">Klicken Sie nach Bedarf auf **Akzeptieren** (oder **Ablehnen).**</span><span class="sxs-lookup"><span data-stu-id="203f6-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Akzeptieren Sie die Übertragungsanforderung.":::

8. <span data-ttu-id="203f6-291">Warten Sie, bis die Übertragungsanforderung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="203f6-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="203f6-292">Indirekter Anbieter: Überprüfen, ob die Übertragungsanforderung abgeschlossen ist</span><span class="sxs-lookup"><span data-stu-id="203f6-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="203f6-293">Nachdem die Übertragungsanforderung erfolgreich abgeschlossen wurde, überprüfen Sie, ob die Abonnements unter **Abonnements** angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="203f6-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="203f6-294">Informieren Sie den übergehenden Partner.</span><span class="sxs-lookup"><span data-stu-id="203f6-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="203f6-295">Übergangspartner : Überprüfen, ob die Übertragungsanforderung abgeschlossen ist</span><span class="sxs-lookup"><span data-stu-id="203f6-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="203f6-296">Der übergehende Partner sollte folgende Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="203f6-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="203f6-297">Melden Sie sich als **Administrator-Agent** oder **Vertriebs-Agent** bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="203f6-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="203f6-298">Wählen Sie auf der Seite **Kunden** den gewünschten Kunden aus, und klicken Sie auf das Symbol **Schnelllinks,** um die Zusammenfassungsansicht des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="203f6-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="203f6-299">Klicken Sie auf **Abonnements anzeigen.**</span><span class="sxs-lookup"><span data-stu-id="203f6-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="203f6-300">Suchen Sie auf der Seite **Abonnements** nach **Abonnementübertragung.**</span><span class="sxs-lookup"><span data-stu-id="203f6-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="203f6-301">Stellen Sie sicher, dass die Übertragungsanforderung als Abgeschlossen **gekennzeichnet ist.**</span><span class="sxs-lookup"><span data-stu-id="203f6-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="203f6-302">Stellen Sie sicher, dass die Abonnements auf der Seite Abonnements nicht mehr als **aktiv angezeigt** werden:</span><span class="sxs-lookup"><span data-stu-id="203f6-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="203f6-303">Wenn es sich um ein Azure-Abonnement (MS-AZR-0145P) handelt, wird es nicht mehr aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="203f6-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="203f6-304">Wenn es sich um ein lizenzbasiertes Abonnement (Office 365, Dynamics, Intune) handelt, wird es mit dem Status **Angehalten aufgelistet.**</span><span class="sxs-lookup"><span data-stu-id="203f6-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Das Abonnement wurde angehalten.":::

### <a name="considerations"></a><span data-ttu-id="203f6-306">Überlegungen</span><span class="sxs-lookup"><span data-stu-id="203f6-306">Considerations</span></span>

- <span data-ttu-id="203f6-307">**Die Abonnement-ID ist nach der Übertragung anders.**</span><span class="sxs-lookup"><span data-stu-id="203f6-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="203f6-308">Wenn es sich um ein Azure-Abonnement (MS-AZR-0145P) handelt, hat es darüber hinaus eine Azure-Abonnement-ID, die vom vorherigen Besitzer beibehalten wird und im Azure-Verwaltungsportal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="203f6-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="203f6-309">**Auf dasselbe Abonnement kann nicht durch mehrere Übertragungsanforderungen verwiesen werden.**</span><span class="sxs-lookup"><span data-stu-id="203f6-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="203f6-310">Nachdem Sie eine Übertragungsanforderung erstellt haben, die ein vorhandenes Abonnement enthält, können Sie keine zusätzlichen Übertragungsanforderungen erstellen, einschließlich desselben Abonnements, bis die erste Übertragungsanforderung abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="203f6-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="203f6-311">**Add-Ons für lizenzbasierte Abonnements müssen zusammen mit ihrem Basisabonnement übertragen werden.**</span><span class="sxs-lookup"><span data-stu-id="203f6-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="203f6-312">Wenn Sie beim Erstellen einer Übertragungsanforderung ein vorhandenes Abonnement mit mindestens einem Add-On auswählen, werden die Add-Ons automatisch in die Übertragungsanforderung einbezogen.</span><span class="sxs-lookup"><span data-stu-id="203f6-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="203f6-313">**Änderungen an der Lizenzanzahl eines Abonnements werden in der vorhandenen Übertragungsanforderung nicht berücksichtigt.**</span><span class="sxs-lookup"><span data-stu-id="203f6-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="203f6-314">Nachdem Sie eine Übertragungsanforderung erstellt haben, die ein vorhandenes Abonnement enthält, sollten Sie vermeiden, die Lizenzmenge des Abonnements (oder der zugehörigen Add-Ons) zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="203f6-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="203f6-315">Wenn Sie dies tun, wird die neue Menge nicht in der Übertragungsanforderung widergespiegelt.</span><span class="sxs-lookup"><span data-stu-id="203f6-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="203f6-316">Nachdem der indirekte Anbieter die Übertragungsanforderung akzeptiert hat, hat das resultierende Abonnement die alte Menge.</span><span class="sxs-lookup"><span data-stu-id="203f6-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="203f6-317">Wenn Die neue Menge an den indirekten Anbieter übertragen werden soll, müssen Sie die vorhandene Übertragungsanforderung abbrechen und eine neue neu erstellen.</span><span class="sxs-lookup"><span data-stu-id="203f6-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="203f6-318">**Nicht alle Käufe können mithilfe der self-served-Abonnementübertragung übertragen werden.**</span><span class="sxs-lookup"><span data-stu-id="203f6-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="203f6-319">Derzeit können Sie mit diesem Feature nur O365-Abonnements und Azure PAYG-Abonnements (MS-AZR-0145P) übertragen.</span><span class="sxs-lookup"><span data-stu-id="203f6-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="203f6-320">Andere Käufe wie Azure-Pläne, reservierte Azure-Instanzen, laufzeitbasierte Abonnements und SaaS-Abonnements für Azure Marketplace werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="203f6-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="203f6-321">Auf der Seite Übertragungsanforderung übermitteln wird ein Grund angezeigt, warum ein Abonnement nicht übertragen werden kann.</span><span class="sxs-lookup"><span data-stu-id="203f6-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="203f6-322">Um diese Abonnements zu übertragen, müssen Sie das vorhandene Abonnement kündigen und ein neues Angebot für den Kunden über einen indirekten Anbieter erwerben. [](create-a-new-subscription.md#suspend-or-cancel-a-subscription)</span><span class="sxs-lookup"><span data-stu-id="203f6-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="203f6-323">**Kann nicht mithilfe einer Sandboxumgebung getestet werden.**</span><span class="sxs-lookup"><span data-stu-id="203f6-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="203f6-324">Registrieren für Incentives für indirekte Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="203f6-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="203f6-325">Nachdem Sie sich unter Ihrem vorhandenen Direktabrechnungspartner-Mandanten erfolgreich als indirekter Wiederverkäufer registriert haben, erhalten Sie innerhalb von 30 Tagen eine Einladung zur Registrierung für Incentives für indirekte Wiederverkäufer.</span><span class="sxs-lookup"><span data-stu-id="203f6-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="203f6-326">Die Einladung basiert auf dem MPN-Partnerkonto, das aktuell Ihrem CSP-Partnermandanten zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="203f6-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="203f6-327">Die Einladung wird an die dem MPN-Partnerkonto zugeordnete E-Mail-Adresse gesendet.</span><span class="sxs-lookup"><span data-stu-id="203f6-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="203f6-328">Mit dem gleichen Partnermandanten können Sie sich auch für Incentive-Programme für die Direktabrechnung registrieren.</span><span class="sxs-lookup"><span data-stu-id="203f6-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="203f6-329">Die Programme müssen separat verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="203f6-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="203f6-330">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="203f6-330">Next steps</span></span>

- [<span data-ttu-id="203f6-331">Weitere Informationen zu den Anforderungen an indirekte Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="203f6-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="203f6-332">Neue Anforderungen für direkte CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="203f6-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="203f6-333">Eingeschränkte Direktabrechnungsfunktionen</span><span class="sxs-lookup"><span data-stu-id="203f6-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
