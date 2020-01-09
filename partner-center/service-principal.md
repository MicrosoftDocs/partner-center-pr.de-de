---
title: Azure AD-Dienstprinzipal | Partner Center
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hinzufügen eines Dienstprinzipals zu Ihrem Azure AD-Mandanten
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure-Plan, Dienstprinzipal, Azure AD-Anwendung
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716891"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="6931a-104">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center</span><span class="sxs-lookup"><span data-stu-id="6931a-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="6931a-105">Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Azure AD-Anwendung (Dienstprinzipal) als Benutzer in Ihrem Partner Center-Konto hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6931a-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="6931a-106">(Dieser Schritt konnte zuvor im CPP-Konto (Cloud-Partnerportal) ausgeführt werden. Nach Ihrer Migration zu Partner Center ist das CPP-Konto jedoch schreibgeschützt.) Beachten Sie, dass der Dienstprinzipal mit der Azure AD-Anwendung identisch ist.</span><span class="sxs-lookup"><span data-stu-id="6931a-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="6931a-107">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal)</span><span class="sxs-lookup"><span data-stu-id="6931a-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="6931a-108">Wählen Sie auf dem Partner Center-Dashboard **Einstellungen** und anschließend **Entwicklereinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="6931a-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="6931a-109">Wählen Sie **Benutzer** und dann **Azure AD-Anwendungen hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="6931a-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="6931a-110">Wählen Sie eine vorhandene Azure AD-Anwendung aus, oder erstellen eine neue.</span><span class="sxs-lookup"><span data-stu-id="6931a-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="6931a-111">Geben Sie bei Erstellung einer neuen Azure AD-Anwendung die folgenden Informationen an:</span><span class="sxs-lookup"><span data-stu-id="6931a-111">If you create a new Azure AD Application, include the following information:</span></span>  

  


<span data-ttu-id="6931a-112">**Antwort-URL**: Dies ist die URL, unter der sich Benutzer zur Verwendung Ihrer Azure AD-Anwendung anmelden können.</span><span class="sxs-lookup"><span data-stu-id="6931a-112">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="6931a-113">**App-ID-URI**: Dies ist ein logischer Bezeichner für die Azure AD-Anwendung, der beim Senden einer Anforderung für einmaliges Anmelden an Azure AD angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="6931a-113">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="6931a-114">**Sicherheitsrollen**: Die Rollen **Manager** (entspricht der Rolle „Besitzer“ im CPP) und **Entwickler** (entspricht der Rolle „Mitwirkender“ im CPP) gelten für das Programm für den kommerziellen Marketplace in Partner Center und können dieser Azure AD-Anwendung zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="6931a-114">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

  
