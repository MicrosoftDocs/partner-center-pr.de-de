---
title: Azure AD-Dienstprinzipal
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie einen Dienstprinzipal zu Ihrem Azure AD-Mandanten hinzufügen. Dabei fügen Sie eine Azure AD-Anwendung (Dienstprinzipal) in Partner Center hinzu.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028467"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="07a8f-104">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center</span><span class="sxs-lookup"><span data-stu-id="07a8f-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="07a8f-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="07a8f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="07a8f-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="07a8f-106">Global admin</span></span>

<span data-ttu-id="07a8f-107">Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Azure AD-Anwendung (Dienstprinzipal) als Benutzer in Ihrem Partner Center-Konto hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="07a8f-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="07a8f-108">(Dies war zuvor in Ihrem Cloud-Partnerportal- oder CPP-Konto möglich.</span><span class="sxs-lookup"><span data-stu-id="07a8f-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="07a8f-109">Nach der Migration zu Partner Center ist das CPP-Konto schreibgeschützt.)</span><span class="sxs-lookup"><span data-stu-id="07a8f-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="07a8f-110">Der Dienstprinzipal ist mit der Azure AD-Anwendung identisch.</span><span class="sxs-lookup"><span data-stu-id="07a8f-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="07a8f-111">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal)</span><span class="sxs-lookup"><span data-stu-id="07a8f-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="07a8f-112">Wählen Sie auf dem Partner Center-Dashboard **Einstellungen** und anschließend **Entwicklereinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="07a8f-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="07a8f-113">Wählen Sie **Benutzer** und dann **Azure AD-Anwendungen hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="07a8f-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="07a8f-114">Wählen Sie eine vorhandene Azure AD-Anwendung aus, oder erstellen eine neue.</span><span class="sxs-lookup"><span data-stu-id="07a8f-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="07a8f-115">Geben Sie bei Erstellung einer neuen Azure AD-Anwendung die folgenden Informationen an:</span><span class="sxs-lookup"><span data-stu-id="07a8f-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="07a8f-116">**Antwort-URL**: Die URL, unter der sich Benutzer zur Verwendung Ihrer Azure AD-Anwendung anmelden können.</span><span class="sxs-lookup"><span data-stu-id="07a8f-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="07a8f-117">**App-ID-URI**: Ein logischer Bezeichner für die Azure AD-Anwendung, der beim Senden einer Anforderung für einmaliges Anmelden an Azure AD angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="07a8f-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="07a8f-118">**Sicherheitsrollen**: Die Rollen **Manager** (entspricht der Rolle „Besitzer“ im CPP) und **Entwickler** (entspricht der Rolle „Mitwirkender“ im CPP) gelten für das Programm für den kommerziellen Marketplace in Partner Center und können dieser Azure AD-Anwendung zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="07a8f-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="07a8f-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="07a8f-119">Next steps</span></span>

- [<span data-ttu-id="07a8f-120">Übersicht über den kommerziellen Marketplace im Partner Center</span><span class="sxs-lookup"><span data-stu-id="07a8f-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)