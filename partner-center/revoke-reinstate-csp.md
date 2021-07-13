---
title: Wiederherstellen von Administratorrechten für Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Kunden dabei helfen können, die Administratorrechte eines Partners wiederherzustellen, damit der Partner dabei helfen kann die Azure CSP-Abonnements eines Kunden zu verwalten.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510175"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="2702f-103">Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden</span><span class="sxs-lookup"><span data-stu-id="2702f-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="2702f-104">**Geeignete Rollen**: Globaler Administrator | Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="2702f-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="2702f-105">Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und Systeme für sie verwalten.</span><span class="sxs-lookup"><span data-stu-id="2702f-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="2702f-106">Dazu benötigen Sie Administratorrechte.</span><span class="sxs-lookup"><span data-stu-id="2702f-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="2702f-107">Einige Rechte werden Ihnen beim Einrichten der Vertriebspartnerschaft mit dem Kunden gewährt.</span><span class="sxs-lookup"><span data-stu-id="2702f-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="2702f-108">Andere werden Ihnen vom Kunden erteilt.</span><span class="sxs-lookup"><span data-stu-id="2702f-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="2702f-109">Administratorrechte für Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="2702f-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="2702f-110">Es gibt zwei Ebenen von Administratorrechten für Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="2702f-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="2702f-111">**Administratorrechte auf Mandantenebene (Delegierte Administratorrechte)** : CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden.</span><span class="sxs-lookup"><span data-stu-id="2702f-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="2702f-112">Delegierte Administratorrechte ermöglichen CSP-Partnern Zugriff auf die Mandanten ihrer Kunden.</span><span class="sxs-lookup"><span data-stu-id="2702f-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="2702f-113">Mit diesem Zugriff können sie administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Passwörtern und die Verwaltung von Benutzerlizenzen durchführen.</span><span class="sxs-lookup"><span data-stu-id="2702f-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="2702f-114">**Administratorrechte auf Abonnementebene**: CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden.</span><span class="sxs-lookup"><span data-stu-id="2702f-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="2702f-115">Mit diesen Rechten haben CSP-Partner vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können.</span><span class="sxs-lookup"><span data-stu-id="2702f-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="2702f-116">Wiederherstellen der Administratorenrechte von CSP-Partnern</span><span class="sxs-lookup"><span data-stu-id="2702f-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="2702f-117">Ihr Kunde kann die CSP-Rollenzuweisung neu erstellen, sofern Sie ihm die `object ID` der Administrator-Agenten-Gruppe bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="2702f-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="2702f-118">Um die delegierten Administratorrechte wiederzuerlangen, müssen Sie mit Ihrem Kunden die folgenden Schritte durchführen.</span><span class="sxs-lookup"><span data-stu-id="2702f-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="2702f-119">Melde dich beim Partner Center-Dashboard an.</span><span class="sxs-lookup"><span data-stu-id="2702f-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="2702f-120">Wählen Sie im Menü „Partner Center” **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="2702f-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="2702f-121">Wählen Sie den Kunden aus, mit dem Sie arbeiten und wählen Sie **Anforderung einer Vertriebspartnerschaft**.</span><span class="sxs-lookup"><span data-stu-id="2702f-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="2702f-122">Durch diese Aktion wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.</span><span class="sxs-lookup"><span data-stu-id="2702f-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="2702f-123">Ihr Kunde muss den Link auswählen und die Anforderung auf eine Vertriebspartnerschaft genehmigen.</span><span class="sxs-lookup"><span data-stu-id="2702f-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-Mail-Beispiel für das Erstellen einer Vertriebspartnerschaft.":::

5. <span data-ttu-id="2702f-125">Sie als Partner müssen eine Verbindung mit dem Partnermandanten herstellen, um die Objekt-ID der Administrator-Agents-Gruppe zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="2702f-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="2702f-126">Ihr Kunde muss dann die folgenden Schritte entweder mithilfe von PowerShell oder mit Azure CLI durchführen.</span><span class="sxs-lookup"><span data-stu-id="2702f-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="2702f-127">Ihr Kunde muss über Folgendes verfügen:</span><span class="sxs-lookup"><span data-stu-id="2702f-127">Your customer must have:</span></span>

- <span data-ttu-id="2702f-128">Rolle des **Besitzers** oder die des **Benutzerzugriffsadministrators**</span><span class="sxs-lookup"><span data-stu-id="2702f-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="2702f-129">Berechtigungen zum Erstellen von Rollenzuweisungen auf Abonnementebene</span><span class="sxs-lookup"><span data-stu-id="2702f-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="2702f-130">a.</span><span class="sxs-lookup"><span data-stu-id="2702f-130">a.</span></span> <span data-ttu-id="2702f-131">Der Kunde muss nur für PowerShell das Modul `Az.Resources` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2702f-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="2702f-132">b.</span><span class="sxs-lookup"><span data-stu-id="2702f-132">b.</span></span> <span data-ttu-id="2702f-133">Der Kunde stellt eine Verbindung mit dem Mandanten her, in dem das CSP-Abonnement besteht.</span><span class="sxs-lookup"><span data-stu-id="2702f-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="2702f-134">c.</span><span class="sxs-lookup"><span data-stu-id="2702f-134">c.</span></span> <span data-ttu-id="2702f-135">Der Kunde stellt eine Verbindung mit dem Abonnement her.</span><span class="sxs-lookup"><span data-stu-id="2702f-135">The customer connects to the subscription.</span></span> <span data-ttu-id="2702f-136">Das ist *nur* anwendbar, wenn der Benutzer über Rollenzuweisungsberechtigungen für mehrere Abonnements im Mandanten verfügt.</span><span class="sxs-lookup"><span data-stu-id="2702f-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="2702f-137">d.</span><span class="sxs-lookup"><span data-stu-id="2702f-137">d.</span></span> <span data-ttu-id="2702f-138">Der Kunde erstellt dann die Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="2702f-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="2702f-139">Anstatt Besitzerberechtigungen im Abonnementbereich zu erteilen, können Sie auf Ressourcengruppen oder Ressourcenebene erteilen.</span><span class="sxs-lookup"><span data-stu-id="2702f-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="2702f-140">Auf Ressourcengruppenebene</span><span class="sxs-lookup"><span data-stu-id="2702f-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="2702f-141">Auf Ressourcenebene</span><span class="sxs-lookup"><span data-stu-id="2702f-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="2702f-142">Wenn die oben genannten Schritte nicht funktionieren oder beim Versuch Fehler auftreten, versuchen Sie, die folgenden „Auffangverfahren“ zu verwenden, um Administratorrechte für Ihren Kunden wiederherzustellen.</span><span class="sxs-lookup"><span data-stu-id="2702f-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="2702f-143">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="2702f-143">Troubleshooting</span></span>

<span data-ttu-id="2702f-144">Wenn der Kunde Schritt 6 oben nicht ausführen kann, lassen Sie es den Kunden mit dem folgenden Befehl versuchen:</span><span class="sxs-lookup"><span data-stu-id="2702f-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="2702f-145">Stellen Sie die resultierende `newRoleAssignment.log` Datei für Microsoft zur weiteren Analyse zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="2702f-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="2702f-146">Wenn das „Auffangverfahren“ während `Import-Module` fehlschlägt, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="2702f-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="2702f-147">Wenn beim Import ein Fehler auftritt, weil das Modul verwendet wird, starten Sie die PowerShell-Sitzung neu, indem Sie alle Fenster schließen und erneut öffnen.</span><span class="sxs-lookup"><span data-stu-id="2702f-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="2702f-148">Überprüfen Sie die Version von `Az.Resources` mit `Get-Module Az.Resources -ListAvailable`.</span><span class="sxs-lookup"><span data-stu-id="2702f-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="2702f-149">Wenn die Version 4.1.1 nicht in der Liste der verfügbaren Versionen enthalten ist, müssen Sie `Update-Module Az.Resources -Force` verwenden.</span><span class="sxs-lookup"><span data-stu-id="2702f-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="2702f-150">Wenn der Fehler besagt, dass `Az.Accounts` eine bestimmte Version benötigt, aktualisieren Sie auch dieses Modul, und ersetzen Sie `Az.Resources` durch `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="2702f-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="2702f-151">Anschließend müssen Sie die PowerShell-Sitzung neu starten.</span><span class="sxs-lookup"><span data-stu-id="2702f-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="2702f-152">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2702f-152">Next steps</span></span>

- [<span data-ttu-id="2702f-153">Verwalten von Abonnements und Ressourcen in einem Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="2702f-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
