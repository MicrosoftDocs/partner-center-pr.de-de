---
title: Wiederherstellen von Administratorrechten für Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Kunden dabei helfen können, die Administratorrechte eines Partners wiederherzustellen, damit der Partner die Azure CSP-Abonnements eines Kunden verwalten kann.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018186"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="8d694-103">Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden</span><span class="sxs-lookup"><span data-stu-id="8d694-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="8d694-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="8d694-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8d694-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8d694-105">Global admin</span></span>
- <span data-ttu-id="8d694-106">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="8d694-106">Admin agent</span></span>

<span data-ttu-id="8d694-107">Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und ihre Systeme für sie verwalten.</span><span class="sxs-lookup"><span data-stu-id="8d694-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="8d694-108">Hierfür müssen Sie über Administratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="8d694-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="8d694-109">Einige Rechte werden Ihnen beim Einrichten der Vertriebspartnerschaft mit dem Kunden gewährt.</span><span class="sxs-lookup"><span data-stu-id="8d694-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="8d694-110">Andere werden Ihnen vom Kunden erteilt.</span><span class="sxs-lookup"><span data-stu-id="8d694-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="8d694-111">Administratorrechte für Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="8d694-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="8d694-112">Es gibt zwei Ebenen von Administratorrechten für Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="8d694-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="8d694-113">**Administratorrechte auf Mandantenebene** (**Delegierte Administratorrechte**) – CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden.</span><span class="sxs-lookup"><span data-stu-id="8d694-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="8d694-114">Durch delegierte Administratorrechte erhalten CSP-Partner Zugriff auf die Mandanten der Kunden, um administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Kennwörtern und das Verwalten von Benutzerlizenzen durchführen zu können.</span><span class="sxs-lookup"><span data-stu-id="8d694-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="8d694-115">**Administratorrechte auf Abonnementebene** – CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden.</span><span class="sxs-lookup"><span data-stu-id="8d694-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="8d694-116">Mit diesen Rechten haben CSP-Partner vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können.</span><span class="sxs-lookup"><span data-stu-id="8d694-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="8d694-117">Reaktivieren von Administratorrechten für CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="8d694-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="8d694-118">Ihr Kunde kann die CSP-Rollenzuweisung neu erstellen, sofern Sie ihm die Objekt-ID der Administrator-Agents-Gruppe bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="8d694-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="8d694-119">Um die delegierten Administratorrechte zu reaktivieren, müssen Sie mit Ihrem Kunden zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="8d694-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="8d694-120">Melden Sie sich beim Partner Center-Dashboard an, und wählen Sie im Partner Center-Menü **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="8d694-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="8d694-121">Wählen Sie den Kunden aus, mit dem Sie arbeiten, und **beantragen Sie eine Vertriebspartnerschaft**.</span><span class="sxs-lookup"><span data-stu-id="8d694-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="8d694-122">Durch diese Aktion wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.</span><span class="sxs-lookup"><span data-stu-id="8d694-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="8d694-123">Dieser Kunde muss den Link auswählen und den Antrag auf Vertriebspartnerschaft genehmigen.</span><span class="sxs-lookup"><span data-stu-id="8d694-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-Mail-Beispiel für das Erstellen einer Vertriebspartnerschaft":::

4. <span data-ttu-id="8d694-125">Sie als Partner müssen eine Verbindung mit dem Partnermandanten herstellen, um die Objekt-ID der Administrator-Agents-Gruppe zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="8d694-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="8d694-126">Ihr Kunde, der die Rolle **Besitzer oder Benutzerzugriffsadministrator** hat und über die Berechtigung zum Erstellen einer Rollenzuweisung auf Abonnementebene verfügt, führt folgende Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="8d694-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="8d694-127">Er stellt eine Verbindung mit dem Mandanten mit dem CSP-Abonnement her.</span><span class="sxs-lookup"><span data-stu-id="8d694-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="8d694-128">Er stellt eine Verbindung mit dem Abonnement her (trifft nur zu, wenn der Benutzer über Rollenzuweisungsberechtigungen für mehrere Abonnements im Mandanten verfügt).</span><span class="sxs-lookup"><span data-stu-id="8d694-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="8d694-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="8d694-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="8d694-130">Er erstellt die Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="8d694-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="8d694-131">Wenn Sie die Besitzerrollenberechtigung auf Ressourcengruppen- oder Ressourcenebene statt auf Abonnementebene erteilen möchten, können Sie die folgenden Befehle verwenden:</span><span class="sxs-lookup"><span data-stu-id="8d694-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="8d694-132">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="8d694-132">Next steps</span></span>

- [<span data-ttu-id="8d694-133">Verwalten von Abonnements und Ressourcen in einem Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="8d694-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
