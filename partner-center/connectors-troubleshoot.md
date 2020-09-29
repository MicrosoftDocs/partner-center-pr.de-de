---
title: Problembehandlung bei Connectors mit Co-Selling-Empfehlungen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Häufig gestellte Fragen zur Problembehandlung bei Co-Selling-Connectors.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: d34a13a6789f3bd712d2cec3a594b8e407f7449d
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422336"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="99f8e-103">Problembehandlung bei Connectors mit Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="99f8e-103">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="99f8e-104">**Gilt für:**</span><span class="sxs-lookup"><span data-stu-id="99f8e-104">**Applies to:**</span></span>

- <span data-ttu-id="99f8e-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="99f8e-105">Partner Center</span></span>
- <span data-ttu-id="99f8e-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="99f8e-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="99f8e-107">Salesforce-CRM</span><span class="sxs-lookup"><span data-stu-id="99f8e-107">Salesforce CRM</span></span>

<span data-ttu-id="99f8e-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="99f8e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="99f8e-109">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="99f8e-109">Referrals admin</span></span>
- <span data-ttu-id="99f8e-110">Systemadministrator oder systemanpassungsprogramm im CRM</span><span class="sxs-lookup"><span data-stu-id="99f8e-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="99f8e-111">Fragen und Antworten zu Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="99f8e-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="99f8e-112">Können Sie für Ihre Umgebung eine "Test-Co-Selling-Connectors"-Lösung verwenden?</span><span class="sxs-lookup"><span data-stu-id="99f8e-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="99f8e-113">Wenn Sie sich in der Test-/Stagingumgebung befinden, können Sie sich für eine Testlösung entscheiden.</span><span class="sxs-lookup"><span data-stu-id="99f8e-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="99f8e-114">Die kostenpflichtige Version der Connectors ist in appsource in US-Dollar 15 USD/Monat verfügbar.</span><span class="sxs-lookup"><span data-stu-id="99f8e-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="99f8e-115">Mit der kostenpflichtigen Verbindung erhalten Sie pro Tag 10K API-Aufrufe.</span><span class="sxs-lookup"><span data-stu-id="99f8e-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="99f8e-116">Die Connectors sind Wrapper zusätzlich zu den Partner Center-Referenz-APIs.</span><span class="sxs-lookup"><span data-stu-id="99f8e-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="99f8e-117">Wenn die Connector-Lösungen für ein Erstellungs-oder **Update** Ereignis für die Verkaufschancen in Partner Center oder auf der CRM-Seite ausgeführt werden, **erfolgt ein API** -Aufruf.</span><span class="sxs-lookup"><span data-stu-id="99f8e-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="99f8e-118">Welche Rolle benötigen Sie, um Abschnitte in der CRM-Umgebung zu erstellen?</span><span class="sxs-lookup"><span data-stu-id="99f8e-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="99f8e-119">Benutzer, die Systemadministratoren oder Systemanpassungen sind, können Änderungen für jeden Benutzer anwenden.</span><span class="sxs-lookup"><span data-stu-id="99f8e-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="99f8e-120">Alle App-Benutzer können das System jedoch personalisieren und sogar einige Ihrer Anpassungen mit anderen Teilen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="99f8e-121">Benötigen Partner Verkäufer spezielle Rollen, um im Partner Center arbeiten zu können?</span><span class="sxs-lookup"><span data-stu-id="99f8e-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="99f8e-122">Partner Verkäufern muss die Rolle "referenrals admin" zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="99f8e-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="99f8e-123">Weitere Informationen finden Sie in der folgenden [Berechtigungs Übersicht) (Create-User-Accounts-and-Set--Berechtigungen).</span><span class="sxs-lookup"><span data-stu-id="99f8e-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="99f8e-124">Welche Felder müssen zuerst in Ihrer CRM-Umgebung eingerichtet werden?</span><span class="sxs-lookup"><span data-stu-id="99f8e-124">What are the fields that need to be set-up first in your CRM environment?</span></span> 

<span data-ttu-id="99f8e-125">• Stellen Sie sicher, dass Ihre Währung für Ihren Standort geeignet ist und sich in Ihrer CRM-Umgebung genau befindet.</span><span class="sxs-lookup"><span data-stu-id="99f8e-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="99f8e-126">• Ihr Vertriebsteam sollte in Ihrer CRM-Umgebung als CRM-Benutzer aufgeführt sein.</span><span class="sxs-lookup"><span data-stu-id="99f8e-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5.  <span data-ttu-id="99f8e-127">Welche Voraussetzungen sind für das Erstellen der Energie automatisierten Umgebung erforderlich?</span><span class="sxs-lookup"><span data-stu-id="99f8e-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="99f8e-128">Um die Energie automatisierte Umgebung zu verwenden, benötigen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="99f8e-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="99f8e-129">Eine Strom Automatisierungs Lizenz ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99f8e-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="99f8e-130">Es ist mindestens 1 GB Speicher erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99f8e-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="99f8e-131">Benötigen Sie ein Dynamics 365-Abonnement, um die Salesforce-Connectors-Lösung zu verwenden?</span><span class="sxs-lookup"><span data-stu-id="99f8e-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="99f8e-132">Die Salesforce-Connector-Lösung ist vom Typ "Dynamics Flow", der die Synchronisierung mit anderen CRM-Systemen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99f8e-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="99f8e-133">Die Lösung erfordert nicht, dass Sie über eine Dynamics 365-Instanz oder ein-Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="99f8e-134">Beim Installieren der Salesforce-Lösung wird möglicherweise eine Dropdown-Datei mit vorhandener CDs-Umgebung in Ihrem Unternehmen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="99f8e-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="99f8e-135">Sie müssen diese Umgebung auswählen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-135">You need to select that environment.</span></span> <span data-ttu-id="99f8e-136">Wenn Sie die Fehlermeldung erhalten, dass eine Dynamics 365-Organisation, die mit dem angemeldeten Benutzer verbunden ist, nicht gefunden werden können, müssen Sie außerdem eine neue Umgebung für den Connector erstellen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-136">In addition, if you get the error we couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="99f8e-137">Fragen und Antworten zur Konfiguration</span><span class="sxs-lookup"><span data-stu-id="99f8e-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="99f8e-138">Was sollten Sie tun, wenn beim Aktivieren von Flows in der Energie automatisierten Plattform der folgende Fehler auftritt?</span><span class="sxs-lookup"><span data-stu-id="99f8e-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="99f8e-139">Fehler: die Anforderung zum Azure Resource Manager ist mit dem folgenden Fehler fehlgeschlagen: "{" Error ": {" Code ":" workflowtriggernotfound "," Message ":" der Workflow "e14d00f1-1fdf-4b1b-aaac-54a5064093d3"-Trigger "Manual" konnte nicht gefunden werden. "}}".</span><span class="sxs-lookup"><span data-stu-id="99f8e-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="99f8e-140">Befolgen Sie diese Schritte zur Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="99f8e-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="99f8e-141">Löschen Sie die CDs-Verbindung, und erstellen Sie dann die CDs-Verbindungen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="99f8e-142">Aktivieren und Deaktivieren des untergeordneten Flows</span><span class="sxs-lookup"><span data-stu-id="99f8e-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="99f8e-143">Löschen Sie die Lösung, und installieren Sie die Projekt Mappe neu.</span><span class="sxs-lookup"><span data-stu-id="99f8e-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="99f8e-144">Was sollten Sie tun, wenn beim Hinzufügen eines Partner Center-Connector in der Energie automatisierten Plattform der folgende Fehler auftritt?</span><span class="sxs-lookup"><span data-stu-id="99f8e-144">What should you do if you face the following error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fehlermeldung, die eine Anmeldung erfordert":::

<span data-ttu-id="99f8e-146">Befolgen Sie diese Schritte zur Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="99f8e-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="99f8e-147">Verwenden Sie die Partner Center-Anmeldung, um sich einmal bei der Flow-Umgebung anzumelden (Flow.Microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="99f8e-147">Use the Partner Center sign-in to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="99f8e-148">Was sollten Sie tun, wenn Sie den folgenden Fehler erhalten, während Sie den Partner Center für CRM-Flow in der Energie automatisierten Plattform aktivieren?</span><span class="sxs-lookup"><span data-stu-id="99f8e-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fehlermeldung, die Updates erfordert":::

<span data-ttu-id="99f8e-150">Befolgen Sie diese Schritte zur Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="99f8e-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="99f8e-151">Aktivieren Sie zuerst die folgenden beiden untergeordneten Flows, bevor Sie das Partner Center für CRM Flow aktivieren.</span><span class="sxs-lookup"><span data-stu-id="99f8e-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="99f8e-152">Partner Center auf CRM-Hilfsobjekt (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="99f8e-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="99f8e-153">Partner Center Microsoft Co-Selling-Verweises Aktualisierungen an CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="99f8e-154">Was sollten Sie tun, wenn Sie keine Verbindungen zum Flow hinzufügen können, wenn Sie versuchen, den Flow zu bearbeiten?</span><span class="sxs-lookup"><span data-stu-id="99f8e-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="99f8e-155">Wenn der Flow ausgeführt wird, fügen Sie Verbindungen zum Flow hinzu, und Sie fügen den einzelnen Flows separat hinzu.</span><span class="sxs-lookup"><span data-stu-id="99f8e-155">You add connections to the flow while the flow is running and you add to each flow separately.</span></span>  <span data-ttu-id="99f8e-156">Wenn das Dialogfeld zum Hinzufügen von Verbindungen beim Bearbeiten des Flows nicht automatisch geöffnet wird, können Sie die einzelnen Schritte und unter Schritte der Flows bearbeiten, um die Verbindungen hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and substeps of the flows to add the connections.</span></span>

- <span data-ttu-id="99f8e-157">Wählen Sie jeden Flow aus, und bearbeiten Sie ihn einzeln.</span><span class="sxs-lookup"><span data-stu-id="99f8e-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="99f8e-158">Alle Schritte im Flow erweitern</span><span class="sxs-lookup"><span data-stu-id="99f8e-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Schritte, die Verbindungen benötigen":::

- <span data-ttu-id="99f8e-160">Wählen Sie die Schritte aus, bei denen das Warnsymbol angezeigt wird, um Verbindungen zuzuordnen, und fügen Sie Verbindungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="99f8e-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Flow Schritt für Schritt bearbeiten":::


5. <span data-ttu-id="99f8e-162">Was sollten Sie tun, wenn die Flows der Connectors-Lösung für Co-Selling-Verweise nicht aktiviert (Einschalten)?</span><span class="sxs-lookup"><span data-stu-id="99f8e-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t activate (turn-on)?</span></span>

<span data-ttu-id="99f8e-163">A.</span><span class="sxs-lookup"><span data-stu-id="99f8e-163">A.</span></span> <span data-ttu-id="99f8e-164">In der Energie Automatisierung müssen Sie Flows in der folgenden Reihenfolge bearbeiten und Sie aktualisieren, um die entsprechenden Verbindungen zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="99f8e-164">In Power Automate, you will need to edit flows in the following order and update them to use respective connections:</span></span>

- <span data-ttu-id="99f8e-165">Partner Center-webhook-Registrierung (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="99f8e-166">Erstellen eines Co-Selling-Verweises-Salesforce an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="99f8e-167">Partner Center Microsoft Co-Selling-Referenz Aktualisierungen an Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="99f8e-168">Partner Center zu Salesforce (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="99f8e-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="99f8e-169">Salesforce zu Partner Center (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="99f8e-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="99f8e-170">Salesforce-Verkaufschance an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="99f8e-171">Salesforce Microsoft-Lösungen an Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="99f8e-172">B.</span><span class="sxs-lookup"><span data-stu-id="99f8e-172">B.</span></span> <span data-ttu-id="99f8e-173">Wählen Sie für jeden Flow die Option **nur Benutzer ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="99f8e-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="99f8e-174">Wählen Sie **Verbindung verwenden** anstelle von **nur Benutzer ohne Benutzer bereit**stellen aus.</span><span class="sxs-lookup"><span data-stu-id="99f8e-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="So aktivieren Sie einen Flow":::


<span data-ttu-id="99f8e-176">C.</span><span class="sxs-lookup"><span data-stu-id="99f8e-176">C.</span></span> <span data-ttu-id="99f8e-177">Aktivieren Sie die folgenden genannten Flows:</span><span class="sxs-lookup"><span data-stu-id="99f8e-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="99f8e-178">Partner Center Microsoft Co-Selling-Referenz Aktualisierungen an Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="99f8e-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="99f8e-179">Salesforce zu Partner Center (Insider Vorschau)</span><span class="sxs-lookup"><span data-stu-id="99f8e-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="99f8e-180">D:</span><span class="sxs-lookup"><span data-stu-id="99f8e-180">D.</span></span> <span data-ttu-id="99f8e-181">Aktivieren Sie alle verbleibenden Flows.</span><span class="sxs-lookup"><span data-stu-id="99f8e-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="99f8e-182">E.</span><span class="sxs-lookup"><span data-stu-id="99f8e-182">E.</span></span> <span data-ttu-id="99f8e-183">Wählen Sie unter Flow Partner Center-webhook-Registrierung die Option **Ausführen**aus.</span><span class="sxs-lookup"><span data-stu-id="99f8e-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="99f8e-184">Geben Sie die **http-URL** aus der ersten Aktion im **Partner Center für den Salesforce** -Flow an.</span><span class="sxs-lookup"><span data-stu-id="99f8e-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="99f8e-185">Wählen Sie unter **zu registrierende Ereignisse** alle vier Optionen aus, und wählen Sie zum Überschreiben **Ja**</span><span class="sxs-lookup"><span data-stu-id="99f8e-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="99f8e-186">Fragen und Antworten zur Wartung und Wartung</span><span class="sxs-lookup"><span data-stu-id="99f8e-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="99f8e-187">Wie werden Probleme bei Fehlern während der Energie automatisierten Fluss Ausführung behoben?</span><span class="sxs-lookup"><span data-stu-id="99f8e-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="99f8e-188">Um sicherzustellen, dass Ihre Energie automatisierenden Flows erwartungsgemäß ausgeführt werden und Fehler während der Ausführung behoben werden können, finden Sie unter [Beheben von Fluss Fehlern](/power-automate/fix-flow-failures)Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="99f8e-189">Was sollten Sie tun, wenn Verweise angezeigt werden, die nicht ordnungsgemäß in der Partner Center-oder CRM-Umgebung synchronisiert sind?</span><span class="sxs-lookup"><span data-stu-id="99f8e-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="99f8e-190">**Wählen Sie**überwachen aus, um den Status der Verweis Synchronisierung zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisieren von verweisen":::

<span data-ttu-id="99f8e-192">Stellen Sie sicher, dass die folgenden Bedingungen erfüllt sind:</span><span class="sxs-lookup"><span data-stu-id="99f8e-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="99f8e-193">Die Lösungs-ID wird als Teil der Verkaufschance bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="99f8e-193">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="99f8e-194">Zwei buchstabiger Ländercode ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99f8e-194">Two letter country code is required.</span></span>

- <span data-ttu-id="99f8e-195">Wenn die Hilfe von Microsoft für die Verkaufschance ausgewählt ist, sind Kundenkontaktinformationen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99f8e-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="99f8e-196">Unter welchen Bedingungen wird ein Verweis nicht bidirektional synchronisiert</span><span class="sxs-lookup"><span data-stu-id="99f8e-196">Under what conditions a referral won’t synchronize bi-directionally</span></span>

<span data-ttu-id="99f8e-197">Stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="99f8e-197">Ensure the following:</span></span>

- <span data-ttu-id="99f8e-198">Partner Verkäufer müssen sicherstellen, dass die **Synchronisierung mit der Partner Center** -Option im CRM-Abschnitt aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="99f8e-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Stellen Sie sicher, dass die Synchronisierung aktiviert ist":::

- <span data-ttu-id="99f8e-200">Verkäufer müssen den Umsatz und das Enddatum angeben, wenn Sie einen Lead qualifizieren.</span><span class="sxs-lookup"><span data-stu-id="99f8e-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="99f8e-201">Wenn die CRM-ID in der Erstellung oder dem Update der Co-Selling-Verkaufschance bereitgestellt wird und ein Lead/eine Gelegenheit mit dieser ID in CRM nicht gefunden wird, wird Update oder CREATE für diese Gelegenheit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="99f8e-201">If CRM id is provided in create or update of co-sell opportunity and if a lead/opportunity with that id is not found in CRM, then update or create will be ignored for that opportunity.</span></span>

- <span data-ttu-id="99f8e-202">Stellen Sie sicher, dass das Feld für die Verweis Währung in der Salesforce-Umgebung</span><span class="sxs-lookup"><span data-stu-id="99f8e-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="99f8e-203">Was Sie tun sollten, wenn der Connector getrennt wird und eine verweissynchronisierung fehlt.</span><span class="sxs-lookup"><span data-stu-id="99f8e-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="99f8e-204">Im folgenden sind einige der Optionen aufgeführt, die Sie ausprobieren können:</span><span class="sxs-lookup"><span data-stu-id="99f8e-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="99f8e-205">Überprüfen Sie, ob der Benutzername oder das Kennwort für den Partner Center-Benutzer mit Referenz Administrator Rollen abgelaufen ist</span><span class="sxs-lookup"><span data-stu-id="99f8e-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="99f8e-206">Sie können zur nicht synchronisierten Gelegenheit wechseln, eine geringfügige Aktualisierung vornehmen und beobachten, ob der Verweis synchronisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="99f8e-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="99f8e-207">Wenn die Flows ausgeführt wurden und fehlgeschlagen sind, wählen Sie den Flow aus, und übermitteln Sie den ausgefallenen Testlauf erneut.</span><span class="sxs-lookup"><span data-stu-id="99f8e-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="99f8e-208">Was sollten Sie tun, wenn Sie Zugriffs Verweigerungs Fehler erhalten?</span><span class="sxs-lookup"><span data-stu-id="99f8e-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="99f8e-209">Stellen Sie sicher, dass die entsprechenden Rollen vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="99f8e-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="99f8e-210">Rolle "Verweis Administrator" für Partner Center-Verkäufer</span><span class="sxs-lookup"><span data-stu-id="99f8e-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="99f8e-211">System Administrator-oder systemanpassungsrolle in Ihrer CRM-Instanz</span><span class="sxs-lookup"><span data-stu-id="99f8e-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="99f8e-212">Stellen Sie sicher, dass sich der Benutzer mit dem Datenfluss Konto automatisch https://flow.microsoft.com bei mindestens einmal anmeldet.</span><span class="sxs-lookup"><span data-stu-id="99f8e-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="99f8e-213">Was sollten Sie tun, wenn Sie sehen, dass der **Ländercode des Kundenkontos** beim Erstellen einer Co-Selling-Verkaufschance fehlt?</span><span class="sxs-lookup"><span data-stu-id="99f8e-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="99f8e-214">Sie müssen dem Kundenkonto in CRM den aus zwei Buchstaben bestehenden ISO-Code hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="99f8e-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="99f8e-215">Was sollten Sie tun, wenn Sie sehen, dass die **Lösungs-ID erforderlich ist** , während Sie eine Co-Selling-Verkaufschance erstellen?</span><span class="sxs-lookup"><span data-stu-id="99f8e-215">What should you do if you see the error that **Solution Id is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="99f8e-216">Um einen Co-Selling-Verweis zu erstellen, benötigen Sie eine Microsoft Co-Selling-Lösung.</span><span class="sxs-lookup"><span data-stu-id="99f8e-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="99f8e-217">Was Sie tun sollten, wenn Sie die Co-Selling-Verkaufschancen in Partner Center sehen, die nicht mit CRM synchronisiert werden, auch wenn keine Datenflussfehler auftreten:</span><span class="sxs-lookup"><span data-stu-id="99f8e-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="99f8e-218">Gehen Sie wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="99f8e-218">Do the following:</span></span>

- <span data-ttu-id="99f8e-219">Nachdem Sie im Partner Center einen neuen Co-Selling-Deal erstellt haben, überprüfen Sie, ob der Flow Partner Center auf Dynamics 365 aufgerufen wird (er wird möglicherweise mehrmals aufgerufen).</span><span class="sxs-lookup"><span data-stu-id="99f8e-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="99f8e-220">Wenn der Flow aufgerufen wird, überprüfen Sie alle aufgerufenen Flows, und identifizieren Sie die flowausführung, die das CRM aktualisieren würde.</span><span class="sxs-lookup"><span data-stu-id="99f8e-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="99f8e-221">Sie können den Aktionen folgen und überprüfen, ob das CRM-Update oder ein Problem aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="99f8e-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="99f8e-222">Überprüfen Sie den *neuen Deal*\* im Partner Center, um festzustellen, ob es mit der CRM-ID aufgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="99f8e-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM id.</span></span>

- <span data-ttu-id="99f8e-223">Stellen Sie sicher, dass das Geschäft im Partner Center nicht versehentlich als "gewonnen" oder "verloren" geschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="99f8e-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="99f8e-224">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="99f8e-224">Next steps</span></span>

- [<span data-ttu-id="99f8e-225">Verwalten von Leads</span><span class="sxs-lookup"><span data-stu-id="99f8e-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="99f8e-226">Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="99f8e-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)