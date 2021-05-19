---
title: Registrierung als Control Panel Vendor
description: Erfahren Sie, wie Sie sich als Systemsteuerung-Anbieter (CPV) bei Partner Center damit Sie CSP-Partnersysteme besser in Partner Center-APIs integrieren können.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147138"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="17f97-103">Registrieren als Control Panel Vendor, um die Integration von CSP-Partnersystemen in Partner Center-APIs zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="17f97-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="17f97-104">**Geeignete Rollen**: Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="17f97-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="17f97-105">Ein Control Panel-Anbieter (Control Panel Vendor, CPV) ist ein unabhängiger Softwarehersteller, der Anwendungen für Cloud-Lösungsanbieter (Cloud Solution Provider, CSP) entwickelt, damit sie ihre Systeme in Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="17f97-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="17f97-106">Ein Control Panel-Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder die Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="17f97-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="17f97-107">Sowohl aktuelle Control Panel-Anbieter (Control Panel Vendor, CPV) als auch neue CPV, die mit Microsoft-Partnern zusammenarbeiten möchten, müssen sich gemäß den neuen Bestimmungen von Microsoft in Partner Center anmelden, um Ihre Anwendungen registrieren und Cloud Solution Provider-Partner zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="17f97-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="17f97-108">Um ein Konto zu erstellen, können CPV-Partner einen vorhandenen CSP- oder CPV-Partnermandanten verwenden oder im Rahmen des Onboarding-Prozesses einen neuen Mandanten erstellen.</span><span class="sxs-lookup"><span data-stu-id="17f97-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="17f97-109">Wenn sich der CPV-Partner für die Verwendung des vorhandenen CSP-Mandanten entscheidet, muss er separate mehr mandantenbasierte Anwendungen erstellen und in Partner Center für CPV-Aktivitäten registrieren.</span><span class="sxs-lookup"><span data-stu-id="17f97-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="17f97-110">Eine Anwendung kann nicht sowohl als CSP- als auch als CPV-Anwendung registriert werden.</span><span class="sxs-lookup"><span data-stu-id="17f97-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="17f97-111">Nachdem Sie sich in Partner Center angemeldet und Ihre Anwendungen registriert haben, können Sie auf Partner Center-APIs zugreifen.</span><span class="sxs-lookup"><span data-stu-id="17f97-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="17f97-112">Wenden Sie sich über eine Microsoft-Support anforderung an Microsoft, wenn Sie ein Sandboxkonto benötigen.</span><span class="sxs-lookup"><span data-stu-id="17f97-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="17f97-113">Wenn Sie bereits über ein Sandboxkonto verfügen, verwenden Sie es weiter.</span><span class="sxs-lookup"><span data-stu-id="17f97-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="17f97-114">Sie benötigen keine neue Sandbox.</span><span class="sxs-lookup"><span data-stu-id="17f97-114">You won't need a new sandbox</span></span>

<span data-ttu-id="17f97-115">Lesen Sie die [Vereinbarung für Microsoft Control Panel-Anbieter](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="17f97-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="17f97-116">Nutzung von Partner Center</span><span class="sxs-lookup"><span data-stu-id="17f97-116">Working in Partner Center</span></span>

<span data-ttu-id="17f97-117">Nachdem Sie sich für die CPV-Partner Center registriert und die CPV-Vereinbarung akzeptiert haben, können Sie:</span><span class="sxs-lookup"><span data-stu-id="17f97-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="17f97-118">Verwalten von mehr mandantenbasierten Anwendungen (Hinzufügen von Anwendungen Azure-Portal, Registrieren und Aufheben der Registrierung in Partner Center).</span><span class="sxs-lookup"><span data-stu-id="17f97-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="17f97-119">CPVs müssen ihre Anwendungen in Partner Center registrieren, um die Autorisierung für Partner Center-APIs zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="17f97-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="17f97-120">Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.</span><span class="sxs-lookup"><span data-stu-id="17f97-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="17f97-121">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="17f97-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="17f97-122">Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.</span><span class="sxs-lookup"><span data-stu-id="17f97-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="17f97-123">Der globale Administrator ist die einzige Rolle, die ein CPV haben kann.</span><span class="sxs-lookup"><span data-stu-id="17f97-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17f97-124">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="17f97-124">Next steps</span></span>

<span data-ttu-id="17f97-125">-[Hinzufügen zusätzlicher Mandanten zu Ihrem Partner Center Konto](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="17f97-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>