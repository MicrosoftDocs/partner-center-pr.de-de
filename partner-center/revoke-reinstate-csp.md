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
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855419"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="6e680-103">Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden</span><span class="sxs-lookup"><span data-stu-id="6e680-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="6e680-104">**Geeignete Rollen**: Globaler Administrator | Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="6e680-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="6e680-105">Als CSP-Partner erwarten Ihre Kunden häufig, dass Sie deren Azure-Nutzung und ihre Systeme für sie verwalten.</span><span class="sxs-lookup"><span data-stu-id="6e680-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="6e680-106">Hierfür müssen Sie über Administratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="6e680-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="6e680-107">Einige Rechte werden Ihnen beim Einrichten der Vertriebspartnerschaft mit dem Kunden gewährt.</span><span class="sxs-lookup"><span data-stu-id="6e680-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="6e680-108">Andere werden Ihnen vom Kunden erteilt.</span><span class="sxs-lookup"><span data-stu-id="6e680-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="6e680-109">Administratorrechte für Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="6e680-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="6e680-110">Es gibt zwei Ebenen von Administratorrechten für Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="6e680-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="6e680-111">**Administratorrechte auf Mandantenebene** (**Delegierte Administratorrechte**) – CSP-Partner erhalten diese Rechte beim Einrichten der CSP-Vertriebspartnerschaft mit Kunden.</span><span class="sxs-lookup"><span data-stu-id="6e680-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="6e680-112">Durch delegierte Administratorrechte erhalten CSP-Partner Zugriff auf die Mandanten der Kunden, um administrative Funktionen wie das Hinzufügen/Verwalten von Benutzern, das Zurücksetzen von Kennwörtern und das Verwalten von Benutzerlizenzen durchführen zu können.</span><span class="sxs-lookup"><span data-stu-id="6e680-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="6e680-113">**Administratorrechte auf Abonnementebene** – CSP-Partner erhalten diese Rechte beim Erstellen von Azure CSP-Abonnements für ihre Kunden.</span><span class="sxs-lookup"><span data-stu-id="6e680-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="6e680-114">Mit diesen Rechten haben CSP-Partner vollen Zugriff auf diese Abonnements, um Azure-Ressourcen bereitstellen und verwalten zu können.</span><span class="sxs-lookup"><span data-stu-id="6e680-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="6e680-115">Reaktivieren von Administratorrechten für CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="6e680-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="6e680-116">Ihr Kunde kann die CSP-Rollenzuweisung neu erstellen, sofern Sie ihm die Objekt-ID der Administrator-Agents-Gruppe bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="6e680-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="6e680-117">Um die delegierten Administratorrechte zu reaktivieren, müssen Sie mit Ihrem Kunden zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="6e680-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="6e680-118">Melden Sie sich beim Partner Center-Dashboard an, und wählen Sie im Partner Center-Menü **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="6e680-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="6e680-119">Wählen Sie den Kunden aus, mit dem Sie arbeiten, und **beantragen Sie eine Vertriebspartnerschaft**.</span><span class="sxs-lookup"><span data-stu-id="6e680-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="6e680-120">Durch diese Aktion wird ein Link zum Kunden mit Mandantenadministratorrechten generiert.</span><span class="sxs-lookup"><span data-stu-id="6e680-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="6e680-121">Dieser Kunde muss den Link auswählen und den Antrag auf Vertriebspartnerschaft genehmigen.</span><span class="sxs-lookup"><span data-stu-id="6e680-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-Mail-Beispiel für das Erstellen einer Vertriebspartnerschaft":::

4. <span data-ttu-id="6e680-123">Sie als Partner müssen eine Verbindung mit dem Partnermandanten herstellen, um die Objekt-ID der Administrator-Agents-Gruppe zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="6e680-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="6e680-124">Ihr Kunde, der die Rolle **Besitzer oder Benutzerzugriffsadministrator** hat und über die Berechtigung zum Erstellen einer Rollenzuweisung auf Abonnementebene verfügt, führt folgende Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="6e680-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="6e680-125">Er stellt eine Verbindung mit dem Mandanten mit dem CSP-Abonnement her.</span><span class="sxs-lookup"><span data-stu-id="6e680-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="6e680-126">Er stellt eine Verbindung mit dem Abonnement her (trifft nur zu, wenn der Benutzer über Rollenzuweisungsberechtigungen für mehrere Abonnements im Mandanten verfügt).</span><span class="sxs-lookup"><span data-stu-id="6e680-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="6e680-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="6e680-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="6e680-128">Er erstellt die Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="6e680-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="6e680-129">Wenn Sie die Besitzerrollenberechtigung auf Ressourcengruppen- oder Ressourcenebene statt auf Abonnementebene erteilen möchten, können Sie die folgenden Befehle verwenden:</span><span class="sxs-lookup"><span data-stu-id="6e680-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="6e680-130">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="6e680-130">Next steps</span></span>

- [<span data-ttu-id="6e680-131">Verwalten von Abonnements und Ressourcen in einem Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="6e680-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
