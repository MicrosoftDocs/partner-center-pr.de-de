---
title: Der Co-Selling-Connector für Dynamics 365 CRM Partner Center
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Ihrer Verweise in Partner Center mit Dynamics 365 CRM
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 3b5170edaaadca3c4045e7ebed174b5d52b06bdd
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991646"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="9dbbd-103">Co-Selling-Connector für Dynamics 365 CRM – Übersicht</span><span class="sxs-lookup"><span data-stu-id="9dbbd-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="9dbbd-104">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-104">Appropriate roles</span></span>

- <span data-ttu-id="9dbbd-105">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="9dbbd-105">Referrals admin</span></span>
- <span data-ttu-id="9dbbd-106">Systemadministrator oder systemanpassungsprogramm im CRM</span><span class="sxs-lookup"><span data-stu-id="9dbbd-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="9dbbd-107">Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="9dbbd-108">Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="9dbbd-109">Verwenden Sie die Co-Selling-Connectors, um einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers zu erstellen, Referenzen von Microsoft-Verkäufern zu erhalten, Verweise zu akzeptieren/ablehnen, Daten zu ändern, wie z. b. den Geschäftswert und das Enddatum.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="9dbbd-110">Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="9dbbd-111">Sie können alle Ihre Verweise im CRM Ihrer Wahl und nicht im Partner Center verwenden.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="9dbbd-112">Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="9dbbd-113">Vor der Installation von-Pre-Requirements</span><span class="sxs-lookup"><span data-stu-id="9dbbd-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="9dbbd-114">**Themen**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-114">**Topics**</span></span>   |<span data-ttu-id="9dbbd-115">**Details**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-115">**Details**</span></span>   |<span data-ttu-id="9dbbd-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="9dbbd-117">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="9dbbd-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="9dbbd-118">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-118">You need a valid MPN ID</span></span>|<span data-ttu-id="9dbbd-119">So fügen Sie [MPN](https://partner.microsoft.com/) an</span><span class="sxs-lookup"><span data-stu-id="9dbbd-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="9dbbd-120">Cosell bereit</span><span class="sxs-lookup"><span data-stu-id="9dbbd-120">Cosell ready</span></span>|<span data-ttu-id="9dbbd-121">Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="9dbbd-122">Vertrieb mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="9dbbd-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="9dbbd-123">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="9dbbd-123">Partner Center account</span></span>|<span data-ttu-id="9dbbd-124">Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="9dbbd-125">Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="9dbbd-126">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="9dbbd-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="9dbbd-127">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-127">Partner Center user roles</span></span>|<span data-ttu-id="9dbbd-128">Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="9dbbd-129">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="9dbbd-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="9dbbd-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="9dbbd-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="9dbbd-131">Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="9dbbd-132">Zuweisen von Rollen in Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9dbbd-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="9dbbd-133">Energie automatisierter Fluss Konto</span><span class="sxs-lookup"><span data-stu-id="9dbbd-133">Power Automate Flow Account</span></span>|<span data-ttu-id="9dbbd-134">Ein aktives, [Energie automatisierbares](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder den SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="9dbbd-135">Dieser Benutzer sollte sich mindestens einmal vor der Installation bei der [Strom Automatisierung](https://flow.microsoft.com) anmelden.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="9dbbd-136">Installieren der Partner Center-Synchronisierung für Dynamics 365 (Energie automatisierte Lösung)</span><span class="sxs-lookup"><span data-stu-id="9dbbd-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="9dbbd-137">Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="9dbbd-138">In diesem Schritt werden die verfügbaren CRM-Instanzen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="9dbbd-139">Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="9dbbd-140">Wählen Sie in der linken Navigationsleiste **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="9dbbd-141">Klicken Sie im oberen Menü auf den Link **appsource öffnen** .</span><span class="sxs-lookup"><span data-stu-id="9dbbd-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Appsource öffnen":::

5. <span data-ttu-id="9dbbd-143">Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Dynamics365** .</span><span class="sxs-lookup"><span data-stu-id="9dbbd-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="9dbbd-144">Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-144">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="9dbbd-145">Dadurch wird die Seite geöffnet, auf der Sie die CRM-Umgebung (Dynamics 365) zum Installieren der Anwendung auswählen können.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="9dbbd-146">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-146">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="9dbbd-147">Anschließend werden Sie zur Seite **Verwalten Ihrer Lösungen** weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="9dbbd-148">Navigieren Sie zu "Partner Center-Verweise", indem Sie die Pfeil Schaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="9dbbd-149">Die **geplante Installation** sollte neben der Projekt Mappe für Partner Center-Verweise angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="9dbbd-150">Die Installation wird 10-15 Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="9dbbd-151">Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="9dbbd-152">Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Dynamics 365** in der Lösungs Liste verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="9dbbd-153">Wählen Sie **Partner Center-Synchronisierungs Referenz für Dynamics 365 aus**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="9dbbd-154">Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Verfügbare CRMs":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="9dbbd-156">Bewährte Vorgehensweise: testen, bevor Sie fortfahren</span><span class="sxs-lookup"><span data-stu-id="9dbbd-156">Best practice: test before you go live</span></span>

<span data-ttu-id="9dbbd-157">Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="9dbbd-158">Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="9dbbd-159">Erstellen Sie eine Kopie der Projekt Mappe, und führen Sie die Konfiguration aus, und führen Sie die Automatisierung der Fluss Anpassungen in der Stagingumgebung durch</span><span class="sxs-lookup"><span data-stu-id="9dbbd-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="9dbbd-160">Testen Sie die Lösung auf einer Staging/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="9dbbd-161">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktions Instanz.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="9dbbd-162">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="9dbbd-162">Configure the solution</span></span>

1. <span data-ttu-id="9dbbd-163">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="9dbbd-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="9dbbd-164">Wählen Sie in der Dropdown- **Umgebung** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="9dbbd-165">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="9dbbd-166">Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="9dbbd-167">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="9dbbd-167">Partner Center Events</span></span>

   - <span data-ttu-id="9dbbd-168">Der CRM-Administrator mit den Energie automatisierten Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="9dbbd-169">Wählen Sie in der linken Navigationsleiste **Verbindungen** aus, und wählen Sie die Projekt Mappe "Partner Center-Verweise" aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="9dbbd-170">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen**klicken.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Erstellen der Verbindung":::

      3. <span data-ttu-id="9dbbd-172">Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .</span><span class="sxs-lookup"><span data-stu-id="9dbbd-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="9dbbd-173">Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".</span><span class="sxs-lookup"><span data-stu-id="9dbbd-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="9dbbd-174">Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="9dbbd-175">Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="9dbbd-176">Um die Strom automatisierten Flows den Verbindungen zuzuordnen, bearbeiten Sie jeden der Strom automatisierten Flows, um eine Verbindung mit Common Data Service-und Partner Center-Referenzen herzustellen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-176">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="9dbbd-177">Speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-177">Save the changes.</span></span>

5. <span data-ttu-id="9dbbd-178">**Schalten** Sie die Strom automatisierten Flows ein.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-178">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="9dbbd-179">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="9dbbd-179">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="9dbbd-180">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-180">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="9dbbd-181">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-181">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="9dbbd-182">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-182">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="9dbbd-183">Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt</span><span class="sxs-lookup"><span data-stu-id="9dbbd-183">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="9dbbd-185">Wenn Sie diese Updates vornehmen, wird Folgendes angezeigt:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-185">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="9dbbd-187">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-187">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="9dbbd-188">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-188">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="9dbbd-189">Wählen Sie **Partner Center auf Dynamics 365 (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-189">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="9dbbd-190">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-190">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="9dbbd-191">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-191">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopieren der URL":::

8. <span data-ttu-id="9dbbd-193">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-193">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="9dbbd-194">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-194">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="9dbbd-195">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-195">Enter the following details:</span></span>

    1. <span data-ttu-id="9dbbd-196">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="9dbbd-196">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="9dbbd-197">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="9dbbd-197">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="9dbbd-198">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="9dbbd-198">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="9dbbd-199">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-199">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="9dbbd-200">Der webhook kann nun auf Create-und Update-Ereignisse lauschen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-200">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="9dbbd-201">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-201">Customize synchronization steps</span></span>

<span data-ttu-id="9dbbd-202">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-202">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="9dbbd-203">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-203">Often CRM systems are highly customized.</span></span> <span data-ttu-id="9dbbd-204">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-204">You can customize the Power Automate flows.</span></span> <span data-ttu-id="9dbbd-205">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-205">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="9dbbd-206">Microsoft Partner Centers für CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-206">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="9dbbd-207">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-207">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="9dbbd-208">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-208">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="9dbbd-209">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-209">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="9dbbd-210">a.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-210">a.</span></span> <span data-ttu-id="9dbbd-211">Wählen Sie Partner Center für Dynamics 365 (Insider Preview) oder Partner Center für Salesforce (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-211">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="9dbbd-212">b.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-212">b.</span></span> <span data-ttu-id="9dbbd-213">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="9dbbd-214">c.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-214">c.</span></span> <span data-ttu-id="9dbbd-215">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-215">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="9dbbd-216">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Erstellungs Ereignisse aus, wenn es sich um eine **neue freigegebene Chance handelt, und**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-216">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="9dbbd-217">Wählen Sie den unterschritt aus, **Falls ja** , und erweitern Sie dann die Option **neue Gelegenheit im CRM**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-217">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="9dbbd-218">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-218">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="9dbbd-219">d.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-219">d.</span></span> <span data-ttu-id="9dbbd-220">Zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="9dbbd-220">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="9dbbd-221">e.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-221">e.</span></span> <span data-ttu-id="9dbbd-222">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-222">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="9dbbd-223">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-223">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="9dbbd-224">f.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-224">f.</span></span> <span data-ttu-id="9dbbd-225">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-225">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="9dbbd-226">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="9dbbd-226">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="9dbbd-227">a.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-227">a.</span></span> <span data-ttu-id="9dbbd-228">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-228">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="9dbbd-229">b.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-229">b.</span></span> <span data-ttu-id="9dbbd-230">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-230">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="9dbbd-231">c.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-231">c.</span></span> <span data-ttu-id="9dbbd-232">Wenn Sie die CRM-Feld Zuordnungen für Update Ereignisse anpassen möchten, wählen Sie aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-232">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="9dbbd-233">d.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-233">d.</span></span> <span data-ttu-id="9dbbd-234">Wählen Sie den unterschritt aus, **Wenn ja** , und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-234">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="9dbbd-235">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-235">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="9dbbd-236">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="9dbbd-236">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="9dbbd-237">a.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-237">a.</span></span> <span data-ttu-id="9dbbd-238">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-238">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="9dbbd-239">b.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-239">b.</span></span> <span data-ttu-id="9dbbd-240">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="9dbbd-240">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="9dbbd-241">c.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-241">c.</span></span> <span data-ttu-id="9dbbd-242">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-242">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="9dbbd-243">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-243">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="9dbbd-244">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="9dbbd-244">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="9dbbd-245">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-245">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="9dbbd-246">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-246">Pre-requisites</span></span>

<span data-ttu-id="9dbbd-247">Um die Verweise auf Partner Center und Dynamics 365 CRM zu synchronisieren, werden die Microsoft-spezifischen verweigerfelder von der Energie automatisierten Lösung eindeutig abgegrenzt.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-247">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="9dbbd-248">Diese Identifikation gibt Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-248">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="9dbbd-249">Ein Satz benutzerdefinierter Felder ist als Teil der Entität " **Chance** " verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-249">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="9dbbd-250">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-250">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="9dbbd-251">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-251">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="9dbbd-252">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="9dbbd-252">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="9dbbd-253">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="9dbbd-253">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="9dbbd-254">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="9dbbd-254">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="9dbbd-255">**Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="9dbbd-255">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="9dbbd-256">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="9dbbd-256">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="9dbbd-257">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-257">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="9dbbd-258">SS</span><span class="sxs-lookup"><span data-stu-id="9dbbd-258">SCENARIOS:</span></span>

1. <span data-ttu-id="9dbbd-259">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-259">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="9dbbd-260">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-260">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="9dbbd-261">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Dynamics 365-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-261">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Verkaufschance":::

   3. <span data-ttu-id="9dbbd-263">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-263">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="9dbbd-264">**Mit Partner Center synchronisieren**: Ja</span><span class="sxs-lookup"><span data-stu-id="9dbbd-264">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="9dbbd-265">**Wie kann Microsoft Help?**: Wählen Sie eine der folgenden Aktionen aus:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-265">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Auswahl von Hilfe":::

      - <span data-ttu-id="9dbbd-267">**Produkte**: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="9dbbd-267">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="9dbbd-268">Wenn die Verkaufschance in Dynamics 365 mit der Option **sync with Partner Center** auf **Ja**festgelegt ist, warten Sie 10 Minuten, und melden Sie sich dann bei Ihrem Partner Center-Konto an.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-268">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="9dbbd-269">Ihre Verweise werden mit Dynamics 365 synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-269">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="9dbbd-270">Für eine Gelegenheit, bei der die Option "Synchronisierung mit Partner Center" auf "Ja" festgelegt wurde, werden die Änderungen bei der Aktualisierung der Gelegenheit in Dynamics 365 CRM in Ihrem Partner Center-Konto synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-270">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="9dbbd-271">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-271">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="9dbbd-272">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="9dbbd-272">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="9dbbd-273">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-273">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="9dbbd-274">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-274">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="9dbbd-275">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-275">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="9dbbd-276">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-276">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="9dbbd-277">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-277">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="9dbbd-278">Der im Microsoft Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-278">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="9dbbd-279">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="9dbbd-279">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9dbbd-280">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="9dbbd-280">Next steps</span></span>

- [<span data-ttu-id="9dbbd-281">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="9dbbd-281">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="9dbbd-282">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="9dbbd-282">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="9dbbd-283">Weitere Informationen zur Microsoft powerautomatisieren-Plattform</span><span class="sxs-lookup"><span data-stu-id="9dbbd-283">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="9dbbd-284">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="9dbbd-284">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)