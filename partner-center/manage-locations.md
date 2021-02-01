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
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098889"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="a46fc-103">Verwalten von MPN-Kontostandorten und Hinzufügen eines neuen Standorts</span><span class="sxs-lookup"><span data-stu-id="a46fc-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="a46fc-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="a46fc-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a46fc-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="a46fc-105">Global admin</span></span>
- <span data-ttu-id="a46fc-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="a46fc-106">Account admin</span></span>

<span data-ttu-id="a46fc-107">Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="a46fc-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="a46fc-108">und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet.</span><span class="sxs-lookup"><span data-stu-id="a46fc-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="a46fc-109">Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).</span><span class="sxs-lookup"><span data-stu-id="a46fc-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="a46fc-110">Ein typisches Szenario:</span><span class="sxs-lookup"><span data-stu-id="a46fc-110">The following is a typical scenario:</span></span>

<span data-ttu-id="a46fc-111">Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich.</span><span class="sxs-lookup"><span data-stu-id="a46fc-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="a46fc-112">Dies ist das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet.</span><span class="sxs-lookup"><span data-stu-id="a46fc-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="a46fc-113">Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen.</span><span class="sxs-lookup"><span data-stu-id="a46fc-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="a46fc-114">In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt.</span><span class="sxs-lookup"><span data-stu-id="a46fc-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="a46fc-115">Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet.</span><span class="sxs-lookup"><span data-stu-id="a46fc-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="a46fc-116">Auszahlungen sind an spezifische Standorte gebunden.</span><span class="sxs-lookup"><span data-stu-id="a46fc-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="a46fc-117">Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.</span><span class="sxs-lookup"><span data-stu-id="a46fc-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="a46fc-119">Voraussetzungen für das Hinzufügen eines neuen Kontos für ein CSP-Geschäft</span><span class="sxs-lookup"><span data-stu-id="a46fc-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="a46fc-120">Zum Hinzufügen eines neuen CSP-Geschäftskontos müssen Sie zunächst sicherstellen, dass die Voraussetzungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="a46fc-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="a46fc-121">Sie müssen über eine Standort-MPN-ID in dem Land verfügen, in dem Sie CSP-Geschäfte tätigen möchten.</span><span class="sxs-lookup"><span data-stu-id="a46fc-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="a46fc-122">Wenn Sie einen neuen MPN-Standort erstellen möchten, lesen Sie „Hinzufügen eines MPN-Standorts“ weiter unten.</span><span class="sxs-lookup"><span data-stu-id="a46fc-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="a46fc-123">Wenn Sie eine neue CSP Indirect Reseller-Registrierung erstellen möchten, lesen Sie [Arbeiten mit indirekten Anbietern](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="a46fc-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="a46fc-124">Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für das **neue** CSP-Konto anzumelden.</span><span class="sxs-lookup"><span data-stu-id="a46fc-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="a46fc-125">Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.</span><span class="sxs-lookup"><span data-stu-id="a46fc-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="a46fc-126">Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.</span><span class="sxs-lookup"><span data-stu-id="a46fc-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="a46fc-127">Anzeigen Ihrer MPN-Standorte</span><span class="sxs-lookup"><span data-stu-id="a46fc-127">View your MPN locations</span></span>

1. <span data-ttu-id="a46fc-128">Melden Sie sich mit den Anmeldeinformationen für Ihr MPN-Konto beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home) an.</span><span class="sxs-lookup"><span data-stu-id="a46fc-128">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="a46fc-129">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="a46fc-129">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="a46fc-130">Wählen Sie über das Symbol **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Rechtliche Hinweise** aus.</span><span class="sxs-lookup"><span data-stu-id="a46fc-130">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="a46fc-131">Vergewissern Sie sich, dass auf der Registerkarte **Partner** keine Fehlermeldung im Banner angezeigt wird, in der Sie dazu aufgefordert werden, von PMC migrierte Standorte zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="a46fc-131">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="a46fc-132">Wenn dies der Fall ist, befolgen Sie die Anweisungen, und korrigieren Sie diese Standorte.</span><span class="sxs-lookup"><span data-stu-id="a46fc-132">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="a46fc-133">Wird keine Fehlermeldung angezeigt, wählen Sie unter **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Bezeichner** aus.</span><span class="sxs-lookup"><span data-stu-id="a46fc-133">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="a46fc-134">Suchen Sie nach der MPN-ID mit dem Typ „Standort“, der dem Land dieses CSP-Kontos entspricht, und verwenden Sie sie für die folgende Suche und um die Zuordnung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="a46fc-134">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="a46fc-135">Wenn Sie die Standort-MPN-ID, die dem zu verwendenden CSP-Konto entspricht, nicht finden, können Sie einen neuen Standort hinzufügen, um eine neue MPN-ID zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="a46fc-135">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="a46fc-136">Weitere Informationen finden Sie im folgenden Abschnitt **Hinzufügen eines MPN-Standorts**.</span><span class="sxs-lookup"><span data-stu-id="a46fc-136">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="a46fc-137">Hinzufügen eines MPN-Standorts</span><span class="sxs-lookup"><span data-stu-id="a46fc-137">Add an MPN location</span></span>

1. <span data-ttu-id="a46fc-138">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="a46fc-138">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a46fc-139">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="a46fc-139">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a46fc-140">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="a46fc-140">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="a46fc-141">Wählen Sie über das Symbol **Einstellungen** die **Kontoeinstellungen** und dann **Organisationsprofil** aus.</span><span class="sxs-lookup"><span data-stu-id="a46fc-141">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="a46fc-142">Wählen Sie **Rechtliche Hinweise** und dann auf der Registerkarte **Partner** die Option **Geschäftsstandorte** aus. Klicken Sie anschließend auf **Standort hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="a46fc-142">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="a46fc-143">Geben Sie die erforderlichen Details einschließlich Firmenname, Adresse und Ansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="a46fc-143">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="a46fc-144">Klicken Sie auf **Standort hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="a46fc-144">Click **Add location**.</span></span> <span data-ttu-id="a46fc-145">Dadurch wird eine neue MPN-ID für den neuen Standort erstellt, die Sie für CSP-Transaktionen und -Incentives verwenden können.</span><span class="sxs-lookup"><span data-stu-id="a46fc-145">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Hinzufügen eines neuen Rechtsgeschäfts":::

> [!NOTE]
> <span data-ttu-id="a46fc-147">In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="a46fc-147">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="a46fc-148">Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a46fc-148">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="a46fc-149">Ändern des Lands für das globale Partnerkonto</span><span class="sxs-lookup"><span data-stu-id="a46fc-149">Change country of Partner global account</span></span> 

1. <span data-ttu-id="a46fc-150">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="a46fc-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a46fc-151">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="a46fc-151">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a46fc-152">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="a46fc-152">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="a46fc-153">Wechseln Sie auf der Registerkarte **Partner** zu **Geschäftsstandorte**, und prüfen Sie die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="a46fc-153">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="a46fc-154">Zum Hinzufügen eines Standorts klicken Sie auf **Standort hinzufügen**, und geben Sie im Flyout die erforderlichen Details einschließlich Firmenname, Adresse und Hauptansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="a46fc-154">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="a46fc-155">Wählen Sie neben der Dropdownliste **Land/Region** die Option **Land ändern** aus, und folgen Sie den angegebenen Schritten.</span><span class="sxs-lookup"><span data-stu-id="a46fc-155">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Flyout mit Daten des Rechtsgeschäftsprofils":::

5. <span data-ttu-id="a46fc-157">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="a46fc-157">Click **Save**.</span></span>

6. <span data-ttu-id="a46fc-158">Das Land des globalen MPN-Kontos wird in das neue rechtsgültige Land geändert.</span><span class="sxs-lookup"><span data-stu-id="a46fc-158">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="a46fc-159">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="a46fc-159">Next steps</span></span>

- <span data-ttu-id="a46fc-160">Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="a46fc-160">Learn about the [verification process](verification-responses.md).</span></span>
