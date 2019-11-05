---
title: Anpassen der Windows-Willkommensseite eines Geräts mit Windows Autopilot-Profilen | Partner Center
description: Vorkonfigurieren der Windows-Willkommensseite eines Geräts mit Autopilot-Profilen.
ms.topic: article
ms.date: 03/18/2019
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Willkommensseite
ms.localizationpriority: medium
ms.openlocfilehash: 7861efa8c0fd7e03488ba3f222fcb3a476c06cc2
ms.sourcegitcommit: 76c34fd8dc544cea93496079df68759a1da9098c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/04/2019
ms.locfileid: "73544054"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="1d8c1-104">Anpassen der Windows-Willkommensseite eines Geräts mit Windows Autopilot-Profilen</span><span class="sxs-lookup"><span data-stu-id="1d8c1-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="1d8c1-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="1d8c1-105">**Applies to**</span></span>

- <span data-ttu-id="1d8c1-106">CSP-Partner mit Direktfakturierung, indirekte Anbieter und indirekte Vertriebspartner</span><span class="sxs-lookup"><span data-stu-id="1d8c1-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="1d8c1-107">Wenn Sie Kundengeräte verwalten, müssen Sie die Windows-Willkommensseite für die Benutzer des Kunden anpassen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="1d8c1-108">Sie können neue Geräte mit Windows Autopilot-Profilen vorkonfigurieren, bevor Sie die Geräte an Kunden ausliefern, und neue Profile auf bereits erworbene Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="1d8c1-109">Beachten Sie, dass OEMs damit begonnen haben, eine Versand Bezeichnung auf der Außenseite des Autopilot-Geräts hinzufügen, die die **Product Key-ID (pkid)** des Geräts anzeigt.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-109">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device’s **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="1d8c1-110">Dieser eindimensionale, lesbare Barcode bietet downstreampartnern eine Möglichkeit, Geräte für Autopilot zu registrieren, ohne die Geräte zu entkacken und die Geräte-ID auf alternative Weise zu erfassen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-110">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="1d8c1-111">In diesem Artikel wird erläutert, wie Sie im Partner Center Autopilot-Profile erstellen und auf Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-111">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="1d8c1-112">Wenn Sie noch nicht mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-112">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="1d8c1-113">Übersicht über Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="1d8c1-113">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="1d8c1-114">Referenzhandbuch für die Bereitstellung mit Autopilot</span><span class="sxs-lookup"><span data-stu-id="1d8c1-114">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="1d8c1-115">Übersicht</span><span class="sxs-lookup"><span data-stu-id="1d8c1-115">Overview</span></span>

<span data-ttu-id="1d8c1-116">Mit der Windows-Funktion Autopilot im Partner Center können Sie benutzerdefinierte Profile erstellen und diese auf Kundengeräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-116">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="1d8c1-117">Zum Zeitpunkt der Veröffentlichung dieses Artikels waren die folgenden Profileinstellungen verfügbar:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-117">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="1d8c1-118">Datenschutzeinstellungen überspringen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-118">Skip privacy settings.</span></span> <span data-ttu-id="1d8c1-119">Diese optionale Einstellung im Autopilot-Profil ermöglicht Organisationen, auf Fragen zu Datenschutzeinstellungen auf der Windows-Willkommensseite zu verzichten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-119">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="1d8c1-120">Erstellung des lokalen Administratorkontos auf dem Gerät deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-120">Disable local admin account creation on the device.</span></span> <span data-ttu-id="1d8c1-121">Organisationen können entscheiden, ob der Benutzer, der das Gerät einrichtet, nach Abschluss des Vorgangs Administratorrechte erhalten soll.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-121">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="1d8c1-122">Gerät automatisch für Arbeit oder Bildungseinrichtung einrichten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-122">Automatically set up device for work or school.</span></span> <span data-ttu-id="1d8c1-123">Alle mit Autopilot registrierten Geräte gelten automatisch als Arbeits- und Bildungseinrichtungsgeräte, weshalb diese Frage im zur Windows-Willkommensseite gehörigen Prozess nicht gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-123">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="1d8c1-124">Setupseiten für Cortana-, OneDrive- und OEM-Registrierung überspringen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-124">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="1d8c1-125">Bei allen mit Autopilot registrierten Geräten werden diese Seiten im zur Windows-Willkommensseite gehörigen Prozess automatisch übersprungen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-125">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="1d8c1-126">Lizenzbedingungen überspringen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-126">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="1d8c1-127">Ab Windows 10 Version 1709 können Organisationen sich entscheiden, ob die im zur Windows-Willkommensseite gehörigen Prozess gezeigte Seite mit den Lizenzbedingungen übersprungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-127">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="1d8c1-128">Unter [Ablehnung der Lizenzbedingungen für Windows Autopilot](#windows-autopilot-eula-dismissal) finden Sie wichtige zu beachtende Informationen beim Überspringen der Seite mit den Lizenzbedingungen während des Setups von Windows.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-128">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="1d8c1-129">Die folgenden Berechtigungen und Einschränkungen für die Verwaltung von Profilen und Geräten gelten:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-129">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="1d8c1-130">CSP-Partner können weiterhin die Autopilot-Profile für Bestandskunden mit Vertriebspartnerschaft verwalten, auch wenn die Kunden die Berechtigungen für die delegierte Verwaltung für den Partner aufgehoben haben.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-130">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="1d8c1-131">Sie können vorhandene Geräte für Ihre Kunden verwalten, die Sie hinzugefügt haben.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-131">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="1d8c1-132">Sie können keine Geräte verwalten, die Ihr Kunde in den Microsoft Store für Unternehmen oder das Microsoft Intune-Portal hochgeladen hat.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-132">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="1d8c1-133">Erstellen und Verwalten von Autopilot-Profilen im Partner Center</span><span class="sxs-lookup"><span data-stu-id="1d8c1-133">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="1d8c1-134">Im Partner Center können Sie Windows Autopilot-Bereitstellungsprofile erstellen und auf Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-134">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="1d8c1-135">Nur Administrator-Agents können Profile erstellen und anwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-135">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="1d8c1-136">Erstellen eines neuen Autopilot-Profils</span><span class="sxs-lookup"><span data-stu-id="1d8c1-136">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="1d8c1-137">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-137">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="1d8c1-138">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-138">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="1d8c1-139">Klicken Sie unter **Windows Autopilot-Profile** auf **Neues Profil hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-139">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="1d8c1-140">Geben Sie Namen und eine Beschreibung des Profils ein, und konfigurieren Sie dann die Einstellungen für die Windows-Willkommensseite.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-140">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="1d8c1-141">Es stehen folgende Optionen zur Auswahl:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-141">Choose from:</span></span>  

   - <span data-ttu-id="1d8c1-142">Datenschutzeinstellungen beim Setup überspringen</span><span class="sxs-lookup"><span data-stu-id="1d8c1-142">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="1d8c1-143">Lokales Administratorkonto beim Setup deaktivieren</span><span class="sxs-lookup"><span data-stu-id="1d8c1-143">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="1d8c1-144">Seiten beim Setup automatisch überspringen</span><span class="sxs-lookup"><span data-stu-id="1d8c1-144">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="1d8c1-145">(Schließt *Setup für Arbeit oder Bildungseinrichtung automatisch auswählen* und *Setupseiten für Cortana-, OneDrive- und OEM-Registrierung überspringen* ein)</span><span class="sxs-lookup"><span data-stu-id="1d8c1-145">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="1d8c1-146">Lizenzbedingungen überspringen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-146">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="1d8c1-147">Unter [Ablehnung der Lizenzbedingungen für Windows Autopilot](#windows-autopilot-eula-dismissal) finden Sie wichtige zu beachtende Informationen beim Überspringen der Seite mit den Lizenzbedingungen während des Setups von Windows.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-147">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="1d8c1-148">Klicken Sie abschließend auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-148">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="1d8c1-149">Anwenden eines Autopilot-Profils auf Kundengeräte</span><span class="sxs-lookup"><span data-stu-id="1d8c1-149">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="1d8c1-150">Die folgenden Anweisungen gehen davon aus, dass Sie die Geräte des Kunden bereits dem Partner Center hinzugefügt haben und dass Sie auf dessen Geräteliste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-150">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="1d8c1-151">Wenn Sie die Geräte des Kunden noch nicht hinzugefügt haben, folgen Sie den Anweisungen unter [Hinzufügen von Geräten zu einem Kundenkonto](#add-devices-to-a-customers-account), und führen Sie dann die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-151">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="1d8c1-152">Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es auf die Geräte des Kunden anwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-152">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="1d8c1-153">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-153">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="1d8c1-154">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-154">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="1d8c1-155">Wählen Sie unter **Profile auf Geräte anwenden** die Geräte oder Gerätegruppen aus, denen Sie Profile hinzufügen möchten, und klicken Sie dann auf **Profil anwenden**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-155">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="1d8c1-156">Das Profil, das Sie soeben angewendet haben, wird in der Spalte **Profil** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-156">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="1d8c1-157">Führen Sie die folgenden Schritte aus, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-157">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="1d8c1-158">a.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-158">a.</span></span>  <span data-ttu-id="1d8c1-159">Schließen Sie ein Gerät an das Netzwerk an, und schalten Sie es ein.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-159">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="1d8c1-160">b.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-160">b.</span></span>  <span data-ttu-id="1d8c1-161">Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-161">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="1d8c1-162">c.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-162">c.</span></span>  <span data-ttu-id="1d8c1-163">Wenn der zur Windows-Willkommensseite gehörige Prozess beendet ist, setzen Sie das Gerät auf die Werkseinstellungen zurück, um es für einen neuen Benutzer vorzubereiten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-163">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="1d8c1-164">Entfernen eines Autopilot-Profils von einem Kundengerät</span><span class="sxs-lookup"><span data-stu-id="1d8c1-164">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="1d8c1-165">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-165">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="1d8c1-166">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-166">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="1d8c1-167">Wählen Sie unter **Profile auf Geräte anwenden** die Geräte aus, von denen Sie das Profil entfernen möchten, und klicken Sie dann auf **Profil entfernen**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-167">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="1d8c1-168">Wenn Sie ein Profil von einem Gerät entfernen, wird das Profil nicht aus Ihrer Liste gelöscht.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-168">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="1d8c1-169">Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen unter [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="1d8c1-169">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="1d8c1-170">Aktualisieren oder Löschen eines AutoPilot-Profils</span><span class="sxs-lookup"><span data-stu-id="1d8c1-170">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="1d8c1-171">Wenn ein Kunde die Windows-Willkommensseite ändern möchte, nachdem Sie ihm Geräte geliefert haben, können Sie das Profil im Partner Center ändern.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-171">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="1d8c1-172">Wenn sich das Gerät des Kunden mit dem Internet verbindet, wird während des zur Windows-Willkommensseite gehörigen Prozesses die neueste Profilversion heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-172">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="1d8c1-173">Außerdem lädt das Gerät jedes Mal, wenn ein Kunde ein Gerät auf die Werkseinstellungen zurücksetzt, während des zur Windows-Willkommensseite gehörigen Prozesses erneut die neueste Profilversion herunter.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-173">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="1d8c1-174">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, dessen Autopilot-Profil Sie ändern sollen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-174">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="1d8c1-175">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-175">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="1d8c1-176">Wählen Sie unter **Windows Autopilot-Profile** das Profil aus, das Sie aktualisieren müssen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-176">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="1d8c1-177">Nehmen Sie die erforderlichen Änderungen vor, und klicken Sie dann auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-177">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="1d8c1-178">Um dieses Profil zu löschen, klicken Sie rechts oben auf der Seite auf **Profil löschen**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-178">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="1d8c1-179">Hinzufügen von Geräten zum Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="1d8c1-179">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="1d8c1-180">Vertriebs- und Verwaltungsmitarbeiter können dem Konto eines Kunden Geräte hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-180">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="1d8c1-181">Bevor Sie benutzerdefinierte Autopilot-Profile auf Kundengeräten anwenden können, müssen Sie Zugriff auf die Geräteliste des Kunden haben.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-181">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="1d8c1-182">Wenn Sie planen, die Kombination aus OEM-Name, Seriennummer und Modell zu verwenden, beachten Sie diese Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-182">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="1d8c1-183">Dieses Tupel funktioniert nur für neuere Geräte (z.B. 4K-Hashes) und wird für 128B-Hashes (RS2 und frühere Geräte) nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-183">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="1d8c1-184">Bei der Registrierung des Tupels wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen die Daten in der Datei mit den Modell- und Herstellernamen ***genau*** mit den Angaben des OEM-Anbieters (Hardwareanbieters) übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-184">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="1d8c1-185">Führen Sie die im Partner Center nachstehenden Anweisungen zum Hinzufügen von Geräten zum Konto eines Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-185">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="1d8c1-186">Wählen Sie im Partner Center-Menü **Kunden** und dann den Kunden aus, dessen Geräte Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-186">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="1d8c1-187">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-187">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="1d8c1-188">Klicken Sie unter **Profile auf Geräte anwenden**  auf **Geräte hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-188">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="1d8c1-189">Geben Sie einen Namen für die Geräteliste aus, und klicken Sie dann auf **Durchsuchen**, um die Kundenliste (im Dateiformat CSV) ins Partner Center hochzuladen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-189">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="1d8c1-190">Beim Kauf Ihres Geräts sollten Sie diese CSV-Datei erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-190">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="1d8c1-191">Wenn Sie keine CSV-Datei erhalten haben, können Sie selbst eine erstellen, indem Sie die Schritte unter [Hinzufügen von Geräten zu Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell) ausführen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-191">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="1d8c1-192">Laden Sie die CSV-Datei hoch, und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-192">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="1d8c1-193">Wenn Sie beim Versuch, die CSV-Datei hochzuladen, eine Fehlermeldung erhalten, überprüfen Sie das Format der Datei.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-193">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="1d8c1-194">Sie können nur den Hardwarehash oder den OEM-Namen, die Seriennummer und das Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID verwenden.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-194">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="1d8c1-195">Sie können auch die CSV-Beispieldatei verwenden, die über den Link neben **Geräte hinzufügen** bereitgestellt wird, um eine Geräteliste zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-195">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="1d8c1-196">Die CSV-Datei sollte in etwa wie folgt aussehen:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-196">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="1d8c1-197">**Seriennummer des Geräts, Windows-Produkt-ID, Hardware Hash, Herstellername, Gerätemodell**</span><span class="sxs-lookup"><span data-stu-id="1d8c1-197">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="1d8c1-198">**{SerialNumber},,, Microsoft Corporation, Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="1d8c1-198">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

<span data-ttu-id="1d8c1-199">Beachten Sie, dass bei "Herstellername" und "Gerätemodell" die Groß-/Kleinschreibung beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-199">Note that "Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="1d8c1-200">Wenn Sie nicht wissen, welchen Wert Sie für Herstellername und Gerätemodell benötigen, können Sie diesen auf dem Gerät ausführen, um die richtigen Werte zu erfassen:</span><span class="sxs-lookup"><span data-stu-id="1d8c1-200">If you don’t know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="1d8c1-201">Ablehnung der Lizenzbedingungen für Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="1d8c1-201">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="1d8c1-202">WICHTIGE INFORMATIONEN</span><span class="sxs-lookup"><span data-stu-id="1d8c1-202">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="1d8c1-203">Mit Windows Autopilot können Sie angepasste Installationen von Windows auf Geräten konfigurieren, die Sie für Ihre Kunden verwalten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-203">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="1d8c1-204">Wenn Sie vom Kunden entsprechend autorisiert wurden, können Sie bestimmte Setupbildschirme unterdrücken oder ausblenden, die Benutzern normalerweise beim Einrichten von Windows angezeigt werden, darunter der Bildschirm für das Annehmen der Lizenzbedingungen.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-204">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="1d8c1-205">Mit der Nutzung dieser Funktion erklären Sie sich damit einverstanden, dass das Unterdrücken oder Ausblenden von Bildschirmen, die dazu bestimmt sind, den Benutzern eine Benachrichtigung oder Akzeptanz von Bedingungen zu ermöglichen, bedeutet, dass Sie von Ihrem Kunden eine ausreichende Zustimmung und Berechtigung erhalten haben, Bedingungen zu verbergen, und dass Sie im Namen Ihres Kunden (unabhängig davon, ob es sich um ein Unternehmen oder einen einzelnen Benutzer handelt) allen Benachrichtigungen zustimmen und alle Bedingungen akzeptieren, die für Ihren Kunden gelten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-205">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="1d8c1-206">Dazu gehört auch die Zustimmung zu den Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-206">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="1d8c1-207">Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Händlern verfügt.</span><span class="sxs-lookup"><span data-stu-id="1d8c1-207">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
