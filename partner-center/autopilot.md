---
title: Anpassen des Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen | Partner Center
description: Vorkonfigurieren eines Geräts Out-of-Box-Experience mit Autopilot-Profilen.
author: maggiepuccievans
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 70740212f433ad6eb4f2f04d63708fff436024ad
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995934"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="9d6a2-104">Anpassen des Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen</span><span class="sxs-lookup"><span data-stu-id="9d6a2-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="9d6a2-105">Betrifft:</span><span class="sxs-lookup"><span data-stu-id="9d6a2-105">Applies to</span></span>**

- <span data-ttu-id="9d6a2-106">CSP-Rechnung Direct-Partner, indirekte Anbieter und indirekte Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="9d6a2-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="9d6a2-107">Wenn Sie Kundengeräte verwalten, müssen Sie die Out-of-Box-Experience (OOBE) für Benutzer des Kunden anpassen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="9d6a2-108">Sie können neue Geräte mit Windows Autopilot-Profilen vorab zu konfigurieren, bevor Sie die Geräte an Kunden liefern und Anwenden von neuen Profilen auf Geräte, die Kunden bereits erworben haben.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="9d6a2-109">In diesem Artikel wird erläutert, wie Sie erstellen und Anwenden von Autopilot-Profilen auf Geräte in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="9d6a2-110">Wenn Sie nicht bereits mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:</span><span class="sxs-lookup"><span data-stu-id="9d6a2-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="9d6a2-111">Übersicht über Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="9d6a2-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="9d6a2-112">Autopilot-Referenz-Bereitstellungshandbuch</span><span class="sxs-lookup"><span data-stu-id="9d6a2-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="9d6a2-113">Übersicht</span><span class="sxs-lookup"><span data-stu-id="9d6a2-113">Overview</span></span>

<span data-ttu-id="9d6a2-114">Mit dem Windows Autopilot-Feature im Partner Center können Sie benutzerdefinierte Profile für Kundengeräte erstellen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="9d6a2-115">Zum Zeitpunkt der Veröffentlichung dieses Artikels, waren die folgenden profileinstellungen verfügbar:</span><span class="sxs-lookup"><span data-stu-id="9d6a2-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="9d6a2-116">Überspringen Sie datenschutzeinstellungen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-116">Skip privacy settings.</span></span> <span data-ttu-id="9d6a2-117">Dieser optionalen Einstellung der Autopilot-Profil kann Organisationen während des Prozesses der Windows-Willkommensseite nicht zu Datenschutz und Fragen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="9d6a2-118">Deaktivieren Sie die Erstellung des lokalen Administratorkontos auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="9d6a2-119">Organisationen können entscheiden, ob der Benutzer das Gerät einrichten Administratorzugriff haben soll, nachdem der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="9d6a2-120">Automatisch Gerät für die Arbeit oder Schule einrichten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="9d6a2-121">Alle Geräte mit Autopilot registriert werden automatisch als Arbeit betrachtet werden oder Geräte, Schule, damit diese Frage nicht während der OOBE-Prozesses aufgefordert wird.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="9d6a2-122">Überspringen Sie Cortana-, Onedrive- und OEM-registrierungssetupseiten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="9d6a2-123">Alle Geräte mit Autopilot registriert werden automatisch diese Seiten während des Out-of-Box-Experience (OOBE) zu überspringen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="9d6a2-124">Überspringen Sie Endbenutzer-Lizenzvertrag (EULA).</span><span class="sxs-lookup"><span data-stu-id="9d6a2-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="9d6a2-125">Ab Windows 10, Version 1709, können Organisationen entscheiden, überspringen die Endbenutzer-Lizenzvertrag-Seite, die bei der Windows-Willkommensseite angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="9d6a2-126">Finden Sie unter [EULA zu Windows Autopilot](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Endbenutzer-Lizenzvertrag Seite während des Windows Setup berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="9d6a2-127">Wenden Sie die folgenden Profil und Geräte-Management-Berechtigungen und Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="9d6a2-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="9d6a2-128">CSP-Partner können weiterhin zum Verwalten von Autopilot Profile für vorhandene Kunden, mit denen sie Reseller-Geschäftsbeziehungen haben, auch wenn die Kunden die delegierten Administratorrechte des Partners entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="9d6a2-129">Sie können vorhandene Geräte für Ihre Kunden verwalten, die von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="9d6a2-130">Sie können keine Geräte verwalten, die Microsoft Store für Unternehmen oder Microsoft Intune-Portal Ihr Kunde hochgeladen hat.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="9d6a2-131">Erstellen Sie und Verwalten von Autopilot-Profilen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="9d6a2-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="9d6a2-132">Im Partner Center können Sie Windows Autopilot-bereitstellungsprofile erstellen und diese auf Geräte anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="9d6a2-133">Nur Admin-Agents können erstellen und Anwenden von Profilen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="9d6a2-134">Erstellen Sie ein neues Autopilot-Profil</span><span class="sxs-lookup"><span data-stu-id="9d6a2-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="9d6a2-135">Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, die, dem Sie für die Autopilot-Bereitstellungsprofil erstellen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="9d6a2-136">Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9d6a2-137">Wählen Sie unter **Windows Autopilot Profile** **Neues Profil hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="9d6a2-138">Geben Sie Namen und eine Beschreibung des Profils, und konfigurieren Sie die Einstellungen für die Windows-Willkommensseite.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="9d6a2-139">Wählen Sie aus:</span><span class="sxs-lookup"><span data-stu-id="9d6a2-139">Choose from:</span></span>  

   - <span data-ttu-id="9d6a2-140">Überspringen der datenschutzeinstellungen im setup</span><span class="sxs-lookup"><span data-stu-id="9d6a2-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="9d6a2-141">Deaktivieren des lokalen Administratorkontos während des Setups</span><span class="sxs-lookup"><span data-stu-id="9d6a2-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="9d6a2-142">Automatisches Überspringen von Seiten im Setup</span><span class="sxs-lookup"><span data-stu-id="9d6a2-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="9d6a2-143">(Einschließlich *Automatisches Setup für Arbeit oder Schule auswählen* und *Überspringen Cortana, OneDrive und OEM-registrierungssetupseiten*)</span><span class="sxs-lookup"><span data-stu-id="9d6a2-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="9d6a2-144">Endbenutzer-Lizenzvertrag (EULA) überspringen</span><span class="sxs-lookup"><span data-stu-id="9d6a2-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="9d6a2-145">Finden Sie unter [EULA zu Windows Autopilot](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Endbenutzer-Lizenzvertrag Seite während des Windows Setup berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="9d6a2-146">Wählen Sie abschließend **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="9d6a2-147">Anwenden einer Autopilot-Profilen auf Kundengeräte</span><span class="sxs-lookup"><span data-stu-id="9d6a2-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="9d6a2-148">Die folgenden Anweisungen wird davon ausgegangen, dass Sie bereits Geräte des Kunden in das Partner Center hinzugefügt haben, und Sie ihre Liste der Geräte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="9d6a2-149">Wenn Sie Geräte des Kunden bereits hinzugefügt haben, folgen Sie den Anweisungen im [Konto eines Kunden Geräte hinzufügen](#add-devices-to-a-customers-account) , und führen Sie dann die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="9d6a2-150">Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es an den Kunden Geräte anwenden.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="9d6a2-151">Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, die, dem Sie für die Autopilot-Profil erstellt.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="9d6a2-152">Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9d6a2-153">Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte oder Gerätegruppen, die Sie Profile für, und wählen Sie dann **Profil anwenden**möchten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="9d6a2-154">Das Profil, das Sie nur angewendet, die in der Spalte **Profil** wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="9d6a2-155">Gehen Sie folgendermaßen vor, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="9d6a2-156">a.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-156">a.</span></span>  <span data-ttu-id="9d6a2-157">Verbinden Sie ein Gerät mit dem Netzwerk, und schalten Sie es ein.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="9d6a2-158">b.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-158">b.</span></span>  <span data-ttu-id="9d6a2-159">Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="9d6a2-160">c.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-160">c.</span></span>  <span data-ttu-id="9d6a2-161">Wenn der OOBE-Prozess beendet wird, wird zurücksetzen Sie das Gerät auf die werksseitigen Standardeinstellungen, die sie für einen neuen Benutzer vorzubereiten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="9d6a2-162">Entfernen Sie ein Autopilot-Profil aus dem Gerät eines Kunden</span><span class="sxs-lookup"><span data-stu-id="9d6a2-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="9d6a2-163">Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, die, dem Sie für die Autopilot-Profil erstellt.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="9d6a2-164">Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9d6a2-165">Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte, die Sie verwenden möchten, entfernen Sie das Profil aus, und wählen Sie dann **Entfernen eines Profils**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="9d6a2-166">Entfernen eines Profils von einem Gerät wird nicht das Profil aus der Liste gelöscht.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="9d6a2-167">Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="9d6a2-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="9d6a2-168">Aktualisieren Sie oder löschen Sie ein Autopilot-Profil</span><span class="sxs-lookup"><span data-stu-id="9d6a2-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="9d6a2-169">Wenn ein Kunde die Out-of-Box-Experience zu ändern möchte, nachdem Sie die Geräte geliefert haben, können Sie das Profil in Partner Center ändern.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="9d6a2-170">Wenn das Gerät des Kunden mit dem Internet verbunden ist, wird es die neueste Version der Profile herunterladen, während der Windows-Willkommensseite.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="9d6a2-171">Außerdem wird jedes Mal ein Kunde ein Gerät auf die werksseitigen Standardeinstellungen wiederherstellt das Gerät erneut herunter die neueste Version der Profile während des Prozesses der Windows-Willkommensseite.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="9d6a2-172">Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, der Sie ein Autopilot-Profil zu ändern möchten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="9d6a2-173">Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9d6a2-174">Wählen Sie unter **Windows Autopilot Profile** das Profil, das Sie aktualisieren müssen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="9d6a2-175">Nehmen Sie die erforderlichen Änderungen vor, und wählen Sie dann **übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="9d6a2-176">Wählen Sie aus der oberen rechten Ecke der Seite **Profil löschen** , um diesem Profil zu löschen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="9d6a2-177">Hinzufügen von Geräten auf dem Konto eines Kunden</span><span class="sxs-lookup"><span data-stu-id="9d6a2-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="9d6a2-178">Verkaufsvertreter und Admin-Agents können Geräte Konto eines Kunden hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="9d6a2-179">Bevor Sie benutzerdefinierte Autopilot Profile auf Kundengeräte anwenden können, müssen Sie auf dem Gerät der Kundenliste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="9d6a2-180">Wenn Sie die OEM-Namen, Seriennummer und Modell Kombination verwenden möchten, achten Sie darauf, dass Sie diese Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="9d6a2-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="9d6a2-181">Das Tupel funktioniert nur für neue Geräte (4 k Hashes, z. B.) und wird für 128b Hashes (RS2 und vorherigen Geräte) nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="9d6a2-182">Die Registrierung Tupel ist groß-und Kleinschreibung unterschieden, damit die Daten in der Datei der Hersteller und Modell Namen ***genau*** entsprechen müssen, wie durch den OEM-Anbieter (Hardwareanbieter) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="9d6a2-183">Führen Sie die folgenden Anweisungen von Geräten auf dem Konto eines Kunden im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="9d6a2-184">Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, deren Geräte, die Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="9d6a2-185">Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9d6a2-186">Wählen Sie unter **Anwenden von Profilen auf Geräte** **Geräte hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="9d6a2-187">Geben Sie einen Namen für die Liste der Geräte, und wählen Sie dann die Kundenliste (im CSV-Format) für das Partner Center hochladen **Durchsuchen** .</span><span class="sxs-lookup"><span data-stu-id="9d6a2-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9d6a2-188">Sie sollten diese CSV-Datei mit dem Gerät Kauf erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="9d6a2-189">Wenn Sie eine CSV-Datei nicht erhalten haben, können Sie selbst erstellen, mithilfe der Schritte im [Windows Autopilot-Geräte hinzufügen](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="9d6a2-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="9d6a2-190">Laden Sie die CSV-Datei, und wählen Sie dann **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="9d6a2-191">Wenn Sie eine Fehlermeldung erhalten, bei dem Versuch, die CSV-Datei hochzuladen, überprüfen Sie das Format der Datei.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="9d6a2-192">Sie können nur den Hardwarehash oder den OEM-Namen, Seriennummer, und Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="9d6a2-193">Die Beispiel-CSV-Datei über den Link neben **Hinzufügen Geräte** bereitgestellt können auch um eine Liste der Geräte zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="9d6a2-194">EULA zu Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="9d6a2-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="9d6a2-195">WICHTIGE INFORMATIONEN</span><span class="sxs-lookup"><span data-stu-id="9d6a2-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="9d6a2-196">Windows Autopilot können Sie benutzerdefinierte Installationen von Windows auf Geräten zu konfigurieren, die Sie für Ihre Kunden verwalten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="9d6a2-197">Wenn dazu berechtigt, durch den Kunden, können Sie unterdrücken oder ausblenden bestimmte Setupbildschirme, die normalerweise für Benutzer beim Einrichten von Windows, einschließlich des Endbenutzer-Lizenzvertrag (End User License Agreement) Annahme Bildschirms angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="9d6a2-198">Durch die Verwendung dieser Funktion stimmen Sie, dass das unterdrücken oder Ausblenden von Bildschirmen, die Benutzer bereitstellen, oder die Annahme von Begriffe bedeutet, dass Sie über ausreichende Zustimmung und Autorisierung von ausblenden Begriffe und, die Sie für Ihre Kunden erworben haben Ihre Kunden (gibt an, ob eine Organisation oder einzelner Benutzer die Groß-/Kleinschreibung), stimmen hinweisen und akzeptiert Begriffe, die an den Kunden relevant sind.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="9d6a2-199">Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="9d6a2-200">Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.</span><span class="sxs-lookup"><span data-stu-id="9d6a2-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>