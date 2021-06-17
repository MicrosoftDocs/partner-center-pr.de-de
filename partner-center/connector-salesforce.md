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
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276976"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="2d1a5-104">Co-Selling-Connector für Salesforce CRM – Übersicht</span><span class="sxs-lookup"><span data-stu-id="2d1a5-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="2d1a5-105">**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Systemadministrator oder Systemanpasser im CRM</span><span class="sxs-lookup"><span data-stu-id="2d1a5-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="2d1a5-106">Partner Center Co-Sell-Connector ermöglicht es Ihren Verkäufern, in Ihren CRM-Systemen gemeinsam mit Microsoft zu verkaufen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="2d1a5-107">Sie müssen nicht trainiert werden, um co-Partner Center verwalten zu können.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="2d1a5-108">Mithilfe der Co-Sell-Connectors können Sie eine neue Co-Sell-Empfehlung erstellen, um einen Microsoft-Verkäufer zu kontaktieren, Empfehlungen vom Microsoft-Verkäufer zu erhalten, Empfehlungen zu akzeptieren/ablehnen, Dealdaten wie den Dealwert und das Abschlussdatum zu ändern.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="2d1a5-109">Sie können auch updates von den Microsoft-Verkäufern zu diesen Co-Sell-Deals erhalten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="2d1a5-110">Sie können alle Ihre Empfehlungen nutzen, während Sie innerhalb des CRM Ihrer Wahl arbeiten und nicht in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="2d1a5-111">Die Lösung basiert auf Microsoft Power Automate Solution und verwendet Partner Center APIs.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="2d1a5-112">Voraussetzungen vor der Installation</span><span class="sxs-lookup"><span data-stu-id="2d1a5-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="2d1a5-113">**Themen**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-113">**Topics**</span></span>   |<span data-ttu-id="2d1a5-114">**Details**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-114">**Details**</span></span>   |<span data-ttu-id="2d1a5-115">**Links**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="2d1a5-116">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="2d1a5-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="2d1a5-117">Sie benötigen eine gültige MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-117">You need a valid MPN ID</span></span>|<span data-ttu-id="2d1a5-118">So treten Sie [MPN bei](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="2d1a5-119">Co-Sell Ready</span><span class="sxs-lookup"><span data-stu-id="2d1a5-119">Co-sell ready</span></span>|<span data-ttu-id="2d1a5-120">Ihre IP/Services-Lösung muss co-sell ready sein.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="2d1a5-121">Verkaufen mit Microsoft</span><span class="sxs-lookup"><span data-stu-id="2d1a5-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="2d1a5-122">Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="2d1a5-122">Partner Center account</span></span>|<span data-ttu-id="2d1a5-123">Die MPN-ID, die dem Partner Center Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die Ihrer Co-Sell-Lösung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="2d1a5-124">Stellen Sie sicher, dass Ihre Co-Sell-Empfehlungen im Partner Center angezeigt werden, bevor Sie die Connectors bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="2d1a5-125">Verwalten Ihres Kontos</span><span class="sxs-lookup"><span data-stu-id="2d1a5-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="2d1a5-126">Partner Center-Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-126">Partner Center user roles</span></span>|<span data-ttu-id="2d1a5-127">Der Mitarbeiter, der die Connectors installiert und verwendet, muss ein Empfehlungsadministrator sein.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="2d1a5-128">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="2d1a5-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="2d1a5-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="2d1a5-129">Salesforce CRM</span></span>|<span data-ttu-id="2d1a5-130">Die CRM-Benutzerrolle ist "Systemadministrator" oder "Systemanpasser".</span><span class="sxs-lookup"><span data-stu-id="2d1a5-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="2d1a5-131">Zuweisen von Rollen in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="2d1a5-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="2d1a5-132">Power Automate Flow-Konto</span><span class="sxs-lookup"><span data-stu-id="2d1a5-132">Power Automate Flow Account</span></span>|<span data-ttu-id="2d1a5-133">Ein [aktives Power Automate](https://flow.microsoft.com) für den CRM-Systemadministrator oder Systemanpasser.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="2d1a5-134">Dieser Benutzer sollte sich vor [der Power Automate](https://flow.microsoft.com) mindestens einmal bei der Anmeldung anmelden.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="2d1a5-135">Installation des Salesforce-Pakets für benutzerdefinierte Microsoft-Felder</span><span class="sxs-lookup"><span data-stu-id="2d1a5-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="2d1a5-136">Um die Empfehlungen über Partner Center Salesforce CRM hinweg zu synchronisieren, muss die Power Automate-Lösung microsoftspezifische Empfehlungsfelder eindeutig identifizieren.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="2d1a5-137">Diese Abgrenzung bietet Partner-Verkäuferteams die Möglichkeit zu entscheiden, welche Empfehlungen sie für den Co-Selling an Microsoft freigeben möchten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="2d1a5-138">Aktivieren Sie in Salesforce **Notizen,** und fügen Sie sie der Liste der Verkaufschancen hinzu.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="2d1a5-139">Referenz</span><span class="sxs-lookup"><span data-stu-id="2d1a5-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="2d1a5-140">Aktivieren **Sie Opportunity-Teams,** indem Sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="2d1a5-141">Verwenden Sie unter Setup das Feld **Schnellstart,** um die Teameinstellungen für Verkaufschance zu suchen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="2d1a5-142">Definieren Sie die Einstellungen nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-142">Define the settings as needed.</span></span>
[<span data-ttu-id="2d1a5-143">Referenz</span><span class="sxs-lookup"><span data-stu-id="2d1a5-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="2d1a5-144">Installieren Sie in Salesforce benutzerdefinierte Felder und Objekte mithilfe des [Paketinstallationsprogramms](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="2d1a5-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="2d1a5-145">Verwenden Sie diese, um das Paket in einem beliebigen Unternehmen zu installieren.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="2d1a5-146">Wenn Sie in einer Sandbox installieren, müssen Sie den anfänglichen Teil der URL durch ersetzen. http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="2d1a5-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="2d1a5-147">Fügen Sie microsoft Solutions in Salesforce der Liste Opportunity related **(Verkaufschance)** hinzu.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="2d1a5-148">Wählen Sie nach dem Hinzugefügten das **Schraubenschlüsselsymbol aus,** und aktualisieren Sie die Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="2d1a5-149">Bewährte Methode: Testen, bevor Sie live gehen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="2d1a5-150">Bevor Sie die Lösung installieren, konfigurieren und Power Automate in der Produktionsumgebung anpassen, müssen Sie die Lösung auf einer CRM-Staginginstanz testen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="2d1a5-151">Installieren Sie die Microsoft Power Automate-Lösung in einer Stagingumgebung/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="2d1a5-152">Erstellen Sie eine Kopie der Projektmappe, und führen Sie Ihre Konfiguration aus, und Power Automate Flowanpassungen in der Stagingumgebung.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="2d1a5-153">Testen Sie die Lösung in einer Staging-/CRM-Instanz.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="2d1a5-154">Importieren Sie bei Erfolg als verwaltete Lösung in die Produktionsinstanz.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="2d1a5-155">Installieren Partner Center Synchronisierung von Empfehlungen für Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="2d1a5-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="2d1a5-156">Wechseln Sie [zu Power Automate,](https://flow.microsoft.com) und wählen **Sie in der** rechten oberen Ecke Umgebungen aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="2d1a5-157">Dadurch werden die verfügbaren CRM-Instanzen gezeigt.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="2d1a5-158">Wählen Sie in der Dropdownliste rechts oben die entsprechende CRM-Instanz aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="2d1a5-159">Wählen **Sie in** der linken Navigationsleiste Lösungen aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="2d1a5-160">Wählen Sie **im oberen Menü den Link AppSource** öffnen aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öffnen Sie AppSource.":::

5. <span data-ttu-id="2d1a5-162">Suchen Sie **Partner Center Popupbildschirm nach Empfehlungsconnectors** für Salesforce.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. <span data-ttu-id="2d1a5-164">Wählen Sie die **Schaltfläche Jetzt holen** und dann Weiter **aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="2d1a5-165">Dadurch wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung auswählen können, um die Anwendung zu installieren.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="2d1a5-166">Stimmen Sie den Geschäftsbedingungen zu.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Verfügbare CRMS.":::

8. <span data-ttu-id="2d1a5-168">Sie werden dann zur Seite Manage **your solutions (Lösungen verwalten)** geleitet.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="2d1a5-169">Navigieren Sie zu "Partner Center Empfehlungen", indem Sie die Pfeilschaltflächen unten auf der Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="2d1a5-170">**Die geplante Installation** sollte neben Partner Center Empfehlungslösung angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="2d1a5-171">Die Installation dauert 10 bis 15 Minuten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="2d1a5-172">Navigieren Sie nach Abschluss der Installation zurück zum Power Automate [und](https://flow.microsoft.com) wählen Sie **im linken** Navigationsbereich Lösungen aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="2d1a5-173">Beachten **Sie, Partner Center Synchronisierung von** Empfehlungen für Salesforce in der Lösungsliste verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="2d1a5-174">Wählen **Partner Center Synchronisierung von Empfehlungen für Salesforce aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="2d1a5-175">Die folgenden Power Automate und Entitäten sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-Flows.":::



## <a name="configure-the-solution"></a><span data-ttu-id="2d1a5-177">Konfigurieren der Projektmappe</span><span class="sxs-lookup"><span data-stu-id="2d1a5-177">Configure the solution</span></span>

1. <span data-ttu-id="2d1a5-178">Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Power Automate.](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="2d1a5-179">Wählen Sie **in der** Dropdownliste Umgebungen in der rechten oberen Ecke die CRM-Instanz aus, in der Sie die Power Automate installiert haben.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="2d1a5-180">Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="2d1a5-181">Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="2d1a5-182">Partner Center-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="2d1a5-182">Partner Center Events</span></span>
    - <span data-ttu-id="2d1a5-183">CRM-Administrator mit den Power Automate Flows in der Lösung.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="2d1a5-184">Wählen **Sie in** der linken Navigationsleiste Verbindungen aus, und wählen Sie die Lösung "Partner Center Empfehlungen" aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="2d1a5-185">Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen klicken.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Erstellen Sie eine Verbindung.":::

- <span data-ttu-id="2d1a5-187">Suchen Sie Partner Center in der Suchleiste in der oberen rechten Ecke nach Empfehlungen (Vorschau).</span><span class="sxs-lookup"><span data-stu-id="2d1a5-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="2d1a5-188">Erstellen Sie eine Verbindung für Ihren Partner Center benutzer mit der Rolle Anmeldeinformationen des Empfehlungsadministrators.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="2d1a5-189">Erstellen Sie als Nächstes eine Partner Center Events-Verbindung für Ihren Partner Center-Benutzer mit den Anmeldeinformationen des Empfehlungsadministrators.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="2d1a5-190">Erstellen Sie eine Verbindung für Salesforce für den CRM-Administratorbenutzer.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="2d1a5-191">Nachdem Sie alle Verbindungen hinzugefügt haben, sollten die folgenden Verbindungen in Ihrer Umgebung zu sehen sein:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Beobachten Sie Verbindungen.":::

### <a name="edit-the-connections"></a><span data-ttu-id="2d1a5-193">Bearbeiten der Verbindungen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-193">Edit the connections</span></span>

1. <span data-ttu-id="2d1a5-194">Kehren Sie zur Seite Lösungen zurück, und wählen Sie **Standardlösung aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="2d1a5-195">Wählen Sie **Verbindungsverweis (Vorschau) aus,** indem Sie auf **Alle klicken.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Beginnen Sie mit der Connectorbearbeitung.":::

2. <span data-ttu-id="2d1a5-197">Bearbeiten Sie die einzelnen Verbindungen einzeln, indem Sie auf das Symbol mit den drei Punkten klicken.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="2d1a5-198">Fügen Sie die relevanten Verbindungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Bearbeiten sie Connectors.":::

3. <span data-ttu-id="2d1a5-200">Aktivieren Sie die Flows in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="2d1a5-201">Partner Center Webhookregistrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="2d1a5-202">Erstellen einer Co-Sell-Empfehlung – Salesforce Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="2d1a5-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="2d1a5-204">Partner Center to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="2d1a5-205">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="2d1a5-206">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="2d1a5-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="2d1a5-208">Verwenden von Webhook-APIs zum Registrieren für Ressourcenänderungsereignisse</span><span class="sxs-lookup"><span data-stu-id="2d1a5-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="2d1a5-209">Mit Partner Center Webhook-APIs können Sie sich für Ressourcenänderungsereignisse registrieren.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="2d1a5-210">Diese Änderungsereignisse werden als HTTP-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="2d1a5-211">Wählen Sie zum Registrieren Ihrer URL Partner Center **Webhookregistrierung (Insider Preview) Power Automate** aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="2d1a5-212">Fügen Sie Verbindungen für (a.) Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen (b.) Partner Center Ereignisse hinzu, wie unten hervorgehoben.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger.":::

3. <span data-ttu-id="2d1a5-214">Wenn Sie diese Updates machen, sehen Sie:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. <span data-ttu-id="2d1a5-216">Speichern Sie Ihre Änderungen, und wählen **Sie Aktivieren aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="2d1a5-217">Um webhooks Partner Center ereignisänderungen zu lauschen, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="2d1a5-218">Wählen **Partner Center Salesforce CRM (Insider Preview) aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="2d1a5-219">Wählen Sie das **Symbol Bearbeiten** aus, und wählen Sie When a HTTP request is **received (Wenn eine HTTP-Anforderung empfangen wird) aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="2d1a5-220">Wählen Sie das **Symbol Kopieren** aus, um die bereitgestellte HTTP POST-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopier-URL.":::

8. <span data-ttu-id="2d1a5-222">Wählen Sie nun den Flow "Partner Center Webhookregistrierung (Insider-Vorschau)" aus Power Automate und wählen Sie **Ausführen aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="2d1a5-223">Stellen Sie sicher, dass das Fenster "Flow ausführen" im rechten Bereich geöffnet wird, und wählen Sie **Weiter aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="2d1a5-224">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-224">Enter the following details:</span></span>

    1. <span data-ttu-id="2d1a5-225">**HTTP-Triggerendpunkt:** URL aus dem früheren Schritt kopiert</span><span class="sxs-lookup"><span data-stu-id="2d1a5-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="2d1a5-226">**Zu registrierende Ereignisse:**"Empfehlung erstellt" und "Empfehlung aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="2d1a5-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="2d1a5-227">**Vorhandene Triggerendpunkte überschreiben, falls vorhanden:** Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="2d1a5-228">Wählen **Sie Ausführen** und dann Fertig **aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="2d1a5-229">Der Webhook kann jetzt lauschen, um Ereignisse zu erstellen und zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="2d1a5-230">Anpassen von Synchronisierungsschritten</span><span class="sxs-lookup"><span data-stu-id="2d1a5-230">Customize synchronization steps</span></span>

<span data-ttu-id="2d1a5-231">Wenn Co-Sell-Empfehlungen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf einem Partner Center PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="2d1a5-232">CRM-Systeme sind häufig stark angepasst.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="2d1a5-233">Sie können die Power Automate anpassen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="2d1a5-234">Befolgen Sie den Leitfaden zur Feldzuordnung, und nehmen Sie bei Bedarf entsprechende Änderungen an den Schritten der Power Automate vor.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="2d1a5-235">Microsoft Partner Center zu CRM-Zuordnungen werden bereitgestellt, aber basierend auf Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="2d1a5-236">Mehrere Schritte der einzelnen Power Automate können basierend auf Ihren Anforderungen angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="2d1a5-237">Im Folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="2d1a5-238">So passen Sie die Felder für die Erstellungs- oder Aktualisierungsereignisse in der Partner Center CRM-Empfehlungssynchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="2d1a5-239">Wählen Partner Center Salesforce CRM (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="2d1a5-240">Wählen **Sie Bearbeiten** aus, um den Power Automate anzupassen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="2d1a5-241">Wählen **Sie (Bereich) Lead oder Verkaufschance synchronisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="2d1a5-242">Um CRM-Feldzuordnungen für Erstellungsereignisse anzupassen, wählen Sie If it es new Shared opportunity (Wenn es sich um eine neue freigegebene **Verkaufschance) und dann aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="2d1a5-243">Wählen Sie den unteren Schritt **aus, falls ja,** und erweitern Sie dann **Erstellen einer neuen Verkaufschance in CRM**.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="2d1a5-244">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Feldzuordnungshandbuchs bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="2d1a5-245">Um CRM-Feldzuordnungen für Updateereignisse anzupassen, wählen Sie den Schritt "(Bereich) Lead oder Verkaufschance synchronisieren" aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="2d1a5-246">Wählen Sie If it es a update to an opportunity (Wenn es sich um **ein Update einer Verkaufschance) und dann um .**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="2d1a5-247">Wählen Sie den unteren Schritt aus, falls **ja,** und erweitern Sie dann If **difference between the opportunity objects in Partner Center and CRM (Wenn** Unterschied zwischen den Opportunityobjekten in Partner Center CRM) und dann .</span><span class="sxs-lookup"><span data-stu-id="2d1a5-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="2d1a5-248">Wählen Sie **Bei Ja** gefolgt von Update existing **opportunity (Vorhandene Verkaufschance aktualisieren) aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="2d1a5-249">So passen Sie die Felder für die CRM-zu-PC-Empfehlungssynchronisierung für Updateereignisse an:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="2d1a5-250">Wählen **Sie Bearbeiten**  aus, um den Power Automate anzupassen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="2d1a5-251">Wählen **Sie (Bereich) Die Verkaufschance synchronisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="2d1a5-252">Wählen Sie zum Anpassen von CRM-Feldzuordnungen (basierend auf dem Leitfaden für Feldzuordnungen) für Updateereignisse die Option Wenn ein Unterschied zwischen den Leadobjekten **in Partner Center und CRM besteht, dann aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="2d1a5-253">Wählen Sie den unteren Schritt **aus, falls ja,** und erweitern Sie dann den Schritt **Empfehlung mit Verkaufschancedaten aktualisieren.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="2d1a5-254">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Feldzuordnungshandbuch bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="2d1a5-255">Zum Anpassen der Felder für die CRM-zu-PC-Empfehlungssynchronisierung zum Erstellen von Ereignissen?</span><span class="sxs-lookup"><span data-stu-id="2d1a5-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="2d1a5-256">Wählen **Sie Bearbeiten**  aus, um den Power Automate anzupassen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="2d1a5-257">Wählen **Sie (Bereich) Empfehlungen synchronisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="2d1a5-258">Wählen Sie zum Anpassen von CRM-Feldzuordnungen (basierend auf dem Feldzuordnungsleitfaden) für Erstellungsereignisse die Option **Microsoft-Empfehlung erstellen aus.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="2d1a5-259">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Feldzuordnungshandbuch bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="2d1a5-260">Bidirektionale End-to-End-Co-Sell-Empfehlungssynchronisierung</span><span class="sxs-lookup"><span data-stu-id="2d1a5-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="2d1a5-261">Nachdem Sie die Power Automate-Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Sell-Empfehlungen zwischen Salesforce CRM und Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="2d1a5-262">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-262">Pre-requisites</span></span>

<span data-ttu-id="2d1a5-263">Um die Empfehlungen über Partner Center Salesforce CRM hinweg zu synchronisieren, muss die Power Automate-Lösung microsoftspezifische Empfehlungsfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="2d1a5-264">Diese Identifizierung bietet Ihren Verkäuferteams die Möglichkeit, zu entscheiden, welche Empfehlungen sie für den Co-Selling an Microsoft freigeben möchten.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="2d1a5-265">Ein Satz benutzerdefinierter Felder ist als Teil der Entität Partner Center Empfehlungssynchronisierung für Salesforce CRM-Lösung **Opportunity verfügbar.**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="2d1a5-266">Ein CRM-Administratorbenutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten **Opportunity-Feldern** erstellen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="2d1a5-267">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="2d1a5-268">**Sync with Partner Center**:Whether to sync the opportunity with Microsoft Partner Center (Synchronisieren mit Microsoft Partner Center)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="2d1a5-269">**Empfehlungsbezeichner:** Ein schreibgeschütztes Bezeichnerfeld für Microsoft Partner Center-Empfehlung</span><span class="sxs-lookup"><span data-stu-id="2d1a5-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="2d1a5-270">**Empfehlungslink:** Ein schreibgeschützter Link zur Empfehlung im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="2d1a5-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="2d1a5-271">**How can Microsoft help**: Help required from Microsoft for the referral (Hilfe von Microsoft für die Empfehlung erforderlich)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="2d1a5-272">**Produkte:** Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="2d1a5-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="2d1a5-273">**Überwachung:** Ein schreibgeschützter Überwachungspfad für die Synchronisierung mit Partner Center Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="2d1a5-274">Szenarien:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-274">SCENARIOS:</span></span>

1. <span data-ttu-id="2d1a5-275">Empfehlungssynchronisierung beim Erstellen oder Aktualisieren von Empfehlungen in CRM und Synchronisierung in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="2d1a5-276">Melden Sie sich bei Ihrer Salesforce CRM-Umgebung mit einem Benutzer an, der über Sichtbarkeit im Abschnitt **Verkaufschance** des CRM verfügt.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="2d1a5-277">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-Umgebung.":::

   3. <span data-ttu-id="2d1a5-279">Um diese Verkaufschance mit Microsoft Partner Center zu synchronisieren, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="2d1a5-280">"Sync with Partner Center": Ja</span><span class="sxs-lookup"><span data-stu-id="2d1a5-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="2d1a5-281">"Wie kann Microsoft helfen?": Wählen Sie eine der folgenden Optionen aus:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="2d1a5-282">Produkte: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="2d1a5-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="2d1a5-283">Nachdem Sie die Option  **Sync with Partner Center** auf **Ja** festgelegt haben, warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="2d1a5-284">Ihre Empfehlungen werden mit Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="2d1a5-285">Wenn die Option "Mit Partner Center synchronisieren" auf "Ja" festgelegt ist und Sie die Verkaufschance in Salesforce CRM aktualisieren, werden die Änderungen mit Ihrem Partner Center synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="2d1a5-286">Verkaufschancen, die erfolgreich mit Partner Center synchronisiert werden, werden mithilfe ✔ in Salesforce CRM identifiziert.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="2d1a5-287">Empfehlungssynchronisierung, wenn die Empfehlung in Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="2d1a5-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="2d1a5-288">Melden Sie sich bei Ihrem [Partner Center-Dashboard an.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="2d1a5-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="2d1a5-289">Wählen **Sie im menü auf** der linken Seite die Option Empfehlungen aus.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="2d1a5-290">Erstellen Sie eine neue Co-Sell-Empfehlung aus Partner Center indem Sie auf die Option "Neuer Deal" klicken.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="2d1a5-291">Melden Sie sich bei Ihrer Salesforce CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="2d1a5-292">Navigieren Sie zu **Open Opportunities (Verkaufschancen öffnen).**</span><span class="sxs-lookup"><span data-stu-id="2d1a5-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="2d1a5-293">Die im Microsoft Partner Center erstellte Empfehlung wird jetzt in Salesforce CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce-Bildschirm für Verkaufschance.":::

    6. <span data-ttu-id="2d1a5-295">Wenn Sie eine synchronisierte Empfehlung auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="2d1a5-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2d1a5-296">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2d1a5-296">Next steps</span></span>

- [<span data-ttu-id="2d1a5-297">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="2d1a5-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="2d1a5-298">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="2d1a5-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="2d1a5-299">Partner Center-Webhooks</span><span class="sxs-lookup"><span data-stu-id="2d1a5-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
