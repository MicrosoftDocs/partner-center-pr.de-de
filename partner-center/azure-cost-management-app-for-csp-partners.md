---
title: Azure Cost Management von cloudyn für CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die cloudyn-Web-App registrieren und einen geheimen Schlüssel für diese in Partner Center verwenden, damit Sie die APP verwenden können, um die Azure-Nutzung und die Kosten des Kunden zu verfolgen.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure Cost Management-App, Kostenmanagement, Web-Apps
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d88f37e0fe653c679df5729fa283336e4c7e144
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908375"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="7dd8d-104">Verfolgen Sie die Azure-Nutzung und die Kosten des Kunden mit der Azure Cost Management-APP für CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="7dd8d-104">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="7dd8d-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="7dd8d-105">**Applies to**</span></span>

- <span data-ttu-id="7dd8d-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="7dd8d-106">Partner Center</span></span>
- <span data-ttu-id="7dd8d-107">Partner im Cloud Solution Provider-Programm</span><span class="sxs-lookup"><span data-stu-id="7dd8d-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="7dd8d-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="7dd8d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="7dd8d-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7dd8d-109">Global admin</span></span>
- <span data-ttu-id="7dd8d-110">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="7dd8d-110">Admin agent</span></span>

[<span data-ttu-id="7dd8d-111">Weitere Informationen zu Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="7dd8d-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="7dd8d-112">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7dd8d-112">Before you begin</span></span>
<span data-ttu-id="7dd8d-113">Bevor Sie Azure Cost Management verwenden können, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="7dd8d-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="7dd8d-114">Sie sind Partner im Cloud Solution Provider-Programm.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="7dd8d-115">Sie haben die Fähigkeit, eine Partner Center-API-Web-App zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="7dd8d-116">Übersicht</span><span class="sxs-lookup"><span data-stu-id="7dd8d-116">Overview</span></span>

<span data-ttu-id="7dd8d-117">Cloudyn ist eine Web-App, mit der Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="7dd8d-118">Sie können die App über die Partner Center-API nutzen.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="7dd8d-119">Registrieren Ihrer Web-App im Partner Center</span><span class="sxs-lookup"><span data-stu-id="7dd8d-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="7dd8d-120">Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie den Zugriff auf die Partner Center-API aktivieren.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="7dd8d-121">Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="7dd8d-122">Wählen Sie im **Partner Center**nacheinander **Kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** aus.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="7dd8d-123">Klicken Sie im Abschnitt **Web-App** auf **Neue Web-App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="7dd8d-124">**Hinweis**: Wenn Sie zuvor eine Web-App erstellt haben, können Sie Schritt 3 überspringen.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="7dd8d-125">Kopieren und speichern Sie die GUIDs für **Commerce-ID**und **App-ID** für Ihre Web-App.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="7dd8d-126">Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="7dd8d-127">Hinzufügen eines geheimen Schlüssels zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="7dd8d-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="7dd8d-128">Wählen Sie in der Dropdownliste neben der Schaltfläche **Schlüssel hinzufügen**eine Dauer von 1 oder 2 Jahren aus.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="7dd8d-129">Klicken Sie auf **Schlüssel hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="7dd8d-130">Kopieren und speichern Sie den Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-130">Copy and save the secret key value.</span></span> <span data-ttu-id="7dd8d-131">Sie benötigen diesen für die kostenlose 30-Tage-Testversion.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="7dd8d-132">Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Laufzeiten.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="7dd8d-133">Speichern Sie den Schlüsselwert für die künftige Verwendung an einem sicheren Ort.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7dd8d-134">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7dd8d-134">Next steps</span></span>
<span data-ttu-id="7dd8d-135">Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="7dd8d-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="7dd8d-136">Zum Start der Testversion benötigen Sie folgende Informationen:</span><span class="sxs-lookup"><span data-stu-id="7dd8d-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="7dd8d-137">Anmeldeinformationen für Partner Center</span><span class="sxs-lookup"><span data-stu-id="7dd8d-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="7dd8d-138">Commerce-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="7dd8d-138">Commerce ID GUID</span></span>
- <span data-ttu-id="7dd8d-139">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="7dd8d-139">App ID GUID</span></span>
- <span data-ttu-id="7dd8d-140">Wert des geheimen Anwendungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="7dd8d-140">Application secret key value</span></span>
