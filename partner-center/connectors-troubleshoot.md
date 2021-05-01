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
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284212"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="12f7e-104">Problembehandlung bei Connectors mit Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="12f7e-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="12f7e-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="12f7e-105">**Applies to**</span></span>

- <span data-ttu-id="12f7e-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="12f7e-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="12f7e-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="12f7e-107">Salesforce CRM</span></span>

<span data-ttu-id="12f7e-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="12f7e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="12f7e-109">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="12f7e-109">Referrals admin</span></span>
- <span data-ttu-id="12f7e-110">Systemadministrator oder Systemanpasser im CRM</span><span class="sxs-lookup"><span data-stu-id="12f7e-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="12f7e-111">Fragen und Antworten zu Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="12f7e-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="12f7e-112">Können Sie eine Testlösung für Co-Selling-Empfehlungsconnectors für Ihre Umgebung verwenden?</span><span class="sxs-lookup"><span data-stu-id="12f7e-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="12f7e-113">Wenn Sie sich in der Test-/Stagingumgebung befinden, können Sie sich für eine Testlösung entscheiden.</span><span class="sxs-lookup"><span data-stu-id="12f7e-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="12f7e-114">Die kostenpflichtige Version der Connectors ist in AppSource unter 15 US$/Monat verfügbar.</span><span class="sxs-lookup"><span data-stu-id="12f7e-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="12f7e-115">Mit der kostenpflichtigen Verbindung erhalten Sie 10.000 API-Aufrufe pro Tag.</span><span class="sxs-lookup"><span data-stu-id="12f7e-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="12f7e-116">Die Connectors sind Wrapper auf Partner Center Empfehlungs-APIs.</span><span class="sxs-lookup"><span data-stu-id="12f7e-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="12f7e-117">Wenn die Connectorlösungen für ein **Create-** oder **Update-Ereignis** für die Verkaufschancen auf Partner Center- oder CRM-Seite ausgeführt werden, wird ein API-Aufruf ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="12f7e-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="12f7e-118">Welche Rolle benötigen Sie zum Erstellen von Abschnitten in der CRM-Umgebung?</span><span class="sxs-lookup"><span data-stu-id="12f7e-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="12f7e-119">Benutzer, die Systemadministratoren oder Systemanpasser sind, können Änderungen für alle Benutzer anwenden.</span><span class="sxs-lookup"><span data-stu-id="12f7e-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="12f7e-120">Alle App-Benutzer können jedoch das System personalisieren und sogar einige ihrer Anpassungen mit anderen teilen.</span><span class="sxs-lookup"><span data-stu-id="12f7e-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="12f7e-121">Benötigen Partnerverkäufer spezielle Rollen, um an Partner Center zu arbeiten?</span><span class="sxs-lookup"><span data-stu-id="12f7e-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="12f7e-122">Partnerverkäufern muss die Rolle "Empfehlungsadministrator" zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="12f7e-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="12f7e-123">Weitere Informationen finden Sie unter [Übersicht über Berechtigungen.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="12f7e-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="12f7e-124">Welche Felder müssen zuerst in Ihrer CRM-Umgebung eingerichtet werden?</span><span class="sxs-lookup"><span data-stu-id="12f7e-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="12f7e-125">• Stellen Sie sicher, dass Ihre Währung für Ihren Standort geeignet ist und sich genau in Ihrer CRM-Umgebung befindet.</span><span class="sxs-lookup"><span data-stu-id="12f7e-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="12f7e-126">• Ihr Vertriebsteam sollte in Ihrer CRM-Umgebung als CRM-Benutzer aufgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="12f7e-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="12f7e-127">Welche Voraussetzungen sind für die Erstellung Power Automate Umgebung erforderlich?</span><span class="sxs-lookup"><span data-stu-id="12f7e-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="12f7e-128">Um die Power Automate verwenden zu können, benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="12f7e-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="12f7e-129">Eine Power Automate Lizenz ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12f7e-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="12f7e-130">Mindestens 1 GB Speicher ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12f7e-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="12f7e-131">Benötigen Sie ein Dynamics 365-Abonnement, um die Salesforce Connectors-Lösung verwenden zu können?</span><span class="sxs-lookup"><span data-stu-id="12f7e-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="12f7e-132">Die Salesforce Connector-Lösung ist vom Typ "Dynamics Flow", der die Synchronisierung mit anderen CRM-Systemen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f7e-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="12f7e-133">Die Lösung erfordert keine Dynamics 365-Instanz oder ein Abonnement.</span><span class="sxs-lookup"><span data-stu-id="12f7e-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="12f7e-134">Während der Installation der Salesforce-Lösung wird möglicherweise eine Dropdownliste mit einer vorhandenen CDS-Umgebung in Ihrem Unternehmen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="12f7e-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="12f7e-135">Sie müssen diese Umgebung auswählen.</span><span class="sxs-lookup"><span data-stu-id="12f7e-135">You need to select that environment.</span></span> <span data-ttu-id="12f7e-136">Wenn Sie außerdem die Fehlermeldung "Wir haben keine Dynamics 365-Organisation finden, die mit einem angemeldeten Benutzer verbunden ist" erhalten, müssen Sie eine neue Umgebung für den Connector erstellen.</span><span class="sxs-lookup"><span data-stu-id="12f7e-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="12f7e-137">Fragen und Antworten zur Konfiguration</span><span class="sxs-lookup"><span data-stu-id="12f7e-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="12f7e-138">Was sollten Sie tun, wenn beim Aktivieren von Flows in Power Automate Platform der folgende Fehler auftritt?</span><span class="sxs-lookup"><span data-stu-id="12f7e-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="12f7e-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span><span class="sxs-lookup"><span data-stu-id="12f7e-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="12f7e-140">Führen Sie die folgenden Schritte zur Problembehandlung aus:</span><span class="sxs-lookup"><span data-stu-id="12f7e-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="12f7e-141">Löschen Sie die CDS-Verbindung, und erstellen Sie dann die CDS-Verbindungen neu.</span><span class="sxs-lookup"><span data-stu-id="12f7e-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="12f7e-142">Deaktivieren und Aktivieren des untergeordneten Datenflusses</span><span class="sxs-lookup"><span data-stu-id="12f7e-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="12f7e-143">Löschen Sie die Projektmappe, und installieren Sie die Lösung erneut.</span><span class="sxs-lookup"><span data-stu-id="12f7e-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="12f7e-144">Was sollten Sie tun, wenn beim Hinzufügen eines Partner Center connectors in Power Automate Platform der Fehler "Anmelden" auftritt?</span><span class="sxs-lookup"><span data-stu-id="12f7e-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fehlermeldung, die eine Anmeldung erfordert":::

<span data-ttu-id="12f7e-146">Führen Sie diesen Problembehandlungsschritt aus:</span><span class="sxs-lookup"><span data-stu-id="12f7e-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="12f7e-147">Verwenden Sie Ihre Partner Center Anmeldeinformationen, um sich einmal bei der Flowumgebung anzumelden (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="12f7e-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="12f7e-148">Was sollten Sie tun, wenn beim Aktivieren des Partner Center zu CRM in Power Automate Platform der folgende Fehler auftritt?</span><span class="sxs-lookup"><span data-stu-id="12f7e-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fehlermeldung, die Updates erfordert":::

<span data-ttu-id="12f7e-150">Führen Sie die folgenden Schritte zur Problembehandlung aus:</span><span class="sxs-lookup"><span data-stu-id="12f7e-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="12f7e-151">Aktivieren Sie zunächst die folgenden beiden untergeordneten Flows, bevor Sie den Partner Center zu CRM aktivieren.</span><span class="sxs-lookup"><span data-stu-id="12f7e-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="12f7e-152">Partner Center zu CRM – Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="12f7e-153">Partner Center Microsoft Co-Selling-Empfehlungsupdates für CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="12f7e-154">Was sollten Sie tun, wenn Sie keine Verbindungen zum Flow hinzufügen können, wenn Sie versuchen, den Flow zu bearbeiten?</span><span class="sxs-lookup"><span data-stu-id="12f7e-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="12f7e-155">Sie fügen verbindungen zum Flow hinzu, während der Flow ausgeführt wird, und fügen jedem Flow separat hinzu.</span><span class="sxs-lookup"><span data-stu-id="12f7e-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="12f7e-156">Wenn das Dialogfeld zum Hinzufügen von Verbindungen während der Bearbeitung des Flows nicht automatisch geöffnet wird, können Sie die einzelnen Schritte und Unterschritte der Flows einzeln bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="12f7e-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="12f7e-157">Wählen Sie jeden Flow aus, und bearbeiten Sie sie einzeln.</span><span class="sxs-lookup"><span data-stu-id="12f7e-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="12f7e-158">Erweitern Sie alle Schritte im Flow.</span><span class="sxs-lookup"><span data-stu-id="12f7e-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Schritte, die Verbindungen benötigen":::

- <span data-ttu-id="12f7e-160">Wählen Sie die Schritte aus, in denen ein Warnsymbol angezeigt wird, in dem Sie aufgefordert werden, Verbindungen zuzuordnen und Verbindungen hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="12f7e-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Flow schritt für Schritt bearbeiten":::


5. <span data-ttu-id="12f7e-162">Was sollten Sie tun, wenn die Flows der Lösung für Co-Selling-Empfehlungsconnectors nicht aktivieren?</span><span class="sxs-lookup"><span data-stu-id="12f7e-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="12f7e-163">A.</span><span class="sxs-lookup"><span data-stu-id="12f7e-163">A.</span></span> <span data-ttu-id="12f7e-164">In Power Automate müssen Sie Flows in der folgenden Reihenfolge bearbeiten und aktualisieren, um die richtigen Verbindungen zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="12f7e-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="12f7e-165">Partner Center Webhookregistrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="12f7e-166">Erstellen einer Co-Selling-Empfehlung – Salesforce zu Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="12f7e-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="12f7e-168">Partner Center to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="12f7e-169">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="12f7e-170">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="12f7e-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="12f7e-172">B.</span><span class="sxs-lookup"><span data-stu-id="12f7e-172">B.</span></span> <span data-ttu-id="12f7e-173">Wählen Sie für jeden Flow die Option **Nur Benutzer ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="12f7e-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="12f7e-174">Wählen **Sie Verbindung anstelle** von Vom Benutzer bereitgestellt verwenden **aus.**</span><span class="sxs-lookup"><span data-stu-id="12f7e-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="So aktivieren Sie einen Flow":::


<span data-ttu-id="12f7e-176">C.</span><span class="sxs-lookup"><span data-stu-id="12f7e-176">C.</span></span> <span data-ttu-id="12f7e-177">Aktivieren Sie die unten genannten Flows:</span><span class="sxs-lookup"><span data-stu-id="12f7e-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="12f7e-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="12f7e-179">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="12f7e-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="12f7e-180">D:</span><span class="sxs-lookup"><span data-stu-id="12f7e-180">D.</span></span> <span data-ttu-id="12f7e-181">Aktivieren Sie alle verbleibenden Flows.</span><span class="sxs-lookup"><span data-stu-id="12f7e-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="12f7e-182">E.</span><span class="sxs-lookup"><span data-stu-id="12f7e-182">E.</span></span> <span data-ttu-id="12f7e-183">Wählen Sie bei Partner Center Webhookregistrierung die Option **Ausführen aus.**</span><span class="sxs-lookup"><span data-stu-id="12f7e-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="12f7e-184">Geben Sie **die HTTP-URL** der ersten Aktion in der Partner Center **Salesforce-Flow** an.</span><span class="sxs-lookup"><span data-stu-id="12f7e-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="12f7e-185">Wählen Sie unter Zu registrierende **Ereignisse alle vier Optionen** aus, und wählen Sie **für** Überschreiben die Option Ja aus.</span><span class="sxs-lookup"><span data-stu-id="12f7e-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="12f7e-186">Fragen und Antworten zur Ausführung/Wartung</span><span class="sxs-lookup"><span data-stu-id="12f7e-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="12f7e-187">Wie beheben Sie Fehler während Power Automate Flowausführung?</span><span class="sxs-lookup"><span data-stu-id="12f7e-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="12f7e-188">Um sicherzustellen, dass Power Automate Flows wie erwartet ausgeführt werden, und um Fehler während der Ausführung zu beheben, lesen Sie [Beheben von Flowfehlern.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="12f7e-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="12f7e-189">Was sollten Sie tun, wenn Empfehlungen angezeigt werden, die nicht ordnungsgemäß in einer Partner Center CRM-Umgebung synchronisiert werden?</span><span class="sxs-lookup"><span data-stu-id="12f7e-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="12f7e-190">Wählen Sie Überwachen aus, um den Status der **Empfehlungssynchronisierung zu ermitteln.**</span><span class="sxs-lookup"><span data-stu-id="12f7e-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisieren von Empfehlungen":::

<span data-ttu-id="12f7e-192">Stellen Sie sicher, dass die folgenden Bedingungen erfüllt sind:</span><span class="sxs-lookup"><span data-stu-id="12f7e-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="12f7e-193">Die Lösungs-ID wird als Teil der Verkaufschance bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="12f7e-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="12f7e-194">Es ist ein zweistelliger Ländercode erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12f7e-194">Two letter country code is required.</span></span>

- <span data-ttu-id="12f7e-195">Wenn Hilfe von Microsoft für die Verkaufschance ausgewählt ist, sind Kundenkontaktinformationen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12f7e-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="12f7e-196">Wie kann sichergestellt werden, dass eine Empfehlung bidirektional synchronisiert wird?</span><span class="sxs-lookup"><span data-stu-id="12f7e-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="12f7e-197">Führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="12f7e-197">Do the following steps:</span></span>

- <span data-ttu-id="12f7e-198">Partnerverkäufer müssen sicherstellen, dass sie die Option **Sync with Partner Center (Mit Partner Center** synchronisieren) im Abschnitt CRM aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="12f7e-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Stellen Sie sicher, dass Sie Synch aktiviert haben.":::

- <span data-ttu-id="12f7e-200">Verkäufer müssen umsatz- und enddatum angeben, wenn sie einen Lead qualifizieren.</span><span class="sxs-lookup"><span data-stu-id="12f7e-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="12f7e-201">Wenn die CRM-ID in der **Erstellungs-** oder **Aktualisierungsphase** der Co-Selling-Verkaufschance bereitgestellt wird, aber eine Leadchance mit dieser ID nicht in CRM gefunden wird, wird das Aktualisieren oder Erstellen ignoriert.</span><span class="sxs-lookup"><span data-stu-id="12f7e-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="12f7e-202">Stellen Sie sicher, dass das Feld "Empfehlungswährung" in der Salesforce-Umgebung konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="12f7e-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="12f7e-203">Was sollten Sie tun, wenn der Connector getrennt wird und Sie eine Empfehlungssynchronisierung übersehen?</span><span class="sxs-lookup"><span data-stu-id="12f7e-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="12f7e-204">Im Folgenden finden Sie einige der Optionen, die Sie ausprobieren können:</span><span class="sxs-lookup"><span data-stu-id="12f7e-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="12f7e-205">Überprüfen Sie, ob benutzername oder password für den Partner Center Benutzer mit Empfehlungsadministratorrollen abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="12f7e-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="12f7e-206">Sie können zu der nicht synchronisierten Verkaufschance wechseln, ein kleineres Update durchführen und beobachten, ob die Empfehlung synchronisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="12f7e-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="12f7e-207">Wenn die Flows ausgeführt wurden und fehlgeschlagen sind, wählen Sie den Flow aus, und übermitteln Sie die fehlgeschlagene Ausführung erneut.</span><span class="sxs-lookup"><span data-stu-id="12f7e-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="12f7e-208">Was sollten Sie tun, wenn Zugriffsverweigerungsfehler auftreten?</span><span class="sxs-lookup"><span data-stu-id="12f7e-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="12f7e-209">Stellen Sie sicher, dass die entsprechenden Rollen vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="12f7e-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="12f7e-210">Rolle "Empfehlungsadministrator" für Partner Center Verkäufer</span><span class="sxs-lookup"><span data-stu-id="12f7e-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="12f7e-211">Rolle "Systemadministrator" oder "Systemanpasser" in Ihrer CRM-Instanz</span><span class="sxs-lookup"><span data-stu-id="12f7e-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="12f7e-212">Stellen Sie sicher Power Automate dass sich der Benutzer des Kontos mindestens https://flow.microsoft.com einmal im Voraus bei anmeldet.</span><span class="sxs-lookup"><span data-stu-id="12f7e-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="12f7e-213">Wenn Sie sehen, dass **der Ländercode des** Kundenkontos beim Erstellen einer Co-Sell-Verkaufschance fehlt, was sollten Sie tun?</span><span class="sxs-lookup"><span data-stu-id="12f7e-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="12f7e-214">Sie müssen dem Kundenkonto in CRM den zwei buchstabenbasierten ISO-Ländercode hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="12f7e-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="12f7e-215">Was sollten Sie tun, wenn der Fehler angezeigt wird, dass die **Lösungs-ID** beim Erstellen einer Co-Sell-Verkaufschance erforderlich ist?</span><span class="sxs-lookup"><span data-stu-id="12f7e-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="12f7e-216">Um eine Co-Sell-Empfehlung zu erstellen, benötigen Sie eine Lösung, die für den Co-Sell-Verkauf von Microsoft bereit ist.</span><span class="sxs-lookup"><span data-stu-id="12f7e-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="12f7e-217">Was sollten Sie tun, wenn in Partner Center Co-Sell-Verkaufschancen entstehen, die nicht mit CRM synchronisiert werden, obwohl keine Flowfehler auftreten?</span><span class="sxs-lookup"><span data-stu-id="12f7e-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="12f7e-218">Gehen Sie folgendermaßen vor:</span><span class="sxs-lookup"><span data-stu-id="12f7e-218">Do the following:</span></span>

- <span data-ttu-id="12f7e-219">Nachdem Sie in Partner Center einen neuen Co-Sell-Deal erstellt haben, überprüfen Sie, ob der Flow Partner Center zu Dynamics 365 aufgerufen wird (er wird möglicherweise mehrmals aufgerufen).</span><span class="sxs-lookup"><span data-stu-id="12f7e-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="12f7e-220">Wenn der Flow aufgerufen wird, überprüfen Sie alle aufgerufenen Flows, und identifizieren Sie die Flow-Ausführung, die das CRM aktualisieren würde.</span><span class="sxs-lookup"><span data-stu-id="12f7e-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="12f7e-221">Sie können die Aktionen ausführen und überprüfen, ob das CRM aktualisiert wurde oder ein Problem aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="12f7e-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="12f7e-222">Überprüfen **Sie in der** Partner Center, ob er mit der CRM-ID aufgefüllt wird.</span><span class="sxs-lookup"><span data-stu-id="12f7e-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="12f7e-223">Stellen Sie sicher, dass der Deal nicht versehentlich als **Won** oder **Lost** in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="12f7e-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="12f7e-224">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="12f7e-224">Next steps</span></span>

- [<span data-ttu-id="12f7e-225">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="12f7e-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="12f7e-226">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="12f7e-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
