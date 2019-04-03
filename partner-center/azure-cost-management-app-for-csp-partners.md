---
title: Azure Cost Management von Cloudyn für CSP-Partner | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management von Cloudyn erfordert einen Zugriff über die Partner Center-API.
author: Janet
ms.author: janet
Keywords: Azure Cost Management-app, Verwalten von Kosten, web-apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: f1627727908eff9c686dd8359558e960d0fbff88
ms.sourcegitcommit: 6578eea4fe6836dad5710f8d22376ad8bba6e307
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "58490342"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="ca0db-104">App zum Azure-Kostenmanagement für Azure CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="ca0db-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="ca0db-105">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="ca0db-105">**Applies to**</span></span>

-  <span data-ttu-id="ca0db-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="ca0db-106">Partner Center</span></span>

[<span data-ttu-id="ca0db-107">Informationen Sie weitere zu Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="ca0db-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="ca0db-108">Vorbemerkungen</span><span class="sxs-lookup"><span data-stu-id="ca0db-108">Before you begin</span></span>
<span data-ttu-id="ca0db-109">Bevor Sie Azure Cost Management verwenden können, sollten Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="ca0db-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="ca0db-110">Sie sind Partner im Cloud-Lösungsanbieter-Programm.</span><span class="sxs-lookup"><span data-stu-id="ca0db-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="ca0db-111">Sie haben die Möglichkeit, eine Partner Center-API-Web-App zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ca0db-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="ca0db-112">Übersicht</span><span class="sxs-lookup"><span data-stu-id="ca0db-112">Overview</span></span>

<span data-ttu-id="ca0db-113">Cloudyn ist eine Web-app, die Ihnen die Möglichkeit zum Nachverfolgen und verwalten, wie viel Ihre Kunden Azure und die Kosten für diese Nutzung verwenden.</span><span class="sxs-lookup"><span data-stu-id="ca0db-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="ca0db-114">Sie können die App über die Partner Center-API nutzen.</span><span class="sxs-lookup"><span data-stu-id="ca0db-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="ca0db-115">Registrieren Ihrer Web-App im Partner Center</span><span class="sxs-lookup"><span data-stu-id="ca0db-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="ca0db-116">Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie auf die Partner Center-API zugreifen.</span><span class="sxs-lookup"><span data-stu-id="ca0db-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="ca0db-117">Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.</span><span class="sxs-lookup"><span data-stu-id="ca0db-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="ca0db-118">Von der **Partner Center**Option **Kontoeinstellungen** &gt;  **[App-Verwaltung](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="ca0db-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="ca0db-119">Klicken Sie im Abschnitt **Web-app** auf **Neue Web-App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="ca0db-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="ca0db-120">**Hinweis**: Wenn Sie zuvor eine Web-app erstellt haben, können Sie Schritt 3 überspringen.</span><span class="sxs-lookup"><span data-stu-id="ca0db-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="ca0db-121">Kopieren und speichern Sie die **Commerce-ID**-GUID und die **App-ID**-GUID für Ihre Web-App.</span><span class="sxs-lookup"><span data-stu-id="ca0db-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="ca0db-122">Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.</span><span class="sxs-lookup"><span data-stu-id="ca0db-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="ca0db-123">Hinzufügen eines geheimen Schlüssels zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="ca0db-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="ca0db-124">Wählen Sie in der Dropdownliste neben der **Schlüssel hinzufügen**-Schaltfläche eine Dauer von 1 oder 2 Jahren aus.</span><span class="sxs-lookup"><span data-stu-id="ca0db-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="ca0db-125">Klicken Sie auf **Schlüssel hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="ca0db-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="ca0db-126">Kopieren Sie und speichern Sie den Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="ca0db-126">Copy and save the secret key value.</span></span> <span data-ttu-id="ca0db-127">Sie benötigen diesen für die kostenlose 30-Tage-Testversion.</span><span class="sxs-lookup"><span data-stu-id="ca0db-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="ca0db-128">Der geheime Anwendungsschlüssel sind wie Kennwörter mit einer längeren Gültigkeitsdauer.</span><span class="sxs-lookup"><span data-stu-id="ca0db-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="ca0db-129">Speichern Sie die Schlüsselwerte für die zukünftige Verwendung an einem sicheren Ort.</span><span class="sxs-lookup"><span data-stu-id="ca0db-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ca0db-130">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ca0db-130">Next steps</span></span>
<span data-ttu-id="ca0db-131">Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="ca0db-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="ca0db-132">Zum Start der Testversion benötigen Sie folgende Informationen:</span><span class="sxs-lookup"><span data-stu-id="ca0db-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="ca0db-133">Anmeldeinformationen für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="ca0db-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="ca0db-134">Commerce-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="ca0db-134">Commerce ID GUID</span></span>
- <span data-ttu-id="ca0db-135">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="ca0db-135">App ID GUID</span></span>
- <span data-ttu-id="ca0db-136">Geheimer Anwendungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="ca0db-136">Application secret key value</span></span>
