---
title: Verwenden von webhooks zum erhalten von Ressourcen Änderungs Ereignissen
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verwenden Sie Partner Center-webhook-APIs, um zu erfahren, wann die Ressourcen Änderungen von Verweisen für Dynamics 365 CRM oder Salesforce CRM auftreten.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2335c06d9c410d44ed5f444574d9bc8fb3e48fc0
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434019"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="1cb4e-103">Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse für Dynamics 365 CRM und Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1cb4e-103">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1cb4e-104">Geeignete Rollen</span><span class="sxs-lookup"><span data-stu-id="1cb4e-104">Appropriate roles</span></span>

- <span data-ttu-id="1cb4e-105">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="1cb4e-105">Referrals admin</span></span>
- <span data-ttu-id="1cb4e-106">Systemadministrator oder systemanpassungsmodul für Dynamics 365 CRM oder Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1cb4e-106">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="1cb4e-107">Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-107">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="1cb4e-108">Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-108">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="1cb4e-109">In diesem Thema werden webhook-APIs für Dynamics 365 CRM und Salesforce CRM erläutert.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-109">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="1cb4e-110">Konfigurieren des Webhooks</span><span class="sxs-lookup"><span data-stu-id="1cb4e-110">Configure the webhook</span></span>

1. <span data-ttu-id="1cb4e-111">Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="1cb4e-112">Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt</span><span class="sxs-lookup"><span data-stu-id="1cb4e-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="1cb4e-114">Wenn Sie diese Updates vornehmen, sehen Sie</span><span class="sxs-lookup"><span data-stu-id="1cb4e-114">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="1cb4e-116">Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-116">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="1cb4e-117">Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen in den IP-Co-Selling/Independent-Referenzobjekten in Partner Center und CRM-Systemen zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="1cb4e-118">Wählen Sie **Partner Center für Dynamics 365 (Insider Preview)** oder **Partner Center für Salesforce (Insider Preview)** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="1cb4e-119">Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="1cb4e-120">Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopieren der URL":::

8. <span data-ttu-id="1cb4e-122">Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="1cb4e-123">Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="1cb4e-124">Geben Sie die folgenden Details ein:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-124">Enter the following details:</span></span>

    1. <span data-ttu-id="1cb4e-125">**Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL</span><span class="sxs-lookup"><span data-stu-id="1cb4e-125">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="1cb4e-126">**Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"</span><span class="sxs-lookup"><span data-stu-id="1cb4e-126">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="1cb4e-127">**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)</span><span class="sxs-lookup"><span data-stu-id="1cb4e-127">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="1cb4e-128">Der webhook kann nun auf Änderungen lauschen (erstellen und Aktualisieren von Ereignissen).</span><span class="sxs-lookup"><span data-stu-id="1cb4e-128">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="1cb4e-129">Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**</span><span class="sxs-lookup"><span data-stu-id="1cb4e-129">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="1cb4e-130">Synchronisierungs Schritte anpassen</span><span class="sxs-lookup"><span data-stu-id="1cb4e-130">Customize synchronization steps</span></span>

<span data-ttu-id="1cb4e-131">Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-131">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="1cb4e-132">Häufig sind CRM-Systeme hochgradig angepasst.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-132">Often CRM systems are highly customized.</span></span> <span data-ttu-id="1cb4e-133">Sie können die Strom automatisierten Flows anpassen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-133">You can customize the Power Automate flows.</span></span> <span data-ttu-id="1cb4e-134">Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-134">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="1cb4e-135">Microsoft Partner Center-zu-CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-135">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="1cb4e-136">Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-136">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="1cb4e-137">Im folgenden finden Sie Beispiele für verfügbare Anpassungen:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-137">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="1cb4e-138">So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-138">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="1cb4e-139">Wählen Sie Partner Center für Dynamics 365 (Insider Preview) oder Partner Center für Salesforce (Insider Preview) aus.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-139">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="1cb4e-140">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-140">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="1cb4e-141">Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-141">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="1cb4e-142">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Erstellungs Ereignisse aus, wenn es sich um eine **neue freigegebene Chance handelt, und**</span><span class="sxs-lookup"><span data-stu-id="1cb4e-142">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="1cb4e-143">Wählen Sie den unterschritt aus, **Falls ja** , und erweitern Sie dann die Option **neue Gelegenheit im CRM**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-143">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="1cb4e-144">Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-144">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="1cb4e-145">Zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".</span><span class="sxs-lookup"><span data-stu-id="1cb4e-145">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="1cb4e-146">Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-146">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="1cb4e-147">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-147">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="1cb4e-148">Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**</span><span class="sxs-lookup"><span data-stu-id="1cb4e-148">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="1cb4e-149">So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an</span><span class="sxs-lookup"><span data-stu-id="1cb4e-149">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="1cb4e-150">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-150">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="1cb4e-151">Select **(Bereich) Synchronisieren der Verkaufschance**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-151">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="1cb4e-152">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-152">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="1cb4e-153">Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-153">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="1cb4e-154">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-154">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="1cb4e-155">Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse</span><span class="sxs-lookup"><span data-stu-id="1cb4e-155">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="1cb4e-156">Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-156">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="1cb4e-157">Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**</span><span class="sxs-lookup"><span data-stu-id="1cb4e-157">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="1cb4e-158">Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-158">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="1cb4e-159">Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-159">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="1cb4e-160">End-to-End-bidirektionale Co-Selling-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="1cb4e-160">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="1cb4e-161">Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 oder Salesforce und Partner Center testen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-161">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="1cb4e-162">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1cb4e-162">Pre-requisites</span></span>

<span data-ttu-id="1cb4e-163">Um die Verweise über Partner Center und Dynamics 365 CRM oder über Partner Center und Salesforce CRM zu synchronisieren, muss die Lösung für die Energie Automatisierung Microsoft-spezifische verweigerfelder eindeutig abgrenzen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-163">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="1cb4e-164">Dies bietet Ihren Verkäufer Teams die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-164">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1cb4e-165">Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für Dynamics 365 Solution **Opportunity** verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-165">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="1cb4e-166">Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-166">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="1cb4e-167">Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-167">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1cb4e-168">**Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll</span><span class="sxs-lookup"><span data-stu-id="1cb4e-168">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1cb4e-169">**Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz</span><span class="sxs-lookup"><span data-stu-id="1cb4e-169">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1cb4e-170">**Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="1cb4e-170">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1cb4e-171">**Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis</span><span class="sxs-lookup"><span data-stu-id="1cb4e-171">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1cb4e-172">**Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="1cb4e-172">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1cb4e-173">Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen</span><span class="sxs-lookup"><span data-stu-id="1cb4e-173">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="1cb4e-174">SS</span><span class="sxs-lookup"><span data-stu-id="1cb4e-174">SCENARIOS:</span></span>

1. <span data-ttu-id="1cb4e-175">Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-175">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="1cb4e-176">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-176">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="1cb4e-177">Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Dynamics 365-Umgebung erstellen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-177">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Möglichkeiten":::

   3. <span data-ttu-id="1cb4e-179">Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-179">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="1cb4e-180">**Mit Partner Center synchronisieren**: Ja</span><span class="sxs-lookup"><span data-stu-id="1cb4e-180">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="1cb4e-181">**Wie kann Microsoft Help?**: Wählen Sie eine der folgenden Aktionen aus:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-181">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Auswahl von Hilfe":::

      - <span data-ttu-id="1cb4e-183">**Produkte**: Lösungs-IDs des Produkts</span><span class="sxs-lookup"><span data-stu-id="1cb4e-183">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="1cb4e-184">Wenn die Verkaufschance in Dynamics 365 mit **sync with Partner Center** auf **Ja**festgelegt ist, warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center-Konto an.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-184">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="1cb4e-185">Ihre Verweise werden mit Dynamics 365 synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-185">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="1cb4e-186">Wenn Sie die Option in Dynamics 365 CRM aktualisieren, werden die Änderungen daher in Ihrem Partner Center-Konto synchronisiert, wenn Sie die Option "mit Partner Center synchronisieren" auf "Ja" festlegen.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-186">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="1cb4e-187">Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-187">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="1cb4e-188">Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:</span><span class="sxs-lookup"><span data-stu-id="1cb4e-188">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="1cb4e-189">Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-189">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="1cb4e-190">Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-190">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="1cb4e-191">Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-191">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="1cb4e-192">Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-192">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="1cb4e-193">Navigieren Sie zu **Open Verkaufschancen**.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-193">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="1cb4e-194">Der im Microsoft Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-194">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="1cb4e-195">Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="1cb4e-195">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1cb4e-196">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="1cb4e-196">Next steps</span></span>

- [<span data-ttu-id="1cb4e-197">Weitere Informationen zur Microsoft powerautomatisieren-Plattform</span><span class="sxs-lookup"><span data-stu-id="1cb4e-197">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="1cb4e-198">Partner Center-webhook-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="1cb4e-198">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="1cb4e-199">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="1cb4e-199">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1cb4e-200">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="1cb4e-200">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
