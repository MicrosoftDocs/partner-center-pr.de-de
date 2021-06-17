---
title: Problembehandlung bei Connectors mit Co-Selling-Empfehlungen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier finden Sie Antworten auf häufig gestellte Fragen zur Verwendung von Co-Selling-Connectors. Lesen Sie diese häufig gestellten Fragen zur Problembehandlung für Co-Selling-Connectors.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276927"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="24e8a-104">Problembehandlung bei Connectors mit Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="24e8a-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="24e8a-105">**Gilt für**: Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="24e8a-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="24e8a-106">**Geeignete Rollen:** Empfehlungsadministrator | Systemadministrator oder Systemanpasser im CRM</span><span class="sxs-lookup"><span data-stu-id="24e8a-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="24e8a-107">Fragen und Antworten zu Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24e8a-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="24e8a-108">Können Sie eine Testlösung für Co-Selling-Empfehlungsconnectors für Ihre Umgebung verwenden?</span><span class="sxs-lookup"><span data-stu-id="24e8a-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="24e8a-109">Wenn Sie sich in der Test-/Stagingumgebung befinden, können Sie sich für eine Testlösung entscheiden.</span><span class="sxs-lookup"><span data-stu-id="24e8a-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="24e8a-110">Die kostenpflichtige Version der Connectors ist in AppSource um 15 US$/Monat verfügbar.</span><span class="sxs-lookup"><span data-stu-id="24e8a-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="24e8a-111">Mit der kostenpflichtigen Verbindung erhalten Sie 10.000 API-Aufrufe pro Tag.</span><span class="sxs-lookup"><span data-stu-id="24e8a-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="24e8a-112">Die Connectors sind Wrapper auf Partner Center Empfehlungs-APIs.</span><span class="sxs-lookup"><span data-stu-id="24e8a-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="24e8a-113">Immer wenn die Connectorlösungen für ein **Create-** oder **Update-Ereignis** für die Verkaufschancen auf Partner Center- oder CRM-Seite ausgeführt werden, wird ein API-Aufruf ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="24e8a-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="24e8a-114">Welche Rolle benötigen Sie zum Erstellen von Abschnitten in der CRM-Umgebung?</span><span class="sxs-lookup"><span data-stu-id="24e8a-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="24e8a-115">Benutzer, die Systemadministratoren oder Systemanpasser sind, können Änderungen für alle Benutzer anwenden.</span><span class="sxs-lookup"><span data-stu-id="24e8a-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="24e8a-116">Alle App-Benutzer können jedoch das System personalisieren und sogar einige ihrer Anpassungen mit anderen teilen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="24e8a-117">Benötigen Partnerverkäufer spezielle Rollen, um an Partner Center zu arbeiten?</span><span class="sxs-lookup"><span data-stu-id="24e8a-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="24e8a-118">Partnerverkäufern muss die Rolle "Empfehlungsadministrator" zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="24e8a-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="24e8a-119">Weitere Informationen finden Sie unter [Übersicht über Berechtigungen.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="24e8a-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="24e8a-120">Welche Felder müssen zuerst in Ihrer CRM-Umgebung eingerichtet werden?</span><span class="sxs-lookup"><span data-stu-id="24e8a-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="24e8a-121">• Stellen Sie sicher, dass Ihre Währung für Ihren Standort geeignet ist und sich genau in Ihrer CRM-Umgebung befindet.</span><span class="sxs-lookup"><span data-stu-id="24e8a-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="24e8a-122">• Ihr Vertriebsteam sollte in Ihrer CRM-Umgebung als CRM-Benutzer aufgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="24e8a-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="24e8a-123">Welche Voraussetzungen sind für die Erstellung Power Automate Umgebung erforderlich?</span><span class="sxs-lookup"><span data-stu-id="24e8a-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="24e8a-124">Um die Power Automate-Umgebung verwenden zu können, benötigen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="24e8a-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="24e8a-125">Eine Power Automate Lizenz ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24e8a-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="24e8a-126">Mindestens 1 GB Speicher ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24e8a-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="24e8a-127">Benötigen Sie ein Dynamics 365-Abonnement, um die Salesforce Connectors-Lösung verwenden zu können?</span><span class="sxs-lookup"><span data-stu-id="24e8a-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="24e8a-128">Die Salesforce Connector-Lösung ist vom Typ "Dynamics Flow", der die Synchronisierung mit anderen CRM-Systemen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24e8a-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="24e8a-129">Für die Lösung ist es nicht erforderlich, dass Sie über eine Dynamics 365-Instanz oder ein Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="24e8a-130">Während der Installation der Salesforce-Lösung wird möglicherweise eine Dropdown-Dropdown-Datei mit vorhandener CDS-Umgebung in Ihrem Unternehmen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="24e8a-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="24e8a-131">Sie müssen diese Umgebung auswählen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-131">You need to select that environment.</span></span> <span data-ttu-id="24e8a-132">Wenn Sie außerdem die Fehlermeldung "Es konnte keine Dynamics 365-Organisation gefunden werden, die mit einem angemeldeten Benutzer verbunden ist" erhalten, müssen Sie eine neue Umgebung für den Connector erstellen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="24e8a-133">Fragen und Antworten zur Konfiguration</span><span class="sxs-lookup"><span data-stu-id="24e8a-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="24e8a-134">Was sollten Sie tun, wenn beim Aktivieren von Flows in Power Automate Platform der folgende Fehler auftritt?</span><span class="sxs-lookup"><span data-stu-id="24e8a-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="24e8a-135">Fehler: Fehler bei Anforderung an Azure Resource Manager mit folgendem Fehler: '{"error":{"code":"WorkflowTriggerNotFound","message":"Der Workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span><span class="sxs-lookup"><span data-stu-id="24e8a-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="24e8a-136">Führen Sie die folgenden Schritte zur Problembehandlung aus:</span><span class="sxs-lookup"><span data-stu-id="24e8a-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="24e8a-137">Löschen Sie die CDS-Verbindung, und erstellen Sie die CDS-Verbindungen neu.</span><span class="sxs-lookup"><span data-stu-id="24e8a-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="24e8a-138">Deaktivieren und Aktivieren des untergeordneten Flows</span><span class="sxs-lookup"><span data-stu-id="24e8a-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="24e8a-139">Löschen Sie die Projektmappe, und installieren Sie sie neu.</span><span class="sxs-lookup"><span data-stu-id="24e8a-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="24e8a-140">Was sollten Sie tun, wenn beim Hinzufügen eines Partner Center Connectors in Power Automate Platform der Fehler "Anmelden" auftritt?</span><span class="sxs-lookup"><span data-stu-id="24e8a-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fehlermeldung, die eine Anmeldung erfordert.":::

<span data-ttu-id="24e8a-142">Führen Sie diesen Problembehandlungsschritt aus:</span><span class="sxs-lookup"><span data-stu-id="24e8a-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="24e8a-143">Verwenden Sie Ihre Partner Center Anmeldeinformationen, um sich einmal bei der Flowumgebung anzumelden (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="24e8a-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="24e8a-144">Was sollten Sie tun, wenn beim Aktivieren des Partner Center zu CRM in Power Automate Platform der folgende Fehler angezeigt wird?</span><span class="sxs-lookup"><span data-stu-id="24e8a-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fehlermeldung, die Updates erfordert.":::

<span data-ttu-id="24e8a-146">Führen Sie die folgenden Schritte zur Problembehandlung aus:</span><span class="sxs-lookup"><span data-stu-id="24e8a-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="24e8a-147">Aktivieren Sie zunächst die folgenden beiden untergeordneten Flows, bevor Sie den Partner Center zu CRM aktivieren.</span><span class="sxs-lookup"><span data-stu-id="24e8a-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="24e8a-148">Partner Center zu CRM – Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="24e8a-149">Partner Center Microsoft Co-Selling-Empfehlungsupdates für CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="24e8a-150">Was sollten Sie tun, wenn Sie keine Verbindungen zum Flow hinzufügen können, wenn Sie versuchen, den Flow zu bearbeiten?</span><span class="sxs-lookup"><span data-stu-id="24e8a-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="24e8a-151">Sie fügen verbindungen zum Flow hinzu, während der Flow ausgeführt wird, und fügen jedem Flow separat hinzu.</span><span class="sxs-lookup"><span data-stu-id="24e8a-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="24e8a-152">Wenn das Dialogfeld zum Hinzufügen von Verbindungen während der Bearbeitung des Flows nicht automatisch geöffnet wird, können Sie die einzelnen Schritte und Unterschritte der Flows einzeln bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="24e8a-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="24e8a-153">Wählen Sie jeden Flow aus, und bearbeiten Sie sie einzeln.</span><span class="sxs-lookup"><span data-stu-id="24e8a-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="24e8a-154">Erweitern Sie alle Schritte im Flow.</span><span class="sxs-lookup"><span data-stu-id="24e8a-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Schritte, die Verbindungen benötigen.":::

- <span data-ttu-id="24e8a-156">Wählen Sie die Schritte aus, in denen ein Warnsymbol angezeigt wird, in dem Sie aufgefordert werden, Verbindungen zuzuordnen und Verbindungen hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Bearbeiten Sie den Flow Schritt für Schritt.":::


5. <span data-ttu-id="24e8a-158">Was sollten Sie tun, wenn die Flows der Lösung für Co-Selling-Empfehlungsconnectors nicht aktivieren?</span><span class="sxs-lookup"><span data-stu-id="24e8a-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="24e8a-159">A.</span><span class="sxs-lookup"><span data-stu-id="24e8a-159">A.</span></span> <span data-ttu-id="24e8a-160">In Power Automate müssen Sie Flows in der folgenden Reihenfolge bearbeiten und aktualisieren, um die richtigen Verbindungen zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="24e8a-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="24e8a-161">Partner Center Webhookregistrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="24e8a-162">Erstellen einer Co-Selling-Empfehlung – Salesforce zu Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="24e8a-163">Partner Center Microsoft Co-Selling-Empfehlungsupdates für Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="24e8a-164">Partner Center zu Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="24e8a-165">Salesforce zu Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="24e8a-166">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="24e8a-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="24e8a-168">B.</span><span class="sxs-lookup"><span data-stu-id="24e8a-168">B.</span></span> <span data-ttu-id="24e8a-169">Wählen Sie für jeden Flow die Option **Nur Benutzer ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="24e8a-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="24e8a-170">Wählen Sie Verbindung anstelle **von Vom benutzer nur ausführen bereitgestellt** **verwenden** aus.</span><span class="sxs-lookup"><span data-stu-id="24e8a-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="So aktivieren Sie einen Flow":::


<span data-ttu-id="24e8a-172">C.</span><span class="sxs-lookup"><span data-stu-id="24e8a-172">C.</span></span> <span data-ttu-id="24e8a-173">Aktivieren Sie diese unten erwähnten Flows:</span><span class="sxs-lookup"><span data-stu-id="24e8a-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="24e8a-174">Partner Center Microsoft Co-Selling-Empfehlungsupdates für Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="24e8a-175">Salesforce zu Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="24e8a-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="24e8a-176">D:</span><span class="sxs-lookup"><span data-stu-id="24e8a-176">D.</span></span> <span data-ttu-id="24e8a-177">Aktivieren Sie alle verbleibenden Flows.</span><span class="sxs-lookup"><span data-stu-id="24e8a-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="24e8a-178">E.</span><span class="sxs-lookup"><span data-stu-id="24e8a-178">E.</span></span> <span data-ttu-id="24e8a-179">Wählen Sie unter Flow Partner Center Webhookregistrierung die Option **Ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="24e8a-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="24e8a-180">Geben Sie die **HTTP-URL** aus der ersten Aktion in Partner Center salesforce flow **an.**</span><span class="sxs-lookup"><span data-stu-id="24e8a-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="24e8a-181">Wählen Sie unter **Zu registrierende Ereignisse** alle vier Optionen aus, und wählen Sie für Overwrite (Überschreiben) die Option **Ja** aus.</span><span class="sxs-lookup"><span data-stu-id="24e8a-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="24e8a-182">Fragen und Antworten zu Ausführung/Wartung</span><span class="sxs-lookup"><span data-stu-id="24e8a-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="24e8a-183">Wie beheben Sie Fehler während Power Automate Flowausführung?</span><span class="sxs-lookup"><span data-stu-id="24e8a-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="24e8a-184">Um sicherzustellen, dass Ihre Power Automate Flows wie erwartet ausgeführt werden, und um Fehler während der Ausführung zu beheben, lesen [Sie Beheben von Flowfehlern.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="24e8a-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="24e8a-185">Was sollten Sie tun, wenn Empfehlungen angezeigt werden, die in Partner Center- oder CRM-Umgebung nicht ordnungsgemäß synchronisiert werden?</span><span class="sxs-lookup"><span data-stu-id="24e8a-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="24e8a-186">Wählen Sie **Überwachen** aus, um den Status der Empfehlungssynchronisierung zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisieren von Empfehlungen":::

<span data-ttu-id="24e8a-188">Stellen Sie sicher, dass die folgenden Bedingungen erfüllt sind:</span><span class="sxs-lookup"><span data-stu-id="24e8a-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="24e8a-189">Die Lösungs-ID wird als Teil der Verkaufschance bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="24e8a-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="24e8a-190">Es ist ein zweistelliger Ländercode erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24e8a-190">Two letter country code is required.</span></span>

- <span data-ttu-id="24e8a-191">Wenn Hilfe von Microsoft für die Verkaufschance ausgewählt ist, sind Kundenkontaktinformationen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24e8a-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="24e8a-192">Wie kann sichergestellt werden, dass eine Empfehlung bidirektional synchronisiert wird?</span><span class="sxs-lookup"><span data-stu-id="24e8a-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="24e8a-193">Führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="24e8a-193">Do the following steps:</span></span>

- <span data-ttu-id="24e8a-194">Partnerverkäufer müssen sicherstellen, dass sie die Option **Sync with Partner Center (Mit Partner Center** synchronisieren) im Abschnitt CRM aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="24e8a-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Stellen Sie sicher, dass Sie Synch aktiviert haben.":::

- <span data-ttu-id="24e8a-196">Verkäufer müssen umsatz- und enddatum angeben, wenn sie einen Lead qualifizieren.</span><span class="sxs-lookup"><span data-stu-id="24e8a-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="24e8a-197">Wenn die CRM-ID in der **Erstellungs-** oder **Aktualisierungsphase** der Co-Selling-Verkaufschance bereitgestellt wird, aber eine Leadchance mit dieser ID nicht in CRM gefunden wird, wird das Aktualisieren oder Erstellen ignoriert.</span><span class="sxs-lookup"><span data-stu-id="24e8a-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="24e8a-198">Stellen Sie sicher, dass das Feld "Empfehlungswährung" in der Salesforce-Umgebung konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="24e8a-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="24e8a-199">Was sollten Sie tun, wenn der Connector getrennt wird und Sie eine Empfehlungssynchronisierung übersehen?</span><span class="sxs-lookup"><span data-stu-id="24e8a-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="24e8a-200">Im Folgenden finden Sie einige der Optionen, die Sie ausprobieren können:</span><span class="sxs-lookup"><span data-stu-id="24e8a-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="24e8a-201">Überprüfen Sie, ob benutzername oder password für den Partner Center Benutzer mit Empfehlungsadministratorrollen abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="24e8a-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="24e8a-202">Sie können zu der nicht synchronisierten Verkaufschance wechseln, ein kleineres Update durchführen und beobachten, ob die Empfehlung synchronisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="24e8a-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="24e8a-203">Wenn die Flows ausgeführt wurden und fehlgeschlagen sind, wählen Sie den Flow aus, und übermitteln Sie die fehlgeschlagene Ausführung erneut.</span><span class="sxs-lookup"><span data-stu-id="24e8a-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="24e8a-204">Was sollten Sie tun, wenn Sie Zugriffsverweigerungsfehler erhalten?</span><span class="sxs-lookup"><span data-stu-id="24e8a-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="24e8a-205">Stellen Sie sicher, dass die entsprechenden Rollen vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="24e8a-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="24e8a-206">Rolle "Empfehlungsadministrator" für Partner Center Verkäufer</span><span class="sxs-lookup"><span data-stu-id="24e8a-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="24e8a-207">Systemadministrator- oder Systemanpasserrolle in Ihrer CRM-Instanz</span><span class="sxs-lookup"><span data-stu-id="24e8a-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="24e8a-208">Stellen Sie sicher, dass sich der Benutzer des Power Automate Flowkontos mindestens einmal im Voraus bei https://flow.microsoft.com anmeldet.</span><span class="sxs-lookup"><span data-stu-id="24e8a-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="24e8a-209">Was sollten Sie tun, wenn Beim Erstellen einer Co-Selling-Verkaufschance der Ländercode des **Kundenkontos** fehlt?</span><span class="sxs-lookup"><span data-stu-id="24e8a-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="24e8a-210">Sie müssen dem Kundenkonto in CRM den zweistelligen ISO-Ländercode hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="24e8a-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="24e8a-211">Was sollten Sie tun, wenn beim Erstellen einer Co-Selling-Verkaufschance der Fehler angezeigt wird, dass die **Lösungs-ID erforderlich ist?**</span><span class="sxs-lookup"><span data-stu-id="24e8a-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="24e8a-212">Um eine Co-Selling-Empfehlung zu erstellen, benötigen Sie eine Microsoft-Lösung, die für den Co-Selling bereit ist.</span><span class="sxs-lookup"><span data-stu-id="24e8a-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="24e8a-213">Was sollten Sie tun, wenn In Partner Center erstellte Co-Selling-Verkaufschancen angezeigt werden, die nicht mit CRM synchronisiert sind, obwohl keine Flowfehler auftreten?</span><span class="sxs-lookup"><span data-stu-id="24e8a-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="24e8a-214">Führen Sie folgende Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="24e8a-214">Do the following:</span></span>

- <span data-ttu-id="24e8a-215">Nachdem Sie in Partner Center einen neuen Co-Selling-Deal erstellt haben, überprüfen Sie, ob Partner Center zum Dynamics 365-Flow aufgerufen wird (er wird möglicherweise mehrmals aufgerufen).</span><span class="sxs-lookup"><span data-stu-id="24e8a-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="24e8a-216">Wenn der Flow aufgerufen wird, überprüfen Sie alle aufgerufenen Flows, und identifizieren Sie die Flow-Ausführung, die das CRM aktualisieren würde.</span><span class="sxs-lookup"><span data-stu-id="24e8a-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="24e8a-217">Sie können die Aktionen ausführen und überprüfen, ob das CRM aktualisiert wurde oder ein Problem aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="24e8a-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="24e8a-218">Überprüfen Sie in Partner Center new **deal (Neuer Deal),** um festzustellen, ob er mit CRM-ID aufgefüllt wird.</span><span class="sxs-lookup"><span data-stu-id="24e8a-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="24e8a-219">Stellen Sie sicher, dass der Deal nicht versehentlich als **Won** oder **Lost** in Partner Center geschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="24e8a-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="24e8a-220">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="24e8a-220">Next steps</span></span>

- [<span data-ttu-id="24e8a-221">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="24e8a-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="24e8a-222">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="24e8a-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
