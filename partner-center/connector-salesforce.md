---
title: Der Co-Selling-Connector für das Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Ihrer Verweise in Partner Center mit Ihrem Salesforce CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145104"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="bed2f-103">Co-Selling-Connector für Salesforce CRM-Übersicht</span><span class="sxs-lookup"><span data-stu-id="bed2f-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="bed2f-104">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="bed2f-104">Appropriate roles</span></span>

- <span data-ttu-id="bed2f-105">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="bed2f-105">Referrals admin</span></span>
- <span data-ttu-id="bed2f-106">Systemadministrator oder systemanpassungsprogramm im CRM</span><span class="sxs-lookup"><span data-stu-id="bed2f-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="bed2f-107">Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme.</span><span class="sxs-lookup"><span data-stu-id="bed2f-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="bed2f-108">Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden.</span><span class="sxs-lookup"><span data-stu-id="bed2f-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="bed2f-109">Mithilfe der Co-Selling-Connectors können Sie einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers erstellen, Referenzen vom Microsoft-Verkäufer erhalten, Verweise akzeptieren/ablehnen, Geschäftsdaten ändern, wie z. b. den Geschäftswert und das Enddatum.</span><span class="sxs-lookup"><span data-stu-id="bed2f-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="bed2f-110">Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten.</span><span class="sxs-lookup"><span data-stu-id="bed2f-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="bed2f-111">Sie können alle Ihre Verweise ausführen, während Sie im CRM Ihrer Wahl arbeiten und nicht im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="bed2f-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="bed2f-112">Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="bed2f-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="bed2f-113">Vor der Installation von-Pre-Requirements</span><span class="sxs-lookup"><span data-stu-id="bed2f-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="bed2f-114">**Themen**</span><span class="sxs-lookup"><span data-stu-id="bed2f-114">**Topics**</span></span>   |<span data-ttu-id="bed2f-115">**Details**</span><span class="sxs-lookup"><span data-stu-id="bed2f-115">**Details**</span></span>   |<span data-ttu-id="bed2f-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="bed2f-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="bed2f-117">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="bed2f-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="bed2f-118">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="bed2f-118">You need a valid MPN ID</span></span>|<span data-ttu-id="bed2f-119">So fügen Sie [MPN](https://partner.microsoft.com/) an</span><span class="sxs-lookup"><span data-stu-id="bed2f-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="bed2f-120">Co-Selling bereit</span><span class="sxs-lookup"><span data-stu-id="bed2f-120">Co-sell ready</span></span>|<span data-ttu-id="bed2f-121">Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.</span><span class="sxs-lookup"><span data-stu-id="bed2f-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="bed2f-122">Vertrieb mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="bed2f-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="bed2f-123">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="bed2f-123">Partner Center account</span></span>|<span data-ttu-id="bed2f-124">Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="bed2f-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="bed2f-125">Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="bed2f-126">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="bed2f-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="bed2f-127">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="bed2f-127">Partner Center user roles</span></span>|<span data-ttu-id="bed2f-128">Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.</span><span class="sxs-lookup"><span data-stu-id="bed2f-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="bed2f-129">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="bed2f-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="bed2f-130">Salesforce-CRM</span><span class="sxs-lookup"><span data-stu-id="bed2f-130">Salesforce CRM</span></span>|<span data-ttu-id="bed2f-131">Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="bed2f-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="bed2f-132">Zuweisen von Rollen in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="bed2f-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="bed2f-133">Energie automatisierter Fluss Konto</span><span class="sxs-lookup"><span data-stu-id="bed2f-133">Power Automate Flow Account</span></span>|<span data-ttu-id="bed2f-134">Ein aktives, [Energie automatisierbares](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder den SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="bed2f-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="bed2f-135">Dieser Benutzer sollte sich mindestens einmal vor der Installation bei der [Strom Automatisierung](https://flow.microsoft.com) anmelden.</span><span class="sxs-lookup"><span data-stu-id="bed2f-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="bed2f-136">Installieren der Partner Center-Synchronisierung für Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="bed2f-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="bed2f-137">Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="bed2f-138">Dadurch werden die verfügbaren CRM-Instanzen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="bed2f-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="bed2f-139">Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="bed2f-140">Wählen Sie in der linken Navigationsleiste **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="bed2f-141">Klicken Sie im oberen Menü auf den Link **appsource öffnen** .</span><span class="sxs-lookup"><span data-stu-id="bed2f-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Appsource öffnen](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="bed2f-143">Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="bed2f-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

![Salesforce](images/salesforce/salesforce1.png)

6. <span data-ttu-id="bed2f-145">Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-145">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="bed2f-146">Daraufhin wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung zum Installieren der Anwendung auswählen können.</span><span class="sxs-lookup"><span data-stu-id="bed2f-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="bed2f-147">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="bed2f-147">Agree to terms and conditions.</span></span>

![Verfügbare CRMs](images/salesforce/available-crm.png)

8. <span data-ttu-id="bed2f-149">Anschließend werden Sie zur Seite **Verwalten Ihrer Lösungen** weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="bed2f-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="bed2f-150">Navigieren Sie zu "Partner Center-Verweise", indem Sie die Pfeil Schaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="bed2f-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="bed2f-151">Die **geplante Installation** sollte neben der Projekt Mappe für Partner Center-Verweise angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="bed2f-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="bed2f-152">Die Installation wird 10-15 Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="bed2f-152">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="bed2f-153">Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="bed2f-154">Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Salesforce** in der Lösungs Liste verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="bed2f-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="bed2f-155">Wählen Sie die **Synchronisierung der Partner Center-Verweise für Salesforce aus**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="bed2f-156">Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="bed2f-156">The following Power Automate flows and entities are available:</span></span>

![Salesforce-Flows](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="bed2f-158">Bewährte Vorgehensweise: testen, bevor Sie fortfahren</span><span class="sxs-lookup"><span data-stu-id="bed2f-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="bed2f-159">Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="bed2f-160">Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="bed2f-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="bed2f-161">Erstellen Sie eine Kopie der Projekt Mappe, und führen Sie die Konfiguration aus, und führen Sie die Automatisierung der Fluss Anpassungen in der Stagingumgebung durch</span><span class="sxs-lookup"><span data-stu-id="bed2f-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="bed2f-162">Testen Sie die Lösung auf einer Staging/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="bed2f-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="bed2f-163">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktions Instanz.</span><span class="sxs-lookup"><span data-stu-id="bed2f-163">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="bed2f-164">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="bed2f-164">Configure the solution</span></span>

1. <span data-ttu-id="bed2f-165">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="bed2f-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="bed2f-166">Wählen Sie in der Dropdown- **Umgebung** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.</span><span class="sxs-lookup"><span data-stu-id="bed2f-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="bed2f-167">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="bed2f-167">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="bed2f-168">Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen</span><span class="sxs-lookup"><span data-stu-id="bed2f-168">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="bed2f-169">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="bed2f-169">Partner Center Events</span></span>
- <span data-ttu-id="bed2f-170">Der CRM-Administrator mit den Energie automatisierten Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="bed2f-170">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="bed2f-171">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-171">a.</span></span> <span data-ttu-id="bed2f-172">Wählen Sie in der linken Navigationsleiste **Verbindungen** aus, und wählen Sie die Projekt Mappe "Partner Center-Verweise" aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-172">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="bed2f-173">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-173">b.</span></span> <span data-ttu-id="bed2f-174">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen**klicken.</span><span class="sxs-lookup"><span data-stu-id="bed2f-174">Create a connection by clicking **Create a connection**.</span></span> 

    ![Erstellen der Verbindung](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="bed2f-176">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-176">c.</span></span> <span data-ttu-id="bed2f-177">Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .</span><span class="sxs-lookup"><span data-stu-id="bed2f-177">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

    <span data-ttu-id="bed2f-178">d.</span><span class="sxs-lookup"><span data-stu-id="bed2f-178">d.</span></span> <span data-ttu-id="bed2f-179">Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".</span><span class="sxs-lookup"><span data-stu-id="bed2f-179">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="bed2f-180">e.</span><span class="sxs-lookup"><span data-stu-id="bed2f-180">e.</span></span> <span data-ttu-id="bed2f-181">Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.</span><span class="sxs-lookup"><span data-stu-id="bed2f-181">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>
    
    <span data-ttu-id="bed2f-182">f.</span><span class="sxs-lookup"><span data-stu-id="bed2f-182">f.</span></span> <span data-ttu-id="bed2f-183">Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.</span><span class="sxs-lookup"><span data-stu-id="bed2f-183">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="bed2f-184">Um die Strom automatisierten Flows den Verbindungen zuzuordnen, bearbeiten Sie jeden der Strom automatisierten Flows, um eine Verbindung mit Common Data Service-und Partner Center-Referenzen herzustellen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-184">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="bed2f-185">Speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-185">Save the changes.</span></span>

5. <span data-ttu-id="bed2f-186">**Schalten** Sie die Strom automatisierten Flows ein.</span><span class="sxs-lookup"><span data-stu-id="bed2f-186">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="bed2f-187">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="bed2f-187">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="bed2f-188">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="bed2f-188">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="bed2f-189">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="bed2f-189">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="bed2f-190">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-190">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="bed2f-191">Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt</span><span class="sxs-lookup"><span data-stu-id="bed2f-191">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Trigger](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="bed2f-193">Wenn Sie diese Updates vornehmen, wird Folgendes angezeigt:</span><span class="sxs-lookup"><span data-stu-id="bed2f-193">When you make these updates, you'll see</span></span>

![webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="bed2f-195">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-195">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="bed2f-196">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="bed2f-196">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="bed2f-197">Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-197">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="bed2f-198">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-198">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="bed2f-199">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="bed2f-199">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Kopieren der URL](images/salesforce/copy-url.png)

8. <span data-ttu-id="bed2f-201">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-201">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="bed2f-202">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-202">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="bed2f-203">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="bed2f-203">Enter the following details:</span></span> 

    <span data-ttu-id="bed2f-204">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-204">a.</span></span> <span data-ttu-id="bed2f-205">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="bed2f-205">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="bed2f-206">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-206">b.</span></span> <span data-ttu-id="bed2f-207">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="bed2f-207">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="bed2f-208">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-208">c.</span></span> <span data-ttu-id="bed2f-209">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="bed2f-209">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="bed2f-210">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="bed2f-210">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="bed2f-211">Der webhook kann nun auf Create-und Update-Ereignisse lauschen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-211">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="bed2f-212">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="bed2f-212">Customize synchronization steps</span></span>

<span data-ttu-id="bed2f-213">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="bed2f-213">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="bed2f-214">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="bed2f-214">Often CRM systems are highly customized.</span></span> <span data-ttu-id="bed2f-215">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-215">You can customize the Power Automate flows.</span></span> <span data-ttu-id="bed2f-216">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="bed2f-216">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="bed2f-217">Microsoft Partner Centers für CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-217">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="bed2f-218">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="bed2f-218">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="bed2f-219">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="bed2f-219">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="bed2f-220">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="bed2f-220">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="bed2f-221">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-221">a.</span></span> <span data-ttu-id="bed2f-222">Wählen Sie Partner Center zu Salesforce CRM (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-222">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

    <span data-ttu-id="bed2f-223">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-223">b.</span></span> <span data-ttu-id="bed2f-224">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-224">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="bed2f-225">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-225">c.</span></span> <span data-ttu-id="bed2f-226">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-226">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="bed2f-227">**Wenn Sie die CRM-** Feld Zuordnungen für Erstellungs Ereignisse anpassen möchten, wählen Sie aus, ob es sich um eine neue Freigabe Chance handelt</span><span class="sxs-lookup"><span data-stu-id="bed2f-227">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="bed2f-228">Wählen Sie den untergeordneten **Schritt** aus, und erweitern Sie dann die Option **Erstellen einer neuen Verkaufschance im CRM**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-228">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="bed2f-229">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="bed2f-229">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="bed2f-230">d.</span><span class="sxs-lookup"><span data-stu-id="bed2f-230">d.</span></span> <span data-ttu-id="bed2f-231">Zum Anpassen von CRM-Feld Zuordnungen für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="bed2f-231">To customize CRM field mappings for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="bed2f-232">e.</span><span class="sxs-lookup"><span data-stu-id="bed2f-232">e.</span></span> <span data-ttu-id="bed2f-233">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-233">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="bed2f-234">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-234">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="bed2f-235">f.</span><span class="sxs-lookup"><span data-stu-id="bed2f-235">f.</span></span> <span data-ttu-id="bed2f-236">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="bed2f-236">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="bed2f-237">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="bed2f-237">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="bed2f-238">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-238">a.</span></span> <span data-ttu-id="bed2f-239">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="bed2f-240">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-240">b.</span></span> <span data-ttu-id="bed2f-241">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-241">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="bed2f-242">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-242">c.</span></span> <span data-ttu-id="bed2f-243">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-243">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="bed2f-244">d.</span><span class="sxs-lookup"><span data-stu-id="bed2f-244">d.</span></span> <span data-ttu-id="bed2f-245">Wählen Sie den unterschritt aus, **Wenn ja** , und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-245">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="bed2f-246">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="bed2f-246">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="bed2f-247">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="bed2f-247">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="bed2f-248">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-248">a.</span></span> <span data-ttu-id="bed2f-249">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-249">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="bed2f-250">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-250">b.</span></span> <span data-ttu-id="bed2f-251">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="bed2f-251">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="bed2f-252">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-252">c.</span></span> <span data-ttu-id="bed2f-253">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-253">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="bed2f-254">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="bed2f-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="bed2f-255">Erstellen eines separaten Abschnitts im Salesforce-CRM-Verkaufschancen Layout</span><span class="sxs-lookup"><span data-stu-id="bed2f-255">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="bed2f-256">Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-256">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="bed2f-257">Dies bietet Ihren Verkäufer Teams die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="bed2f-257">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="bed2f-258">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM-Verkaufs **Chancen** Entität verfügbar.</span><span class="sxs-lookup"><span data-stu-id="bed2f-258">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="bed2f-259">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="bed2f-260">Der Salesforce CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt erstellen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-260">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="bed2f-261">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="bed2f-261">The following custom fields should be part of the CRM section:</span></span>

<span data-ttu-id="bed2f-262">• **Synchronisieren mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="bed2f-262">• **Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

<span data-ttu-id="bed2f-263">• **Referenz Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="bed2f-263">• **Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

<span data-ttu-id="bed2f-264">• **Referenz Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="bed2f-264">• **Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

<span data-ttu-id="bed2f-265">• **Wie kann Microsoft helfen?**</span><span class="sxs-lookup"><span data-stu-id="bed2f-265">• **How can Microsoft help?**</span></span> <span data-ttu-id="bed2f-266">Von Microsoft für den Verweis erforderliche Hilfe</span><span class="sxs-lookup"><span data-stu-id="bed2f-266">Help required from Microsoft for the referral</span></span>

<span data-ttu-id="bed2f-267">• **Produkte**: Liste der Produkte, die mit dieser Verkaufschance verknüpft sind</span><span class="sxs-lookup"><span data-stu-id="bed2f-267">• **Products**: List of products associated with this opportunity</span></span>

<span data-ttu-id="bed2f-268">• **Audit**: ein Schreib geschützter Überwachungs Pfad für die Synchronisierung mit dem Microsoft Partner Center-Verweis</span><span class="sxs-lookup"><span data-stu-id="bed2f-268">• **Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="bed2f-269">Einrichten von Feldern und Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bed2f-269">Set up fields and relationships</span></span>

1. <span data-ttu-id="bed2f-270">Melden **Sie sich bei**Ihrem Salesforce-Konto an.</span><span class="sxs-lookup"><span data-stu-id="bed2f-270">Sign into your Salesforce account and go to **Opportunity**.</span></span> 

2. <span data-ttu-id="bed2f-271">Klicken Sie auf die Optionen **Setup** und **Objekt bearbeiten** , um die erforderlichen Felder hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-271">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>


3. <span data-ttu-id="bed2f-272">**Felder & Beziehungen** im linken Navigationsbereich auswählen</span><span class="sxs-lookup"><span data-stu-id="bed2f-272">Select **Fields & Relationships** from the left navigation</span></span>

![Felder](images/salesforce/fields1.png)

4. <span data-ttu-id="bed2f-274">Fügen Sie die folgenden Felder in der Tabelle "Felder & Beziehung" hinzu:</span><span class="sxs-lookup"><span data-stu-id="bed2f-274">Add the following fields in the “Fields & Relationship” table:</span></span>

|<span data-ttu-id="bed2f-275">**Feld Bezeichnung**</span><span class="sxs-lookup"><span data-stu-id="bed2f-275">**Field label**</span></span>   |<span data-ttu-id="bed2f-276">**Feldname**</span><span class="sxs-lookup"><span data-stu-id="bed2f-276">**Field name**</span></span>|<span data-ttu-id="bed2f-277">**Datentyp**</span><span class="sxs-lookup"><span data-stu-id="bed2f-277">**Data type**</span></span>|<span data-ttu-id="bed2f-278">**Zierenden**</span><span class="sxs-lookup"><span data-stu-id="bed2f-278">**Indexed**</span></span>|
|---------------------|:-------------------|:--------------|:----------------|
|<span data-ttu-id="bed2f-279">Mit Partner Center synchronisieren</span><span class="sxs-lookup"><span data-stu-id="bed2f-279">Sync with Partner Center</span></span>|<span data-ttu-id="bed2f-280">Sync-with-Partner-Center-c</span><span class="sxs-lookup"><span data-stu-id="bed2f-280">sync-with-partner-center-c</span></span>|<span data-ttu-id="bed2f-281">CheckBox (Standardeinstellung deaktiviert)</span><span class="sxs-lookup"><span data-stu-id="bed2f-281">Checkbox (default unchecked)</span></span>||
|<span data-ttu-id="bed2f-282">Produkte</span><span class="sxs-lookup"><span data-stu-id="bed2f-282">Products</span></span>|<span data-ttu-id="bed2f-283">Produkte-c</span><span class="sxs-lookup"><span data-stu-id="bed2f-283">Products-c</span></span>|<span data-ttu-id="bed2f-284">Text (255)</span><span class="sxs-lookup"><span data-stu-id="bed2f-284">text (255)</span></span>||
|<span data-ttu-id="bed2f-285">Referral</span><span class="sxs-lookup"><span data-stu-id="bed2f-285">Referral</span></span> | <span data-ttu-id="bed2f-286">Referral_Identifier__c</span><span class="sxs-lookup"><span data-stu-id="bed2f-286">Referral_Identifier__c</span></span>|<span data-ttu-id="bed2f-287">Text (100) (externe ID)</span><span class="sxs-lookup"><span data-stu-id="bed2f-287">Text(100)(External ID)</span></span>|<span data-ttu-id="bed2f-288">ja</span><span class="sxs-lookup"><span data-stu-id="bed2f-288">yes</span></span>|
|<span data-ttu-id="bed2f-289">Verweis Link</span><span class="sxs-lookup"><span data-stu-id="bed2f-289">Referral Link</span></span>| <span data-ttu-id="bed2f-290">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="bed2f-290">Referral_Link__c_</span></span>|<span data-ttu-id="bed2f-291">URL (255)</span><span class="sxs-lookup"><span data-stu-id="bed2f-291">URL(255)</span></span>||
|<span data-ttu-id="bed2f-292">Audit</span><span class="sxs-lookup"><span data-stu-id="bed2f-292">Audit</span></span>| <span data-ttu-id="bed2f-293">Audit__c</span><span class="sxs-lookup"><span data-stu-id="bed2f-293">Audit__c</span></span>|<span data-ttu-id="bed2f-294">Long-Text Bereich (100000) (sichtbare Zeile 4)</span><span class="sxs-lookup"><span data-stu-id="bed2f-294">Long Text Area(100000)(visible line 4)</span></span>||
|<span data-ttu-id="bed2f-295">Wie kann Microsoft helfen?</span><span class="sxs-lookup"><span data-stu-id="bed2f-295">How can Microsoft help?</span></span>|<span data-ttu-id="bed2f-296">How_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="bed2f-296">How_can_Microsoft_help__c</span></span>|<span data-ttu-id="bed2f-297">Auswahlliste</span><span class="sxs-lookup"><span data-stu-id="bed2f-297">Picklist\*</span></span>|

<span data-ttu-id="bed2f-298">\* Picklist-Werte:</span><span class="sxs-lookup"><span data-stu-id="bed2f-298">\*Picklist values:</span></span>

<span data-ttu-id="bed2f-299">• Arbeits Auslastungs spezifischer Wertbeitrag</span><span class="sxs-lookup"><span data-stu-id="bed2f-299">• Workload specific value proposition</span></span>

<span data-ttu-id="bed2f-300">• Technische Kunden Architektur</span><span class="sxs-lookup"><span data-stu-id="bed2f-300">• Customer technical architecture</span></span>

<span data-ttu-id="bed2f-301">• Proof of Concept oder Demo</span><span class="sxs-lookup"><span data-stu-id="bed2f-301">• Proof of concept or demo</span></span>

<span data-ttu-id="bed2f-302">• Anführungszeichen oder Lizenzierung</span><span class="sxs-lookup"><span data-stu-id="bed2f-302">• Quotes or licensing</span></span>

<span data-ttu-id="bed2f-303">• Kunden Erfolg nach dem Verkauf</span><span class="sxs-lookup"><span data-stu-id="bed2f-303">• Post sales customer success</span></span>

<span data-ttu-id="bed2f-304">• Allgemein oder andere</span><span class="sxs-lookup"><span data-stu-id="bed2f-304">• General or other</span></span>

<span data-ttu-id="bed2f-305">5. die Felder werden unter "Felder & Beziehungen" erstellt.</span><span class="sxs-lookup"><span data-stu-id="bed2f-305">5.The fields would get created under “Fields & Relationships”</span></span>

![Erstellte Felder](images/salesforce/fields2.png)

6. <span data-ttu-id="bed2f-307">Erstellen Sie im Layout der Verkaufschancen einen separaten Abschnitt mit den oben aufgeführten Feldern.</span><span class="sxs-lookup"><span data-stu-id="bed2f-307">In the Opportunity layout, create a separate section with the fields as listed above.</span></span> 

    <span data-ttu-id="bed2f-308">• Dieser Abschnitt sollte für die Verkäufer im Verkaufschancen Layout verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="bed2f-308">• This section should be available for the sellers in the Opportunity layout</span></span>


![Layout der Partner Center-Felder](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="bed2f-310">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="bed2f-310">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="bed2f-311">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Salesforce CRM und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-311">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="bed2f-312">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bed2f-312">Pre-requisites</span></span>

<span data-ttu-id="bed2f-313">Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-313">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="bed2f-314">Diese Identifikation bietet Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="bed2f-314">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="bed2f-315">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM Solution **Opportunity** -Entität verfügbar.</span><span class="sxs-lookup"><span data-stu-id="bed2f-315">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="bed2f-316">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-316">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="bed2f-317">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="bed2f-317">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="bed2f-318">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="bed2f-318">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="bed2f-319">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="bed2f-319">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="bed2f-320">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="bed2f-320">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="bed2f-321">**Wie kann Microsoft Help**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="bed2f-321">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="bed2f-322">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="bed2f-322">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="bed2f-323">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="bed2f-323">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="bed2f-324">SS</span><span class="sxs-lookup"><span data-stu-id="bed2f-324">SCENARIOS:</span></span>

1. <span data-ttu-id="bed2f-325">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="bed2f-325">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="bed2f-326">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-326">a.</span></span> <span data-ttu-id="bed2f-327">Melden Sie sich bei ihrer Salesforce CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="bed2f-327">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="bed2f-328">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-328">b.</span></span> <span data-ttu-id="bed2f-329">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="bed2f-329">Ensure that the following section is present when you create a “New Opportunity” in Salesforce CRM environment</span></span>

    ![Salesforce-Umgebung](images/salesforce/salesforce-scenario-1.png)

   

    <span data-ttu-id="bed2f-331">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-331">c.</span></span> <span data-ttu-id="bed2f-332">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="bed2f-332">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="bed2f-333">"Mit Partner Center synchronisieren": Ja</span><span class="sxs-lookup"><span data-stu-id="bed2f-333">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="bed2f-334">"Wie kann Microsoft Help?": Wählen Sie eine der folgenden Optionen aus:</span><span class="sxs-lookup"><span data-stu-id="bed2f-334">"How can Microsoft help?”: Select from the following options:</span></span>

   

    - <span data-ttu-id="bed2f-335">Produkte: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="bed2f-335">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="bed2f-336">d.</span><span class="sxs-lookup"><span data-stu-id="bed2f-336">d.</span></span> <span data-ttu-id="bed2f-337">Nachdem Sie die Option für die Verkaufschancen **Synchronisierung mit Partner Center** auf **Ja**festgelegt haben, können Sie sich bei Ihrem Partner Center-Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="bed2f-337">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="bed2f-338">Ihre Verweise werden mit Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bed2f-338">Your referrals will be synchronized with Salesforce CRM.</span></span>

    <span data-ttu-id="bed2f-339">e.</span><span class="sxs-lookup"><span data-stu-id="bed2f-339">e.</span></span> <span data-ttu-id="bed2f-340">Wenn die Option "Sync with Partner Center" auf "yes" festgelegt ist, werden die Änderungen, wenn Sie die Verkaufschance in Salesforce CRM aktualisieren, mit Ihrem Partner Center-Konto synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bed2f-340">When the “Sync with Partner Center” option is set to “Yes”, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

    <span data-ttu-id="bed2f-341">f.</span><span class="sxs-lookup"><span data-stu-id="bed2f-341">f.</span></span> <span data-ttu-id="bed2f-342">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Salesforce CRM identifiziert.</span><span class="sxs-lookup"><span data-stu-id="bed2f-342">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="bed2f-343">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="bed2f-343">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span> 

    <span data-ttu-id="bed2f-344">a.</span><span class="sxs-lookup"><span data-stu-id="bed2f-344">a.</span></span> <span data-ttu-id="bed2f-345">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="bed2f-345">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="bed2f-346">b.</span><span class="sxs-lookup"><span data-stu-id="bed2f-346">b.</span></span> <span data-ttu-id="bed2f-347">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="bed2f-347">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="bed2f-348">c.</span><span class="sxs-lookup"><span data-stu-id="bed2f-348">c.</span></span> <span data-ttu-id="bed2f-349">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="bed2f-349">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="bed2f-350">d.</span><span class="sxs-lookup"><span data-stu-id="bed2f-350">d.</span></span> <span data-ttu-id="bed2f-351">Melden Sie sich bei ihrer Salesforce CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="bed2f-351">Sign into your Salesforce CRM environment.</span></span> 

    <span data-ttu-id="bed2f-352">e.</span><span class="sxs-lookup"><span data-stu-id="bed2f-352">e.</span></span> <span data-ttu-id="bed2f-353">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="bed2f-353">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="bed2f-354">Der im Microsoft Partner Center erstellte Verweis ist nun in Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bed2f-354">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    ![Salesforce-Verkaufschancen Bildschirm](images/salesforce/salesforce-casino-e.png)

    <span data-ttu-id="bed2f-356">f.</span><span class="sxs-lookup"><span data-stu-id="bed2f-356">f.</span></span> <span data-ttu-id="bed2f-357">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="bed2f-357">When you select a synchronized referral, the card view details are populated.</span></span>





## <a name="next-steps"></a><span data-ttu-id="bed2f-358">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="bed2f-358">Next steps</span></span>

- [<span data-ttu-id="bed2f-359">Weitere Informationen zur Microsoft powerautomatisieren-Plattform</span><span class="sxs-lookup"><span data-stu-id="bed2f-359">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="bed2f-360">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="bed2f-360">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="bed2f-361">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="bed2f-361">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="bed2f-362">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="bed2f-362">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)