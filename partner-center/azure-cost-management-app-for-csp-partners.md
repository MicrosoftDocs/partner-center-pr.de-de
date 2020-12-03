---
title: Azure Cost Management von Cloudyn für CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die cloudyn-Web-App registrieren und einen geheimen Schlüssel für diese in Partner Center verwenden, damit Sie die APP verwenden können, um die Azure-Nutzung und die Kosten des Kunden zu verfolgen.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534987"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="f7c74-103">Verfolgen Sie die Azure-Nutzung und die Kosten des Kunden mit der Azure Cost Management-APP für CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="f7c74-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="f7c74-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="f7c74-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f7c74-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="f7c74-105">Global admin</span></span>
- <span data-ttu-id="f7c74-106">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="f7c74-106">Admin agent</span></span>

[<span data-ttu-id="f7c74-107">Weitere Informationen zu Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="f7c74-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="f7c74-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f7c74-108">Before you begin</span></span>
<span data-ttu-id="f7c74-109">Bevor Sie Azure Cost Management verwenden können, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="f7c74-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="f7c74-110">Sie sind Partner im Cloud Solution Provider-Programm.</span><span class="sxs-lookup"><span data-stu-id="f7c74-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="f7c74-111">Sie haben die Fähigkeit, eine Partner Center-API-Web-App zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f7c74-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="f7c74-112">Übersicht</span><span class="sxs-lookup"><span data-stu-id="f7c74-112">Overview</span></span>

<span data-ttu-id="f7c74-113">Cloudyn ist eine Web-App, mit der Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können.</span><span class="sxs-lookup"><span data-stu-id="f7c74-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="f7c74-114">Sie können die App über die Partner Center-API nutzen.</span><span class="sxs-lookup"><span data-stu-id="f7c74-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="f7c74-115">Registrieren Ihrer Web-App im Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7c74-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="f7c74-116">Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie den Zugriff auf die Partner Center-API aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f7c74-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="f7c74-117">Melden Sie sich mit einem Konto für den [globalen Administrator oder Administrator-Agent](create-user-accounts-and-set-permissions.md)beim [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) an.</span><span class="sxs-lookup"><span data-stu-id="f7c74-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="f7c74-118">Wählen Sie im **Partner Center** **Kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** aus.</span><span class="sxs-lookup"><span data-stu-id="f7c74-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="f7c74-119">Klicken Sie im Abschnitt **Web-App** auf **Neue Web-App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="f7c74-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="f7c74-120">**Hinweis**: Wenn Sie zuvor eine Web-App erstellt haben, können Sie Schritt 3 überspringen.</span><span class="sxs-lookup"><span data-stu-id="f7c74-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="f7c74-121">Kopieren und speichern Sie die GUIDs für **Commerce-ID** und **App-ID** für Ihre Web-App.</span><span class="sxs-lookup"><span data-stu-id="f7c74-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="f7c74-122">Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.</span><span class="sxs-lookup"><span data-stu-id="f7c74-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="f7c74-123">Hinzufügen eines geheimen Schlüssels zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="f7c74-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="f7c74-124">Wählen Sie in der Dropdownliste neben der Schaltfläche **Schlüssel hinzufügen** eine Dauer von 1 oder 2 Jahren aus.</span><span class="sxs-lookup"><span data-stu-id="f7c74-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="f7c74-125">Klicken Sie auf **Schlüssel hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="f7c74-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="f7c74-126">Kopieren und speichern Sie den Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="f7c74-126">Copy and save the secret key value.</span></span> <span data-ttu-id="f7c74-127">Sie benötigen diesen für die kostenlose 30-Tage-Testversion.</span><span class="sxs-lookup"><span data-stu-id="f7c74-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="f7c74-128">Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Laufzeiten.</span><span class="sxs-lookup"><span data-stu-id="f7c74-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="f7c74-129">Speichern Sie den Schlüsselwert für die künftige Verwendung an einem sicheren Ort.</span><span class="sxs-lookup"><span data-stu-id="f7c74-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f7c74-130">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f7c74-130">Next steps</span></span>
<span data-ttu-id="f7c74-131">Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="f7c74-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="f7c74-132">Zum Start der Testversion benötigen Sie folgende Informationen:</span><span class="sxs-lookup"><span data-stu-id="f7c74-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="f7c74-133">Anmeldeinformationen für Partner Center</span><span class="sxs-lookup"><span data-stu-id="f7c74-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="f7c74-134">Commerce-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="f7c74-134">Commerce ID GUID</span></span>
- <span data-ttu-id="f7c74-135">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="f7c74-135">App ID GUID</span></span>
- <span data-ttu-id="f7c74-136">Wert des geheimen Anwendungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="f7c74-136">Application secret key value</span></span>
