---
title: Anpassen eines Geräts Out-of-Box-Erfahrung mit Windows Autopilot-Profile | Partner Center
description: Konfigurieren eines Geräts Out-of-Box-Experience mit Autopilot-Profile.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero Touch-Bereitstellung, Oobe, Anmeldung Bildschirme, Out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586913"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="7c098-104">Anpassen eines Geräts Out-of-Box-Erfahrung mit Windows Autopilot-Profile</span><span class="sxs-lookup"><span data-stu-id="7c098-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="7c098-105">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="7c098-105">**Applies to**</span></span>

- <span data-ttu-id="7c098-106">Direkt vor kurzem verstorbenen Bill CSP-Partner, indirekte Anbieter und indirekten Vertriebspartner</span><span class="sxs-lookup"><span data-stu-id="7c098-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="7c098-107">Wenn Sie die Customer-Geräte verwalten, müssen Sie die Out-of-Box-Experience (OOBE) für den Kunden eines Benutzers anpassen.</span><span class="sxs-lookup"><span data-stu-id="7c098-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="7c098-108">Sie können neue Geräte mit Windows Autopilot-Profile vorkonfigurieren, bevor die Bereitstellung von Geräten für Kunden, und wenden neue Profile für Geräte, die Kunden bereits gekauft haben.</span><span class="sxs-lookup"><span data-stu-id="7c098-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="7c098-109">In diesem Artikel wird erläutert, wie zum Erstellen und Anwenden von Autopilot-Profile für Geräte im Partner Center wird.</span><span class="sxs-lookup"><span data-stu-id="7c098-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="7c098-110">Wenn Sie nicht bereits mit Autopilot vertraut sind, überprüfen Sie die Informationen in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="7c098-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="7c098-111">Übersicht über Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="7c098-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="7c098-112">Autopilot Deployment-Referenzhandbuch</span><span class="sxs-lookup"><span data-stu-id="7c098-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="7c098-113">Übersicht</span><span class="sxs-lookup"><span data-stu-id="7c098-113">Overview</span></span>

<span data-ttu-id="7c098-114">Mit dem Windows Autopilot-Feature im Partner Center können Sie benutzerdefinierte Profile gelten für Kundengeräte erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c098-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="7c098-115">Die folgenden profileinstellungen, waren zum Zeitpunkt der Veröffentlichung dieses Artikels verfügbar:</span><span class="sxs-lookup"><span data-stu-id="7c098-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="7c098-116">Überspringen Sie die datenschutzeinstellungen.</span><span class="sxs-lookup"><span data-stu-id="7c098-116">Skip privacy settings.</span></span> <span data-ttu-id="7c098-117">Diese optionale Einstellung des Autopilot-Profil kann Organisationen nicht während des OOBE-Prozesses zu datenschutzeinstellungen zu stellen.</span><span class="sxs-lookup"><span data-stu-id="7c098-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="7c098-118">Deaktivieren Sie die Erstellung des Kontos Lokaler Administrator auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="7c098-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="7c098-119">Organisationen können entscheiden, ob der Benutzer, die zum Einrichten des Geräts Administratorzugriff erhalten soll, sobald der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="7c098-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="7c098-120">Richten Sie automatisch Geräte für Geschäfts-, Schul- oder unikonto ein.</span><span class="sxs-lookup"><span data-stu-id="7c098-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="7c098-121">Alle Autopilot registrierten Geräte automatisch betrachtet Arbeit oder Schule Geräte aus, damit diese Frage nicht während des OOBE-Prozesses aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="7c098-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="7c098-122">Skip Cortana, OneDrive und OEM-Setup Registrierungsseiten.</span><span class="sxs-lookup"><span data-stu-id="7c098-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="7c098-123">Alle Autopilot registrierten Geräte werden auf diesen Seiten automatisch bei der Out-of-Box-Experience (OOBE) übersprungen werden.</span><span class="sxs-lookup"><span data-stu-id="7c098-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="7c098-124">Überspringen Sie die Endbenutzer-Lizenzvertrag (EULA).</span><span class="sxs-lookup"><span data-stu-id="7c098-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="7c098-125">Ab Windows 10 Version 1709, können Organisationen entscheiden, um die EULA-Seite angezeigt, die während des OOBE-Prozesses zu überspringen.</span><span class="sxs-lookup"><span data-stu-id="7c098-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="7c098-126">Finden Sie unter [Windows Autopilot-Endbenutzer-Lizenzvertrag Kündigung](#windows-autopilot-eula-dismissal) unten für wichtige Informationen, die über die Seite "LIZENZBEDINGUNGEN" wird übersprungen, während Windows einrichten.</span><span class="sxs-lookup"><span data-stu-id="7c098-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="7c098-127">Die folgenden Profile und Device Management-Berechtigungen und Einschränkungen gelten:</span><span class="sxs-lookup"><span data-stu-id="7c098-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="7c098-128">CSP-Partner können weiterhin zum Verwalten von Autopilot-Profile für bestehende Kunden, mit denen sie Reseller Beziehungen haben, auch wenn Kunden die delegierte Administration Berechtigungen des Partners entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="7c098-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="7c098-129">Sie können ein vorhandenes Gerät für Ihre Kunden verwalten, die von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="7c098-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="7c098-130">Sie können keine Geräte verwalten, die Ihren Kunden zu Microsoft Store für Unternehmen oder das Microsoft Intune-Portal hochgeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="7c098-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="7c098-131">Erstellen und Verwalten von Autopilot-Profile im Partner Center</span><span class="sxs-lookup"><span data-stu-id="7c098-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="7c098-132">Im Partner Center können Sie Windows Autopilot-bereitstellungsprofile erstellen und auf Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="7c098-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="7c098-133">Nur Administrator-Agents erstellen und Anwenden von Profilen.</span><span class="sxs-lookup"><span data-stu-id="7c098-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="7c098-134">Erstellen eines neuen Autopilot-Profils</span><span class="sxs-lookup"><span data-stu-id="7c098-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="7c098-135">Wählen Sie **Kunden** aus dem Partner Center-Menü und wählen Sie dann den Kunden Sie erstellen das Autopilot-Profil für.</span><span class="sxs-lookup"><span data-stu-id="7c098-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="7c098-136">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="7c098-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="7c098-137">Klicken Sie unter **Windows Autopilot-Profile** wählen **neues Profil hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="7c098-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="7c098-138">Geben Sie Namen und eine Beschreibung des Profils, und klicken Sie dann konfigurieren Sie die OOBE-Einstellungen zu.</span><span class="sxs-lookup"><span data-stu-id="7c098-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="7c098-139">Es stehen folgende Optionen zur Auswahl:</span><span class="sxs-lookup"><span data-stu-id="7c098-139">Choose from:</span></span>  

   - <span data-ttu-id="7c098-140">Datenschutzeinstellungen für in-Setup überspringen</span><span class="sxs-lookup"><span data-stu-id="7c098-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="7c098-141">Deaktivieren des lokalen Administratorkontos während des Setups</span><span class="sxs-lookup"><span data-stu-id="7c098-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="7c098-142">Automatisches Überspringen von Seiten im Setup</span><span class="sxs-lookup"><span data-stu-id="7c098-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="7c098-143">(Umfasst *automatisch auswählen des Setupprogramms für Geschäfts-, Schul- oder unikonto* und *Skip Cortana, OneDrive und OEM-Setup Registrierungsseiten*)</span><span class="sxs-lookup"><span data-stu-id="7c098-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="7c098-144">Endbenutzer-Lizenzvertrag (EULA) überspringen</span><span class="sxs-lookup"><span data-stu-id="7c098-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="7c098-145">Finden Sie unter [Windows Autopilot-Endbenutzer-Lizenzvertrag Kündigung](#windows-autopilot-eula-dismissal) unten für wichtige Informationen, die über die Seite "LIZENZBEDINGUNGEN" wird übersprungen, während Windows einrichten.</span><span class="sxs-lookup"><span data-stu-id="7c098-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="7c098-146">Wählen Sie abschließend **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="7c098-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="7c098-147">Ein Autopilot-Profil auf kundengeräten anwenden</span><span class="sxs-lookup"><span data-stu-id="7c098-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="7c098-148">Die folgenden Anweisungen wird davon ausgegangen, dass Sie bereits des Kunden Geräte zum Partner Center hinzugefügt haben und Sie ihre Geräteliste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="7c098-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="7c098-149">Falls Sie bereits die Kunden-Geräte hinzugefügt haben, befolgen Sie die Anweisungen in [Geräte hinzufügen, um ein Kundenkonto](#add-devices-to-a-customers-account) und befolgen Sie dann die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="7c098-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="7c098-150">Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es an den Kunden Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="7c098-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="7c098-151">Wählen Sie **Kunden** über das Partner Center-Menü, und wählen Sie dann den Kunden Sie erstellt haben das Autopilot-Profil für.</span><span class="sxs-lookup"><span data-stu-id="7c098-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="7c098-152">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="7c098-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="7c098-153">Klicken Sie unter **gelten Profile für Geräte** wählen Sie die Geräte oder Gerätegruppen, die Sie verwenden möchten, Hinzufügen von Profilen, und wählen Sie dann **Profil anwenden**.</span><span class="sxs-lookup"><span data-stu-id="7c098-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="7c098-154">Das Profil, das Sie soeben angewendet wird, der **Profil** Spalte.</span><span class="sxs-lookup"><span data-stu-id="7c098-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="7c098-155">Gehen Sie folgendermaßen vor, um sicherzustellen, dass das Profil wird erfolgreich an das Gerät angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="7c098-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="7c098-156">a.</span><span class="sxs-lookup"><span data-stu-id="7c098-156">a.</span></span>  <span data-ttu-id="7c098-157">Verbinden Sie ein Gerät mit dem Netzwerk, und aktivieren Sie ihn.</span><span class="sxs-lookup"><span data-stu-id="7c098-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="7c098-158">b.</span><span class="sxs-lookup"><span data-stu-id="7c098-158">b.</span></span>  <span data-ttu-id="7c098-159">Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="7c098-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="7c098-160">c.</span><span class="sxs-lookup"><span data-stu-id="7c098-160">c.</span></span>  <span data-ttu-id="7c098-161">Wenn Sie den OOBE-Prozess beendet wird, Zurücksetzen des Geräts, auf die werkseitigen Standardeinstellungen für die vorzubereitende für einen neuen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7c098-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="7c098-162">Entfernen Sie ein Autopilot-Profil von einem Kunden-Gerät</span><span class="sxs-lookup"><span data-stu-id="7c098-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="7c098-163">Wählen Sie **Kunden** über das Partner Center-Menü, und wählen Sie dann den Kunden Sie erstellt haben das Autopilot-Profil für.</span><span class="sxs-lookup"><span data-stu-id="7c098-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="7c098-164">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="7c098-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="7c098-165">Klicken Sie unter **gelten Profile für Geräte** wählen Sie die Geräte, die Sie verwenden möchten, entfernen Sie das Profil aus, und wählen Sie dann **Profil entfernen**.</span><span class="sxs-lookup"><span data-stu-id="7c098-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="7c098-166">Ein Profil von einem Gerät entfernen, wird das Profil nicht aus der Liste gelöscht.</span><span class="sxs-lookup"><span data-stu-id="7c098-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="7c098-167">Wenn Sie ein Profil löschen möchten, befolgen Sie die Anweisungen in [Update- oder Delete ein Autopilot-Profil](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="7c098-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="7c098-168">Aktualisieren Sie oder löschen Sie ein Autopilot-Profil</span><span class="sxs-lookup"><span data-stu-id="7c098-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="7c098-169">Wenn ein Kunde die Out-of-Box-Experience zu ändern möchte, nachdem Sie die Geräte auf diese geliefert haben, können Sie das Profil im Partner Center ändern.</span><span class="sxs-lookup"><span data-stu-id="7c098-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="7c098-170">Wenn die das Gerät eines Kunden mit dem Internet verbunden ist, wird die aktuelle Profilversion während des OOBE-Prozesses heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="7c098-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="7c098-171">Außerdem wird jedes Mal ein Kunde ein Gerät auf die werkseitigen Standardeinstellungen zurückgesetzt wird das Gerät erneut die neueste Profilversion während des OOBE-Prozesses herunterladen.</span><span class="sxs-lookup"><span data-stu-id="7c098-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="7c098-172">Wählen Sie **Kunden** aus dem Partner Center-Menü und wählen Sie dann den Kunden mit der Sie ein Autopilot-Profil ändern möchte.</span><span class="sxs-lookup"><span data-stu-id="7c098-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="7c098-173">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="7c098-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="7c098-174">Klicken Sie unter **Windows Autopilot-Profile** wählen Sie das Profil, das Sie aktualisieren müssen.</span><span class="sxs-lookup"><span data-stu-id="7c098-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="7c098-175">Die erforderlichen Änderungen vornehmen, und wählen Sie dann **senden**.</span><span class="sxs-lookup"><span data-stu-id="7c098-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="7c098-176">Wählen Sie zum Löschen dieses Profils **Profil löschen** der oberen rechten Ecke der Seite.</span><span class="sxs-lookup"><span data-stu-id="7c098-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="7c098-177">Fügen Sie Geräte hinzu, um ein Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="7c098-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="7c098-178">Vertreter und Administrator-Agents können Geräte, ein Kundenkonto hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="7c098-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="7c098-179">Bevor Sie benutzerdefinierte Autopilot-Profile auf kundengeräten anwenden können, müssen Sie Geräteliste des Kunden Zugriff auf sein.</span><span class="sxs-lookup"><span data-stu-id="7c098-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="7c098-180">Wenn Sie die OEM-Name, Seriennummer und Modell Kombination verwenden möchten, achten Sie darauf, dass Sie diese Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="7c098-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="7c098-181">Diese Tupel funktioniert nur für neuere Geräte (4 k Hashes, z. B.) und wird für 128b-Hashes (RS2 und vorherige Geräten) nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c098-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="7c098-182">Die Registrierung des Tupel ist Groß-/ Kleinschreibung, damit die Daten in der Datei den Hersteller und Modell-Namen übereinstimmen müssen ***genau*** gemäß der OEM-Anbieter (Hardwareanbieter).</span><span class="sxs-lookup"><span data-stu-id="7c098-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="7c098-183">Führen Sie die nachstehenden Anweisungen zum Hinzufügen von Geräten zum Konto eines Kunden im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="7c098-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="7c098-184">Wählen Sie **Kunden** aus dem Partner Center-Menü und wählen Sie dann den Kunden, deren Geräte, die Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="7c098-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="7c098-185">Wählen Sie auf der Detailseite des Kunden **Geräte**.</span><span class="sxs-lookup"><span data-stu-id="7c098-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="7c098-186">Klicken Sie unter **gelten Profile für Geräte** wählen **Geräte hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="7c098-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="7c098-187">Geben Sie einen Namen für die Geräteliste aus, und wählen Sie dann **Durchsuchen** die Kundenliste (im Format der CSV-Datei) in Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="7c098-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="7c098-188">Sie sollten diese CSV-Datei mit dem Gerät Kauf erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="7c098-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="7c098-189">Wenn Sie eine CSV-Datei nicht angezeigt wird, können Sie selbst eine erstellen, indem Sie die Schritte in [Hinzufügen von Geräten in Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="7c098-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="7c098-190">Hochladen die CSV-Datei, und wählen Sie dann **speichern**.</span><span class="sxs-lookup"><span data-stu-id="7c098-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="7c098-191">Wenn Sie eine Fehlermeldung erhalten, bei dem Versuch, die zum Hochladen der CSV-Datei, überprüfen Sie das Format der Datei ein.</span><span class="sxs-lookup"><span data-stu-id="7c098-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="7c098-192">Sie können nur der Hardwarehash oder der OEM-Name, Seriennummer und -Modell (in dieser Reihenfolge) oder die Windows-Produkt-ID verwenden.</span><span class="sxs-lookup"><span data-stu-id="7c098-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="7c098-193">Sie können auch die Beispiel-CSV-Datei bereitgestellt über den Link neben **Geräte hinzufügen** um eine Liste der Geräte zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c098-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="7c098-194">Windows Autopilot-Endbenutzer-Lizenzvertrag Kündigung</span><span class="sxs-lookup"><span data-stu-id="7c098-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="7c098-195">WICHTIGE INFORMATIONEN</span><span class="sxs-lookup"><span data-stu-id="7c098-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="7c098-196">Windows Autopilot können Sie zum Konfigurieren von benutzerdefinierter Installationen von Windows auf Geräten, die Sie für Ihre Kunden zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="7c098-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="7c098-197">Wenn dazu autorisiert, durch den Kunden, können bestimmte Einrichtung-Seiten, die normalerweise für Benutzer, beim Einrichten von Windows angezeigt werden, einschließlich des Bildschirms des Endbenutzer-Lizenzvertrag (End User License Agreement) akzeptieren Sie unterdrücken oder ausblenden.</span><span class="sxs-lookup"><span data-stu-id="7c098-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="7c098-198">Mit dieser Funktion stimmen Sie folgendem zu unterdrücken oder Ausblenden der Bildschirme, mit denen Benutzern bereitstellen, beachten Sie, dass oder Akzeptanz von Nutzungsbedingungen bedeutet, dass Sie ausreichend Zustimmung und Autorisierung aus Ihrem Kunden, die Begriffe und, die von Ihnen im Auftrag von ausblenden erhalten haben der Kunde (gibt an, ob eine Organisation oder einen einzelnen Benutzer als der Fall sein kann), stimmen von Hinweisen und akzeptieren Sie alle Bedingungen, die an den Kunden anwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="7c098-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="7c098-199">Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten.</span><span class="sxs-lookup"><span data-stu-id="7c098-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="7c098-200">Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.</span><span class="sxs-lookup"><span data-stu-id="7c098-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>