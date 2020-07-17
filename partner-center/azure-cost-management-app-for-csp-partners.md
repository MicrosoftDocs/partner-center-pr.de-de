---
title: Azure Cost Management von cloudyn für CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die cloudyn-Web-App registrieren und einen geheimen Schlüssel für diese in Partner Center verwenden, damit Sie die APP verwenden können, um die Azure-Nutzung und die Kosten des Kunden zu verfolgen.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435909"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="858c6-103">Verfolgen Sie die Azure-Nutzung und die Kosten des Kunden mit der Azure Cost Management-APP für CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="858c6-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="858c6-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="858c6-104">**Applies to**</span></span>

- <span data-ttu-id="858c6-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="858c6-105">Partner Center</span></span>
- <span data-ttu-id="858c6-106">Partner im Cloud Solution Provider-Programm</span><span class="sxs-lookup"><span data-stu-id="858c6-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="858c6-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="858c6-107">**Appropriate roles**</span></span>

- <span data-ttu-id="858c6-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="858c6-108">Global admin</span></span>
- <span data-ttu-id="858c6-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="858c6-109">Admin agent</span></span>

[<span data-ttu-id="858c6-110">Weitere Informationen zu Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="858c6-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="858c6-111">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="858c6-111">Before you begin</span></span>
<span data-ttu-id="858c6-112">Bevor Sie Azure Cost Management verwenden können, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="858c6-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="858c6-113">Sie sind Partner im Cloud Solution Provider-Programm.</span><span class="sxs-lookup"><span data-stu-id="858c6-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="858c6-114">Sie haben die Fähigkeit, eine Partner Center-API-Web-App zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="858c6-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="858c6-115">Übersicht</span><span class="sxs-lookup"><span data-stu-id="858c6-115">Overview</span></span>

<span data-ttu-id="858c6-116">Cloudyn ist eine Web-App, mit der Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können.</span><span class="sxs-lookup"><span data-stu-id="858c6-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="858c6-117">Sie können die App über die Partner Center-API nutzen.</span><span class="sxs-lookup"><span data-stu-id="858c6-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="858c6-118">Registrieren Ihrer Web-App im Partner Center</span><span class="sxs-lookup"><span data-stu-id="858c6-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="858c6-119">Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie den Zugriff auf die Partner Center-API aktivieren.</span><span class="sxs-lookup"><span data-stu-id="858c6-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="858c6-120">Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.</span><span class="sxs-lookup"><span data-stu-id="858c6-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="858c6-121">Wählen Sie im **Partner Center**nacheinander **Kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** aus.</span><span class="sxs-lookup"><span data-stu-id="858c6-121">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="858c6-122">Klicken Sie im Abschnitt **Web-App** auf **Neue Web-App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="858c6-122">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="858c6-123">**Hinweis**: Wenn Sie zuvor eine Web-App erstellt haben, können Sie Schritt 3 überspringen.</span><span class="sxs-lookup"><span data-stu-id="858c6-123">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="858c6-124">Kopieren und speichern Sie die GUIDs für **Commerce-ID**und **App-ID** für Ihre Web-App.</span><span class="sxs-lookup"><span data-stu-id="858c6-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="858c6-125">Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.</span><span class="sxs-lookup"><span data-stu-id="858c6-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="858c6-126">Hinzufügen eines geheimen Schlüssels zu Ihrer App</span><span class="sxs-lookup"><span data-stu-id="858c6-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="858c6-127">Wählen Sie in der Dropdownliste neben der Schaltfläche **Schlüssel hinzufügen**eine Dauer von 1 oder 2 Jahren aus.</span><span class="sxs-lookup"><span data-stu-id="858c6-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="858c6-128">Klicken Sie auf **Schlüssel hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="858c6-128">Click **Add key**.</span></span> 
3. <span data-ttu-id="858c6-129">Kopieren und speichern Sie den Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="858c6-129">Copy and save the secret key value.</span></span> <span data-ttu-id="858c6-130">Sie benötigen diesen für die kostenlose 30-Tage-Testversion.</span><span class="sxs-lookup"><span data-stu-id="858c6-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="858c6-131">Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Laufzeiten.</span><span class="sxs-lookup"><span data-stu-id="858c6-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="858c6-132">Speichern Sie den Schlüsselwert für die künftige Verwendung an einem sicheren Ort.</span><span class="sxs-lookup"><span data-stu-id="858c6-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="858c6-133">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="858c6-133">Next steps</span></span>
<span data-ttu-id="858c6-134">Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="858c6-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="858c6-135">Zum Start der Testversion benötigen Sie folgende Informationen:</span><span class="sxs-lookup"><span data-stu-id="858c6-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="858c6-136">Anmeldeinformationen für Partner Center</span><span class="sxs-lookup"><span data-stu-id="858c6-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="858c6-137">Commerce-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="858c6-137">Commerce ID GUID</span></span>
- <span data-ttu-id="858c6-138">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="858c6-138">App ID GUID</span></span>
- <span data-ttu-id="858c6-139">Wert des geheimen Anwendungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="858c6-139">Application secret key value</span></span>
