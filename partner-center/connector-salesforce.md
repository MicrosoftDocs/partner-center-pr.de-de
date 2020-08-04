---
title: Der Co-Selling-Connector für das Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Ihrer Verweise in Partner Center mit Ihrem Salesforce CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4f636da49504c69c1e0e44c176fb76a4d7f8a78e
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527833"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="ecfa5-103">Co-Selling-Connector für Salesforce CRM – Übersicht</span><span class="sxs-lookup"><span data-stu-id="ecfa5-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="ecfa5-104">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-104">Appropriate roles</span></span>

- <span data-ttu-id="ecfa5-105">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="ecfa5-105">Referrals admin</span></span>
- <span data-ttu-id="ecfa5-106">Systemadministrator oder systemanpassungsprogramm im CRM</span><span class="sxs-lookup"><span data-stu-id="ecfa5-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="ecfa5-107">Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="ecfa5-108">Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="ecfa5-109">Mithilfe der Co-Selling-Connectors können Sie einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers erstellen, Referenzen vom Microsoft-Verkäufer erhalten, Verweise akzeptieren/ablehnen, Geschäftsdaten ändern, wie z. b. den Geschäftswert und das Enddatum.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="ecfa5-110">Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="ecfa5-111">Sie können alle Ihre Verweise ausführen, während Sie im CRM Ihrer Wahl arbeiten und nicht im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="ecfa5-112">Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="ecfa5-113">Vor der Installation von-Pre-Requirements</span><span class="sxs-lookup"><span data-stu-id="ecfa5-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="ecfa5-114">**Sonder**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-114">**Topics**</span></span>   |<span data-ttu-id="ecfa5-115">**Details**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-115">**Details**</span></span>   |<span data-ttu-id="ecfa5-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="ecfa5-117">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="ecfa5-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="ecfa5-118">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-118">You need a valid MPN ID</span></span>|<span data-ttu-id="ecfa5-119">So fügen Sie [MPN](https://partner.microsoft.com/) an</span><span class="sxs-lookup"><span data-stu-id="ecfa5-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="ecfa5-120">Co-Selling bereit</span><span class="sxs-lookup"><span data-stu-id="ecfa5-120">Co-sell ready</span></span>|<span data-ttu-id="ecfa5-121">Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="ecfa5-122">Vertrieb mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="ecfa5-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="ecfa5-123">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="ecfa5-123">Partner Center account</span></span>|<span data-ttu-id="ecfa5-124">Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="ecfa5-125">Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="ecfa5-126">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="ecfa5-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ecfa5-127">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-127">Partner Center user roles</span></span>|<span data-ttu-id="ecfa5-128">Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="ecfa5-129">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="ecfa5-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ecfa5-130">Salesforce-CRM</span><span class="sxs-lookup"><span data-stu-id="ecfa5-130">Salesforce CRM</span></span>|<span data-ttu-id="ecfa5-131">Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="ecfa5-132">Zuweisen von Rollen in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ecfa5-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="ecfa5-133">Energie automatisierter Fluss Konto</span><span class="sxs-lookup"><span data-stu-id="ecfa5-133">Power Automate Flow Account</span></span>|<span data-ttu-id="ecfa5-134">Ein aktives, [Energie automatisierbares](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder den SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="ecfa5-135">Dieser Benutzer sollte sich mindestens einmal vor der Installation bei der [Strom Automatisierung](https://flow.microsoft.com) anmelden.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="ecfa5-136">Installieren der Partner Center-Synchronisierung für Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ecfa5-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="ecfa5-137">Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="ecfa5-138">Dadurch werden die verfügbaren CRM-Instanzen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="ecfa5-139">Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="ecfa5-140">Wählen Sie in der linken Navigationsleiste **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="ecfa5-141">Klicken Sie im oberen Menü auf den Link **appsource öffnen** .</span><span class="sxs-lookup"><span data-stu-id="ecfa5-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Appsource öffnen":::

5. <span data-ttu-id="ecfa5-143">Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="ecfa5-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="ecfa5-145">Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="ecfa5-146">Daraufhin wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung zum Installieren der Anwendung auswählen können.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="ecfa5-147">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Verfügbare CRMs":::

8. <span data-ttu-id="ecfa5-149">Anschließend werden Sie zur Seite **Verwalten Ihrer Lösungen** weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="ecfa5-150">Navigieren Sie zu "Partner Center-Verweise", indem Sie die Pfeil Schaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="ecfa5-151">Die **geplante Installation** sollte neben der Projekt Mappe für Partner Center-Verweise angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="ecfa5-152">Die Installation wird 10-15 Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="ecfa5-153">Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="ecfa5-154">Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Salesforce** in der Lösungs Liste verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="ecfa5-155">Wählen Sie die **Synchronisierung der Partner Center-Verweise für Salesforce aus**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="ecfa5-156">Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce-Flows":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="ecfa5-158">Bewährte Vorgehensweise: testen, bevor Sie fortfahren</span><span class="sxs-lookup"><span data-stu-id="ecfa5-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="ecfa5-159">Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="ecfa5-160">Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="ecfa5-161">Erstellen Sie eine Kopie der Projekt Mappe, und führen Sie die Konfiguration aus, und führen Sie die Automatisierung der Fluss Anpassungen in der Stagingumgebung durch</span><span class="sxs-lookup"><span data-stu-id="ecfa5-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="ecfa5-162">Testen Sie die Lösung auf einer Staging/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="ecfa5-163">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktions Instanz.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="ecfa5-164">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="ecfa5-164">Configure the solution</span></span>

1. <span data-ttu-id="ecfa5-165">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="ecfa5-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="ecfa5-166">Wählen Sie in der Dropdown- **Umgebung** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="ecfa5-167">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="ecfa5-168">Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="ecfa5-169">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="ecfa5-169">Partner Center Events</span></span>
   - <span data-ttu-id="ecfa5-170">Der CRM-Administrator mit den Energie automatisierten Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="ecfa5-171">Wählen Sie in der linken Navigationsleiste **Verbindungen** aus, und wählen Sie die Projekt Mappe "Partner Center-Verweise" aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="ecfa5-172">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen**klicken.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Erstellen der Verbindung":::

   3. <span data-ttu-id="ecfa5-174">Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .</span><span class="sxs-lookup"><span data-stu-id="ecfa5-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="ecfa5-175">Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".</span><span class="sxs-lookup"><span data-stu-id="ecfa5-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="ecfa5-176">Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="ecfa5-177">Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="ecfa5-178">Um die Strom automatisierten Flows den Verbindungen zuzuordnen, bearbeiten Sie jeden der Strom automatisierten Flows, um eine Verbindung mit Common Data Service-und Partner Center-Referenzen herzustellen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="ecfa5-179">Speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-179">Save the changes.</span></span>

5. <span data-ttu-id="ecfa5-180">**Schalten** Sie die Strom automatisierten Flows ein.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="ecfa5-181">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="ecfa5-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="ecfa5-182">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="ecfa5-183">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="ecfa5-184">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="ecfa5-185">Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt</span><span class="sxs-lookup"><span data-stu-id="ecfa5-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="ecfa5-187">Wenn Sie diese Updates vornehmen, wird Folgendes angezeigt:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="ecfa5-189">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="ecfa5-190">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="ecfa5-191">Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="ecfa5-192">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="ecfa5-193">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieren der URL":::

8. <span data-ttu-id="ecfa5-195">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="ecfa5-196">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="ecfa5-197">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-197">Enter the following details:</span></span>

    1. <span data-ttu-id="ecfa5-198">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="ecfa5-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="ecfa5-199">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="ecfa5-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="ecfa5-200">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="ecfa5-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="ecfa5-201">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="ecfa5-202">Der webhook kann nun auf Create-und Update-Ereignisse lauschen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="ecfa5-203">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-203">Customize synchronization steps</span></span>

<span data-ttu-id="ecfa5-204">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="ecfa5-205">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="ecfa5-206">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="ecfa5-207">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="ecfa5-208">Microsoft Partner Centers für CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="ecfa5-209">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="ecfa5-210">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="ecfa5-211">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="ecfa5-212">Wählen Sie Partner Center zu Salesforce CRM (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="ecfa5-213">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="ecfa5-214">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="ecfa5-215">**Wenn Sie die CRM-** Feld Zuordnungen für Erstellungs Ereignisse anpassen möchten, wählen Sie aus, ob es sich um eine neue Freigabe Chance handelt</span><span class="sxs-lookup"><span data-stu-id="ecfa5-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="ecfa5-216">Wählen Sie den untergeordneten **Schritt** aus, und erweitern Sie dann die Option **Erstellen einer neuen Verkaufschance im CRM**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="ecfa5-217">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="ecfa5-218">Zum Anpassen von CRM-Feld Zuordnungen für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="ecfa5-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="ecfa5-219">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="ecfa5-220">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="ecfa5-221">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="ecfa5-222">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="ecfa5-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="ecfa5-223">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ecfa5-224">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="ecfa5-225">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="ecfa5-226">Wählen Sie den unterschritt aus, **Wenn ja** , und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="ecfa5-227">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="ecfa5-228">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="ecfa5-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="ecfa5-229">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ecfa5-230">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="ecfa5-231">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="ecfa5-232">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="ecfa5-233">Erstellen eines separaten Abschnitts im Salesforce-CRM-Verkaufschancen Layout</span><span class="sxs-lookup"><span data-stu-id="ecfa5-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="ecfa5-234">Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="ecfa5-235">Dies bietet Ihren Verkäufer Teams die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="ecfa5-236">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM-Verkaufs **Chancen** Entität verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="ecfa5-237">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="ecfa5-238">Der Salesforce CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt erstellen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="ecfa5-239">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="ecfa5-240">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="ecfa5-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="ecfa5-241">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="ecfa5-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="ecfa5-242">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="ecfa5-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="ecfa5-243">**Wie kann Microsoft helfen?**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-243">**How can Microsoft help?**</span></span> <span data-ttu-id="ecfa5-244">Von Microsoft für den Verweis erforderliche Hilfe</span><span class="sxs-lookup"><span data-stu-id="ecfa5-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="ecfa5-245">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="ecfa5-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="ecfa5-246">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit dem Microsoft Partner Center-Verweis</span><span class="sxs-lookup"><span data-stu-id="ecfa5-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="ecfa5-247">Einrichten von Feldern und Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="ecfa5-248">Melden **Sie sich bei**Ihrem Salesforce-Konto an.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="ecfa5-249">Klicken Sie auf die Optionen **Setup** und **Objekt bearbeiten** , um die erforderlichen Felder hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="ecfa5-250">**Felder & Beziehungen** im linken Navigationsbereich auswählen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Felder":::

4. <span data-ttu-id="ecfa5-252">Fügen Sie die folgenden Felder in den **Feldern & Beziehungs** Tabelle hinzu:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="ecfa5-253">**Feld Bezeichnung**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-253">**Field label**</span></span>   |<span data-ttu-id="ecfa5-254">**Feldname**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-254">**Field name**</span></span>|<span data-ttu-id="ecfa5-255">**Datentyp**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-255">**Data type**</span></span>|<span data-ttu-id="ecfa5-256">**Zierenden**</span><span class="sxs-lookup"><span data-stu-id="ecfa5-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="ecfa5-257">Audit</span><span class="sxs-lookup"><span data-stu-id="ecfa5-257">Audit</span></span>| <span data-ttu-id="ecfa5-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="ecfa5-258">Audit__c</span></span>|<span data-ttu-id="ecfa5-259">Long-Text Bereich (100000) (sichtbare Zeile 4)</span><span class="sxs-lookup"><span data-stu-id="ecfa5-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="ecfa5-260">Wie kann Microsoft helfen?</span><span class="sxs-lookup"><span data-stu-id="ecfa5-260">How can Microsoft help?</span></span>|<span data-ttu-id="ecfa5-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="ecfa5-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="ecfa5-262">Auswahlliste</span><span class="sxs-lookup"><span data-stu-id="ecfa5-262">Picklist\*</span></span>|
   |<span data-ttu-id="ecfa5-263">Produkte</span><span class="sxs-lookup"><span data-stu-id="ecfa5-263">Products</span></span>|<span data-ttu-id="ecfa5-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="ecfa5-264">Products_c</span></span>|<span data-ttu-id="ecfa5-265">Text (255)</span><span class="sxs-lookup"><span data-stu-id="ecfa5-265">text (255)</span></span>||
   |<span data-ttu-id="ecfa5-266">Referral</span><span class="sxs-lookup"><span data-stu-id="ecfa5-266">Referral</span></span> | <span data-ttu-id="ecfa5-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="ecfa5-267">Referral_Identfier_c</span></span>|<span data-ttu-id="ecfa5-268">Text (100) (externe ID)</span><span class="sxs-lookup"><span data-stu-id="ecfa5-268">Text(100)(External ID)</span></span>|<span data-ttu-id="ecfa5-269">ja</span><span class="sxs-lookup"><span data-stu-id="ecfa5-269">yes</span></span>|
   |<span data-ttu-id="ecfa5-270">Verweis Link</span><span class="sxs-lookup"><span data-stu-id="ecfa5-270">Referral Link</span></span>| <span data-ttu-id="ecfa5-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="ecfa5-271">Referral_Link_c_</span></span>|<span data-ttu-id="ecfa5-272">URL (255)</span><span class="sxs-lookup"><span data-stu-id="ecfa5-272">URL(255)</span></span>||
   |<span data-ttu-id="ecfa5-273">Mit Partner Center synchronisieren</span><span class="sxs-lookup"><span data-stu-id="ecfa5-273">Sync with Partner Center</span></span>|<span data-ttu-id="ecfa5-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="ecfa5-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="ecfa5-275">CheckBox (Standardeinstellung deaktiviert)</span><span class="sxs-lookup"><span data-stu-id="ecfa5-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="ecfa5-276">\* Picklist-Werte:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-276">\*Picklist values:</span></span>

   - <span data-ttu-id="ecfa5-277">Auslastungs spezifischer Wert-Vorschlag</span><span class="sxs-lookup"><span data-stu-id="ecfa5-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="ecfa5-278">Technische Kunden Architektur</span><span class="sxs-lookup"><span data-stu-id="ecfa5-278">Customer technical architecture</span></span>
   - <span data-ttu-id="ecfa5-279">Proof of Concept oder Demo</span><span class="sxs-lookup"><span data-stu-id="ecfa5-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="ecfa5-280">Anführungszeichen oder Lizenzierung</span><span class="sxs-lookup"><span data-stu-id="ecfa5-280">Quotes or licensing</span></span>
   - <span data-ttu-id="ecfa5-281">Kunden Erfolg nach dem Verkauf</span><span class="sxs-lookup"><span data-stu-id="ecfa5-281">Post sales customer success</span></span>
   - <span data-ttu-id="ecfa5-282">Allgemein oder andere</span><span class="sxs-lookup"><span data-stu-id="ecfa5-282">General or other</span></span>

5. <span data-ttu-id="ecfa5-283">Die Felder werden unter " **Felder & Beziehungen** " erstellt.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Erstellte Felder":::

6. <span data-ttu-id="ecfa5-285">Erstellen Sie im Layout der Verkaufschancen einen separaten Abschnitt mit den oben aufgeführten Feldern.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="ecfa5-286">Dieser Abschnitt sollte für die Verkäufer im Verkaufschancen Layout verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Layout der Partner Center-Felder":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="ecfa5-288">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="ecfa5-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="ecfa5-289">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Salesforce CRM und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="ecfa5-290">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-290">Pre-requisites</span></span>

<span data-ttu-id="ecfa5-291">Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="ecfa5-292">Diese Identifikation bietet Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="ecfa5-293">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM Solution **Opportunity** -Entität verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="ecfa5-294">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="ecfa5-295">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="ecfa5-296">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="ecfa5-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="ecfa5-297">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="ecfa5-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="ecfa5-298">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="ecfa5-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="ecfa5-299">**Wie kann Microsoft Help**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="ecfa5-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="ecfa5-300">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="ecfa5-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="ecfa5-301">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="ecfa5-302">SS</span><span class="sxs-lookup"><span data-stu-id="ecfa5-302">SCENARIOS:</span></span>

1. <span data-ttu-id="ecfa5-303">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="ecfa5-304">Melden Sie sich bei ihrer Salesforce CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="ecfa5-305">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-Umgebung":::

   3. <span data-ttu-id="ecfa5-307">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="ecfa5-308">"Mit Partner Center synchronisieren": Ja</span><span class="sxs-lookup"><span data-stu-id="ecfa5-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="ecfa5-309">"Wie kann Microsoft Help?": Wählen Sie eine der folgenden Optionen aus:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="ecfa5-310">Produkte: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="ecfa5-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="ecfa5-311">Nachdem Sie die Option für die Verkaufschancen **Synchronisierung mit Partner Center** auf **Ja**festgelegt haben, können Sie sich bei Ihrem Partner Center-Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="ecfa5-312">Ihre Verweise werden mit Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="ecfa5-313">Wenn die Option "Sync with Partner Center" auf "yes" festgelegt ist, werden die Änderungen, wenn Sie die Verkaufschance in Salesforce CRM aktualisieren, mit Ihrem Partner Center-Konto synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="ecfa5-314">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Salesforce CRM identifiziert.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="ecfa5-315">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="ecfa5-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="ecfa5-316">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="ecfa5-317">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="ecfa5-318">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="ecfa5-319">Melden Sie sich bei ihrer Salesforce CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="ecfa5-320">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="ecfa5-321">Der im Microsoft Partner Center erstellte Verweis ist nun in Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce-Verkaufschancen Bildschirm":::

    6. <span data-ttu-id="ecfa5-323">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="ecfa5-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ecfa5-324">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ecfa5-324">Next steps</span></span>

- [<span data-ttu-id="ecfa5-325">Weitere Informationen zur Microsoft powerautomatisieren-Plattform</span><span class="sxs-lookup"><span data-stu-id="ecfa5-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="ecfa5-326">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="ecfa5-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="ecfa5-327">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="ecfa5-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="ecfa5-328">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="ecfa5-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)