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
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010381"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="acab7-104">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center</span><span class="sxs-lookup"><span data-stu-id="acab7-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="acab7-105">Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Azure AD-Anwendung (Dienstprinzipal) als Benutzer in Ihrem Azure AD-Mandanten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="acab7-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Azure AD tenant.</span></span> <span data-ttu-id="acab7-106">(Dieser Schritt konnte zuvor im CPP-Konto (Cloud-Partnerportal) ausgeführt werden. Nach Ihrer Migration zu Partner Center ist das CPP-Konto jedoch schreibgeschützt.) Beachten Sie, dass der Dienstprinzipal mit der Azure AD-Anwendung identisch ist.</span><span class="sxs-lookup"><span data-stu-id="acab7-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="acab7-107">Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal)</span><span class="sxs-lookup"><span data-stu-id="acab7-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="acab7-108">Wählen Sie auf dem Partner Center-Dashboard **Einstellungen** und anschließend **Entwicklereinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="acab7-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="acab7-109">Wählen Sie **Benutzer** und dann **Azure AD-Anwendungen hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="acab7-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="acab7-110">Wählen Sie eine vorhandene Azure AD-Anwendung aus, oder erstellen eine neue.</span><span class="sxs-lookup"><span data-stu-id="acab7-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="acab7-111">Geben Sie bei Erstellung einer neuen Azure AD-Anwendung die folgenden Informationen an:</span><span class="sxs-lookup"><span data-stu-id="acab7-111">If you create a new Azure AD Application, include the following information:</span></span>  
<span data-ttu-id="acab7-112">  
\*\*Name\*\*: Dies ähnelt dem Feld „Anzeigename“ im CPP.</span><span class="sxs-lookup"><span data-stu-id="acab7-112">  
\*\*Name\*\*: This is similar to the ‘friendly name’ field in the CPP portal.</span></span>

<span data-ttu-id="acab7-113">**Antwort-URL**: Dies ist die URL, unter der sich Benutzer zur Verwendung Ihrer Azure AD-Anwendung anmelden können.</span><span class="sxs-lookup"><span data-stu-id="acab7-113">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="acab7-114">**App-ID-URI**: Dies ist ein logischer Bezeichner für die Azure AD-App, der beim Senden einer Anforderung für einmaliges Anmelden an Azure AD angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="acab7-114">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="acab7-115">**Sicherheitsrollen**: Die Rollen **Manager** (entspricht der Rolle „Besitzer“ im CPP) und **Entwickler** (entspricht der Rolle „Mitwirkender“ im CPP) gelten für das Programm für den kommerziellen Marketplace in Partner Center und können dieser Azure AD-Anwendung zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="acab7-115">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

<span data-ttu-id="acab7-116">Wenn Sie zur Erstellung in Partner Center **Speichern** auswählen, werden die Informationen auch mit dem CPP-System synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="acab7-116">When you select **Save**,  to create this in Partner Center, the information is also synced back to the CPP system.</span></span>  
