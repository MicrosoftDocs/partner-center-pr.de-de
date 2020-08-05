---
title: Registrierung als Control Panel Vendor
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie Sie sich als System Steuerungs Anbieter (CPV) im Partner Center registrieren.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b6258f54120e0a40f94ad74a76821c4222eb0ef4
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/04/2020
ms.locfileid: "87545891"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="b788c-103">Registrieren als Anbieter der Systemsteuerung zur Unterstützung der Integration von CSP-Partnersystemen in Partner Center-APIs</span><span class="sxs-lookup"><span data-stu-id="b788c-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="b788c-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="b788c-104">**Applies to**</span></span>

- <span data-ttu-id="b788c-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="b788c-105">Partner Center</span></span>

<span data-ttu-id="b788c-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="b788c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b788c-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b788c-107">Global admin</span></span>

<span data-ttu-id="b788c-108">Ein Control Panel-Anbieter (Control Panel Vendor, CPV) ist ein unabhängiger Softwarehersteller, der Anwendungen für Cloud-Lösungsanbieter (Cloud Solution Provider, CSP) entwickelt, damit sie ihre Systeme in Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="b788c-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="b788c-109">Ein Control Panel-Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder die Partner Center-APIs.</span><span class="sxs-lookup"><span data-stu-id="b788c-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="b788c-110">Sowohl aktuelle Control Panel-Anbieter (Control Panel Vendor, CPV) als auch neue CPV, die mit Microsoft-Partnern zusammenarbeiten möchten, müssen sich gemäß den neuen Bestimmungen von Microsoft in Partner Center anmelden, um Ihre Anwendungen registrieren und Cloud Solution Provider-Partner zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b788c-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="b788c-111">Um ein Konto zu erstellen, können CPV-Partner einen vorhandenen CSP- oder CPV-Partnermandanten verwenden oder im Rahmen des Onboarding-Prozesses einen neuen Mandanten erstellen.</span><span class="sxs-lookup"><span data-stu-id="b788c-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="b788c-112">Wenn der CPV-Partner den vorhandenen CSP-Mandanten verwendet, muss er separate mehr Instanzen fähige Anwendungen erstellen und diese in Partner Center für CPV-Aktivitäten registrieren.</span><span class="sxs-lookup"><span data-stu-id="b788c-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="b788c-113">Eine Anwendung kann nicht als CSP-und CPV-Anwendung registriert werden.</span><span class="sxs-lookup"><span data-stu-id="b788c-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="b788c-114">Nachdem Sie sich in Partner Center angemeldet und Ihre Anwendungen registriert haben, können Sie auf Partner Center-APIs zugreifen.</span><span class="sxs-lookup"><span data-stu-id="b788c-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="b788c-115">Microsoft teilt Ihnen über eine Benachrichtigung in Partner Center Ihre Sandbox-Informationen mit.</span><span class="sxs-lookup"><span data-stu-id="b788c-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="b788c-116">Wenn Sie bereits über ein Sandbox Konto verfügen, verwenden Sie es weiter.</span><span class="sxs-lookup"><span data-stu-id="b788c-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="b788c-117">Sie benötigen keinen neuen Sandkasten.</span><span class="sxs-lookup"><span data-stu-id="b788c-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="b788c-118">Lesen Sie die [Vereinbarung für Microsoft Control Panel-Anbieter](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="b788c-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="b788c-119">Nutzung von Partner Center</span><span class="sxs-lookup"><span data-stu-id="b788c-119">Working in Partner Center</span></span>
<span data-ttu-id="b788c-120">Nachdem Sie sich beim Partner Center CPV-Prozess angemeldet und die CPV-Vereinbarung akzeptiert haben, können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="b788c-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="b788c-121">Verwalten von mehr Instanzen fähigen Anwendungen (Hinzufügen von Anwendungen zu Azure-Portal, registrieren und Aufheben der Registrierung von Anwendungen im Partner Center).</span><span class="sxs-lookup"><span data-stu-id="b788c-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="b788c-122">CPVs müssen ihre Anwendungen in Partner Center registrieren, um die Autorisierung für Partner Center-APIs zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="b788c-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="b788c-123">Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.</span><span class="sxs-lookup"><span data-stu-id="b788c-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="b788c-124">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="b788c-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="b788c-125">Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.</span><span class="sxs-lookup"><span data-stu-id="b788c-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="b788c-126">Der globale Administrator ist die einzige Rolle, die eine CPV aufweisen kann.</span><span class="sxs-lookup"><span data-stu-id="b788c-126">Global admin is the only role a CPV can have.</span></span>


