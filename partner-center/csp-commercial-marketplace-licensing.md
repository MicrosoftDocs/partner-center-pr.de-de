---
title: Verwalten der Lizenzierung in Marketplace-Angeboten
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die Lizenzierung für Ihre Angebote im kommerziellen ISV-Marketplace einrichten und verwalten.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328014"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="19e6d-103">Verwalten der Lizenzierung in Marketplace-Angeboten</span><span class="sxs-lookup"><span data-stu-id="19e6d-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="19e6d-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="19e6d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="19e6d-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="19e6d-105">Global admin</span></span>
- <span data-ttu-id="19e6d-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="19e6d-106">Account admin</span></span>

<span data-ttu-id="19e6d-107">In diesem Artikel wird beschrieben, wie Sie ein Angebot in Partner Center einrichten, in Microsoft AppSource verfügbar machen und dann Lizenzen für dieses Angebot verwalten.</span><span class="sxs-lookup"><span data-stu-id="19e6d-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="19e6d-108">Die Funktionen in diesem Artikel befinden sich derzeit in Public Preview.</span><span class="sxs-lookup"><span data-stu-id="19e6d-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="19e6d-109">Vorbereitung</span><span class="sxs-lookup"><span data-stu-id="19e6d-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="19e6d-110">Grundlagen des kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="19e6d-110">Commercial marketplace basics</span></span>

<span data-ttu-id="19e6d-111">Bevor Sie mit diesem Prozess beginnen, sollten Sie sich mit den Grundlagen des kommerziellen Marketplace vertraut machen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="19e6d-112">Die Artikel in der folgenden Tabelle helfen Ihnen beim Einstieg.</span><span class="sxs-lookup"><span data-stu-id="19e6d-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="19e6d-113">Thema</span><span class="sxs-lookup"><span data-stu-id="19e6d-113">Topic</span></span>  | <span data-ttu-id="19e6d-114">Artikel</span><span class="sxs-lookup"><span data-stu-id="19e6d-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="19e6d-115">Pläne für den kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="19e6d-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="19e6d-116">Pläne und Preise für Angebote im kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="19e6d-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="19e6d-117">Angebote für den kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="19e6d-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="19e6d-118">Auflisten von Typen</span><span class="sxs-lookup"><span data-stu-id="19e6d-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="19e6d-119">Konten im kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="19e6d-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="19e6d-120">Erstellen eines Kontos im kommerziellen Marketplace in Partner Center</span><span class="sxs-lookup"><span data-stu-id="19e6d-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="19e6d-121">Ermitteln Ihrer Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="19e6d-121">Determine your Offer ID</span></span>

<span data-ttu-id="19e6d-122">In den folgenden Verfahren werden Sie aufgefordert, eine Angebots-ID ein geben.</span><span class="sxs-lookup"><span data-stu-id="19e6d-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="19e6d-123">Nehmen Sie sich nun etwas Zeit, um eine geeignete Angebots-ID zu finden, und beachten Sie dabei die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="19e6d-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="19e6d-124">Diese ID wird für Kunden unter der Webadresse für das Marketplace-Angebot und ggf. in Azure Resource Manager-Vorlagen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19e6d-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="19e6d-125">Die Angebots-ID darf zusammen mit der Herausgeber-ID nicht länger als 40 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="19e6d-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="19e6d-126">Verwenden Sie nur Kleinbuchstaben und Zahlen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="19e6d-127">Die Angebots-ID kann Bindestriche und Unterstriche enthalten, aber keine Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="19e6d-128">Wenn Ihre Herausgeber-ID beispielsweise ist und `testpublisherid` Sie `test-offer-1` eingeben, ist die Webadresse des Angebots `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="19e6d-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="19e6d-129">Diese ID kann nach dem Auswählen von **Erstellen** nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="19e6d-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="19e6d-130">Bestimmen Ihres Angebotsalias</span><span class="sxs-lookup"><span data-stu-id="19e6d-130">Determine your Offer alias</span></span>

<span data-ttu-id="19e6d-131">Der Angebotsalias ist der Name, der für das Angebot in der Partner Center.</span><span class="sxs-lookup"><span data-stu-id="19e6d-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="19e6d-132">Außerdem benötigen Sie einen geeigneten Angebotsalias, der den folgenden Richtlinien entspricht:</span><span class="sxs-lookup"><span data-stu-id="19e6d-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="19e6d-133">Dieser Name wird im Marketplace nicht verwendet und unterscheidet sich vom Angebotsnamen und anderen Werten, die den Kunden angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="19e6d-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="19e6d-134">Dieser Name kann nach der Auswahl von Erstellen nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="19e6d-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="19e6d-135">Erstellen Ihres Angebots</span><span class="sxs-lookup"><span data-stu-id="19e6d-135">Create your offer</span></span>

<span data-ttu-id="19e6d-136">Der erste Schritt im Lizenzierungsprozess besteht darin, Ihr Angebot für den kommerziellen Marketplace zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="19e6d-137">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="19e6d-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="19e6d-138">Wählen Sie im linken Navigationsmenü **kommerzieller Marketplace/Übersicht** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="19e6d-139">Wählen Sie oben auf der Seite Übersicht die Option **Neues Angebot** und dann **Dynamics 365 for Customer Engagement & PowerApps aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="19e6d-140">Geben Sie die **Angebots-ID** und den **Angebotsalias ein,** die Sie zuvor erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="19e6d-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="19e6d-141">Wählen Sie **Erstellen** aus, um das Angebot zu generieren und fortzufahren.</span><span class="sxs-lookup"><span data-stu-id="19e6d-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="19e6d-142">Wählen Sie Ihre Lizenzierungsoptionen aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="19e6d-143">Um die Lizenzverwaltung für Ihr Angebot zu aktivieren, wählen **Sie App-Lizenzverwaltung über Microsoft aktivieren** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="19e6d-144">Dies ist eine einmalige Einstellung, die Sie nach der Veröffentlichung Ihres Angebots nicht mehr ändern können.</span><span class="sxs-lookup"><span data-stu-id="19e6d-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="19e6d-145">Sie können Es Kunden auch ermöglichen, die Basisfunktionen Ihrer App ohne Lizenz auszuführen und Premium-Features auszuführen, sobald sie eine Lizenz erworben haben.</span><span class="sxs-lookup"><span data-stu-id="19e6d-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="19e6d-146">Wählen Sie hierzu Allow customers to install my app even if licenses are not assigned (Kunden erlauben, **meine App zu installieren, auch wenn lizenzen nicht zugewiesen sind)** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="19e6d-147">Wenn Sie nicht möchten, dass die Lizenzverwaltung für Ihr Angebot aktiviert ist, wählen **Sie Jetzt abrufen (kostenlos)**, **Kostenlose Testversion** oder Kontakt mit **mir aufnehmen** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="19e6d-148">Erstellen Ihres Plans</span><span class="sxs-lookup"><span data-stu-id="19e6d-148">Create your plan</span></span>

<span data-ttu-id="19e6d-149">In diesen Schritten definieren Sie den Plan oder die Pläne, die Sie für Ihr Angebot aktivieren möchten.</span><span class="sxs-lookup"><span data-stu-id="19e6d-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="19e6d-150">Wählen Sie im linken Navigationsmenü **plan overview (Planübersicht)** und dann **Create new plan (Neuen Plan erstellen)** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="19e6d-151">Geben Sie eine **Plan-ID** und einen **Plannamen** ein, und wählen Sie dann **Erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="19e6d-152">Geben Sie auf der Seite **Planlisting** Ihre **Planbeschreibung ein.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="19e6d-153">Wählen Sie Entwurf **speichern** aus, um die Beschreibung zu speichern und später abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="19e6d-154">Wenn Sie fertig sind, wählen Sie **Überprüfen und veröffentlichen** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="19e6d-155">Die Planinformationen werden nun auf appsource.microsoft.com unter Angebotsliste (Abschnitt "Pläne") angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19e6d-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="19e6d-156">Nachdem Sie alle Pläne für dieses Angebot erstellt haben, müssen Sie die Dienst-ID jedes Plans kopieren.</span><span class="sxs-lookup"><span data-stu-id="19e6d-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="19e6d-157">Wählen Sie oben auf der Seite Planlisting die Option **Planübersicht** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="19e6d-158">Kopieren Sie die Dienst-ID für jeden Plan an einen sicheren Speicherort.</span><span class="sxs-lookup"><span data-stu-id="19e6d-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="19e6d-159">Hinzufügen von Dienst-IDs zu Ihrer Lösung</span><span class="sxs-lookup"><span data-stu-id="19e6d-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="19e6d-160">Im nächsten Schritt aktualisieren Sie Ihre Lösung, indem Sie die Dienst-IDs für jeden Plan hinzufügen, den Sie gerade kopiert haben.</span><span class="sxs-lookup"><span data-stu-id="19e6d-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="19e6d-161">Anleitungen hierzu finden Sie unter [Erstellen eines AppSource-Pakets für Ihre Lösung.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="19e6d-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="19e6d-162">Hochladen Ihres Pakets und Veröffentlichen Ihres Angebots</span><span class="sxs-lookup"><span data-stu-id="19e6d-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="19e6d-163">Wählen Sie im linken Navigationsbereich kommerzieller **Marketplace** und dann Technische **Konfiguration aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="19e6d-164">Wählen Sie **unter Basislizenzmodell** die Option **Benutzer aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="19e6d-165">Geben **Sie unter CRM-Paket** die URL Ihres Paketspeicherorts ein.</span><span class="sxs-lookup"><span data-stu-id="19e6d-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="19e6d-166">Verwenden Sie die anderen Registerkarten im linken Navigationsbereich, um weitere erforderliche Informationen ein.</span><span class="sxs-lookup"><span data-stu-id="19e6d-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="19e6d-167">Wenn Sie fertig sind, wählen Sie **Überprüfen und veröffentlichen aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="19e6d-168">Nachdem Sie das Angebot veröffentlicht haben, überprüfen und überprüfen wir Ihre Informationen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="19e6d-169">Wenn probleme mit diesem Prozess liegen, werden wir Sie benachrichtigen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="19e6d-170">Wenn alle Probleme behoben wurden, erhalten Sie eine Benachrichtigung, dass Ihr Angebot in AppSource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="19e6d-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="19e6d-171">An diesem Punkt können Sie es live machen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="19e6d-172">Machen Sie Ihr Angebot in Partner Center</span><span class="sxs-lookup"><span data-stu-id="19e6d-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="19e6d-173">Das folgende Verfahren erläutert, wie Sie Ihr Angebot in AppSource live machen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="19e6d-174">Weitere Informationen zu diesem Prozess finden Sie unter [Einführung in Auflistungsoptionen.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="19e6d-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="19e6d-175">Nachdem Sie Ihr Angebot veröffentlicht haben, dauert es 4 bis 6 Stunden, bis es live veröffentlichungen kann.</span><span class="sxs-lookup"><span data-stu-id="19e6d-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="19e6d-176">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="19e6d-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="19e6d-177">Wählen Sie im linken Navigationsmenü **kommerzieller Marketplace/Übersicht aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="19e6d-178">Suchen Sie **auf** der Seite Übersicht nach dem Angebot, das Sie suchen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="19e6d-179">Angebote, die veröffentlicht werden können, haben den Status **Vorschau.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="19e6d-180">Wählen Sie das Angebot aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-180">Select the offer.</span></span>
4. <span data-ttu-id="19e6d-181">Wählen Sie auf der Seite **Angebotsübersicht** die Option **Liveschalten** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="19e6d-182">Das Angebot ist in 4 bis 6 Stunden live lebbar.</span><span class="sxs-lookup"><span data-stu-id="19e6d-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="19e6d-183">Wählen Sie unten auf der Seite Angebotsübersicht den Link AppSource aus, um Ihre Angebotsliste in **AppSource** **anzuzeigen.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="19e6d-184">**Für lizenzfähige Angebote:** Wenn Ihr Angebot eine Lizenzprüfung erfordert, können Benutzer nur durch Klicken auf Kontakt mit **mir** aufnehmen einen Lead eingeben, damit Sie mit ihnen kommunizieren können.</span><span class="sxs-lookup"><span data-stu-id="19e6d-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="19e6d-185">**Für lizenzaktivierte Angebote mit kostenloser Installationsoption:** Wenn für Ihr Angebot keine Lizenzprüfung erforderlich ist, wird Administratorbenutzern zusätzlich zu **Kontakt mit mir** die Schaltfläche **Jetzt** anfordern angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19e6d-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="19e6d-186">Benutzer, die Ihre kostenlose Installationsoption ausprobieren möchten, sollten auf **Jetzt abrufen** klicken, um das Angebot in Power Platform Admin Center zu installieren.</span><span class="sxs-lookup"><span data-stu-id="19e6d-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="19e6d-187">Benutzer können weiterhin **Kontakt mit mir aufnehmen,** wenn sie Fragen haben oder ein Upgrade auf einen kostenpflichtigen Plan durchführen möchten.</span><span class="sxs-lookup"><span data-stu-id="19e6d-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="19e6d-188">Registrieren des ISV Connect-Abschlusses bei der Dealregistrierung</span><span class="sxs-lookup"><span data-stu-id="19e6d-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="19e6d-189">Bevor Sie einem Kunden Lizenzen zuweisen können, muss jeder Verkauf in Partner Center registriert werden.</span><span class="sxs-lookup"><span data-stu-id="19e6d-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="19e6d-190">Informationen hierzu finden Sie unter [Registrieren Ihrer Angebote.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="19e6d-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="19e6d-191">Einladen des Kunden</span><span class="sxs-lookup"><span data-stu-id="19e6d-191">Invite the customer</span></span>

<span data-ttu-id="19e6d-192">Gehen Sie wie folgt vor, um den Kunden zur Teilnahme an diesem Deal einzuladen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="19e6d-193">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="19e6d-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="19e6d-194">Wählen Sie im linken Navigationsmenü **kommerzieller Marketplace/Übersicht** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="19e6d-195">Wählen Sie im linken **Navigationsmenü Empfehlungen** und dann **Deal Registration (Dealregistrierung)** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="19e6d-196">Filtern Sie nach **Übermittelte** Angebote, wählen Sie die Registerkarte **In Bearbeitung** aus, und wählen Sie dann das gewünschte Angebot aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="19e6d-197">Wählen Sie auf der Übersichtsseite für diesen Deal die Option **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="19e6d-198">Wählen **Sie** im Fenster Lizenzen verwalten in der Dropdownliste **Kundendetails** den Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="19e6d-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="19e6d-199">Wenn die Kundenbeziehung noch nicht vorhanden ist, wählen Sie + Neuen Kunden einladen **aus, um zuzustimmen.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="19e6d-200">Kopieren Sie den angezeigten Link.</span><span class="sxs-lookup"><span data-stu-id="19e6d-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="19e6d-201">Senden Sie diesen Link per E-Mail an den Abrechnungsadministrator oder globalen Administrator Ihres Kunden, und lassen Sie diesen über diesen Link auf admin.microsoft.com zugreifen und die Beziehung akzeptieren und autorisieren, die Sie einrichten.</span><span class="sxs-lookup"><span data-stu-id="19e6d-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="19e6d-202">Die Beziehung wird erst hergestellt, wenn der Kunde diesen Schritt ausführt.</span><span class="sxs-lookup"><span data-stu-id="19e6d-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="19e6d-203">Aktivieren, Verwalten und Entfernen Ihrer Lizenzen</span><span class="sxs-lookup"><span data-stu-id="19e6d-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="19e6d-204">Nachdem Ihr Kunde die Beziehung mit Ihnen autorisiert hat, können Sie mit dem Hinzufügen von Plänen aus Ihrem Angebot und dem Zuweisen von Lizenzen zu jedem Plan beginnen.</span><span class="sxs-lookup"><span data-stu-id="19e6d-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="19e6d-205">Wählen Sie im Fenster Lizenzen für diesen Deal verwalten **die Option + Plan hinzufügen aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="19e6d-206">Füllen Sie **die Felder Pläne für diese Lösung und** Anzahl von Lizenzen **aus,** und wählen Sie dann **Lizenzen aktualisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="19e6d-207">Die Lizenzen sind auf der admin.microsoft.com verfügbar, die Kunden verwalten und Mitarbeitern zuweisen können.</span><span class="sxs-lookup"><span data-stu-id="19e6d-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="19e6d-208">Um die Anzahl der Lizenzen für einen vorhandenen Plan zu ändern, geben Sie die neue Nummer in das Feld **Anzahl der** Lizenzen ein, und wählen Sie dann Lizenzen **aktualisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="19e6d-209">Um Lizenzen für einen Deal zu deaktivieren oder zu entfernen, wählen Sie im Feld **Aktionen** das Papierkorbsymbol und dann **Lizenzen aktualisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="19e6d-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="19e6d-210">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="19e6d-210">Next steps</span></span>

[<span data-ttu-id="19e6d-211">Ressourcen zu „Lizenzierung“</span><span class="sxs-lookup"><span data-stu-id="19e6d-211">Licensing resources</span></span>](support-resources-licensing.md)