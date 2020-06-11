---
title: Anpassen der Out-of-Box-Funktion eines Geräts
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bevor Sie das neue Gerät eines Kunden bereitstellen können, können Sie Windows Autopilot-Profile verwenden, um die Out-of-Box-Benutzerfreundlichkeit (OOBE) des Geräts anzupassen oder vorab zu konfigurieren.
author: LauraBrenner
ms.author: labrenne
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Willkommensseite
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a3067b674b7784df34fba3de9cfaa5b44349b8c4
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679187"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="12f0a-104">Verwenden von Windows Autopilot-Profilen auf neuen Geräten zum Anpassen der Standardbenutzer Freundlichkeit eines Kunden</span><span class="sxs-lookup"><span data-stu-id="12f0a-104">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="12f0a-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="12f0a-105">**Applies to**</span></span>

- <span data-ttu-id="12f0a-106">CSP-Partner mit Direktfakturierung, indirekte Anbieter und indirekte Vertriebspartner</span><span class="sxs-lookup"><span data-stu-id="12f0a-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="12f0a-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="12f0a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="12f0a-108">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="12f0a-108">Admin agent</span></span>
- <span data-ttu-id="12f0a-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="12f0a-109">Global admin</span></span>
- <span data-ttu-id="12f0a-110">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="12f0a-110">Sales agent</span></span>
- <span data-ttu-id="12f0a-111">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="12f0a-111">User management admin</span></span>

<span data-ttu-id="12f0a-112">Wenn Sie Kundengeräte verwalten, müssen Sie die Windows-Willkommensseite für die Benutzer des Kunden anpassen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-112">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="12f0a-113">Sie können neue Geräte mit Windows Autopilot-Profilen vorkonfigurieren, bevor Sie die Geräte an Kunden ausliefern, und neue Profile auf bereits erworbene Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-113">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="12f0a-114">Beachten Sie, dass OEMs damit begonnen haben, eine Versand Bezeichnung auf der Außenseite des Autopilot-Geräts hinzufügen, die die **Product Key-ID (pkid)** des Geräts anzeigt.</span><span class="sxs-lookup"><span data-stu-id="12f0a-114">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="12f0a-115">Dieser eindimensionale, lesbare Barcode bietet downstreampartnern eine Möglichkeit, Geräte für Autopilot zu registrieren, ohne die Geräte zu entkacken und die Geräte-ID auf alternative Weise zu erfassen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-115">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="12f0a-116">In diesem Artikel wird erläutert, wie Sie im Partner Center Autopilot-Profile erstellen und auf Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-116">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="12f0a-117">Wenn Sie noch nicht mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:</span><span class="sxs-lookup"><span data-stu-id="12f0a-117">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="12f0a-118">Übersicht über Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="12f0a-118">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="12f0a-119">Referenzhandbuch für die Bereitstellung mit Autopilot</span><span class="sxs-lookup"><span data-stu-id="12f0a-119">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="12f0a-120">Übersicht</span><span class="sxs-lookup"><span data-stu-id="12f0a-120">Overview</span></span>

<span data-ttu-id="12f0a-121">Mit der Windows-Funktion Autopilot im Partner Center können Sie benutzerdefinierte Profile erstellen und diese auf Kundengeräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-121">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="12f0a-122">Zum Zeitpunkt der Veröffentlichung dieses Artikels waren die folgenden Profileinstellungen verfügbar:</span><span class="sxs-lookup"><span data-stu-id="12f0a-122">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="12f0a-123">Datenschutzeinstellungen überspringen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-123">Skip privacy settings.</span></span> <span data-ttu-id="12f0a-124">Diese optionale Einstellung im Autopilot-Profil ermöglicht Organisationen, auf Fragen zu Datenschutzeinstellungen auf der Windows-Willkommensseite zu verzichten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-124">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="12f0a-125">Erstellung des lokalen Administratorkontos auf dem Gerät deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="12f0a-125">Disable local admin account creation on the device.</span></span> <span data-ttu-id="12f0a-126">Organisationen können entscheiden, ob der Benutzer, der das Gerät einrichtet, nach Abschluss des Vorgangs Administratorrechte erhalten soll.</span><span class="sxs-lookup"><span data-stu-id="12f0a-126">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="12f0a-127">Gerät automatisch für Arbeit oder Bildungseinrichtung einrichten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-127">Automatically set up device for work or school.</span></span> <span data-ttu-id="12f0a-128">Alle mit Autopilot registrierten Geräte gelten automatisch als Arbeits- und Bildungseinrichtungsgeräte, weshalb diese Frage im zur Windows-Willkommensseite gehörigen Prozess nicht gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="12f0a-128">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="12f0a-129">Setupseiten für Cortana-, OneDrive- und OEM-Registrierung überspringen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-129">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="12f0a-130">Bei allen mit Autopilot registrierten Geräten werden diese Seiten im zur Windows-Willkommensseite gehörigen Prozess automatisch übersprungen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-130">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="12f0a-131">Lizenzbedingungen überspringen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-131">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="12f0a-132">Ab Windows 10 Version 1709 können Organisationen sich entscheiden, ob die im zur Windows-Willkommensseite gehörigen Prozess gezeigte Seite mit den Lizenzbedingungen übersprungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="12f0a-132">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="12f0a-133">Unter [Ablehnung der Lizenzbedingungen für Windows Autopilot](#windows-autopilot-eula-dismissal) finden Sie wichtige zu beachtende Informationen beim Überspringen der Seite mit den Lizenzbedingungen während des Setups von Windows.</span><span class="sxs-lookup"><span data-stu-id="12f0a-133">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="12f0a-134">Die folgenden Berechtigungen und Einschränkungen für die Verwaltung von Profilen und Geräten gelten:</span><span class="sxs-lookup"><span data-stu-id="12f0a-134">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="12f0a-135">CSP-Partner können weiterhin die Autopilot-Profile für Bestandskunden mit Vertriebspartnerschaft verwalten, auch wenn die Kunden die Berechtigungen für die delegierte Verwaltung für den Partner aufgehoben haben.</span><span class="sxs-lookup"><span data-stu-id="12f0a-135">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="12f0a-136">Sie können vorhandene Geräte für Ihre Kunden verwalten, die Sie hinzugefügt haben.</span><span class="sxs-lookup"><span data-stu-id="12f0a-136">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="12f0a-137">Sie können keine Geräte verwalten, die Ihr Kunde in Microsoft Store für Unternehmen oder das Microsoft InTune Portal hochgeladen hat.</span><span class="sxs-lookup"><span data-stu-id="12f0a-137">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="12f0a-138">Erstellen und Verwalten von Autopilot-Profilen im Partner Center</span><span class="sxs-lookup"><span data-stu-id="12f0a-138">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="12f0a-139">Im Partner Center können Sie Windows Autopilot-Bereitstellungsprofile erstellen und auf Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-139">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="12f0a-140">Nur Administrator-Agents können Profile erstellen und anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-140">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="12f0a-141">Erstellen eines neuen Autopilot-Profils</span><span class="sxs-lookup"><span data-stu-id="12f0a-141">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="12f0a-142">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-142">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="12f0a-143">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-143">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="12f0a-144">Klicken Sie unter **Windows Autopilot-Profile** auf **Neues Profil hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-144">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="12f0a-145">Geben Sie Namen und eine Beschreibung des Profils ein, und konfigurieren Sie dann die Einstellungen für die Windows-Willkommensseite.</span><span class="sxs-lookup"><span data-stu-id="12f0a-145">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="12f0a-146">Es stehen die folgenden Optionen zur Auswahl:</span><span class="sxs-lookup"><span data-stu-id="12f0a-146">Choose from:</span></span>  

   - <span data-ttu-id="12f0a-147">Datenschutzeinstellungen beim Setup überspringen</span><span class="sxs-lookup"><span data-stu-id="12f0a-147">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="12f0a-148">Lokales Administratorkonto beim Setup deaktivieren</span><span class="sxs-lookup"><span data-stu-id="12f0a-148">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="12f0a-149">Seiten beim Setup automatisch überspringen</span><span class="sxs-lookup"><span data-stu-id="12f0a-149">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="12f0a-150">(Schließt *Setup für Arbeit oder Bildungseinrichtung automatisch auswählen* und *Setupseiten für Cortana-, OneDrive- und OEM-Registrierung überspringen* ein)</span><span class="sxs-lookup"><span data-stu-id="12f0a-150">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="12f0a-151">Lizenzbedingungen überspringen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-151">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="12f0a-152">Unter [Ablehnung der Lizenzbedingungen für Windows Autopilot](#windows-autopilot-eula-dismissal) finden Sie wichtige zu beachtende Informationen beim Überspringen der Seite mit den Lizenzbedingungen während des Setups von Windows.</span><span class="sxs-lookup"><span data-stu-id="12f0a-152">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="12f0a-153">Klicken Sie abschließend auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-153">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="12f0a-154">Anwenden eines Autopilot-Profils auf Kundengeräte</span><span class="sxs-lookup"><span data-stu-id="12f0a-154">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="12f0a-155">Die folgenden Anweisungen gehen davon aus, dass Sie die Geräte des Kunden bereits dem Partner Center hinzugefügt haben und dass Sie auf dessen Geräteliste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="12f0a-155">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="12f0a-156">Wenn Sie die Geräte des Kunden noch nicht hinzugefügt haben, folgen Sie den Anweisungen unter [Hinzufügen von Geräten zu einem Kundenkonto](#add-devices-to-a-customers-account), und führen Sie dann die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-156">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="12f0a-157">Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es auf die Geräte des Kunden anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-157">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="12f0a-158">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="12f0a-158">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="12f0a-159">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-159">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="12f0a-160">Wählen Sie unter **Profile auf Geräte anwenden** die Geräte oder Gerätegruppen aus, denen Sie Profile hinzufügen möchten, und klicken Sie dann auf **Profil anwenden**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-160">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="12f0a-161">Das Profil, das Sie soeben angewendet haben, wird in der Spalte **Profil** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="12f0a-161">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="12f0a-162">Führen Sie die folgenden Schritte aus, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="12f0a-162">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="12f0a-163">a.</span><span class="sxs-lookup"><span data-stu-id="12f0a-163">a.</span></span>  <span data-ttu-id="12f0a-164">Schließen Sie ein Gerät an das Netzwerk an, und schalten Sie es ein.</span><span class="sxs-lookup"><span data-stu-id="12f0a-164">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="12f0a-165">b.</span><span class="sxs-lookup"><span data-stu-id="12f0a-165">b.</span></span>  <span data-ttu-id="12f0a-166">Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-166">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="12f0a-167">c.</span><span class="sxs-lookup"><span data-stu-id="12f0a-167">c.</span></span>  <span data-ttu-id="12f0a-168">Wenn der zur Windows-Willkommensseite gehörige Prozess beendet ist, setzen Sie das Gerät auf die Werkseinstellungen zurück, um es für einen neuen Benutzer vorzubereiten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-168">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="12f0a-169">Entfernen eines Autopilot-Profils von einem Kundengerät</span><span class="sxs-lookup"><span data-stu-id="12f0a-169">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="12f0a-170">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="12f0a-170">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="12f0a-171">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-171">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="12f0a-172">Wählen Sie unter **Profile auf Geräte anwenden** die Geräte aus, von denen Sie das Profil entfernen möchten, und klicken Sie dann auf **Profil entfernen**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-172">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="12f0a-173">Wenn Sie ein Profil von einem Gerät entfernen, wird das Profil nicht aus Ihrer Liste gelöscht.</span><span class="sxs-lookup"><span data-stu-id="12f0a-173">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="12f0a-174">Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen unter [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="12f0a-174">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="12f0a-175">Aktualisieren oder Löschen eines AutoPilot-Profils</span><span class="sxs-lookup"><span data-stu-id="12f0a-175">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="12f0a-176">Wenn ein Kunde die Windows-Willkommensseite ändern möchte, nachdem Sie ihm Geräte geliefert haben, können Sie das Profil im Partner Center ändern.</span><span class="sxs-lookup"><span data-stu-id="12f0a-176">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="12f0a-177">Wenn sich das Gerät des Kunden mit dem Internet verbindet, wird während des zur Windows-Willkommensseite gehörigen Prozesses die neueste Profilversion heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-177">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="12f0a-178">Außerdem lädt das Gerät jedes Mal, wenn ein Kunde ein Gerät auf die Werkseinstellungen zurücksetzt, während des zur Windows-Willkommensseite gehörigen Prozesses erneut die neueste Profilversion herunter.</span><span class="sxs-lookup"><span data-stu-id="12f0a-178">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="12f0a-179">Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, dessen Autopilot-Profil Sie ändern sollen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-179">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="12f0a-180">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-180">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="12f0a-181">Wählen Sie unter **Windows Autopilot-Profile** das Profil aus, das Sie aktualisieren müssen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-181">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="12f0a-182">Nehmen Sie die erforderlichen Änderungen vor, und klicken Sie dann auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-182">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="12f0a-183">Um dieses Profil zu löschen, klicken Sie rechts oben auf der Seite auf **Profil löschen**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-183">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="12f0a-184">Hinzufügen von Geräten zum Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="12f0a-184">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="12f0a-185">Vertriebs- und Verwaltungsmitarbeiter können dem Konto eines Kunden Geräte hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-185">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="12f0a-186">Bevor Sie benutzerdefinierte Autopilot-Profile auf Kundengeräten anwenden können, müssen Sie Zugriff auf die Geräteliste des Kunden haben.</span><span class="sxs-lookup"><span data-stu-id="12f0a-186">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="12f0a-187">Wenn Sie planen, die Kombination aus OEM-Name, Seriennummer und Modell zu verwenden, beachten Sie diese Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="12f0a-187">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="12f0a-188">Dieses Tupel funktioniert nur für neuere Geräte (z.B. 4K-Hashes) und wird für 128B-Hashes (RS2 und frühere Geräte) nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f0a-188">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="12f0a-189">Bei der Registrierung des Tupels wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen die Daten in der Datei mit den Modell- und Herstellernamen ***genau*** mit den Angaben des OEM-Anbieters (Hardwareanbieters) übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-189">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="12f0a-190">Führen Sie die im Partner Center nachstehenden Anweisungen zum Hinzufügen von Geräten zum Konto eines Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-190">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="12f0a-191">Wählen Sie im Partner Center-Menü **Kunden** und dann den Kunden aus, dessen Geräte Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-191">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="12f0a-192">Wählen Sie auf der Detailseite des Kunden **Geräte** aus.</span><span class="sxs-lookup"><span data-stu-id="12f0a-192">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="12f0a-193">Klicken Sie unter \*\*Profile auf Geräte anwenden \*\* auf **Geräte hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-193">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="12f0a-194">Geben Sie einen Namen für die Geräteliste aus, und klicken Sie dann auf **Durchsuchen**, um die Kundenliste (im Dateiformat CSV) ins Partner Center hochzuladen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-194">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="12f0a-195">Beim Kauf Ihres Geräts sollten Sie diese CSV-Datei erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="12f0a-195">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="12f0a-196">Wenn Sie keine CSV-Datei erhalten haben, können Sie selbst eine erstellen, indem Sie die Schritte unter [Hinzufügen von Geräten zu Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell) ausführen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-196">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="12f0a-197">Laden Sie die CSV-Datei hoch, und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="12f0a-197">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="12f0a-198">Wenn Sie beim Versuch, die CSV-Datei hochzuladen, eine Fehlermeldung erhalten, überprüfen Sie das Format der Datei.</span><span class="sxs-lookup"><span data-stu-id="12f0a-198">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="12f0a-199">Sie können nur den Hardwarehash oder den OEM-Namen, die Seriennummer und das Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID verwenden.</span><span class="sxs-lookup"><span data-stu-id="12f0a-199">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="12f0a-200">Sie können auch die CSV-Beispieldatei verwenden, die über den Link neben **Geräte hinzufügen** bereitgestellt wird, um eine Geräteliste zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-200">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="12f0a-201">Die CSV-Datei sollte in etwa wie folgt aussehen:</span><span class="sxs-lookup"><span data-stu-id="12f0a-201">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="12f0a-202">**Seriennummer des Geräts, Windows-Produkt-ID, Hardware Hash, Herstellername, Gerätemodell**</span><span class="sxs-lookup"><span data-stu-id="12f0a-202">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="12f0a-203">**{SerialNumber},,, Microsoft Corporation, Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="12f0a-203">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="12f0a-204">Bei "Herstellername" und "Gerätemodell" wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="12f0a-204">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="12f0a-205">Wenn Sie nicht wissen, welchen Wert Sie für Herstellername und Gerätemodell benötigen, können Sie diesen auf dem Gerät ausführen, um die richtigen Werte zu erfassen:</span><span class="sxs-lookup"><span data-stu-id="12f0a-205">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="12f0a-206">Ablehnung der Lizenzbedingungen für Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="12f0a-206">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="12f0a-207">WICHTIGE INFORMATIONEN</span><span class="sxs-lookup"><span data-stu-id="12f0a-207">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="12f0a-208">Mit Windows Autopilot können Sie angepasste Installationen von Windows auf Geräten konfigurieren, die Sie für Ihre Kunden verwalten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-208">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="12f0a-209">Wenn Sie vom Kunden entsprechend autorisiert wurden, können Sie bestimmte Setupbildschirme unterdrücken oder ausblenden, die Benutzern normalerweise beim Einrichten von Windows angezeigt werden, darunter der Bildschirm für das Annehmen der Lizenzbedingungen.</span><span class="sxs-lookup"><span data-stu-id="12f0a-209">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="12f0a-210">Mit der Nutzung dieser Funktion erklären Sie sich damit einverstanden, dass das Unterdrücken oder Ausblenden von Bildschirmen, die dazu bestimmt sind, den Benutzern eine Benachrichtigung oder Akzeptanz von Bedingungen zu ermöglichen, bedeutet, dass Sie von Ihrem Kunden eine ausreichende Zustimmung und Berechtigung erhalten haben, Bedingungen zu verbergen, und dass Sie im Namen Ihres Kunden (unabhängig davon, ob es sich um ein Unternehmen oder einen einzelnen Benutzer handelt) allen Benachrichtigungen zustimmen und alle Bedingungen akzeptieren, die für Ihren Kunden gelten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-210">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="12f0a-211">Dazu gehört auch die Zustimmung zu den Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten.</span><span class="sxs-lookup"><span data-stu-id="12f0a-211">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="12f0a-212">Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Händlern verfügt.</span><span class="sxs-lookup"><span data-stu-id="12f0a-212">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
