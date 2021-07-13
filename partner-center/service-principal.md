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
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551553"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="1387e-104">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center</span><span class="sxs-lookup"><span data-stu-id="1387e-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="1387e-105">**Geeignete Rollen**: Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="1387e-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="1387e-106">Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Microsoft Azure Active Directory (Azure AD) Anwendung (Dienstprinzipal) als Benutzer in Ihrem Partner Center-Konto hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1387e-106">In the Commercial Marketplace program in Partner Center, you are now able to add a Microsoft Azure Active Directory (Azure AD) application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="1387e-107">(Dies war zuvor in Ihrem Cloud-Partnerportal Konto möglich).</span><span class="sxs-lookup"><span data-stu-id="1387e-107">(You were able to do so previously in your Cloud Partner Portal (CPP) account.</span></span> <span data-ttu-id="1387e-108">Nach der Migration zu Partner Center ist das CPP-Konto schreibgeschützt.)</span><span class="sxs-lookup"><span data-stu-id="1387e-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="1387e-109">Der Dienstprinzipal ist mit der Azure AD-Anwendung identisch.</span><span class="sxs-lookup"><span data-stu-id="1387e-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="1387e-110">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal)</span><span class="sxs-lookup"><span data-stu-id="1387e-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="1387e-111">Wählen Sie auf dem Partner Center-Dashboard **Einstellungen** und anschließend **Entwicklereinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="1387e-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="1387e-112">Wählen Sie **Benutzer** und dann **Azure AD-Anwendungen hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="1387e-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="1387e-113">Wählen Sie eine vorhandene Azure AD-Anwendung aus, oder erstellen eine neue.</span><span class="sxs-lookup"><span data-stu-id="1387e-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="1387e-114">Geben Sie bei Erstellung einer neuen Azure AD-Anwendung die folgenden Informationen an:</span><span class="sxs-lookup"><span data-stu-id="1387e-114">If you create a new Azure AD application, include the following information:</span></span>  

   - <span data-ttu-id="1387e-115">**Antwort-URL**: Die URL, unter der sich Benutzer zur Verwendung Ihrer Azure AD-Anwendung anmelden können.</span><span class="sxs-lookup"><span data-stu-id="1387e-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="1387e-116">**App-ID-URI**: Ein logischer Bezeichner für die Azure AD-Anwendung, der beim Senden einer Anforderung für einmaliges Anmelden an Azure AD angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1387e-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="1387e-117">**Sicherheitsrollen**: Die Rollen **Manager** (entspricht der Rolle „Besitzer“ im CPP) und **Entwickler** (entspricht der Rolle „Mitwirkender“ im CPP) gelten für das Programm für den kommerziellen Marketplace in Partner Center und können dieser Azure AD-Anwendung zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="1387e-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="1387e-118">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="1387e-118">Next steps</span></span>

- [<span data-ttu-id="1387e-119">Übersicht über den kommerziellen Marketplace im Partner Center</span><span class="sxs-lookup"><span data-stu-id="1387e-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)