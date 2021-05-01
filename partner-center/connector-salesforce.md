---
title: Der Co-Sell-Connector für Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Sie Ihre Empfehlungen in Partner Center Salesforce CRM. Verkäufer können dann in Ihren CRM-Systemen gemeinsam mit Microsoft verkaufen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284382"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="454fc-104">Co-Selling-Connector für Salesforce CRM – Übersicht</span><span class="sxs-lookup"><span data-stu-id="454fc-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="454fc-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="454fc-105">**Appropriate roles**</span></span>

- <span data-ttu-id="454fc-106">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="454fc-106">Referrals admin</span></span>
- <span data-ttu-id="454fc-107">Systemadministrator oder Systemanpasser im CRM</span><span class="sxs-lookup"><span data-stu-id="454fc-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="454fc-108">Partner Center Co-Sell-Connector ermöglicht es Ihren Verkäufern, in Ihren CRM-Systemen gemeinsam mit Microsoft zu verkaufen.</span><span class="sxs-lookup"><span data-stu-id="454fc-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="454fc-109">Sie müssen nicht trainiert werden, um co-Partner Center verwalten zu können.</span><span class="sxs-lookup"><span data-stu-id="454fc-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="454fc-110">Mithilfe der Co-Sell-Connectors können Sie eine neue Co-Sell-Empfehlung erstellen, um einen Microsoft-Verkäufer zu kontaktieren, Empfehlungen vom Microsoft-Verkäufer zu erhalten, Empfehlungen zu akzeptieren/ablehnen, Dealdaten wie den Dealwert und das Abschlussdatum zu ändern.</span><span class="sxs-lookup"><span data-stu-id="454fc-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="454fc-111">Sie können auch updates von den Microsoft-Verkäufern zu diesen Co-Sell-Deals erhalten.</span><span class="sxs-lookup"><span data-stu-id="454fc-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="454fc-112">Sie können alle Ihre Empfehlungen nutzen, während Sie innerhalb des CRM Ihrer Wahl arbeiten und nicht in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="454fc-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="454fc-113">Die Lösung basiert auf Microsoft Power Automate Solution und verwendet Partner Center APIs.</span><span class="sxs-lookup"><span data-stu-id="454fc-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="454fc-114">Voraussetzungen vor der Installation</span><span class="sxs-lookup"><span data-stu-id="454fc-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="454fc-115">**Themen**</span><span class="sxs-lookup"><span data-stu-id="454fc-115">**Topics**</span></span>   |<span data-ttu-id="454fc-116">**Details**</span><span class="sxs-lookup"><span data-stu-id="454fc-116">**Details**</span></span>   |<span data-ttu-id="454fc-117">**Links**</span><span class="sxs-lookup"><span data-stu-id="454fc-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="454fc-118">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="454fc-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="454fc-119">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="454fc-119">You need a valid MPN ID</span></span>|<span data-ttu-id="454fc-120">So treten Sie [MPN bei](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="454fc-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="454fc-121">Co-Sell Ready</span><span class="sxs-lookup"><span data-stu-id="454fc-121">Co-sell ready</span></span>|<span data-ttu-id="454fc-122">Ihre IP/Services-Lösung muss co-sell ready sein.</span><span class="sxs-lookup"><span data-stu-id="454fc-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="454fc-123">Verkaufen mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="454fc-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="454fc-124">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="454fc-124">Partner Center account</span></span>|<span data-ttu-id="454fc-125">Die MPN-ID, die dem Partner Center Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die Ihrer Co-Sell-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="454fc-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="454fc-126">Stellen Sie sicher, dass Ihre Co-Sell-Empfehlungen im Partner Center angezeigt werden, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="454fc-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="454fc-127">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="454fc-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="454fc-128">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="454fc-128">Partner Center user roles</span></span>|<span data-ttu-id="454fc-129">Der Mitarbeiter, der die Connectors installiert und verwendet, muss ein Empfehlungsadministrator sein.</span><span class="sxs-lookup"><span data-stu-id="454fc-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="454fc-130">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="454fc-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="454fc-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="454fc-131">Salesforce CRM</span></span>|<span data-ttu-id="454fc-132">Die CRM-Benutzerrolle ist "Systemadministrator" oder "Systemanpasser".</span><span class="sxs-lookup"><span data-stu-id="454fc-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="454fc-133">Zuweisen von Rollen in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="454fc-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="454fc-134">Power Automate Flow-Konto</span><span class="sxs-lookup"><span data-stu-id="454fc-134">Power Automate Flow Account</span></span>|<span data-ttu-id="454fc-135">Ein aktives [Power Automate](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder systemanpasser.</span><span class="sxs-lookup"><span data-stu-id="454fc-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="454fc-136">Dieser Benutzer sollte sich mindestens einmal vor der Installation bei [Power Automate](https://flow.microsoft.com) anmelden.</span><span class="sxs-lookup"><span data-stu-id="454fc-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="454fc-137">Installation des Salesforce-Pakets für benutzerdefinierte Microsoft-Felder</span><span class="sxs-lookup"><span data-stu-id="454fc-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="454fc-138">Um die Empfehlungen über Partner Center und Salesforce CRM hinweg zu synchronisieren, muss die Power Automate Lösung microsoftspezifische Empfehlungsfelder eindeutig identifizieren.</span><span class="sxs-lookup"><span data-stu-id="454fc-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="454fc-139">Diese Demarkation bietet Partnerverkäuferteams die Möglichkeit zu entscheiden, welche Empfehlungen sie für den Co-Selling mit Microsoft teilen möchten.</span><span class="sxs-lookup"><span data-stu-id="454fc-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="454fc-140">Aktivieren Sie in Salesforce **Notizen,** und fügen Sie sie der Liste der Verkaufschancen hinzu.</span><span class="sxs-lookup"><span data-stu-id="454fc-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="454fc-141">Verweis</span><span class="sxs-lookup"><span data-stu-id="454fc-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="454fc-142">Aktivieren Sie **Opportunity-Teams,** indem Sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="454fc-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="454fc-143">Verwenden Sie im Setup das Feld **Schnellsuche,** um die Einstellungen des Opportunity-Teams zu suchen.</span><span class="sxs-lookup"><span data-stu-id="454fc-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="454fc-144">Definieren Sie die Einstellungen nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="454fc-144">Define the settings as needed.</span></span>
[<span data-ttu-id="454fc-145">Verweis</span><span class="sxs-lookup"><span data-stu-id="454fc-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="454fc-146">Installieren Sie in Salesforce benutzerdefinierte Felder und Objekte mithilfe des [Paketinstallationsprogramms](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="454fc-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="454fc-147">Verwenden Sie diese, um das Paket in einem beliebigen Unternehmen zu installieren.</span><span class="sxs-lookup"><span data-stu-id="454fc-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="454fc-148">Wenn Sie in einer Sandbox installieren, müssen Sie den ursprünglichen Teil der URL durch ersetzen. http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="454fc-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="454fc-149">Fügen Sie in Salesforce Microsoft-Lösungen zur Liste **Verkaufschancen** hinzu.</span><span class="sxs-lookup"><span data-stu-id="454fc-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="454fc-150">Wählen Sie nach dem Hinzufügen das **Schraubenschlüsselsymbol** aus, und aktualisieren Sie die Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="454fc-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="454fc-151">Bewährte Methode: Testen, bevor Sie live gehen</span><span class="sxs-lookup"><span data-stu-id="454fc-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="454fc-152">Bevor Sie die Power Automate Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen, stellen Sie sicher, dass Sie die Lösung auf einer STAGING-CRM-Instanz testen.</span><span class="sxs-lookup"><span data-stu-id="454fc-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="454fc-153">Installieren Sie Microsoft Power Automate Lösung in einer Stagingumgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="454fc-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="454fc-154">Erstellen Sie eine Kopie der Projektmappe, und führen Sie Ihre Konfiguration aus, und Power Automate Flowanpassungen in der Stagingumgebung.</span><span class="sxs-lookup"><span data-stu-id="454fc-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="454fc-155">Testen Sie die Lösung in einer Staging-/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="454fc-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="454fc-156">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktionsinstanz.</span><span class="sxs-lookup"><span data-stu-id="454fc-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="454fc-157">Installieren Partner Center Synchronisierung von Empfehlungen für Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="454fc-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="454fc-158">Wechseln Sie [zu Power Automate,](https://flow.microsoft.com) und wählen **Sie in der** rechten oberen Ecke Umgebungen aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="454fc-159">Dadurch werden die verfügbaren CRM-Instanzen gezeigt.</span><span class="sxs-lookup"><span data-stu-id="454fc-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="454fc-160">Wählen Sie in der Dropdownliste rechts oben die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="454fc-161">Wählen **Sie in** der linken Navigationsleiste Lösungen aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="454fc-162">Wählen Sie **im oberen Menü den Link AppSource** öffnen aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öffnen von AppSource":::

5. <span data-ttu-id="454fc-164">Suchen Sie **Partner Center Popupbildschirm nach Empfehlungsconnectors** für Salesforce.</span><span class="sxs-lookup"><span data-stu-id="454fc-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="454fc-166">Wählen Sie die **Schaltfläche Jetzt holen** und dann Weiter **aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="454fc-167">Dadurch wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung auswählen können, um die Anwendung zu installieren.</span><span class="sxs-lookup"><span data-stu-id="454fc-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="454fc-168">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="454fc-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Verfügbare CRMS":::

8. <span data-ttu-id="454fc-170">Sie werden dann zur Seite Manage **your solutions (Lösungen verwalten)** geleitet.</span><span class="sxs-lookup"><span data-stu-id="454fc-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="454fc-171">Navigieren Sie zu "Partner Center Empfehlungen", indem Sie die Pfeilschaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="454fc-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="454fc-172">**Die geplante Installation** sollte neben Partner Center Empfehlungslösung angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="454fc-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="454fc-173">Die Installation dauert 10 bis 15 Minuten.</span><span class="sxs-lookup"><span data-stu-id="454fc-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="454fc-174">Navigieren Sie nach Abschluss der Installation zurück zum Power Automate [und](https://flow.microsoft.com) wählen Sie **im linken** Navigationsbereich Lösungen aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="454fc-175">Beachten Sie, dass **Partner Center Empfehlungssynchronisierung für Salesforce** in der Liste Lösungen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="454fc-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="454fc-176">Wählen Sie **Partner Center Synchronisierung von Empfehlungen für Salesforce** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="454fc-177">Die folgenden Power Automate Flows und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="454fc-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-Flows":::



## <a name="configure-the-solution"></a><span data-ttu-id="454fc-179">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="454fc-179">Configure the solution</span></span>

1. <span data-ttu-id="454fc-180">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="454fc-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="454fc-181">Wählen Sie in der Dropdown-Dropdownseite **Umgebungen** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Power Automate-Lösung installiert haben.</span><span class="sxs-lookup"><span data-stu-id="454fc-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="454fc-182">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="454fc-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="454fc-183">Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="454fc-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="454fc-184">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="454fc-184">Partner Center Events</span></span>
    - <span data-ttu-id="454fc-185">CRM-Administrator mit den Power Automate Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="454fc-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="454fc-186">Klicken Sie in der linken Navigationsleiste auf **Verbindungen,** und wählen Sie in der Liste die Lösung "Partner Center Empfehlungen" aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="454fc-187">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen** klicken.</span><span class="sxs-lookup"><span data-stu-id="454fc-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Erstellen der Verbindung":::

- <span data-ttu-id="454fc-189">Suchen Sie in der Suchleiste in der oberen rechten Ecke nach Partner Center Empfehlungen (Vorschau).</span><span class="sxs-lookup"><span data-stu-id="454fc-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="454fc-190">Erstellen Sie eine Verbindung für Ihren Partner Center Benutzer mit der Rolle "Anmeldeinformationen" des Empfehlungsadministrators.</span><span class="sxs-lookup"><span data-stu-id="454fc-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="454fc-191">Erstellen Sie als Nächstes eine Partner Center Events-Verbindung für Ihren Partner Center-Benutzer mit den Anmeldeinformationen des Empfehlungsadministrators.</span><span class="sxs-lookup"><span data-stu-id="454fc-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="454fc-192">Erstellen Sie eine Verbindung für Salesforce für den CRM-Administratorbenutzer.</span><span class="sxs-lookup"><span data-stu-id="454fc-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="454fc-193">Nachdem Sie alle Verbindungen hinzugefügt haben, sollten in Ihrer Umgebung die folgenden Verbindungen angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="454fc-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Beobachten von Verbindungen":::

### <a name="edit-the-connections"></a><span data-ttu-id="454fc-195">Bearbeiten der Verbindungen</span><span class="sxs-lookup"><span data-stu-id="454fc-195">Edit the connections</span></span>

1. <span data-ttu-id="454fc-196">Kehren Sie zur Seite Lösungen zurück, und wählen Sie **Standardlösung** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="454fc-197">Wählen Sie **Verbindungsverweis (Vorschau)** aus, indem Sie auf **Alle** klicken.</span><span class="sxs-lookup"><span data-stu-id="454fc-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Connectorbearbeitung starten":::

2. <span data-ttu-id="454fc-199">Bearbeiten Sie die einzelnen Verbindungen einzeln, indem Sie auf das Symbol mit den drei Punkten klicken.</span><span class="sxs-lookup"><span data-stu-id="454fc-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="454fc-200">Fügen Sie die relevanten Verbindungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="454fc-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Bearbeiten von Connectors":::

3. <span data-ttu-id="454fc-202">Aktivieren Sie die Flows in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="454fc-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="454fc-203">Partner Center Webhookregistrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="454fc-204">Erstellen einer Co-Sell-Empfehlung – Salesforce Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="454fc-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="454fc-206">Partner Center to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="454fc-207">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="454fc-208">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="454fc-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="454fc-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="454fc-210">Verwenden von Webhook-APIs zum Registrieren für Ressourcenänderungsereignisse</span><span class="sxs-lookup"><span data-stu-id="454fc-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="454fc-211">Mit Partner Center Webhook-APIs können Sie sich für Ressourcenänderungsereignisse registrieren.</span><span class="sxs-lookup"><span data-stu-id="454fc-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="454fc-212">Diese Änderungsereignisse werden als HTTP-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="454fc-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="454fc-213">Wählen Sie zum Registrieren Ihrer URL Partner Center **Webhookregistrierung (Insider Preview) Power Automate** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="454fc-214">Fügen Sie Verbindungen für (a.) Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen (b.) Partner Center Ereignisse hinzu, wie unten hervorgehoben.</span><span class="sxs-lookup"><span data-stu-id="454fc-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="454fc-216">Wenn Sie diese Updates machen, sehen Sie:</span><span class="sxs-lookup"><span data-stu-id="454fc-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="454fc-218">Speichern Sie Ihre Änderungen, und wählen **Sie Aktivieren aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="454fc-219">Um webhooks Partner Center ereignisänderungen zu lauschen, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="454fc-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="454fc-220">Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="454fc-221">Wählen Sie das Symbol **Bearbeiten** und **dann When a HTTP request is received (Wenn eine HTTP-Anforderung empfangen wird)** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="454fc-222">Wählen Sie das Symbol **Kopieren** aus, um die angegebene HTTP POST-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="454fc-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieren der URL":::

8. <span data-ttu-id="454fc-224">Wählen Sie nun den Flow "Partner Center Webhookregistrierung (Insider Preview)" Power Automate aus, und wählen Sie **Ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="454fc-225">Stellen Sie sicher, dass das Fenster "Flow ausführen" im rechten Bereich geöffnet wird, und wählen Sie **Weiter** aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="454fc-226">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="454fc-226">Enter the following details:</span></span>

    1. <span data-ttu-id="454fc-227">**HTTP-Triggerendpunkt:** URL aus dem vorherigen Schritt kopiert</span><span class="sxs-lookup"><span data-stu-id="454fc-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="454fc-228">**Zu registrierende Ereignisse:**"Empfehlung erstellt" und "Empfehlung aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="454fc-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="454fc-229">**Vorhandene Triggerendpunkte überschreiben, sofern vorhanden:** Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="454fc-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="454fc-230">Wählen Sie **Ausführen** und dann **Fertig aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="454fc-231">Der Webhook kann jetzt auf Erstellungs- und Aktualisierungsereignisse lauschen.</span><span class="sxs-lookup"><span data-stu-id="454fc-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="454fc-232">Anpassen der Synchronisierungsschritte</span><span class="sxs-lookup"><span data-stu-id="454fc-232">Customize synchronization steps</span></span>

<span data-ttu-id="454fc-233">Wenn Co-Selling-Empfehlungen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf Partner Center PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="454fc-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="454fc-234">CRM-Systeme sind häufig stark angepasst.</span><span class="sxs-lookup"><span data-stu-id="454fc-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="454fc-235">Sie können die Power Automate Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="454fc-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="454fc-236">Befolgen Sie die Anleitung für die Feldzuordnung, und nehmen Sie bei Bedarf entsprechende Änderungen in den Schritten der Power Automate Flows vor.</span><span class="sxs-lookup"><span data-stu-id="454fc-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="454fc-237">Microsoft Partner Center-to-CRM-Zuordnungen werden bereitgestellt, aber basierend auf Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="454fc-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="454fc-238">Mehrere Schritte der einzelnen Power Automate Flows können je nach Ihren Anforderungen angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="454fc-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="454fc-239">Im Folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="454fc-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="454fc-240">So passen Sie die Felder für die Erstellungs- oder Aktualisierungsereignisse im Partner Center zur CRM-Empfehlungssynchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="454fc-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="454fc-241">Wählen Sie Partner Center salesforce CRM (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="454fc-242">Wählen **Sie Bearbeiten** aus, um den Power Automate anzupassen.</span><span class="sxs-lookup"><span data-stu-id="454fc-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="454fc-243">Wählen **Sie (Bereich) Lead oder Verkaufschance synchronisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="454fc-244">Um CRM-Feldzuordnungen für Erstellungsereignisse anzupassen, wählen Sie If it es new Shared opportunity (Wenn es sich um eine neue freigegebene **Verkaufschance) und dann aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="454fc-245">Wählen Sie den unteren Schritt **aus, falls ja,** und erweitern Sie dann **Erstellen einer neuen Verkaufschance in CRM**.</span><span class="sxs-lookup"><span data-stu-id="454fc-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="454fc-246">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Feldzuordnungshandbuchs bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="454fc-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="454fc-247">Um CRM-Feldzuordnungen für Updateereignisse anzupassen, wählen Sie den Schritt "(Bereich) Lead oder Verkaufschance synchronisieren" aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="454fc-248">Wählen Sie If it es a update to an opportunity (Wenn es sich um **ein Update einer Verkaufschance) und dann um .**</span><span class="sxs-lookup"><span data-stu-id="454fc-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="454fc-249">Wählen Sie den unteren Schritt aus, falls **ja,** und erweitern Sie dann If **difference between the opportunity objects in Partner Center and CRM (Wenn** Unterschied zwischen den Opportunityobjekten in Partner Center CRM) und dann .</span><span class="sxs-lookup"><span data-stu-id="454fc-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="454fc-250">Wählen Sie **Bei Ja** gefolgt von Update existing **opportunity (Vorhandene Verkaufschance aktualisieren) aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="454fc-251">So passen Sie die Felder für die CRM-zu-PC-Empfehlungssynchronisierung für Updateereignisse an:</span><span class="sxs-lookup"><span data-stu-id="454fc-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="454fc-252">Wählen **Sie Bearbeiten**  aus, um den Power Automate anzupassen.</span><span class="sxs-lookup"><span data-stu-id="454fc-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="454fc-253">Wählen **Sie (Bereich) Die Verkaufschance synchronisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="454fc-254">Wählen Sie zum Anpassen von CRM-Feldzuordnungen (basierend auf dem Leitfaden für Feldzuordnungen) für Updateereignisse die Option Wenn ein Unterschied zwischen den Leadobjekten **in Partner Center und CRM besteht, dann aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="454fc-255">Wählen Sie den unteren Schritt **aus, falls ja,** und erweitern Sie dann den Schritt **Empfehlung mit Verkaufschancedaten aktualisieren.**</span><span class="sxs-lookup"><span data-stu-id="454fc-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="454fc-256">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Feldzuordnungshandbuch bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="454fc-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="454fc-257">Zum Anpassen der Felder für die CRM-zu-PC-Empfehlungssynchronisierung zum Erstellen von Ereignissen?</span><span class="sxs-lookup"><span data-stu-id="454fc-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="454fc-258">Wählen **Sie Bearbeiten**  aus, um den Power Automate anzupassen.</span><span class="sxs-lookup"><span data-stu-id="454fc-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="454fc-259">Wählen **Sie (Bereich) Empfehlungen synchronisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="454fc-260">Wählen Sie zum Anpassen von CRM-Feldzuordnungen (basierend auf dem Feldzuordnungsleitfaden) für Erstellungsereignisse die Option **Microsoft-Empfehlung erstellen aus.**</span><span class="sxs-lookup"><span data-stu-id="454fc-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="454fc-261">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Feldzuordnungshandbuch bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="454fc-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="454fc-262">End-to-End-Synchronisierung bidirektionaler Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="454fc-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="454fc-263">Nachdem Sie die Power Automate Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Empfehlungen zwischen Salesforce CRM und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="454fc-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="454fc-264">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="454fc-264">Pre-requisites</span></span>

<span data-ttu-id="454fc-265">Um die Empfehlungen über Partner Center und Salesforce CRM hinweg zu synchronisieren, muss die Power Automate Lösung microsoftspezifische Empfehlungsfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="454fc-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="454fc-266">Diese Identifizierung bietet Ihren Verkäuferteams die Möglichkeit zu entscheiden, welche Empfehlungen sie für den Co-Selling mit Microsoft teilen möchten.</span><span class="sxs-lookup"><span data-stu-id="454fc-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="454fc-267">Eine Reihe von benutzerdefinierten Feldern ist als Teil Partner Center Entität Empfehlungssynchronisierung für Salesforce CRM-Lösung **Opportunity** verfügbar.</span><span class="sxs-lookup"><span data-stu-id="454fc-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="454fc-268">Ein CRM-Administratorbenutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern **Opportunity** erstellen.</span><span class="sxs-lookup"><span data-stu-id="454fc-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="454fc-269">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="454fc-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="454fc-270">**Synchronisierung mit Partner Center:** Gibt an, ob die Verkaufschance mit Microsoft Partner Center synchronisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="454fc-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="454fc-271">**Empfehlungsbezeichner:** Ein schreibgeschütztes Bezeichnerfeld für Microsoft Partner Center-Empfehlung</span><span class="sxs-lookup"><span data-stu-id="454fc-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="454fc-272">**Empfehlungslink:** Ein schreibgeschützter Link zur Empfehlung in Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="454fc-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="454fc-273">**How can Microsoft help**: Help required from Microsoft for the referral (Hilfe von Microsoft für die Empfehlung erforderlich)</span><span class="sxs-lookup"><span data-stu-id="454fc-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="454fc-274">**Produkte:** Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="454fc-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="454fc-275">**Audit**: Ein schreibgeschützter Überwachungspfad für die Synchronisierung mit Partner Center Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="454fc-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="454fc-276">Szenarien:</span><span class="sxs-lookup"><span data-stu-id="454fc-276">SCENARIOS:</span></span>

1. <span data-ttu-id="454fc-277">Empfehlungssynchronisierung, wenn die Empfehlung in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="454fc-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="454fc-278">Melden Sie sich mit einem Benutzer bei Ihrer Salesforce CRM-Umgebung an, der im Abschnitt **Opportunity** des CRM-Abschnitts über Sichtbarkeit verfügt.</span><span class="sxs-lookup"><span data-stu-id="454fc-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="454fc-279">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "Neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="454fc-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-Umgebung":::

   3. <span data-ttu-id="454fc-281">Um diese Verkaufschance mit Microsoft Partner Center zu synchronisieren, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="454fc-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="454fc-282">"Sync with Partner Center": Yes</span><span class="sxs-lookup"><span data-stu-id="454fc-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="454fc-283">"Wie kann Microsoft helfen?": Wählen Sie eine der folgenden Optionen aus:</span><span class="sxs-lookup"><span data-stu-id="454fc-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="454fc-284">Produkte: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="454fc-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="454fc-285">Nachdem Sie die Option  **Sync with Partner Center** auf **Ja** festgelegt haben, warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="454fc-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="454fc-286">Ihre Empfehlungen werden mit Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="454fc-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="454fc-287">Wenn die Option "Mit Partner Center synchronisieren" auf "Ja" festgelegt ist und Sie die Verkaufschance in Salesforce CRM aktualisieren, werden die Änderungen mit Ihrem Partner Center synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="454fc-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="454fc-288">Verkaufschancen, die erfolgreich mit Partner Center synchronisiert werden, werden mithilfe ✔ in Salesforce CRM identifiziert.</span><span class="sxs-lookup"><span data-stu-id="454fc-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="454fc-289">Empfehlungssynchronisierung, wenn die Empfehlung in Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="454fc-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="454fc-290">Melden Sie sich bei Ihrem [Partner Center-Dashboard an.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="454fc-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="454fc-291">Wählen **Sie im menü auf** der linken Seite die Option Empfehlungen aus.</span><span class="sxs-lookup"><span data-stu-id="454fc-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="454fc-292">Erstellen Sie eine neue Co-Sell-Empfehlung aus Partner Center indem Sie auf die Option "Neuer Deal" klicken.</span><span class="sxs-lookup"><span data-stu-id="454fc-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="454fc-293">Melden Sie sich bei Ihrer Salesforce CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="454fc-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="454fc-294">Navigieren Sie zu **Open Opportunities (Verkaufschancen öffnen).**</span><span class="sxs-lookup"><span data-stu-id="454fc-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="454fc-295">Die im Microsoft Partner Center erstellte Empfehlung wird jetzt in Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="454fc-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Bildschirm &quot;Salesforce-Verkaufschance&quot;":::

    6. <span data-ttu-id="454fc-297">Wenn Sie eine synchronisierte Empfehlung auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="454fc-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="454fc-298">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="454fc-298">Next steps</span></span>

- [<span data-ttu-id="454fc-299">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="454fc-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="454fc-300">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="454fc-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="454fc-301">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="454fc-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
