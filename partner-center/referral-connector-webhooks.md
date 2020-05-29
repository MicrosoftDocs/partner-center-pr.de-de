---
title: Verwenden von webhooks zum erhalten von Ressourcen Änderungs Ereignissen
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verwenden Sie die webhook-APIs, um herauszufinden, wann Ressourcen Änderungen der Verweise auftreten.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: Verweise, webhook-API, Ressourcen Änderungs Ereignisse
ms.localizationpriority: medium
ms.openlocfilehash: 4e1eb2e9bd8ceb4f8c4bf43684305504c8594e5c
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145084"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="caa5d-104">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="caa5d-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="caa5d-105">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="caa5d-105">Appropriate roles</span></span>

- <span data-ttu-id="caa5d-106">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="caa5d-106">Referrals admin</span></span>
- <span data-ttu-id="caa5d-107">Systemadministrator oder systemanpassungsmodul für Dynamics 365 CRM oder Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="caa5d-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="caa5d-108">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="caa5d-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="caa5d-109">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="caa5d-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="caa5d-110">In diesem Thema werden webhook-APIs für Dynamics 365 CRM und Salesforce CRM erläutert.</span><span class="sxs-lookup"><span data-stu-id="caa5d-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="caa5d-111">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="caa5d-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="caa5d-112">Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt</span><span class="sxs-lookup"><span data-stu-id="caa5d-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Trigger](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="caa5d-114">Wenn Sie diese Updates vornehmen, sehen Sie</span><span class="sxs-lookup"><span data-stu-id="caa5d-114">When you make these updates, you will see</span></span>

![webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="caa5d-116">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="caa5d-117">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen in den IP-Co-Selling/Independent-Referenzobjekten in Partner Center und CRM-Systemen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="caa5d-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="caa5d-118">Wählen Sie **Partner Center für Dynamics 365 (Insider Preview)** oder **Partner Center für Salesforce (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="caa5d-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="caa5d-119">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.</span><span class="sxs-lookup"><span data-stu-id="caa5d-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="caa5d-120">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="caa5d-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Kopieren der URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="caa5d-122">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="caa5d-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="caa5d-123">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="caa5d-124">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="caa5d-124">Enter the following details:</span></span> 

    <span data-ttu-id="caa5d-125">a.</span><span class="sxs-lookup"><span data-stu-id="caa5d-125">a.</span></span> <span data-ttu-id="caa5d-126">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="caa5d-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="caa5d-127">b.</span><span class="sxs-lookup"><span data-stu-id="caa5d-127">b.</span></span> <span data-ttu-id="caa5d-128">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="caa5d-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="caa5d-129">c.</span><span class="sxs-lookup"><span data-stu-id="caa5d-129">c.</span></span> <span data-ttu-id="caa5d-130">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="caa5d-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="caa5d-131">Der webhook kann nun auf Änderungen lauschen (erstellen und Aktualisieren von Ereignissen).</span><span class="sxs-lookup"><span data-stu-id="caa5d-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="caa5d-132">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="caa5d-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="caa5d-133">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="caa5d-133">Customize synchronization steps</span></span>

<span data-ttu-id="caa5d-134">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="caa5d-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="caa5d-135">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="caa5d-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="caa5d-136">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="caa5d-137">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="caa5d-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="caa5d-138">Microsoft Partner Center-zu-CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="caa5d-139">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="caa5d-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="caa5d-140">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="caa5d-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="caa5d-141">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="caa5d-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="caa5d-142">a.</span><span class="sxs-lookup"><span data-stu-id="caa5d-142">a.</span></span> <span data-ttu-id="caa5d-143">Wählen Sie Partner Center für Dynamics 365 (Insider Preview) oder Partner Center für Salesforce (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="caa5d-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="caa5d-144">b.</span><span class="sxs-lookup"><span data-stu-id="caa5d-144">b.</span></span> <span data-ttu-id="caa5d-145">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="caa5d-146">c.</span><span class="sxs-lookup"><span data-stu-id="caa5d-146">c.</span></span> <span data-ttu-id="caa5d-147">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="caa5d-148">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Erstellungs Ereignisse aus, wenn es sich um eine **neue freigegebene Chance handelt, und**</span><span class="sxs-lookup"><span data-stu-id="caa5d-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="caa5d-149">Wählen Sie den unterschritt aus, **Falls ja** , und erweitern Sie dann die Option **neue Gelegenheit im CRM**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="caa5d-150">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="caa5d-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="caa5d-151">d.</span><span class="sxs-lookup"><span data-stu-id="caa5d-151">d.</span></span> <span data-ttu-id="caa5d-152">Zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="caa5d-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="caa5d-153">e.</span><span class="sxs-lookup"><span data-stu-id="caa5d-153">e.</span></span> <span data-ttu-id="caa5d-154">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="caa5d-155">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="caa5d-156">f.</span><span class="sxs-lookup"><span data-stu-id="caa5d-156">f.</span></span> <span data-ttu-id="caa5d-157">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="caa5d-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="caa5d-158">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="caa5d-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="caa5d-159">a.</span><span class="sxs-lookup"><span data-stu-id="caa5d-159">a.</span></span> <span data-ttu-id="caa5d-160">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="caa5d-161">b.</span><span class="sxs-lookup"><span data-stu-id="caa5d-161">b.</span></span> <span data-ttu-id="caa5d-162">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="caa5d-163">c.</span><span class="sxs-lookup"><span data-stu-id="caa5d-163">c.</span></span> <span data-ttu-id="caa5d-164">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="caa5d-165">d.</span><span class="sxs-lookup"><span data-stu-id="caa5d-165">d.</span></span> <span data-ttu-id="caa5d-166">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="caa5d-167">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="caa5d-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="caa5d-168">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="caa5d-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="caa5d-169">a.</span><span class="sxs-lookup"><span data-stu-id="caa5d-169">a.</span></span> <span data-ttu-id="caa5d-170">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="caa5d-171">b.</span><span class="sxs-lookup"><span data-stu-id="caa5d-171">b.</span></span> <span data-ttu-id="caa5d-172">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="caa5d-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="caa5d-173">c.</span><span class="sxs-lookup"><span data-stu-id="caa5d-173">c.</span></span> <span data-ttu-id="caa5d-174">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="caa5d-175">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="caa5d-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="caa5d-176">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="caa5d-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="caa5d-177">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 oder Salesforce und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="caa5d-178">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="caa5d-178">Pre-requisites</span></span>

<span data-ttu-id="caa5d-179">Um die Verweise über Partner Center und Dynamics 365 CRM oder über Partner Center und Salesforce CRM zu synchronisieren, muss die Lösung für die Energie Automatisierung Microsoft-spezifische verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="caa5d-180">Dies bietet Ihren Verkäufer Teams die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="caa5d-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="caa5d-181">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für Dynamics 365 Solution **Opportunity** verfügbar.</span><span class="sxs-lookup"><span data-stu-id="caa5d-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="caa5d-182">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="caa5d-183">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="caa5d-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="caa5d-184">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="caa5d-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="caa5d-185">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="caa5d-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="caa5d-186">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="caa5d-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="caa5d-187">**Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="caa5d-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="caa5d-188">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="caa5d-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="caa5d-189">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="caa5d-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="caa5d-190">SS</span><span class="sxs-lookup"><span data-stu-id="caa5d-190">SCENARIOS:</span></span>

1. <span data-ttu-id="caa5d-191">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="caa5d-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="caa5d-192">a.</span><span class="sxs-lookup"><span data-stu-id="caa5d-192">a.</span></span> <span data-ttu-id="caa5d-193">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="caa5d-193">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="caa5d-194">b.</span><span class="sxs-lookup"><span data-stu-id="caa5d-194">b.</span></span> <span data-ttu-id="caa5d-195">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Dynamics 365-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Verkaufschance](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="caa5d-197">c.</span><span class="sxs-lookup"><span data-stu-id="caa5d-197">c.</span></span> <span data-ttu-id="caa5d-198">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="caa5d-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="caa5d-199">"Mit Partner Center synchronisieren": Ja</span><span class="sxs-lookup"><span data-stu-id="caa5d-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="caa5d-200">"Wie kann Microsoft Help?": Wählen Sie eine der folgenden Aktionen aus:</span><span class="sxs-lookup"><span data-stu-id="caa5d-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![Auswahl von Hilfe](images/cosellconnectors/help.png)

    - <span data-ttu-id="caa5d-202">Produkte: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="caa5d-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="caa5d-203">d.</span><span class="sxs-lookup"><span data-stu-id="caa5d-203">d.</span></span> <span data-ttu-id="caa5d-204">Wenn die Verkaufschance in Dynamics 365 mit **sync with Partner Center** auf **Ja**festgelegt ist, warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center-Konto an.</span><span class="sxs-lookup"><span data-stu-id="caa5d-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="caa5d-205">Ihre Verweise werden mit Dynamics 365 synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="caa5d-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="caa5d-206">e.</span><span class="sxs-lookup"><span data-stu-id="caa5d-206">e.</span></span> <span data-ttu-id="caa5d-207">Wenn Sie die Option in Dynamics 365 CRM aktualisieren, werden die Änderungen daher in Ihrem Partner Center-Konto synchronisiert, wenn Sie die Option "mit Partner Center synchronisieren" auf "Ja" festlegen.</span><span class="sxs-lookup"><span data-stu-id="caa5d-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="caa5d-208">f.</span><span class="sxs-lookup"><span data-stu-id="caa5d-208">f.</span></span> <span data-ttu-id="caa5d-209">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.</span><span class="sxs-lookup"><span data-stu-id="caa5d-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="caa5d-210">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="caa5d-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="caa5d-211">a.</span><span class="sxs-lookup"><span data-stu-id="caa5d-211">a.</span></span> <span data-ttu-id="caa5d-212">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="caa5d-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="caa5d-213">b.</span><span class="sxs-lookup"><span data-stu-id="caa5d-213">b.</span></span> <span data-ttu-id="caa5d-214">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="caa5d-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="caa5d-215">c.</span><span class="sxs-lookup"><span data-stu-id="caa5d-215">c.</span></span> <span data-ttu-id="caa5d-216">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="caa5d-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="caa5d-217">d.</span><span class="sxs-lookup"><span data-stu-id="caa5d-217">d.</span></span> <span data-ttu-id="caa5d-218">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="caa5d-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="caa5d-219">e.</span><span class="sxs-lookup"><span data-stu-id="caa5d-219">e.</span></span> <span data-ttu-id="caa5d-220">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="caa5d-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="caa5d-221">Der im Microsoft Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="caa5d-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="caa5d-222">f.</span><span class="sxs-lookup"><span data-stu-id="caa5d-222">f.</span></span> <span data-ttu-id="caa5d-223">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="caa5d-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="caa5d-224">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="caa5d-224">Next steps</span></span>

- [<span data-ttu-id="caa5d-225">Weitere Informationen zur Microsoft powerautomatisieren-Plattform</span><span class="sxs-lookup"><span data-stu-id="caa5d-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="caa5d-226">Partner Center-webhook-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="caa5d-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="caa5d-227">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="caa5d-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="caa5d-228">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="caa5d-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
