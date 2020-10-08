---
title: Verwalten von Standorten im Partnerkonto
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663895"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="f68e3-103">Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts</span><span class="sxs-lookup"><span data-stu-id="f68e3-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="f68e3-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="f68e3-104">**Applies to**</span></span>

- <span data-ttu-id="f68e3-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="f68e3-105">Partner Center</span></span>

<span data-ttu-id="f68e3-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="f68e3-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f68e3-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="f68e3-107">Global admin</span></span>
- <span data-ttu-id="f68e3-108">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="f68e3-108">Account admin</span></span>

<span data-ttu-id="f68e3-109">Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="f68e3-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="f68e3-110">und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet.</span><span class="sxs-lookup"><span data-stu-id="f68e3-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="f68e3-111">Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).</span><span class="sxs-lookup"><span data-stu-id="f68e3-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="f68e3-112">Ein typisches Szenario:</span><span class="sxs-lookup"><span data-stu-id="f68e3-112">The following is a typical scenario:</span></span>

<span data-ttu-id="f68e3-113">Contoso hat seinen globalen Partnerkontostandort (Partner Global Account, PGA) im Vereinigten Königreich.</span><span class="sxs-lookup"><span data-stu-id="f68e3-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="f68e3-114">Dies ist das registrierte Unternehmen, das über eine einzelne MPN-ID verfügt, die für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f68e3-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="f68e3-115">Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen.</span><span class="sxs-lookup"><span data-stu-id="f68e3-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="f68e3-116">In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt.</span><span class="sxs-lookup"><span data-stu-id="f68e3-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="f68e3-117">Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet.</span><span class="sxs-lookup"><span data-stu-id="f68e3-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="f68e3-118">Auszahlungen sind an spezifische Standorte gebunden.</span><span class="sxs-lookup"><span data-stu-id="f68e3-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="f68e3-119">Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.</span><span class="sxs-lookup"><span data-stu-id="f68e3-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="f68e3-121">Voraussetzungen für das Hinzufügen eines neuen Standorts für ein CSP-Geschäft</span><span class="sxs-lookup"><span data-stu-id="f68e3-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="f68e3-122">Zum Hinzufügen eines neuen CSP-Geschäftsstandorts müssen mehrere Voraussetzungen erfüllt sein:</span><span class="sxs-lookup"><span data-stu-id="f68e3-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="f68e3-123">Sie müssen über eine Standort-MPN-ID in dem Land verfügen, in dem Sie geschäftlich tätig sein möchten.</span><span class="sxs-lookup"><span data-stu-id="f68e3-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="f68e3-124">Sie benötigen einen neuen Azure AD-Mandanten in der Geschäftsregion, der nicht bereits in CSP registriert ist.</span><span class="sxs-lookup"><span data-stu-id="f68e3-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="f68e3-125">Erstellen Sie diesen bei der Registrierung in CSP.</span><span class="sxs-lookup"><span data-stu-id="f68e3-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="f68e3-126">Verwenden Sie den neuen AAD-Mandanten, um sich beim CSP-Programm in der Region zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="f68e3-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="f68e3-127">Geben Sie rechtliche Firmendetails an, einschließlich des rechtsgültigen Firmennamens, der Adresse sowie Angaben zum primären Kontakt.</span><span class="sxs-lookup"><span data-stu-id="f68e3-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="f68e3-128">Dieses Konto wird überprüft. Stellen Sie daher sicher, dass Sie gültige Informationen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f68e3-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="f68e3-129">Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für den **neuen** Azure AD-Mandanten anzumelden.</span><span class="sxs-lookup"><span data-stu-id="f68e3-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="f68e3-130">Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.</span><span class="sxs-lookup"><span data-stu-id="f68e3-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="f68e3-131">Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.</span><span class="sxs-lookup"><span data-stu-id="f68e3-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="f68e3-132">Hinzufügen eines Standorts</span><span class="sxs-lookup"><span data-stu-id="f68e3-132">Add a location</span></span>

1. <span data-ttu-id="f68e3-133">Wählen Sie das **Einstellungssymbol** und anschließend die **Partnereinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="f68e3-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="f68e3-134">Wählen Sie **Standorte** aus.</span><span class="sxs-lookup"><span data-stu-id="f68e3-134">Select **Locations.**</span></span>

3. <span data-ttu-id="f68e3-135">Wählen Sie **Standort hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="f68e3-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="f68e3-136">Fügen Sie auf der Seite **Standort hinzufügen** die Adressdetails des Standorts ein, den Sie Ihrem Unternehmen hinzufügen möchten, und geben Sie auch einen Hauptansprechpartner für den Standort an.</span><span class="sxs-lookup"><span data-stu-id="f68e3-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="f68e3-137">In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="f68e3-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="f68e3-138">Ändern des globalen Partnerkontostandorts</span><span class="sxs-lookup"><span data-stu-id="f68e3-138">Change Global partner account location</span></span>

1. <span data-ttu-id="f68e3-139">Überprüfen Sie auf der Seite **Standorte** die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="f68e3-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="f68e3-140">Wenn dies nicht der Fall ist, fügen Sie ihn hinzu.</span><span class="sxs-lookup"><span data-stu-id="f68e3-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Struktur von MPN-Standorten":::

2. <span data-ttu-id="f68e3-142">Wählen Sie **Partnerprofil** aus, und wählen Sie dann **Firmenprofil aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="f68e3-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Struktur von MPN-Standorten":::

3. <span data-ttu-id="f68e3-144">Wählen Sie die Region und die juristische Entität aus, und klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="f68e3-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Struktur von MPN-Standorten":::

## <a name="next-steps"></a><span data-ttu-id="f68e3-146">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f68e3-146">Next steps</span></span>

- <span data-ttu-id="f68e3-147">Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="f68e3-147">Learn about the [verification process](verification-responses.md).</span></span>
