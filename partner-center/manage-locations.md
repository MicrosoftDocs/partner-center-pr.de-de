---
title: Verwalten von Standorten im Partnerkonto
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514797"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="bdf01-103">Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts</span><span class="sxs-lookup"><span data-stu-id="bdf01-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="bdf01-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="bdf01-104">**Applies to**</span></span>

- <span data-ttu-id="bdf01-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="bdf01-105">Partner Center</span></span>

<span data-ttu-id="bdf01-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="bdf01-106">**Appropriate roles**</span></span>

- <span data-ttu-id="bdf01-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="bdf01-107">Global admin</span></span>
- <span data-ttu-id="bdf01-108">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="bdf01-108">Account admin</span></span>

<span data-ttu-id="bdf01-109">Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="bdf01-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="bdf01-110">und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet.</span><span class="sxs-lookup"><span data-stu-id="bdf01-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="bdf01-111">Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).</span><span class="sxs-lookup"><span data-stu-id="bdf01-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="bdf01-112">Ein typisches Szenario:</span><span class="sxs-lookup"><span data-stu-id="bdf01-112">The following is a typical scenario:</span></span>

<span data-ttu-id="bdf01-113">Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich.</span><span class="sxs-lookup"><span data-stu-id="bdf01-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="bdf01-114">Dies ist das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet.</span><span class="sxs-lookup"><span data-stu-id="bdf01-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="bdf01-115">Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen.</span><span class="sxs-lookup"><span data-stu-id="bdf01-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="bdf01-116">In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt.</span><span class="sxs-lookup"><span data-stu-id="bdf01-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="bdf01-117">Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet.</span><span class="sxs-lookup"><span data-stu-id="bdf01-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="bdf01-118">Auszahlungen sind an spezifische Standorte gebunden.</span><span class="sxs-lookup"><span data-stu-id="bdf01-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="bdf01-119">Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.</span><span class="sxs-lookup"><span data-stu-id="bdf01-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="bdf01-121">Voraussetzungen für das Hinzufügen eines neuen Standorts für ein CSP-Geschäft</span><span class="sxs-lookup"><span data-stu-id="bdf01-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="bdf01-122">Zum Hinzufügen eines neuen CSP-Geschäftsstandorts müssen mehrere Voraussetzungen erfüllt sein:</span><span class="sxs-lookup"><span data-stu-id="bdf01-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="bdf01-123">Sie müssen über eine Standort-MPN-ID in dem Land/der Region verfügen, in dem/der Sie geschäftlich tätig sein möchten.</span><span class="sxs-lookup"><span data-stu-id="bdf01-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="bdf01-124">Sie benötigen einen neuen Azure AD-Mandanten in der [Geschäftsregion](regional-authorization-overview.md), der nicht bereits in CSP registriert ist.</span><span class="sxs-lookup"><span data-stu-id="bdf01-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="bdf01-125">Erstellen Sie diesen bei der Registrierung in CSP.</span><span class="sxs-lookup"><span data-stu-id="bdf01-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="bdf01-126">Verwenden Sie den neuen AAD-Mandanten, um sich beim CSP-Programm in der Region zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="bdf01-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="bdf01-127">Geben Sie rechtliche Firmendetails an, einschließlich des rechtsgültigen Firmennamens, der Adresse sowie Angaben zum primären Kontakt.</span><span class="sxs-lookup"><span data-stu-id="bdf01-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="bdf01-128">Dieses Konto wird überprüft. Stellen Sie daher sicher, dass Sie gültige Informationen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="bdf01-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="bdf01-129">Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für den **neuen** Azure AD-Mandanten anzumelden.</span><span class="sxs-lookup"><span data-stu-id="bdf01-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="bdf01-130">Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.</span><span class="sxs-lookup"><span data-stu-id="bdf01-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="bdf01-131">Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.</span><span class="sxs-lookup"><span data-stu-id="bdf01-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="bdf01-132">Fügen Sie einen Standort für das MPN hinzu.</span><span class="sxs-lookup"><span data-stu-id="bdf01-132">Add an MPN location</span></span>

1. <span data-ttu-id="bdf01-133">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="bdf01-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="bdf01-134">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="bdf01-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="bdf01-135">Wählen Sie das **Einstellungssymbol** und anschließend die **Organisationseinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="bdf01-135">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="bdf01-136">Wählen Sie **Rechtliche Hinweise** und dann **Standorte** aus.</span><span class="sxs-lookup"><span data-stu-id="bdf01-136">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="bdf01-137">Wählen Sie **Standort hinzufügen** aus, und fügen Sie die Adressdetails des Standorts ein, den Sie Ihrem Unternehmen hinzufügen möchten. Geben Sie auch einen Hauptansprechpartner für den Standort an.</span><span class="sxs-lookup"><span data-stu-id="bdf01-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="bdf01-138">In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="bdf01-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="bdf01-139">Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.</span><span class="sxs-lookup"><span data-stu-id="bdf01-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="bdf01-140">Ändern des globalen Partnerkontostandorts</span><span class="sxs-lookup"><span data-stu-id="bdf01-140">Change Global partner account location</span></span>

1. <span data-ttu-id="bdf01-141">Überprüfen Sie auf der Seite **[Geschäftsstandorte](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="bdf01-141">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="bdf01-142">Wenn dies nicht der Fall ist, fügen Sie ihn hinzu.</span><span class="sxs-lookup"><span data-stu-id="bdf01-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Screenshot: Liste aller aktuellen Standorte auf der Seite mit den Standorten für Partner Center-Konten":::

2. <span data-ttu-id="bdf01-144">Wählen Sie **Rechtliche Hinweise** aus, und wählen Sie dann **Firmenprofil aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="bdf01-144">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="bdf01-145">Wählen Sie die Region und die juristische Entität aus, und klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="bdf01-145">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="bdf01-146">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="bdf01-146">Next steps</span></span>

- <span data-ttu-id="bdf01-147">Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="bdf01-147">Learn about the [verification process](verification-responses.md).</span></span>
