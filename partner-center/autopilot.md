---
title: Anpassen eines Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen | Partner Center
description: Vorkonfigurieren eines Geräts Out-of-Box-Experience mit Autopilot-Profilen.
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062278"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="cc432-104">Anpassen eines Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen</span><span class="sxs-lookup"><span data-stu-id="cc432-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="cc432-105">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="cc432-105">Applies to</span></span>**

- <span data-ttu-id="cc432-106">CSP-Direct-Rechnung-Partner, indirekte Anbieter und indirekte Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="cc432-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="cc432-107">Wenn Sie Kundengeräte verwalten, müssen Sie die Out-of-Box-Experience (OOBE) für die Kunden eines Benutzers anpassen.</span><span class="sxs-lookup"><span data-stu-id="cc432-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="cc432-108">Sie können neue Geräte mit Windows Autopilot-Profilen vorab zu konfigurieren, bevor die Geräte an Kunden und Anwenden von neuen Profilen auf Geräte, die Kunden bereits erworben haben.</span><span class="sxs-lookup"><span data-stu-id="cc432-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="cc432-109">In diesem Artikel wird erläutert, wie Sie erstellen und Anwenden von Autopilot-Profilen auf Geräte in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cc432-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="cc432-110">Wenn Sie nicht bereits mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:</span><span class="sxs-lookup"><span data-stu-id="cc432-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="cc432-111">Übersicht über Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="cc432-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="cc432-112">Autopilot-Referenz-Bereitstellungshandbuch</span><span class="sxs-lookup"><span data-stu-id="cc432-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="cc432-113">Übersicht</span><span class="sxs-lookup"><span data-stu-id="cc432-113">Overview</span></span>

<span data-ttu-id="cc432-114">Mit dem Windows Autopilot-Feature im Partner Center können Sie benutzerdefinierte Profile für Kundengeräte erstellen.</span><span class="sxs-lookup"><span data-stu-id="cc432-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="cc432-115">Die folgenden profileinstellungen waren zum Zeitpunkt der Veröffentlichung dieses Artikels verfügbar:</span><span class="sxs-lookup"><span data-stu-id="cc432-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="cc432-116">Überspringen Sie datenschutzeinstellungen.</span><span class="sxs-lookup"><span data-stu-id="cc432-116">Skip privacy settings.</span></span> <span data-ttu-id="cc432-117">Dieser optionalen Einstellung der Autopilot-Profil kann Organisationen nicht datenschutzeinstellungen während der OOBE-Prozesses Fragen.</span><span class="sxs-lookup"><span data-stu-id="cc432-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="cc432-118">Deaktivieren Sie die Erstellung des lokalen Administratorkontos auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="cc432-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="cc432-119">Organisationen können entscheiden, ob der Benutzer das Gerät einrichten Administratorzugriff haben soll, nachdem der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="cc432-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="cc432-120">Automatisch Gerät für die Arbeit oder Schule einrichten.</span><span class="sxs-lookup"><span data-stu-id="cc432-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="cc432-121">Alle Geräte mit Autopilot registriert automatisch berücksichtigt werden Arbeit, Schule oder UNI Geräte, damit diese Frage nicht während der OOBE-Prozesses aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="cc432-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="cc432-122">Überspringen Sie Cortana-, Onedrive- und OEM-registrierungssetupseiten.</span><span class="sxs-lookup"><span data-stu-id="cc432-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="cc432-123">Alle Geräte mit Autopilot registriert werden automatisch diese Seiten während des Out-of-Box-Experience (OOBE) zu überspringen.</span><span class="sxs-lookup"><span data-stu-id="cc432-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="cc432-124">Überspringen Sie Endbenutzer-Lizenzvertrag (EULA)</span><span class="sxs-lookup"><span data-stu-id="cc432-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="cc432-125">Ab Windows 10, Version 1709, können Organisationen entscheiden, auf die Seite EULA während der OOBE-Prozess zu überspringen.</span><span class="sxs-lookup"><span data-stu-id="cc432-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="cc432-126">Finden Sie unter [Ablehnung der EULA für Windows Autopilot zu](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Seite "EULA" während des Windows Setup berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="cc432-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="cc432-127">Das folgende Profil und Gerät Delegieren von Berechtigungen und Einschränkungen gelten:</span><span class="sxs-lookup"><span data-stu-id="cc432-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="cc432-128">CSP-Partner können weiterhin zum Verwalten von Autopilot Profile für vorhandene Kunden, mit denen sie Reseller-Geschäftsbeziehungen, haben, auch wenn die Kunden delegierten Administratorrechte des Partners entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="cc432-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="cc432-129">Sie können vorhandene Geräte für Ihre Kunden verwalten, die entweder von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="cc432-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="cc432-130">Sie können keine Geräte verwalten, die Microsoft Store für Unternehmen oder Microsoft Intune-Portal Ihr Kunde hochgeladen hat.</span><span class="sxs-lookup"><span data-stu-id="cc432-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="cc432-131">Erstellen Sie und Verwalten von Autopilot-Profilen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="cc432-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="cc432-132">Im Partner Center können Sie Windows Autopilot-bereitstellungsprofile erstellen und auf Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="cc432-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="cc432-133">Nur Admin-Agents können erstellen und Anwenden von Profilen.</span><span class="sxs-lookup"><span data-stu-id="cc432-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="cc432-134">Erstellen Sie ein neues Autopilot-Profil</span><span class="sxs-lookup"><span data-stu-id="cc432-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="cc432-135">Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, die, dem Sie für das Autopilot-Profil erstellen.</span><span class="sxs-lookup"><span data-stu-id="cc432-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="cc432-136">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="cc432-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cc432-137">Wählen Sie unter **Windows Autopilot Profile** **Neues Profil hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="cc432-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="cc432-138">Geben Sie Namen und eine Beschreibung des Profils, und konfigurieren Sie die Windows-Willkommensseite-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="cc432-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="cc432-139">Wählen Sie aus:</span><span class="sxs-lookup"><span data-stu-id="cc432-139">Choose from:</span></span>  

   - <span data-ttu-id="cc432-140">Überspringen der datenschutzeinstellungen im setup</span><span class="sxs-lookup"><span data-stu-id="cc432-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="cc432-141">Deaktivieren des lokalen Administratorkontos während des Setups</span><span class="sxs-lookup"><span data-stu-id="cc432-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="cc432-142">Automatisches Überspringen von Seiten im Setup</span><span class="sxs-lookup"><span data-stu-id="cc432-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="cc432-143">(Einschließlich *Automatisches Setup für Arbeit oder Schule auswählen* und *Überspringen Cortana, OneDrive und OEM-registrierungssetupseiten*)</span><span class="sxs-lookup"><span data-stu-id="cc432-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="cc432-144">Endbenutzer-Lizenzvertrag (EULA) überspringen</span><span class="sxs-lookup"><span data-stu-id="cc432-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="cc432-145">Finden Sie unter [Ablehnung der EULA für Windows Autopilot zu](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Seite "EULA" während des Windows Setup berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="cc432-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="cc432-146">Wählen Sie abschließend **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="cc432-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="cc432-147">Anwenden einer Autopilot-Profilen auf Kundengeräte</span><span class="sxs-lookup"><span data-stu-id="cc432-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="cc432-148">Die folgenden Anweisungen wird davon ausgegangen, dass Sie bereits Geräte des Kunden in das Partner Center hinzugefügt haben und dass Sie ihre Liste der Geräte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="cc432-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="cc432-149">Wenn Sie Geräte des Kunden bereits hinzugefügt haben, folgen Sie den Anweisungen im [Konto eines Kunden Geräte hinzufügen](#add-devices-to-a-customers-account) , und führen Sie dann die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="cc432-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="cc432-150">Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es auf Geräte des Kunden anwenden.</span><span class="sxs-lookup"><span data-stu-id="cc432-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="cc432-151">Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, die, dem Sie für das Autopilot-Profil erstellt.</span><span class="sxs-lookup"><span data-stu-id="cc432-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="cc432-152">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="cc432-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cc432-153">Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte oder Gerätegruppen, die Sie Profile hinzufügen, und wählen Sie dann **Profil anwenden**möchten.</span><span class="sxs-lookup"><span data-stu-id="cc432-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="cc432-154">Das Profil, das Sie gerade angewendet wird in der Spalte **Profil** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cc432-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="cc432-155">Gehen Sie folgendermaßen vor, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="cc432-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="cc432-156">a.</span><span class="sxs-lookup"><span data-stu-id="cc432-156">a.</span></span>  <span data-ttu-id="cc432-157">Verbinden Sie ein Gerät mit dem Netzwerk, und schalten Sie es ein.</span><span class="sxs-lookup"><span data-stu-id="cc432-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="cc432-158">b.</span><span class="sxs-lookup"><span data-stu-id="cc432-158">b.</span></span>  <span data-ttu-id="cc432-159">Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="cc432-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="cc432-160">c.</span><span class="sxs-lookup"><span data-stu-id="cc432-160">c.</span></span>  <span data-ttu-id="cc432-161">Wenn der OOBE-Prozess beendet wird, setzen Sie das Gerät auf die werksseitigen Standardeinstellungen, um sie für einen neuen Benutzer vorzubereiten.</span><span class="sxs-lookup"><span data-stu-id="cc432-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="cc432-162">Entfernen Sie ein Autopilot-Profil aus dem Gerät eines Kunden</span><span class="sxs-lookup"><span data-stu-id="cc432-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="cc432-163">Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, die, dem Sie für das Autopilot-Profil erstellt.</span><span class="sxs-lookup"><span data-stu-id="cc432-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="cc432-164">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="cc432-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cc432-165">Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte, die Sie entfernen Sie das Profil aus, und wählen Sie dann **Profil entfernen**möchten.</span><span class="sxs-lookup"><span data-stu-id="cc432-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="cc432-166">Entfernen ein Profil von einem Gerät wird nicht das Profil aus der Liste gelöscht.</span><span class="sxs-lookup"><span data-stu-id="cc432-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="cc432-167">Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen in [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="cc432-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="cc432-168">Aktualisieren Sie oder löschen Sie ein Autopilot-Profil</span><span class="sxs-lookup"><span data-stu-id="cc432-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="cc432-169">Wenn ein Kunde die Out-of-Box-Erfahrung zu ändern möchte, nachdem Sie die Geräte darauf geliefert haben, können Sie das Profil in Partner Center ändern.</span><span class="sxs-lookup"><span data-stu-id="cc432-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="cc432-170">Wenn dem Gerät des Kunden mit dem Internet verbunden ist, wird es die neueste Version der Profile herunterladen, während der Windows-Willkommensseite.</span><span class="sxs-lookup"><span data-stu-id="cc432-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="cc432-171">Darüber hinaus wird jedes Mal ein Kunde ein Gerät auf die werksseitigen Standardeinstellungen wiederherstellt das Gerät erneut herunter die neueste Version der Profile während der OOBE-Prozesses.</span><span class="sxs-lookup"><span data-stu-id="cc432-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="cc432-172">Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, der Sie ein Autopilot-Profil zu ändern möchten.</span><span class="sxs-lookup"><span data-stu-id="cc432-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="cc432-173">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="cc432-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cc432-174">Wählen Sie unter **Windows Autopilot Profile** das Profil, das Sie aktualisieren müssen.</span><span class="sxs-lookup"><span data-stu-id="cc432-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="cc432-175">Nehmen Sie die erforderlichen Änderungen vor, und wählen Sie dann **übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="cc432-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="cc432-176">Wählen Sie aus der oberen rechten Ecke der Seite **Profil löschen** , um diesem Profil zu löschen.</span><span class="sxs-lookup"><span data-stu-id="cc432-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="cc432-177">Hinzufügen von Geräten auf dem Konto eines Kunden</span><span class="sxs-lookup"><span data-stu-id="cc432-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="cc432-178">Verkaufsvertreter und Admin-Agents können Geräte auf dem Konto eines Kunden hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="cc432-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="cc432-179">Bevor Sie benutzerdefinierte Autopilot Profile auf Kundengeräte anwenden können, müssen Sie auf dem Gerät der Kundenliste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="cc432-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="cc432-180">Wenn Sie die OEM Name Seriennummer und Modell Kombination verwenden möchten, achten Sie darauf, dass Sie diese Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="cc432-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="cc432-181">Das Tupel funktioniert nur für neuere Geräte (4 k Hashes, z. B.) und wird für 128b Hashes (RS2 und vorherigen Geräte) nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cc432-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="cc432-182">Die Tupel-Registrierung wird Groß-/Kleinschreibung, damit die Daten in der Datei der Hersteller und Modell Namen ***genau*** übereinstimmen müssen von der OEM-Anbieter (Hardwareanbieter) bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="cc432-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="cc432-183">Gehen Sie von Geräten auf dem Konto eines Kunden im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cc432-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="cc432-184">Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, deren Geräte, die Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="cc432-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="cc432-185">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="cc432-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cc432-186">Wählen Sie unter **Anwenden von Profilen auf Geräte** **Geräte hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="cc432-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="cc432-187">Geben Sie einen Namen für die Liste der Geräte, und wählen Sie dann zum Hochladen des Kunden Liste (CSV-Format) in Partner Center **Durchsuchen** .</span><span class="sxs-lookup"><span data-stu-id="cc432-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="cc432-188">Sie sollten diese CSV-Datei mit dem Gerät Kauf erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="cc432-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="cc432-189">Wenn Sie eine CSV-Datei nicht erhalten haben, können Sie selbst erstellen, mithilfe der Schritte im [Windows Autopilot-Geräte hinzufügen](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="cc432-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="cc432-190">Laden Sie die CSV-Datei, und wählen Sie dann **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="cc432-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="cc432-191">Wenn Sie eine Fehlermeldung, beim Versuch erhalten, die CSV-Datei hochzuladen, überprüfen Sie das Format der Datei.</span><span class="sxs-lookup"><span data-stu-id="cc432-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="cc432-192">Sie können nur den Hardwarehash oder den OEM-Namen, Seriennummer, und Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID verwenden.</span><span class="sxs-lookup"><span data-stu-id="cc432-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="cc432-193">Sie können auch die Beispiel-CSV-Datei über den Link neben **Hinzufügen Geräte** bereitgestellt verwenden, um eine Liste der Geräte zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="cc432-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="cc432-194">Ablehnung der EULA für Windows Autopilot zu</span><span class="sxs-lookup"><span data-stu-id="cc432-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="cc432-195">WICHTIGE INFORMATIONEN</span><span class="sxs-lookup"><span data-stu-id="cc432-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="cc432-196">Windows Autopilot können Sie benutzerdefinierte Installationen von Windows auf Geräten zu konfigurieren, die Sie für Ihre Kunden verwalten.</span><span class="sxs-lookup"><span data-stu-id="cc432-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="cc432-197">Wenn dazu berechtigt, vom Kunden, können bestimmte Setupbildschirme, die normalerweise für Benutzer beim Einrichten von Windows, darunter der Bildschirm für die Annahme EULA (End User License Agreement) angezeigt werden Sie unterdrücken oder ausblenden.</span><span class="sxs-lookup"><span data-stu-id="cc432-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="cc432-198">Durch die Verwendung dieser Funktion stimmen Sie, dass das unterdrücken oder Ausblenden von Bildschirmen, die so konzipiert sind, um Benutzern zu liefern oder die Annahme von Begriffe bedeutet, dass Sie über ausreichende Zustimmung und Autorisierung von Ihrem Kunden Begriffe und, dass Sie im Auftrag von ausblenden abgerufen haben Ihr Kunde (gibt an, ob eine Organisation oder einzelner Benutzer der Fall sein kann), um solche Zustimmung und akzeptiert Begriffe, die an den Kunden relevant sind.</span><span class="sxs-lookup"><span data-stu-id="cc432-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="cc432-199">Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten.</span><span class="sxs-lookup"><span data-stu-id="cc432-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="cc432-200">Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.</span><span class="sxs-lookup"><span data-stu-id="cc432-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>