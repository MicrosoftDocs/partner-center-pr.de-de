---
title: Problembehandlung bei Connectors mit Co-Selling-Empfehlungen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier finden Sie Antworten auf häufig gestellte Fragen zur Verwendung von Co-Sell-Connectors. Lesen Sie diese häufig gestellten Fragen zur Problembehandlung für Co-Sell-Connectors.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148345"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="77c1e-104">Problembehandlung bei Connectors mit Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="77c1e-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="77c1e-105">**Gilt für**: Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="77c1e-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="77c1e-106">**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Systemadministrator oder Systemanpasser im CRM</span><span class="sxs-lookup"><span data-stu-id="77c1e-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="77c1e-107">Fragen und Antworten zu Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77c1e-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="77c1e-108">Können Sie eine Testlösung für Co-Sell-Empfehlungsconnectors für Ihre Umgebung verwenden?</span><span class="sxs-lookup"><span data-stu-id="77c1e-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="77c1e-109">Wenn Sie sich in der Test-/Stagingumgebung befinden, können Sie eine Testlösung wählen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="77c1e-110">Die kostenpflichtige Version der Connectors ist in AppSource für 15 US-Dollar pro Monat verfügbar.</span><span class="sxs-lookup"><span data-stu-id="77c1e-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="77c1e-111">Mit der kostenpflichtigen Verbindung erhalten Sie 10.000 API-Aufrufe pro Tag.</span><span class="sxs-lookup"><span data-stu-id="77c1e-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="77c1e-112">Die Connectors sind Wrapper auf Partner Center Empfehlungs-APIs.</span><span class="sxs-lookup"><span data-stu-id="77c1e-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="77c1e-113">Wenn die Connectorlösungen für ein **Create-** oder **Update-Ereignis** für die Verkaufschancen auf Partner Center crm-Seite ausgeführt werden, wird ein API-Aufruf ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="77c1e-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="77c1e-114">Welche Rolle benötigen Sie, um Abschnitte in der CRM-Umgebung zu erstellen?</span><span class="sxs-lookup"><span data-stu-id="77c1e-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="77c1e-115">Benutzer, die Systemadministratoren oder Systemanpasser sind, können Änderungen für alle Benutzer anwenden.</span><span class="sxs-lookup"><span data-stu-id="77c1e-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="77c1e-116">Alle App-Benutzer können jedoch das System personalisieren und sogar einige ihrer Anpassungen mit anderen teilen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="77c1e-117">Benötigen Partnerverkäufer spezielle Rollen, um an Partner Center?</span><span class="sxs-lookup"><span data-stu-id="77c1e-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="77c1e-118">Partnerverkäufern muss die Rolle "Empfehlungsadministrator" zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="77c1e-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="77c1e-119">Weitere Informationen finden Sie unter [Übersicht über Berechtigungen.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="77c1e-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="77c1e-120">Welche Felder müssen zuerst in Ihrer CRM-Umgebung eingerichtet werden?</span><span class="sxs-lookup"><span data-stu-id="77c1e-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="77c1e-121">• Stellen Sie sicher, dass Ihre Währung für Ihren Standort geeignet ist und sich genau in Ihrer CRM-Umgebung befindet.</span><span class="sxs-lookup"><span data-stu-id="77c1e-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="77c1e-122">• Ihr Vertriebsteam sollte in Ihrer CRM-Umgebung als CRM-Benutzer aufgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="77c1e-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="77c1e-123">Welche Voraussetzungen sind für die Erstellung Power Automate Umgebung erforderlich?</span><span class="sxs-lookup"><span data-stu-id="77c1e-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="77c1e-124">Um die Power Automate-Umgebung verwenden zu können, benötigen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="77c1e-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="77c1e-125">Eine Power Automate Lizenz ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77c1e-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="77c1e-126">Mindestens 1 GB Speicher ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77c1e-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="77c1e-127">Benötigen Sie ein Dynamics 365-Abonnement, um die Salesforce Connectors-Lösung verwenden zu können?</span><span class="sxs-lookup"><span data-stu-id="77c1e-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="77c1e-128">Die Salesforce Connector-Lösung ist vom Typ "Dynamics Flow", der die Synchronisierung mit anderen CRM-Systemen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77c1e-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="77c1e-129">Für die Lösung ist es nicht erforderlich, dass Sie über eine Dynamics 365-Instanz oder ein Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="77c1e-130">Während der Installation der Salesforce-Lösung wird möglicherweise eine Dropdown-Datei mit vorhandener CDS-Umgebung in Ihrem Unternehmen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="77c1e-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="77c1e-131">Sie müssen diese Umgebung auswählen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-131">You need to select that environment.</span></span> <span data-ttu-id="77c1e-132">Wenn Sie außerdem die Fehlermeldung "Es konnte keine Dynamics 365-Organisation gefunden werden, die mit einem angemeldeten Benutzer verbunden ist" erhalten, müssen Sie eine neue Umgebung für den Connector erstellen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="77c1e-133">Fragen und Antworten zur Konfiguration</span><span class="sxs-lookup"><span data-stu-id="77c1e-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="77c1e-134">Was sollten Sie tun, wenn beim Aktivieren von Flows in Power Automate Platform der folgende Fehler auftritt?</span><span class="sxs-lookup"><span data-stu-id="77c1e-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="77c1e-135">Fehler: Fehler bei Anforderung an Azure Resource Manager mit folgendem Fehler: '{"error":{"code":"WorkflowTriggerNotFound","message":"Der Workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span><span class="sxs-lookup"><span data-stu-id="77c1e-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="77c1e-136">Führen Sie die folgenden Schritte zur Problembehandlung aus:</span><span class="sxs-lookup"><span data-stu-id="77c1e-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="77c1e-137">Löschen Sie die CDS-Verbindung, und erstellen Sie die CDS-Verbindungen neu.</span><span class="sxs-lookup"><span data-stu-id="77c1e-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="77c1e-138">Deaktivieren und Aktivieren des untergeordneten Flows</span><span class="sxs-lookup"><span data-stu-id="77c1e-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="77c1e-139">Löschen Sie die Projektmappe, und installieren Sie sie neu.</span><span class="sxs-lookup"><span data-stu-id="77c1e-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="77c1e-140">Was sollten Sie tun, wenn beim Hinzufügen eines Partner Center Connectors in Power Automate Platform der Fehler "Anmelden" auftritt?</span><span class="sxs-lookup"><span data-stu-id="77c1e-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fehlermeldung, die eine Anmeldung erfordert":::

<span data-ttu-id="77c1e-142">Führen Sie diesen Problembehandlungsschritt aus:</span><span class="sxs-lookup"><span data-stu-id="77c1e-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="77c1e-143">Verwenden Sie Partner Center Anmeldeinformationen, um sich einmal bei der Flowumgebung anzumelden (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="77c1e-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="77c1e-144">Was sollten Sie tun, wenn sie beim Aktivieren des Partner Center crm-Flusses in der Power Automate-Plattform die folgende Fehlermeldung erhalten?</span><span class="sxs-lookup"><span data-stu-id="77c1e-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fehlermeldung, die Updates erfordert":::

<span data-ttu-id="77c1e-146">Führen Sie die folgenden Schritte zur Problembehandlung aus:</span><span class="sxs-lookup"><span data-stu-id="77c1e-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="77c1e-147">Aktivieren Sie zuerst die folgenden beiden untergeordneten Flows, bevor Sie den Partner Center CRM-Flow aktivieren.</span><span class="sxs-lookup"><span data-stu-id="77c1e-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="77c1e-148">Partner Center crm – Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="77c1e-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="77c1e-150">Was sollten Sie tun, wenn Sie keine Verbindungen zum Flow hinzufügen können, wenn Sie versuchen, den Flow zu bearbeiten?</span><span class="sxs-lookup"><span data-stu-id="77c1e-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="77c1e-151">Sie fügen verbindungen zum Flow hinzu, während der Flow ausgeführt wird, und fügen sie jedem Flow separat hinzu.</span><span class="sxs-lookup"><span data-stu-id="77c1e-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="77c1e-152">Wenn das Dialogfeld zum Hinzufügen von Verbindungen beim Bearbeiten des Flows nicht automatisch geöffnet wird, können Sie die einzelnen Schritte und Unterschritte der Flows einzeln bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="77c1e-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="77c1e-153">Wählen Sie jeden Flow aus, und bearbeiten Sie sie einzeln.</span><span class="sxs-lookup"><span data-stu-id="77c1e-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="77c1e-154">Erweitern aller Schritte im Flow</span><span class="sxs-lookup"><span data-stu-id="77c1e-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Schritte, die Verbindungen benötigen":::

- <span data-ttu-id="77c1e-156">Wählen Sie die Schritte aus, in denen ein Warnsymbol angezeigt wird, in dem Sie aufgefordert werden, Verbindungen zu verknüpfen und Verbindungen hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Schritt-für-Schritt-Bearbeiten des Datenflusses":::


5. <span data-ttu-id="77c1e-158">Was sollten Sie tun, wenn die Flows der Lösung für Co-Sell-Empfehlungsconnectors nicht ein aktivieren?</span><span class="sxs-lookup"><span data-stu-id="77c1e-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="77c1e-159">A.</span><span class="sxs-lookup"><span data-stu-id="77c1e-159">A.</span></span> <span data-ttu-id="77c1e-160">In Power Automate müssen Sie Flows in der folgenden Reihenfolge bearbeiten und aktualisieren, um die richtigen Verbindungen zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="77c1e-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="77c1e-161">Partner Center Webhookregistrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="77c1e-162">Erstellen einer Co-Sell-Empfehlung – Salesforce Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="77c1e-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="77c1e-164">Partner Center zu Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="77c1e-165">Salesforce zu Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="77c1e-166">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="77c1e-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="77c1e-168">B.</span><span class="sxs-lookup"><span data-stu-id="77c1e-168">B.</span></span> <span data-ttu-id="77c1e-169">Wählen Sie für jeden Flow die Option **Nur Benutzer ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="77c1e-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="77c1e-170">Wählen Sie Verbindung anstelle **von Vom benutzer nur ausführen bereitgestellt** **verwenden** aus.</span><span class="sxs-lookup"><span data-stu-id="77c1e-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="So aktivieren Sie einen Flow":::


<span data-ttu-id="77c1e-172">C.</span><span class="sxs-lookup"><span data-stu-id="77c1e-172">C.</span></span> <span data-ttu-id="77c1e-173">Aktivieren Sie diese unten erwähnten Flows:</span><span class="sxs-lookup"><span data-stu-id="77c1e-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="77c1e-174">Partner Center Microsoft Co-Selling-Empfehlungsupdates für Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="77c1e-175">Salesforce zu Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="77c1e-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="77c1e-176">D:</span><span class="sxs-lookup"><span data-stu-id="77c1e-176">D.</span></span> <span data-ttu-id="77c1e-177">Aktivieren Sie alle verbleibenden Flows.</span><span class="sxs-lookup"><span data-stu-id="77c1e-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="77c1e-178">E.</span><span class="sxs-lookup"><span data-stu-id="77c1e-178">E.</span></span> <span data-ttu-id="77c1e-179">Wählen Sie unter Flow Partner Center Webhookregistrierung die Option **Ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="77c1e-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="77c1e-180">Geben Sie die **HTTP-URL** aus der ersten Aktion in Partner Center salesforce flow **an.**</span><span class="sxs-lookup"><span data-stu-id="77c1e-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="77c1e-181">Wählen Sie unter **Zu registrierende Ereignisse** alle vier Optionen aus, und wählen Sie für Überschreiben die Option **Ja** aus.</span><span class="sxs-lookup"><span data-stu-id="77c1e-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="77c1e-182">Fragen und Antworten zu Ausführung/Wartung</span><span class="sxs-lookup"><span data-stu-id="77c1e-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="77c1e-183">Wie beheben Sie Fehler während Power Automate Flowausführung?</span><span class="sxs-lookup"><span data-stu-id="77c1e-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="77c1e-184">Um sicherzustellen, dass Ihre Power Automate Flows erwartungsvoll ausgeführt werden und Fehler während der Ausführung behoben werden können, lesen Sie [Beheben von Flowfehlern.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="77c1e-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="77c1e-185">Was sollten Sie tun, wenn Empfehlungen angezeigt werden, die in Partner Center- oder CRM-Umgebung nicht ordnungsgemäß synchronisiert werden?</span><span class="sxs-lookup"><span data-stu-id="77c1e-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="77c1e-186">Wählen Sie **Überwachen** aus, um den Status der Empfehlungssynchronisierung zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisieren von Empfehlungen":::

<span data-ttu-id="77c1e-188">Stellen Sie sicher, dass die folgenden Bedingungen erfüllt sind:</span><span class="sxs-lookup"><span data-stu-id="77c1e-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="77c1e-189">Die Lösungs-ID wird im Rahmen der Verkaufschance bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="77c1e-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="77c1e-190">Der Ländercode mit zwei Buchstaben ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77c1e-190">Two letter country code is required.</span></span>

- <span data-ttu-id="77c1e-191">Wenn hilfe von Microsoft für die Verkaufschance ausgewählt ist, sind Kundenkontaktinformationen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77c1e-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="77c1e-192">Wie kann sichergestellt werden, dass eine Empfehlung bidirektional synchronisiert wird?</span><span class="sxs-lookup"><span data-stu-id="77c1e-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="77c1e-193">Führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="77c1e-193">Do the following steps:</span></span>

- <span data-ttu-id="77c1e-194">Partnerverkäufer müssen sicherstellen, dass sie die Option **Sync with Partner Center** im CRM-Abschnitt aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="77c1e-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Stellen Sie sicher, dass Synch aktiviert ist.":::

- <span data-ttu-id="77c1e-196">Verkäufer müssen umsatz- und enddatumsgemäß bereitstellen, wenn sie einen Lead qualifizieren.</span><span class="sxs-lookup"><span data-stu-id="77c1e-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="77c1e-197">Wenn die CRM-ID  in  der Erstellungs- oder Aktualisierungsphase der Co-Sell-Verkaufschance angegeben wird, aber eine Leadchance mit dieser ID in CRM nicht gefunden wird, wird das Aktualisieren oder Erstellen ignoriert.</span><span class="sxs-lookup"><span data-stu-id="77c1e-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="77c1e-198">Stellen Sie sicher, dass das Feld für die Empfehlungswährung in der Salesforce-Umgebung konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="77c1e-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="77c1e-199">Was sollten Sie tun, wenn der Connector getrennt wird und Sie eine Empfehlungssynchronisierung verpasst haben?</span><span class="sxs-lookup"><span data-stu-id="77c1e-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="77c1e-200">Im Folgenden finden Sie einige der Optionen, die Sie ausprobieren können:</span><span class="sxs-lookup"><span data-stu-id="77c1e-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="77c1e-201">Überprüfen Sie, ob der Benutzername oder das Kennwort für den Partner Center Benutzer mit Administratorrollen für Empfehlungen abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="77c1e-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="77c1e-202">Sie können zur nicht synchronisierten Verkaufschance wechseln, ein kleineres Update machen und beobachten, ob die Empfehlung synchronisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="77c1e-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="77c1e-203">Wenn die Flows ausgeführt wurden und fehlgeschlagen sind, wählen Sie den Flow aus, und übermitteln Sie die fehlgeschlagene Ausführung erneut.</span><span class="sxs-lookup"><span data-stu-id="77c1e-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="77c1e-204">Was sollten Sie tun, wenn Sie Zugriffsfehler erhalten?</span><span class="sxs-lookup"><span data-stu-id="77c1e-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="77c1e-205">Stellen Sie sicher, dass die entsprechenden Rollen vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="77c1e-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="77c1e-206">Rolle "Empfehlungsadministrator" für Partner Center Verkäufer</span><span class="sxs-lookup"><span data-stu-id="77c1e-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="77c1e-207">Systemadministrator oder Systemanpasserrolle für Ihre CRM-Instanz</span><span class="sxs-lookup"><span data-stu-id="77c1e-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="77c1e-208">Stellen Sie sicher Power Automate dass sich der Benutzer des Kontos mindestens https://flow.microsoft.com einmal im Voraus bei anmeldet.</span><span class="sxs-lookup"><span data-stu-id="77c1e-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="77c1e-209">Wenn Sie sehen, dass **der Ländercode des** Kundenkontos beim Erstellen einer Co-Sell-Verkaufschance fehlt, was sollten Sie tun?</span><span class="sxs-lookup"><span data-stu-id="77c1e-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="77c1e-210">Sie müssen dem Kundenkonto in CRM den zwei buchstabenbasierten ISO-Ländercode hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="77c1e-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="77c1e-211">Was sollten Sie tun, wenn der Fehler angezeigt wird, dass die **Lösungs-ID** beim Erstellen einer Co-Sell-Verkaufschance erforderlich ist?</span><span class="sxs-lookup"><span data-stu-id="77c1e-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="77c1e-212">Um eine Co-Sell-Empfehlung zu erstellen, benötigen Sie eine Microsoft-Lösung, die für den Co-Sell bereit ist.</span><span class="sxs-lookup"><span data-stu-id="77c1e-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="77c1e-213">Was sollten Sie tun, wenn in Partner Center Co-Sell-Verkaufschancen entstehen, die nicht mit CRM synchronisiert werden, obwohl keine Flowfehler auftreten?</span><span class="sxs-lookup"><span data-stu-id="77c1e-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="77c1e-214">Gehen Sie folgendermaßen vor:</span><span class="sxs-lookup"><span data-stu-id="77c1e-214">Do the following:</span></span>

- <span data-ttu-id="77c1e-215">Nachdem Sie in Partner Center einen neuen Co-Sell-Deal erstellt haben, überprüfen Sie, ob der Flow Partner Center zu Dynamics 365 aufgerufen wird (er wird möglicherweise mehrmals aufgerufen).</span><span class="sxs-lookup"><span data-stu-id="77c1e-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="77c1e-216">Wenn der Flow aufgerufen wird, überprüfen Sie alle aufgerufenen Flows, und identifizieren Sie die Flow-Ausführung, die das CRM aktualisieren würde.</span><span class="sxs-lookup"><span data-stu-id="77c1e-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="77c1e-217">Sie können die Aktionen ausführen und überprüfen, ob das CRM aktualisiert wurde oder ein Problem aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="77c1e-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="77c1e-218">Überprüfen **Sie in der** Partner Center, ob er mit der CRM-ID aufgefüllt wird.</span><span class="sxs-lookup"><span data-stu-id="77c1e-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="77c1e-219">Stellen Sie sicher, dass der Deal nicht versehentlich als **Won** oder **Lost** in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="77c1e-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="77c1e-220">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="77c1e-220">Next steps</span></span>

- [<span data-ttu-id="77c1e-221">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="77c1e-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="77c1e-222">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="77c1e-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
