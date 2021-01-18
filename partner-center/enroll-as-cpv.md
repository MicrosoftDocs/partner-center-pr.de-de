---
title: Registrierung als Control Panel Vendor
description: Erfahren Sie, wie Sie sich als System Steuerungs Anbieter (CPV) im Partner Center registrieren, damit Sie CSP-Partner Systeme besser mit Partner Center-APIs integrieren können.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560509"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="b5a95-103">Registrieren als Control Panel Vendor, um die Integration von CSP-Partnersystemen in Partner Center-APIs zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b5a95-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="b5a95-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="b5a95-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b5a95-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b5a95-105">Global admin</span></span>

<span data-ttu-id="b5a95-106">Ein Control Panel-Anbieter (Control Panel Vendor, CPV) ist ein unabhängiger Softwarehersteller, der Anwendungen für Cloud-Lösungsanbieter (Cloud Solution Provider, CSP) entwickelt, damit sie ihre Systeme in Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="b5a95-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="b5a95-107">Ein Control Panel-Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder die Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="b5a95-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="b5a95-108">Sowohl aktuelle Control Panel-Anbieter (Control Panel Vendor, CPV) als auch neue CPV, die mit Microsoft-Partnern zusammenarbeiten möchten, müssen sich gemäß den neuen Bestimmungen von Microsoft in Partner Center anmelden, um Ihre Anwendungen registrieren und Cloud Solution Provider-Partner zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b5a95-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="b5a95-109">Um ein Konto zu erstellen, können CPV-Partner einen vorhandenen CSP- oder CPV-Partnermandanten verwenden oder im Rahmen des Onboarding-Prozesses einen neuen Mandanten erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5a95-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="b5a95-110">Wenn der CPV-Partner den vorhandenen CSP-Mandanten verwendet, muss er separate mehr Instanzen fähige Anwendungen erstellen und diese in Partner Center für CPV-Aktivitäten registrieren.</span><span class="sxs-lookup"><span data-stu-id="b5a95-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="b5a95-111">Eine Anwendung kann nicht als CSP-und CPV-Anwendung registriert werden.</span><span class="sxs-lookup"><span data-stu-id="b5a95-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="b5a95-112">Nachdem Sie sich in Partner Center angemeldet und Ihre Anwendungen registriert haben, können Sie auf Partner Center-APIs zugreifen.</span><span class="sxs-lookup"><span data-stu-id="b5a95-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="b5a95-113">Wenn Sie ein Sandkasten Konto benötigen, wenden Sie sich über eine Microsoft-Support Anforderung an Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b5a95-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="b5a95-114">Wenn Sie bereits über ein Sandbox Konto verfügen, verwenden Sie es weiter.</span><span class="sxs-lookup"><span data-stu-id="b5a95-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="b5a95-115">Sie benötigen keinen neuen Sandkasten.</span><span class="sxs-lookup"><span data-stu-id="b5a95-115">You won't need a new sandbox</span></span>

<span data-ttu-id="b5a95-116">Lesen Sie die [Vereinbarung für Microsoft Control Panel-Anbieter](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="b5a95-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="b5a95-117">Nutzung von Partner Center</span><span class="sxs-lookup"><span data-stu-id="b5a95-117">Working in Partner Center</span></span>

<span data-ttu-id="b5a95-118">Nachdem Sie sich beim Partner Center CPV-Prozess angemeldet und die CPV-Vereinbarung akzeptiert haben, können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="b5a95-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="b5a95-119">Verwalten von mehr Instanzen fähigen Anwendungen (Hinzufügen von Anwendungen zu Azure-Portal, registrieren und Aufheben der Registrierung von Anwendungen im Partner Center).</span><span class="sxs-lookup"><span data-stu-id="b5a95-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="b5a95-120">CPVs müssen ihre Anwendungen in Partner Center registrieren, um die Autorisierung für Partner Center-APIs zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="b5a95-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="b5a95-121">Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.</span><span class="sxs-lookup"><span data-stu-id="b5a95-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="b5a95-122">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="b5a95-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="b5a95-123">Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.</span><span class="sxs-lookup"><span data-stu-id="b5a95-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="b5a95-124">Der globale Administrator ist die einzige Rolle, die eine CPV aufweisen kann.</span><span class="sxs-lookup"><span data-stu-id="b5a95-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b5a95-125">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="b5a95-125">Next steps</span></span>

<span data-ttu-id="b5a95-126">-[Fügen Sie Ihrem Partner Center-Konto weitere Mandanten hinzu.](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="b5a95-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>