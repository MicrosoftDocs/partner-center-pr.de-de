---
title: Azure Cost Management von Cloudyn für CSP-Partner | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Azure Cost Management von Cloudyn erfordert einen Zugriff über die Partner Center-API.
author: Janet
ms.author: janet
Keywords: Azure Cost Management-App, Kostenmanagement, Web-Apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 14b94e94c349fa142cb6bd37ed4ca94f7a9397b6
ms.sourcegitcommit: f916aa2884239b205398c24d04d1f1dc41b63c2b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2019
ms.locfileid: "64668664"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="286d5-104">Azure Cost Management-App für Azure CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="286d5-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="286d5-105">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="286d5-105">**Applies to**</span></span>

-  <span data-ttu-id="286d5-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="286d5-106">Partner Center</span></span>

[<span data-ttu-id="286d5-107">Weitere Informationen zu Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="286d5-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="286d5-108">Vorbemerkungen</span><span class="sxs-lookup"><span data-stu-id="286d5-108">Before you begin</span></span>
<span data-ttu-id="286d5-109">Bevor Sie Azure Cost Management verwenden können, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="286d5-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="286d5-110">Sie sind Partner im Cloud Solution Provider-Programm.</span><span class="sxs-lookup"><span data-stu-id="286d5-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="286d5-111">Sie haben die Fähigkeit, eine Partner Center-API-Web-App zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="286d5-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="286d5-112">Übersicht</span><span class="sxs-lookup"><span data-stu-id="286d5-112">Overview</span></span>

<span data-ttu-id="286d5-113">Cloudyn ist eine Web-App, mit der Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können.</span><span class="sxs-lookup"><span data-stu-id="286d5-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="286d5-114">Sie können die App über die Partner Center-API nutzen.</span><span class="sxs-lookup"><span data-stu-id="286d5-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="286d5-115">Registrieren Ihrer Web-App im Partner Center</span><span class="sxs-lookup"><span data-stu-id="286d5-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="286d5-116">Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie auf die Partner Center-API zugreifen.</span><span class="sxs-lookup"><span data-stu-id="286d5-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="286d5-117">Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.</span><span class="sxs-lookup"><span data-stu-id="286d5-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="286d5-118">Wählen Sie im **Partner Center**nacheinander **Kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** aus.</span><span class="sxs-lookup"><span data-stu-id="286d5-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="286d5-119">Klicken Sie im Abschnitt **Web-App** auf **Neue Web-App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="286d5-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="286d5-120">**Hinweis**: Wenn Sie bereits zuvor eine Web-App erstellt haben, können Sie Schritt 3 überspringen.</span><span class="sxs-lookup"><span data-stu-id="286d5-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="286d5-121">Kopieren und speichern Sie die GUIDs für **Commerce-ID**und **App-ID** für Ihre Web-App.</span><span class="sxs-lookup"><span data-stu-id="286d5-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="286d5-122">Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.</span><span class="sxs-lookup"><span data-stu-id="286d5-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="286d5-123">Hinzufügen eines geheimen Schlüssels zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="286d5-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="286d5-124">Wählen Sie in der Dropdownliste neben der Schaltfläche **Schlüssel hinzufügen**eine Dauer von 1 oder 2 Jahren aus.</span><span class="sxs-lookup"><span data-stu-id="286d5-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="286d5-125">Klicken Sie auf **Schlüssel hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="286d5-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="286d5-126">Kopieren und speichern Sie den Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="286d5-126">Copy and save the secret key value.</span></span> <span data-ttu-id="286d5-127">Sie benötigen diesen für die kostenlose 30-Tage-Testversion.</span><span class="sxs-lookup"><span data-stu-id="286d5-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="286d5-128">Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Laufzeiten.</span><span class="sxs-lookup"><span data-stu-id="286d5-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="286d5-129">Speichern Sie den Schlüsselwert für die künftige Verwendung an einem sicheren Ort.</span><span class="sxs-lookup"><span data-stu-id="286d5-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="286d5-130">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="286d5-130">Next steps</span></span>
<span data-ttu-id="286d5-131">Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="286d5-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="286d5-132">Zum Start der Testversion benötigen Sie folgende Informationen:</span><span class="sxs-lookup"><span data-stu-id="286d5-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="286d5-133">Anmeldeinformationen für Partner Center</span><span class="sxs-lookup"><span data-stu-id="286d5-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="286d5-134">Commerce-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="286d5-134">Commerce ID GUID</span></span>
- <span data-ttu-id="286d5-135">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="286d5-135">App ID GUID</span></span>
- <span data-ttu-id="286d5-136">Wert des geheimen Anwendungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="286d5-136">Application secret key value</span></span>
