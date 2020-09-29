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
ms.openlocfilehash: 4b96be195788ccc8b82aafd0bddb90dd34a672f9
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422446"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="521ac-103">Co-Selling-Connector für Salesforce CRM – Übersicht</span><span class="sxs-lookup"><span data-stu-id="521ac-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="521ac-104">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="521ac-104">Appropriate roles</span></span>

- <span data-ttu-id="521ac-105">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="521ac-105">Referrals admin</span></span>
- <span data-ttu-id="521ac-106">Systemadministrator oder systemanpassungsprogramm im CRM</span><span class="sxs-lookup"><span data-stu-id="521ac-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="521ac-107">Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme.</span><span class="sxs-lookup"><span data-stu-id="521ac-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="521ac-108">Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden.</span><span class="sxs-lookup"><span data-stu-id="521ac-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="521ac-109">Mithilfe der Co-Selling-Connectors können Sie einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers erstellen, Referenzen vom Microsoft-Verkäufer erhalten, Verweise akzeptieren/ablehnen, Geschäftsdaten ändern, wie z. b. den Geschäftswert und das Enddatum.</span><span class="sxs-lookup"><span data-stu-id="521ac-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="521ac-110">Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten.</span><span class="sxs-lookup"><span data-stu-id="521ac-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="521ac-111">Sie können alle Ihre Verweise ausführen, während Sie im CRM Ihrer Wahl arbeiten und nicht im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="521ac-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="521ac-112">Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="521ac-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="521ac-113">Vor der Installation von-Pre-Requirements</span><span class="sxs-lookup"><span data-stu-id="521ac-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="521ac-114">**Themen**</span><span class="sxs-lookup"><span data-stu-id="521ac-114">**Topics**</span></span>   |<span data-ttu-id="521ac-115">**Details**</span><span class="sxs-lookup"><span data-stu-id="521ac-115">**Details**</span></span>   |<span data-ttu-id="521ac-116">**Links**</span><span class="sxs-lookup"><span data-stu-id="521ac-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="521ac-117">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="521ac-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="521ac-118">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="521ac-118">You need a valid MPN ID</span></span>|<span data-ttu-id="521ac-119">So fügen Sie [MPN](https://partner.microsoft.com/) an</span><span class="sxs-lookup"><span data-stu-id="521ac-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="521ac-120">Co-Sell Ready</span><span class="sxs-lookup"><span data-stu-id="521ac-120">Co-sell ready</span></span>|<span data-ttu-id="521ac-121">Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.</span><span class="sxs-lookup"><span data-stu-id="521ac-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="521ac-122">Vertrieb mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="521ac-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="521ac-123">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="521ac-123">Partner Center account</span></span>|<span data-ttu-id="521ac-124">Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="521ac-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="521ac-125">Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="521ac-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="521ac-126">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="521ac-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="521ac-127">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="521ac-127">Partner Center user roles</span></span>|<span data-ttu-id="521ac-128">Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.</span><span class="sxs-lookup"><span data-stu-id="521ac-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="521ac-129">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="521ac-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="521ac-130">Salesforce-CRM</span><span class="sxs-lookup"><span data-stu-id="521ac-130">Salesforce CRM</span></span>|<span data-ttu-id="521ac-131">Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="521ac-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="521ac-132">Zuweisen von Rollen in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="521ac-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="521ac-133">Energie automatisierter Fluss Konto</span><span class="sxs-lookup"><span data-stu-id="521ac-133">Power Automate Flow Account</span></span>|<span data-ttu-id="521ac-134">Ein aktives, [Energie automatisierbares](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder den SystemCustomizer.</span><span class="sxs-lookup"><span data-stu-id="521ac-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="521ac-135">Dieser Benutzer sollte sich mindestens einmal vor der Installation bei der [Strom Automatisierung](https://flow.microsoft.com) anmelden.</span><span class="sxs-lookup"><span data-stu-id="521ac-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="521ac-136">Installation des Salesforce-Pakets für benutzerdefinierte Microsoft-Felder</span><span class="sxs-lookup"><span data-stu-id="521ac-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="521ac-137">Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Lösung für die Energie Automatisierung bestimmte Verweis Felder von Microsoft eindeutig identifizieren.</span><span class="sxs-lookup"><span data-stu-id="521ac-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="521ac-138">Diese Abgrenzung bietet Partnern von Partner Verkäufern die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="521ac-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="521ac-139">Aktivieren Sie in Salesforce **Notizen** , und fügen Sie es der Liste Verkaufschancen hinzu.</span><span class="sxs-lookup"><span data-stu-id="521ac-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="521ac-140">Verweis</span><span class="sxs-lookup"><span data-stu-id="521ac-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="521ac-141">Aktivieren Sie **Opportunity-Teams** anhand der folgenden Schritte:</span><span class="sxs-lookup"><span data-stu-id="521ac-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="521ac-142">Verwenden Sie in Setup das Feld für die **Schnellsuche** , um die Einstellungen für das Team zu suchen.</span><span class="sxs-lookup"><span data-stu-id="521ac-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="521ac-143">Definieren Sie die Einstellungen nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="521ac-143">Define the settings as needed.</span></span>
[<span data-ttu-id="521ac-144">Verweis</span><span class="sxs-lookup"><span data-stu-id="521ac-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="521ac-145">Installieren Sie in Salesforce benutzerdefinierte Felder und Objekte mithilfe des unten aufgeführten Paketinstallers.</span><span class="sxs-lookup"><span data-stu-id="521ac-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="521ac-146">Wechseln Sie [hier](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) , um das Paket in einem beliebigen Unternehmen zu installieren:</span><span class="sxs-lookup"><span data-stu-id="521ac-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="521ac-147">Hinweis: Wenn Sie in einem Sandkasten installieren, müssen Sie den anfänglichen Teil der URL durch ersetzen. http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="521ac-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="521ac-148">Fügen Sie in Salesforce Microsoft-Lösungen zur Liste mit den Verkaufs **Chancen** hinzu.</span><span class="sxs-lookup"><span data-stu-id="521ac-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="521ac-149">Klicken Sie nach dem Hinzufügen auf das Symbol für den **Schraubendreher** , und aktualisieren Sie Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="521ac-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="521ac-150">Bewährte Vorgehensweise: testen, bevor Sie fortfahren</span><span class="sxs-lookup"><span data-stu-id="521ac-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="521ac-151">Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.</span><span class="sxs-lookup"><span data-stu-id="521ac-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="521ac-152">Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="521ac-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="521ac-153">Erstellen Sie eine Kopie der Projekt Mappe, und führen Sie die Konfiguration aus, und führen Sie die Automatisierung der Fluss Anpassungen in der Stagingumgebung durch</span><span class="sxs-lookup"><span data-stu-id="521ac-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="521ac-154">Testen Sie die Lösung auf einer Staging/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="521ac-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="521ac-155">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktions Instanz.</span><span class="sxs-lookup"><span data-stu-id="521ac-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="521ac-156">Installieren der Partner Center-Synchronisierung für Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="521ac-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="521ac-157">Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="521ac-158">Dadurch werden die verfügbaren CRM-Instanzen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="521ac-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="521ac-159">Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="521ac-160">Wählen Sie in der linken Navigationsleiste **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="521ac-161">Klicken Sie im oberen Menü auf den Link **appsource öffnen** .</span><span class="sxs-lookup"><span data-stu-id="521ac-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Appsource öffnen":::

5. <span data-ttu-id="521ac-163">Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="521ac-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="521ac-165">Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="521ac-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="521ac-166">Daraufhin wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung zum Installieren der Anwendung auswählen können.</span><span class="sxs-lookup"><span data-stu-id="521ac-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="521ac-167">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="521ac-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Verfügbare CRMs":::

8. <span data-ttu-id="521ac-169">Anschließend werden Sie zur Seite **Verwalten Ihrer Lösungen** weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="521ac-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="521ac-170">Navigieren Sie zu "Partner Center-Verweise", indem Sie die Pfeil Schaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="521ac-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="521ac-171">Die **geplante Installation** sollte neben der Projekt Mappe für Partner Center-Verweise angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="521ac-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="521ac-172">Die Installation wird 10-15 Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="521ac-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="521ac-173">Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="521ac-174">Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Salesforce** in der Lösungs Liste verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="521ac-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="521ac-175">Wählen Sie die **Synchronisierung der Partner Center-Verweise für Salesforce aus**.</span><span class="sxs-lookup"><span data-stu-id="521ac-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="521ac-176">Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="521ac-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-Flows":::



## <a name="configure-the-solution"></a><span data-ttu-id="521ac-178">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="521ac-178">Configure the solution</span></span>

1. <span data-ttu-id="521ac-179">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="521ac-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="521ac-180">Wählen Sie in der Dropdown- **Umgebung** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.</span><span class="sxs-lookup"><span data-stu-id="521ac-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="521ac-181">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="521ac-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="521ac-182">Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen</span><span class="sxs-lookup"><span data-stu-id="521ac-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="521ac-183">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="521ac-183">Partner Center Events</span></span>
    - <span data-ttu-id="521ac-184">Der CRM-Administrator mit den Energie automatisierten Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="521ac-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="521ac-185">Wählen Sie in der linken Navigationsleiste **Verbindungen** aus, und wählen Sie die Projekt Mappe "Partner Center-Verweise" aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="521ac-186">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen**klicken.</span><span class="sxs-lookup"><span data-stu-id="521ac-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Erstellen der Verbindung":::

- <span data-ttu-id="521ac-188">Suchen Sie in der Suchleiste in der oberen rechten Ecke nach Partner Center-Referenzen (Vorschau).</span><span class="sxs-lookup"><span data-stu-id="521ac-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="521ac-189">Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".</span><span class="sxs-lookup"><span data-stu-id="521ac-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="521ac-190">Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.</span><span class="sxs-lookup"><span data-stu-id="521ac-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="521ac-191">Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.</span><span class="sxs-lookup"><span data-stu-id="521ac-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="521ac-192">Nachdem Sie alle Verbindungen hinzugefügt haben, sollten in Ihrer Umgebung die folgenden Verbindungen angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="521ac-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Verbindungen beobachten":::

### <a name="edit-the-connections"></a><span data-ttu-id="521ac-194">Verbindungen bearbeiten</span><span class="sxs-lookup"><span data-stu-id="521ac-194">Edit the connections</span></span>

1. <span data-ttu-id="521ac-195">Kehren Sie zur Seite Lösungen zurück, und wählen Sie **Standard**Projekt Mappe aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="521ac-196">Wählen Sie **Verbindungs Verweis (Vorschau)** aus, indem Sie auf **alle**klicken.</span><span class="sxs-lookup"><span data-stu-id="521ac-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Connector-Bearbeitung starten":::

2. <span data-ttu-id="521ac-198">Bearbeiten Sie jede der Verbindungen nacheinander, indem Sie das Symbol drei Punkte auswählen.</span><span class="sxs-lookup"><span data-stu-id="521ac-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="521ac-199">Fügen Sie die relevanten Verbindungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="521ac-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Connectors bearbeiten":::

3. <span data-ttu-id="521ac-201">Aktivieren Sie die Flows in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="521ac-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="521ac-202">Partner Center-webhook-Registrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="521ac-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="521ac-203">Erstellen eines Co-Selling-Verweises-Salesforce an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="521ac-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="521ac-204">Partner Center Microsoft Co-Selling-Referenz Aktualisierungen an Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="521ac-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="521ac-205">Partner Center zu Salesforce (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="521ac-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="521ac-206">Salesforce zu Partner Center (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="521ac-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="521ac-207">Salesforce-Verkaufschance an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="521ac-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="521ac-208">Salesforce Microsoft-Lösungen an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="521ac-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="521ac-209">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="521ac-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="521ac-210">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="521ac-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="521ac-211">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="521ac-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="521ac-212">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="521ac-213">Fügen Sie Verbindungen für den (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b.) Partner Center-Veranstaltungen hinzu, wie unten gezeigt.</span><span class="sxs-lookup"><span data-stu-id="521ac-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="521ac-215">Wenn Sie diese Updates vornehmen, wird Folgendes angezeigt:</span><span class="sxs-lookup"><span data-stu-id="521ac-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="521ac-217">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="521ac-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="521ac-218">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="521ac-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="521ac-219">Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="521ac-220">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="521ac-221">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="521ac-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieren der URL":::

8. <span data-ttu-id="521ac-223">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="521ac-224">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="521ac-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="521ac-225">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="521ac-225">Enter the following details:</span></span>

    1. <span data-ttu-id="521ac-226">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="521ac-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="521ac-227">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="521ac-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="521ac-228">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="521ac-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="521ac-229">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="521ac-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="521ac-230">Der webhook kann nun auf Create-und Update-Ereignisse lauschen.</span><span class="sxs-lookup"><span data-stu-id="521ac-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="521ac-231">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="521ac-231">Customize synchronization steps</span></span>

<span data-ttu-id="521ac-232">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="521ac-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="521ac-233">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="521ac-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="521ac-234">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="521ac-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="521ac-235">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="521ac-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="521ac-236">Microsoft Partner Centers für CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="521ac-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="521ac-237">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="521ac-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="521ac-238">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="521ac-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="521ac-239">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="521ac-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="521ac-240">Wählen Sie Partner Center zu Salesforce CRM (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="521ac-241">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="521ac-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="521ac-242">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="521ac-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="521ac-243">**Wenn Sie die CRM-** Feld Zuordnungen für Erstellungs Ereignisse anpassen möchten, wählen Sie aus, ob es sich um eine neue Freigabe Chance handelt</span><span class="sxs-lookup"><span data-stu-id="521ac-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="521ac-244">Wählen Sie den untergeordneten **Schritt** aus, und erweitern Sie dann die Option **Erstellen einer neuen Verkaufschance im CRM**.</span><span class="sxs-lookup"><span data-stu-id="521ac-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="521ac-245">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="521ac-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="521ac-246">Zum Anpassen von CRM-Feld Zuordnungen für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="521ac-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="521ac-247">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="521ac-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="521ac-248">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="521ac-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="521ac-249">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="521ac-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="521ac-250">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="521ac-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="521ac-251">Wählen Sie **Bearbeiten**  aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="521ac-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="521ac-252">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="521ac-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="521ac-253">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="521ac-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="521ac-254">Wählen Sie den unterschritt aus, **Wenn ja** , und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="521ac-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="521ac-255">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="521ac-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="521ac-256">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="521ac-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="521ac-257">Wählen Sie **Bearbeiten**  aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="521ac-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="521ac-258">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="521ac-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="521ac-259">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="521ac-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="521ac-260">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="521ac-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="521ac-261">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="521ac-261">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="521ac-262">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Salesforce CRM und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="521ac-262">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="521ac-263">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="521ac-263">Pre-requisites</span></span>

<span data-ttu-id="521ac-264">Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="521ac-264">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="521ac-265">Diese Identifikation bietet Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="521ac-265">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="521ac-266">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM Solution **Opportunity** -Entität verfügbar.</span><span class="sxs-lookup"><span data-stu-id="521ac-266">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="521ac-267">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="521ac-267">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="521ac-268">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="521ac-268">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="521ac-269">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="521ac-269">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="521ac-270">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="521ac-270">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="521ac-271">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="521ac-271">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="521ac-272">**Wie kann Microsoft Help**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="521ac-272">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="521ac-273">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="521ac-273">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="521ac-274">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="521ac-274">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="521ac-275">SS</span><span class="sxs-lookup"><span data-stu-id="521ac-275">SCENARIOS:</span></span>

1. <span data-ttu-id="521ac-276">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="521ac-276">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="521ac-277">Melden Sie sich bei ihrer Salesforce CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="521ac-277">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="521ac-278">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="521ac-278">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-Umgebung":::

   3. <span data-ttu-id="521ac-280">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="521ac-280">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="521ac-281">"Mit Partner Center synchronisieren": Ja</span><span class="sxs-lookup"><span data-stu-id="521ac-281">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="521ac-282">"Wie kann Microsoft Help?": Wählen Sie eine der folgenden Optionen aus:</span><span class="sxs-lookup"><span data-stu-id="521ac-282">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="521ac-283">Produkte: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="521ac-283">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="521ac-284">Nachdem Sie die Option für die Verkaufschancen  **Synchronisierung mit Partner Center** auf **Ja**festgelegt haben, können Sie sich bei Ihrem Partner Center-Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="521ac-284">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="521ac-285">Ihre Verweise werden mit Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="521ac-285">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="521ac-286">Wenn die Option "Sync with Partner Center" auf "yes" festgelegt ist, werden die Änderungen, wenn Sie die Verkaufschance in Salesforce CRM aktualisieren, mit Ihrem Partner Center-Konto synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="521ac-286">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="521ac-287">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Salesforce CRM identifiziert.</span><span class="sxs-lookup"><span data-stu-id="521ac-287">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="521ac-288">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="521ac-288">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="521ac-289">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="521ac-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="521ac-290">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="521ac-290">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="521ac-291">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="521ac-291">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="521ac-292">Melden Sie sich bei ihrer Salesforce CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="521ac-292">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="521ac-293">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="521ac-293">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="521ac-294">Der im Microsoft Partner Center erstellte Verweis ist nun in Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="521ac-294">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce-Verkaufschancen Bildschirm":::

    6. <span data-ttu-id="521ac-296">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="521ac-296">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="521ac-297">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="521ac-297">Next steps</span></span>

- [<span data-ttu-id="521ac-298">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="521ac-298">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="521ac-299">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="521ac-299">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="521ac-300">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="521ac-300">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)