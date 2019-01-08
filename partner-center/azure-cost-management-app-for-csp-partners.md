---
title: Azure Cost Management von Cloudyn für CSP-Partner | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management von Cloudyn erfordert einen Zugriff über die Partner Center-API.
author: Janet
ms.author: janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995794"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="1a48f-103">App zum Azure-Kostenmanagement für Azure CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="1a48f-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="1a48f-104">Betrifft:</span><span class="sxs-lookup"><span data-stu-id="1a48f-104">Applies to</span></span>**

-  <span data-ttu-id="1a48f-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="1a48f-105">Partner Center</span></span>

[<span data-ttu-id="1a48f-106">Weitere Informationen zu Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="1a48f-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="1a48f-107">Vorbemerkungen</span><span class="sxs-lookup"><span data-stu-id="1a48f-107">Before you begin</span></span>
<span data-ttu-id="1a48f-108">Bevor Sie Azure Cost Management verwenden können, sollten Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="1a48f-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="1a48f-109">Sie sind Partner im Cloud Solution Provider-Programm.</span><span class="sxs-lookup"><span data-stu-id="1a48f-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="1a48f-110">Sie haben die Möglichkeit, eine Partner Center-API-Web-App zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1a48f-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="1a48f-111">Übersicht</span><span class="sxs-lookup"><span data-stu-id="1a48f-111">Overview</span></span>

<span data-ttu-id="1a48f-112">Azure Cost Management von Cloudyn ist eine Web-App, mit dem Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können.</span><span class="sxs-lookup"><span data-stu-id="1a48f-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="1a48f-113">Sie können die App über die Partner Center-API nutzen.</span><span class="sxs-lookup"><span data-stu-id="1a48f-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="1a48f-114">Registrieren Ihrer Web-App im Partner Center</span><span class="sxs-lookup"><span data-stu-id="1a48f-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="1a48f-115">Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie auf die Partner Center-API zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1a48f-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="1a48f-116">Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.</span><span class="sxs-lookup"><span data-stu-id="1a48f-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="1a48f-117">Wählen Sie aus dem **Partner Center**, **kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="1a48f-117">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="1a48f-118">Klicken Sie im Abschnitt **Web-app** auf **Neue Web-App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="1a48f-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="1a48f-119">**Hinweis:**: Wenn Sie bereits zuvor eine Web-App erstellt haben, können Sie Schritt3 überspringen.</span><span class="sxs-lookup"><span data-stu-id="1a48f-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="1a48f-120">Kopieren und speichern Sie die **Commerce-ID**-GUID und die **App-ID**-GUID für Ihre Web-App.</span><span class="sxs-lookup"><span data-stu-id="1a48f-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="1a48f-121">Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.</span><span class="sxs-lookup"><span data-stu-id="1a48f-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="1a48f-122">Hinzufügen eines geheimen Schlüssels zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="1a48f-122">Add a secret key to your app</span></span>
1. <span data-ttu-id="1a48f-123">Wählen Sie in der Dropdownliste neben der **Schlüssel hinzufügen**-Schaltfläche eine Dauer von 1 oder 2Jahren aus.</span><span class="sxs-lookup"><span data-stu-id="1a48f-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="1a48f-124">Klicken Sie auf **Schlüssel hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="1a48f-124">Click **Add key**.</span></span> 
3. <span data-ttu-id="1a48f-125">Kopieren Sie und speichern Sie den Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="1a48f-125">Copy and save the secret key value.</span></span> <span data-ttu-id="1a48f-126">Sie benötigen diesen für die kostenlose 30-Tage-Testversion.</span><span class="sxs-lookup"><span data-stu-id="1a48f-126">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="1a48f-127">Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Ablaufdaten.</span><span class="sxs-lookup"><span data-stu-id="1a48f-127">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="1a48f-128">Speichern Sie die Schlüsselwerte für die zukünftige Verwendung an einem sicheren Ort.</span><span class="sxs-lookup"><span data-stu-id="1a48f-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a48f-129">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="1a48f-129">Next steps</span></span>
<span data-ttu-id="1a48f-130">Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="1a48f-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="1a48f-131">Zum Start der Testversion benötigen Sie folgende Informationen:</span><span class="sxs-lookup"><span data-stu-id="1a48f-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="1a48f-132">Anmeldeinformationen für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="1a48f-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="1a48f-133">Commerce-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="1a48f-133">Commerce ID GUID</span></span>
- <span data-ttu-id="1a48f-134">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="1a48f-134">App ID GUID</span></span>
- <span data-ttu-id="1a48f-135">Geheimer Anwendungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="1a48f-135">Application secret key value</span></span>
