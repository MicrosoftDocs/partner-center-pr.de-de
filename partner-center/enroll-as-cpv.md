---
title: Registrieren als Control Panel-Anbieter in Partner Center| Partner Center
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie Sie sich als System Steuerungs Anbieter (CPV) im Partner Center registrieren.
author: LauraBrenner
ms.author: labrenne
keywords: Control Panel-Anbieter, CPV-Apps registrieren, CPV-Apps verwalten
ms.localizationpriority: medium
ms.openlocfilehash: d8320c584a9beefb6163a1072f90d66bdbaa8454
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722556"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="83af1-104">Registrieren als Control Panel-Anbieter in Partner Center</span><span class="sxs-lookup"><span data-stu-id="83af1-104">Enroll in Partner Center as a Control Panel Vendor</span></span>

<span data-ttu-id="83af1-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="83af1-105">**Applies to**</span></span>

- <span data-ttu-id="83af1-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="83af1-106">Partner Center</span></span>

<span data-ttu-id="83af1-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="83af1-107">**Appropriate roles**</span></span>

- <span data-ttu-id="83af1-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="83af1-108">Global admin</span></span>

<span data-ttu-id="83af1-109">Ein Control Panel-Anbieter (Control Panel Vendor, CPV) ist ein unabhängiger Softwarehersteller, der Anwendungen für Cloud-Lösungsanbieter (Cloud Solution Provider, CSP) entwickelt, damit sie ihre Systeme in Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="83af1-109">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="83af1-110">Ein Control Panel-Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder die Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="83af1-110">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="83af1-111">Sowohl aktuelle Control Panel-Anbieter (Control Panel Vendor, CPV) als auch neue CPV, die mit Microsoft-Partnern zusammenarbeiten möchten, müssen sich gemäß den neuen Bestimmungen von Microsoft in Partner Center anmelden, um Ihre Anwendungen registrieren und Cloud Solution Provider-Partner zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="83af1-111">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="83af1-112">Um ein Konto zu erstellen, können CPV-Partner einen vorhandenen CSP- oder CPV-Partnermandanten verwenden oder im Rahmen des Onboarding-Prozesses einen neuen Mandanten erstellen.</span><span class="sxs-lookup"><span data-stu-id="83af1-112">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="83af1-113">Wenn der CPV-Partner den vorhandenen CSP-Mandanten verwendet, muss er separate mehr Instanzen fähige Anwendungen erstellen und diese in Partner Center für CPV-Aktivitäten registrieren.</span><span class="sxs-lookup"><span data-stu-id="83af1-113">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="83af1-114">Eine Anwendung kann nicht als CSP-und CPV-Anwendung registriert werden.</span><span class="sxs-lookup"><span data-stu-id="83af1-114">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="83af1-115">Nachdem Sie sich in Partner Center angemeldet und Ihre Anwendungen registriert haben, können Sie auf Partner Center-APIs zugreifen.</span><span class="sxs-lookup"><span data-stu-id="83af1-115">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="83af1-116">Microsoft teilt Ihnen über eine Benachrichtigung in Partner Center Ihre Sandbox-Informationen mit.</span><span class="sxs-lookup"><span data-stu-id="83af1-116">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="83af1-117">Wenn Sie bereits über ein Sandboxkonto verfügen, verwenden Sie dieses weiterhin.</span><span class="sxs-lookup"><span data-stu-id="83af1-117">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="83af1-118">Sie benötigen keinen neuen Sandkasten.</span><span class="sxs-lookup"><span data-stu-id="83af1-118">You won't need a new sandbox.</span></span>   

<span data-ttu-id="83af1-119">Lesen Sie die [Vereinbarung für Microsoft Control Panel-Anbieter](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="83af1-119">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="83af1-120">Nutzung von Partner Center</span><span class="sxs-lookup"><span data-stu-id="83af1-120">Working in Partner Center</span></span>
<span data-ttu-id="83af1-121">Sobald Sie sich auf der Partner Center CPV-Oberfläche registriert haben und die CPV-Vereinbarung akzeptiert haben, ist Folgendes möglich:</span><span class="sxs-lookup"><span data-stu-id="83af1-121">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="83af1-122">Verwalten von Multi-Tenant-Anwendungen (Anwendungen im Azure-Portal hinzufügen, Anwendungen in Partner Center registrieren und deren Registrierung aufheben)</span><span class="sxs-lookup"><span data-stu-id="83af1-122">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="83af1-123">CPVs müssen ihre Anwendungen in Partner Center registrieren, um die Autorisierung für Partner Center-APIs zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="83af1-123">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="83af1-124">Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.</span><span class="sxs-lookup"><span data-stu-id="83af1-124">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="83af1-125">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="83af1-125">View and manage your CPV profile</span></span> 

- <span data-ttu-id="83af1-126">Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.</span><span class="sxs-lookup"><span data-stu-id="83af1-126">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="83af1-127">Die einzige Rolle, die eine CPV einnehmen kann, ist der globale Administrator.</span><span class="sxs-lookup"><span data-stu-id="83af1-127">The only role a CPV can have is global admin.</span></span>


