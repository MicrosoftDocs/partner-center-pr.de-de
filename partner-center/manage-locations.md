---
title: Verwalten von Standorten im Partnerkonto
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925045"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="523ba-103">Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts</span><span class="sxs-lookup"><span data-stu-id="523ba-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="523ba-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="523ba-104">**Appropriate roles**</span></span>

- <span data-ttu-id="523ba-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="523ba-105">Global admin</span></span>
- <span data-ttu-id="523ba-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="523ba-106">Account admin</span></span>

<span data-ttu-id="523ba-107">Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="523ba-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="523ba-108">und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet.</span><span class="sxs-lookup"><span data-stu-id="523ba-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="523ba-109">Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).</span><span class="sxs-lookup"><span data-stu-id="523ba-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="523ba-110">Ein typisches Szenario:</span><span class="sxs-lookup"><span data-stu-id="523ba-110">The following is a typical scenario:</span></span>

<span data-ttu-id="523ba-111">Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich.</span><span class="sxs-lookup"><span data-stu-id="523ba-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="523ba-112">Dies ist das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet.</span><span class="sxs-lookup"><span data-stu-id="523ba-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="523ba-113">Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen.</span><span class="sxs-lookup"><span data-stu-id="523ba-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="523ba-114">In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt.</span><span class="sxs-lookup"><span data-stu-id="523ba-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="523ba-115">Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet.</span><span class="sxs-lookup"><span data-stu-id="523ba-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="523ba-116">Auszahlungen sind an spezifische Standorte gebunden.</span><span class="sxs-lookup"><span data-stu-id="523ba-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="523ba-117">Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.</span><span class="sxs-lookup"><span data-stu-id="523ba-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="523ba-119">Voraussetzungen für das Hinzufügen eines neuen Kontos für ein CSP-Geschäft</span><span class="sxs-lookup"><span data-stu-id="523ba-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="523ba-120">Zum Hinzufügen eines neuen CSP-Geschäftskontos müssen Sie zunächst sicherstellen, dass die Voraussetzungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="523ba-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="523ba-121">Sie müssen über eine Standort-MPN-ID in dem Land verfügen, in dem Sie CSP-Geschäfte tätigen möchten.</span><span class="sxs-lookup"><span data-stu-id="523ba-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="523ba-122">Wenn Sie einen neuen MPN-Standort erstellen möchten, lesen Sie „Hinzufügen eines MPN-Standorts“ weiter unten.</span><span class="sxs-lookup"><span data-stu-id="523ba-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="523ba-123">Wenn Sie eine neue CSP Indirect Reseller-Registrierung erstellen möchten, lesen Sie [Arbeiten mit indirekten Anbietern](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="523ba-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="523ba-124">Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für das **neue** CSP-Konto anzumelden.</span><span class="sxs-lookup"><span data-stu-id="523ba-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="523ba-125">Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.</span><span class="sxs-lookup"><span data-stu-id="523ba-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="523ba-126">Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.</span><span class="sxs-lookup"><span data-stu-id="523ba-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="523ba-127">Hinzufügen eines MPN-Standorts</span><span class="sxs-lookup"><span data-stu-id="523ba-127">Add an MPN location</span></span>

1. <span data-ttu-id="523ba-128">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="523ba-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="523ba-129">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="523ba-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="523ba-130">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="523ba-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="523ba-131">Wählen Sie über das Symbol **Einstellungen** die **Kontoeinstellungen** und dann **Organisationsprofil** aus.</span><span class="sxs-lookup"><span data-stu-id="523ba-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="523ba-132">Wählen Sie **Rechtliche Hinweise** und dann auf der Registerkarte **Partner** die Option **Geschäftsstandorte** aus. Klicken Sie anschließend auf **Standort hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="523ba-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="523ba-133">Geben Sie die erforderlichen Details einschließlich Firmenname, Adresse und Ansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="523ba-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="523ba-134">Klicken Sie auf **Standort hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="523ba-134">Click **Add location**.</span></span> <span data-ttu-id="523ba-135">Dadurch wird eine neue MPN-ID für den neuen Standort erstellt, die Sie für CSP-Transaktionen und -Incentives verwenden können.</span><span class="sxs-lookup"><span data-stu-id="523ba-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Hinzufügen eines neuen Rechtsgeschäfts":::

> [!NOTE]
> <span data-ttu-id="523ba-137">In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="523ba-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="523ba-138">Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.</span><span class="sxs-lookup"><span data-stu-id="523ba-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="523ba-139">Ändern des Lands für das globale Partnerkonto</span><span class="sxs-lookup"><span data-stu-id="523ba-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="523ba-140">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="523ba-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="523ba-141">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="523ba-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="523ba-142">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="523ba-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="523ba-143">Wechseln Sie auf der Registerkarte **Partner** zu **Geschäftsstandorte**, und prüfen Sie die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="523ba-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="523ba-144">Zum Hinzufügen eines Standorts klicken Sie auf **Standort hinzufügen**, und geben Sie im Flyout die erforderlichen Details einschließlich Firmenname, Adresse und Hauptansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="523ba-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="523ba-145">Wählen Sie neben der Dropdownliste **Land/Region** die Option **Land ändern** aus, und folgen Sie den angegebenen Schritten.</span><span class="sxs-lookup"><span data-stu-id="523ba-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Flyout mit Daten des Rechtsgeschäftsprofils":::

5. <span data-ttu-id="523ba-147">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="523ba-147">Click **Save**.</span></span>

6. <span data-ttu-id="523ba-148">Das Land des globalen MPN-Kontos wird in das neue rechtsgültige Land geändert.</span><span class="sxs-lookup"><span data-stu-id="523ba-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="523ba-149">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="523ba-149">Next steps</span></span>

- <span data-ttu-id="523ba-150">Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="523ba-150">Learn about the [verification process](verification-responses.md).</span></span>
