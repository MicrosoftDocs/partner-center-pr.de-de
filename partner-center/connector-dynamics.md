---
title: Der Co-Selling-Connector für Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Sie Ihre Verweise im Partner Center mit Ihrem Co-Selling-Connector für Dynamics 365 CRM. Verkäufer können sich dann in Ihrem CRM-System mit Microsoft zusammen verkaufen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947781"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="1891e-104">Co-Selling-Connector für Dynamics 365 CRM – Übersicht</span><span class="sxs-lookup"><span data-stu-id="1891e-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1891e-105">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="1891e-105">Appropriate roles</span></span>

- <span data-ttu-id="1891e-106">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="1891e-106">Referrals admin</span></span>
- <span data-ttu-id="1891e-107">Systemadministrator oder systemanpassungsprogramm im CRM</span><span class="sxs-lookup"><span data-stu-id="1891e-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1891e-108">Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme.</span><span class="sxs-lookup"><span data-stu-id="1891e-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1891e-109">Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden.</span><span class="sxs-lookup"><span data-stu-id="1891e-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1891e-110">Verwenden Sie die Co-Selling-Connectors, um einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers zu erstellen, Referenzen von Microsoft-Verkäufern zu erhalten, Verweise zu akzeptieren/ablehnen, Daten zu ändern, wie z. b. den Geschäftswert und das Enddatum.</span><span class="sxs-lookup"><span data-stu-id="1891e-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="1891e-111">Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten.</span><span class="sxs-lookup"><span data-stu-id="1891e-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1891e-112">Sie können alle Ihre Verweise im CRM Ihrer Wahl und nicht im Partner Center verwenden.</span><span class="sxs-lookup"><span data-stu-id="1891e-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1891e-113">Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="1891e-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1891e-114">Vor der Installation von-Pre-Requirements</span><span class="sxs-lookup"><span data-stu-id="1891e-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1891e-115">**Themen**</span><span class="sxs-lookup"><span data-stu-id="1891e-115">**Topics**</span></span>   |<span data-ttu-id="1891e-116">**Details**</span><span class="sxs-lookup"><span data-stu-id="1891e-116">**Details**</span></span>   |<span data-ttu-id="1891e-117">**Links**</span><span class="sxs-lookup"><span data-stu-id="1891e-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1891e-118">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="1891e-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1891e-119">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="1891e-119">You need a valid MPN ID</span></span>|<span data-ttu-id="1891e-120">So fügen Sie [MPN](https://partner.microsoft.com/) an</span><span class="sxs-lookup"><span data-stu-id="1891e-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1891e-121">Cosell bereit</span><span class="sxs-lookup"><span data-stu-id="1891e-121">Cosell ready</span></span>|<span data-ttu-id="1891e-122">Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.</span><span class="sxs-lookup"><span data-stu-id="1891e-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1891e-123">Vertrieb mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="1891e-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1891e-124">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="1891e-124">Partner Center account</span></span>|<span data-ttu-id="1891e-125">Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="1891e-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1891e-126">Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="1891e-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="1891e-127">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="1891e-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1891e-128">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="1891e-128">Partner Center user roles</span></span>|<span data-ttu-id="1891e-129">Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.</span><span class="sxs-lookup"><span data-stu-id="1891e-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1891e-130">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="1891e-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="1891e-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="1891e-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="1891e-132">Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="1891e-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1891e-133">Zuweisen von Rollen in Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1891e-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1891e-134">Energie automatisierter Fluss Konto</span><span class="sxs-lookup"><span data-stu-id="1891e-134">Power Automate Flow Account</span></span>|<span data-ttu-id="1891e-135">Ein aktives, [Energie automatisierbares](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder den SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="1891e-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1891e-136">Dieser Benutzer sollte sich mindestens einmal vor der Installation bei der [Strom Automatisierung](https://flow.microsoft.com) anmelden.</span><span class="sxs-lookup"><span data-stu-id="1891e-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="1891e-137">Installieren der Partner Center-Synchronisierung für Dynamics 365 (Energie automatisierte Lösung)</span><span class="sxs-lookup"><span data-stu-id="1891e-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="1891e-138">Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1891e-139">In diesem Schritt werden die verfügbaren CRM-Instanzen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1891e-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1891e-140">Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="1891e-141">Wählen Sie in der linken Navigationsleiste **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1891e-142">Klicken Sie im oberen Menü auf den Link **appsource öffnen** .</span><span class="sxs-lookup"><span data-stu-id="1891e-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Appsource öffnen":::

5. <span data-ttu-id="1891e-144">Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Dynamics365** .</span><span class="sxs-lookup"><span data-stu-id="1891e-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="1891e-145">Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="1891e-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="1891e-146">Dadurch wird die Seite geöffnet, auf der Sie die CRM-Umgebung (Dynamics 365) zum Installieren der Anwendung auswählen können.</span><span class="sxs-lookup"><span data-stu-id="1891e-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="1891e-147">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="1891e-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="1891e-148">Anschließend werden Sie zur Seite **Verwalten Ihrer Lösungen** weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="1891e-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1891e-149">Navigieren Sie zu "Partner Center-Verweise", indem Sie die Pfeil Schaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="1891e-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1891e-150">Die **geplante Installation** sollte neben der Projekt Mappe für Partner Center-Verweise angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="1891e-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1891e-151">Die Installation wird 10-15 Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="1891e-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="1891e-152">Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1891e-153">Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Dynamics 365** in der Lösungs Liste verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="1891e-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1891e-154">Wählen Sie **Partner Center-Synchronisierungs Referenz für Dynamics 365 aus**.</span><span class="sxs-lookup"><span data-stu-id="1891e-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="1891e-155">Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="1891e-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Verfügbare CRMs":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1891e-157">Bewährte Vorgehensweise: testen, bevor Sie fortfahren</span><span class="sxs-lookup"><span data-stu-id="1891e-157">Best practice: test before you go live</span></span>

<span data-ttu-id="1891e-158">Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.</span><span class="sxs-lookup"><span data-stu-id="1891e-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1891e-159">Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="1891e-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="1891e-160">Erstellen Sie eine Kopie der Projekt Mappe, und führen Sie die Konfiguration aus, und führen Sie die Automatisierung der Fluss Anpassungen in der Stagingumgebung durch</span><span class="sxs-lookup"><span data-stu-id="1891e-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="1891e-161">Testen Sie die Lösung auf einer Staging/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="1891e-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="1891e-162">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktions Instanz.</span><span class="sxs-lookup"><span data-stu-id="1891e-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="1891e-163">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="1891e-163">Configure the solution</span></span>

1. <span data-ttu-id="1891e-164">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1891e-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="1891e-165">Wählen Sie in der Dropdown- **Umgebung** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.</span><span class="sxs-lookup"><span data-stu-id="1891e-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="1891e-166">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="1891e-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="1891e-167">Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen</span><span class="sxs-lookup"><span data-stu-id="1891e-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="1891e-168">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="1891e-168">Partner Center Events</span></span>

   - <span data-ttu-id="1891e-169">Der CRM-Administrator mit den Energie automatisierten Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="1891e-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="1891e-170">Wählen Sie in der linken Navigationsleiste **Verbindungen** aus, und wählen Sie die Projekt Mappe "Partner Center-Verweise" aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="1891e-171">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen** klicken.</span><span class="sxs-lookup"><span data-stu-id="1891e-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Erstellen der Verbindung":::

      3. <span data-ttu-id="1891e-173">Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .</span><span class="sxs-lookup"><span data-stu-id="1891e-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="1891e-174">Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".</span><span class="sxs-lookup"><span data-stu-id="1891e-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="1891e-175">Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.</span><span class="sxs-lookup"><span data-stu-id="1891e-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="1891e-176">Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.</span><span class="sxs-lookup"><span data-stu-id="1891e-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="1891e-177">Nachdem Sie alle Verbindungen hinzugefügt haben, sollten in Ihrer Umgebung die folgenden Verbindungen angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="1891e-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Verbindungen":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="1891e-179">Verbindungen bearbeiten</span><span class="sxs-lookup"><span data-stu-id="1891e-179">Edit the connections</span></span>

1. <span data-ttu-id="1891e-180">Kehren Sie zur Seite **Lösungen** zurück, und wählen Sie **Standard** Projekt Mappe aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="1891e-181">Wählen Sie **Verbindungs Verweis (Vorschau)** aus, indem Sie auf **alle** klicken.</span><span class="sxs-lookup"><span data-stu-id="1891e-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Herstellen einer Verbindung":::

2. <span data-ttu-id="1891e-183">Bearbeiten Sie jede der Verbindungen nacheinander, indem Sie das Symbol drei Punkte auswählen.</span><span class="sxs-lookup"><span data-stu-id="1891e-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="1891e-184">Fügen Sie die relevanten Verbindungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="1891e-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Aufgeführte Verbindungen"::: 

3.  <span data-ttu-id="1891e-186">Aktivieren Sie die Flows in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="1891e-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="1891e-187">Partner Center-webhook-Registrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1891e-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1891e-188">Erstellen einer Co-Selling-Referenz – Dynamics 365 to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1891e-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1891e-189">Partner Center Microsoft Co-Selling-Verweises Aktualisierungen an Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1891e-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="1891e-190">Partner Center auf Dynamics 365 (Insider-Vorschau)</span><span class="sxs-lookup"><span data-stu-id="1891e-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="1891e-191">Dynamics 365 to Partner Center (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="1891e-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1891e-192">Dynamics 365-Chance an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1891e-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1891e-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1891e-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="1891e-194">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="1891e-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="1891e-195">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="1891e-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="1891e-196">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="1891e-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="1891e-197">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="1891e-198">Fügen Sie Verbindungen für den (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b.) Partner Center-Veranstaltungen hinzu, wie unten gezeigt.</span><span class="sxs-lookup"><span data-stu-id="1891e-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="1891e-200">Wenn Sie diese Updates vornehmen, wird Folgendes angezeigt:</span><span class="sxs-lookup"><span data-stu-id="1891e-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="1891e-202">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="1891e-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="1891e-203">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="1891e-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="1891e-204">Wählen Sie **Partner Center auf Dynamics 365 (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="1891e-205">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="1891e-206">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="1891e-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopieren der URL":::

8. <span data-ttu-id="1891e-208">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="1891e-209">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="1891e-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="1891e-210">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="1891e-210">Enter the following details:</span></span>

    1. <span data-ttu-id="1891e-211">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="1891e-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="1891e-212">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="1891e-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="1891e-213">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="1891e-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="1891e-214">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="1891e-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="1891e-215">Der webhook kann nun auf Create-und Update-Ereignisse lauschen.</span><span class="sxs-lookup"><span data-stu-id="1891e-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="1891e-216">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="1891e-216">Customize synchronization steps</span></span>

<span data-ttu-id="1891e-217">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="1891e-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="1891e-218">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="1891e-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="1891e-219">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="1891e-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="1891e-220">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="1891e-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="1891e-221">Microsoft Partner Centers für CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="1891e-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="1891e-222">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="1891e-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="1891e-223">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="1891e-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="1891e-224">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="1891e-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="1891e-225">a.</span><span class="sxs-lookup"><span data-stu-id="1891e-225">a.</span></span> <span data-ttu-id="1891e-226">Wählen Sie Partner Center für Dynamics 365 (Insider Preview) oder Partner Center für Salesforce (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="1891e-227">b.</span><span class="sxs-lookup"><span data-stu-id="1891e-227">b.</span></span> <span data-ttu-id="1891e-228">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1891e-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="1891e-229">c.</span><span class="sxs-lookup"><span data-stu-id="1891e-229">c.</span></span> <span data-ttu-id="1891e-230">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="1891e-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="1891e-231">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Erstellungs Ereignisse aus, wenn es sich um eine **neue freigegebene Chance handelt, und**</span><span class="sxs-lookup"><span data-stu-id="1891e-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="1891e-232">Wählen Sie den unterschritt aus, **Falls ja** , und erweitern Sie dann die Option **neue Gelegenheit im CRM**.</span><span class="sxs-lookup"><span data-stu-id="1891e-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="1891e-233">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1891e-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="1891e-234">d.</span><span class="sxs-lookup"><span data-stu-id="1891e-234">d.</span></span> <span data-ttu-id="1891e-235">Zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="1891e-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="1891e-236">e.</span><span class="sxs-lookup"><span data-stu-id="1891e-236">e.</span></span> <span data-ttu-id="1891e-237">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="1891e-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="1891e-238">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="1891e-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="1891e-239">f.</span><span class="sxs-lookup"><span data-stu-id="1891e-239">f.</span></span> <span data-ttu-id="1891e-240">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="1891e-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="1891e-241">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="1891e-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="1891e-242">a.</span><span class="sxs-lookup"><span data-stu-id="1891e-242">a.</span></span> <span data-ttu-id="1891e-243">Wählen Sie **Bearbeiten**  aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1891e-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="1891e-244">b.</span><span class="sxs-lookup"><span data-stu-id="1891e-244">b.</span></span> <span data-ttu-id="1891e-245">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="1891e-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="1891e-246">c.</span><span class="sxs-lookup"><span data-stu-id="1891e-246">c.</span></span> <span data-ttu-id="1891e-247">Wenn Sie die CRM-Feld Zuordnungen für Update Ereignisse anpassen möchten, wählen Sie aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="1891e-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="1891e-248">d.</span><span class="sxs-lookup"><span data-stu-id="1891e-248">d.</span></span> <span data-ttu-id="1891e-249">Wählen Sie den unterschritt aus, **Wenn ja** , und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="1891e-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="1891e-250">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1891e-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="1891e-251">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="1891e-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="1891e-252">a.</span><span class="sxs-lookup"><span data-stu-id="1891e-252">a.</span></span> <span data-ttu-id="1891e-253">Wählen Sie **Bearbeiten**  aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1891e-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="1891e-254">b.</span><span class="sxs-lookup"><span data-stu-id="1891e-254">b.</span></span> <span data-ttu-id="1891e-255">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="1891e-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="1891e-256">c.</span><span class="sxs-lookup"><span data-stu-id="1891e-256">c.</span></span> <span data-ttu-id="1891e-257">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="1891e-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="1891e-258">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1891e-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="1891e-259">Es werden zwei Umgebungsvariablen erstellt:</span><span class="sxs-lookup"><span data-stu-id="1891e-259">There are two environment variables created:</span></span>

- <span data-ttu-id="1891e-260">Häkchen: gibt an, ob Sie neben Verkaufschancen, die bidirektional zwischen Partner Center und Dynamics 365 CRM synchronisiert werden, ein Häkchen benötigen.</span><span class="sxs-lookup"><span data-stu-id="1891e-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="1891e-261">Nur Co-Selling-Verkaufschancen synchronisieren: gibt an, ob nur Co-Selling-Verkaufschancen synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1891e-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="1891e-262">Sie können den Standardwert für die Umgebungsvariablen bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1891e-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Bearbeitungsfeld für Standardwerte":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="1891e-264">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="1891e-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="1891e-265">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="1891e-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="1891e-266">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1891e-266">Pre-requisites</span></span>

<span data-ttu-id="1891e-267">Um die Verweise auf Partner Center und Dynamics 365 CRM zu synchronisieren, werden die Microsoft-spezifischen verweigerfelder von der Energie automatisierten Lösung eindeutig abgegrenzt.</span><span class="sxs-lookup"><span data-stu-id="1891e-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="1891e-268">Diese Identifikation gibt Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="1891e-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1891e-269">Ein Satz benutzerdefinierter Felder ist als Teil der Entität " **Chance** " verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1891e-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="1891e-270">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="1891e-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="1891e-271">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="1891e-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1891e-272">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="1891e-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1891e-273">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="1891e-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1891e-274">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="1891e-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1891e-275">**Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="1891e-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1891e-276">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="1891e-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1891e-277">Überwachung **: ein** Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="1891e-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="1891e-278">Aktualisieren Sie das Verkaufschancen Formular in Dynamics 365 CRM, um Lösungen für Produkte zu enthalten.</span><span class="sxs-lookup"><span data-stu-id="1891e-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Verkaufschancen Formular":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="1891e-281">SS</span><span class="sxs-lookup"><span data-stu-id="1891e-281">SCENARIOS:</span></span>

1. <span data-ttu-id="1891e-282">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="1891e-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="1891e-283">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="1891e-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="1891e-284">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Dynamics 365-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="1891e-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Der Abschnitt &quot;Beispiel Verkaufschancen&quot; zeigt Informationen zum Microsoft Partner Center in Dynamics 365 an.":::

   3. <span data-ttu-id="1891e-286">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="1891e-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="1891e-287">**Mit Partner Center synchronisieren**: Ja</span><span class="sxs-lookup"><span data-stu-id="1891e-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="1891e-288">**Wie kann Microsoft Help?**: Wählen Sie eine der folgenden Aktionen aus:</span><span class="sxs-lookup"><span data-stu-id="1891e-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Beispiel für eine Verkaufschance in Dynamics 365, das Microsoft Partner Center-Hilfe Optionen neben einem Feld mit dem Namen &quot;wie kann Microsoft Hilfe&quot; angezeigt wird?":::

      - <span data-ttu-id="1891e-290">**Produkte**: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="1891e-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="1891e-291">Wenn die Verkaufschance in Dynamics 365 mit der Option **sync with Partner Center** auf **Ja** festgelegt ist, warten Sie 10 Minuten, und melden Sie sich dann bei Ihrem Partner Center-Konto an.</span><span class="sxs-lookup"><span data-stu-id="1891e-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="1891e-292">Ihre Verweise werden mit Dynamics 365 synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="1891e-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="1891e-293">Für eine Gelegenheit, bei der die Option "Synchronisierung mit Partner Center" auf "Ja" festgelegt wurde, werden die Änderungen bei der Aktualisierung der Gelegenheit in Dynamics 365 CRM in Ihrem Partner Center-Konto synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="1891e-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="1891e-294">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.</span><span class="sxs-lookup"><span data-stu-id="1891e-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="1891e-295">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="1891e-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="1891e-296">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="1891e-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="1891e-297">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="1891e-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="1891e-298">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="1891e-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="1891e-299">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="1891e-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="1891e-300">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="1891e-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="1891e-301">Der im Microsoft Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="1891e-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="1891e-302">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="1891e-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1891e-303">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="1891e-303">Next steps</span></span>

- [<span data-ttu-id="1891e-304">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="1891e-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1891e-305">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="1891e-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="1891e-306">Weitere Informationen zur Microsoft powerautomatisieren-Plattform</span><span class="sxs-lookup"><span data-stu-id="1891e-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="1891e-307">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="1891e-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)