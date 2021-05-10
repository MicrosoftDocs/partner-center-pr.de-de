---
title: Behandeln von Problemen beim Einrichten Ihres Partner Center-Kontos oder der MPN-Verlängerung
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Behandeln von Problemen beim Versuch, sich bei Partner Center zu registrieren. Antworten behandeln Herausforderungen bei Zahlungsmethoden, vergessenen Kennwörtern und mehr.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686261"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="2c435-104">Behandeln von Problemen mit der Kontoeinrichtung oder MPN-Verlängerung</span><span class="sxs-lookup"><span data-stu-id="2c435-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="2c435-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="2c435-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2c435-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2c435-106">Global admin</span></span>
- <span data-ttu-id="2c435-107">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="2c435-107">MPN partner admin</span></span>
 
<span data-ttu-id="2c435-108">Hier finden Sie einige Vorschläge zur Behandlung häufiger Probleme, die beim Einrichten Ihres Partner Center-Kontos auftreten.</span><span class="sxs-lookup"><span data-stu-id="2c435-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="2c435-109">Was geschieht, wenn Sie von Partner Membership Center migrieren und keine Unternehmensinformationsfelder bearbeiten können?</span><span class="sxs-lookup"><span data-stu-id="2c435-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="2c435-110">In Fällen, in denen Ihr Unternehmen bereits in Partner Center (z. B. einem CSP-Konto) vorhanden ist, wird ihnen ein schreibgeschützter Bildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2c435-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="2c435-111">Auf diesem Bildschirm werden alle Informationen zu Ihrem Unternehmen angezeigt, die in Partner Center vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="2c435-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="2c435-112">Sie können die Details auf diesem Bildschirm nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="2c435-112">You can't change the details on this screen.</span></span> <span data-ttu-id="2c435-113">Dies ist entwurfshalber und kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="2c435-113">This is by design and not an error.</span></span>

<span data-ttu-id="2c435-114">Wählen Sie **Akzeptieren** und **Fortfahren** aus, um den Vorgang fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="2c435-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="2c435-115">Wenn die IT-Abteilung die **Registrierung für Partner Center** deaktiviert hat</span><span class="sxs-lookup"><span data-stu-id="2c435-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="2c435-116">Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder die virale Registrierung auf dem Azure AD Mandanten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2c435-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="2c435-117">Der globale Administrator für Ihr Azure AD-Konto kann die erforderlichen Features aktivieren, indem er den folgenden PowerShell-Befehl ausführt:</span><span class="sxs-lookup"><span data-stu-id="2c435-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="2c435-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="2c435-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="2c435-119">Weitere Informationen finden Sie unter [Self-Service-Registrierung.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="2c435-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="2c435-120">Sie haben Ihr Kennwort vergessen.</span><span class="sxs-lookup"><span data-stu-id="2c435-120">You forgot your password</span></span>

<span data-ttu-id="2c435-121">Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link Kann nicht auf **Ihr Konto zugreifen?** aus.</span><span class="sxs-lookup"><span data-stu-id="2c435-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="2c435-122">Mit dieser Option können Sie Ihr Kennwort zurücksetzen oder Ihren globalen Administrator bitten, Ihnen neue Anmeldeinformationen zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="2c435-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="2c435-123">Auf dem Bildschirm "Informieren Sie uns über Ihr Unternehmen" wird der Fehler "Es ist etwas schief gelaufen" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2c435-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="2c435-124">Diese Fehlermeldung wird normalerweise angezeigt, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercodes in Ihrer Unternehmenstelefonnummer verwenden.</span><span class="sxs-lookup"><span data-stu-id="2c435-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="2c435-125">Der im Feld Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="2c435-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="2c435-126">Für Ihren Kreditkartenkauf wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihre Bestellung abgelehnt wurde.</span><span class="sxs-lookup"><span data-stu-id="2c435-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="2c435-127">Überprüfen Sie Ihre Informationen."</span><span class="sxs-lookup"><span data-stu-id="2c435-127">Please verify your information”</span></span>


<span data-ttu-id="2c435-128">Verwenden Sie immer die Adresse, die Ihrer Kreditkarte und nicht Ihrer juristischen Person entspricht.</span><span class="sxs-lookup"><span data-stu-id="2c435-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="2c435-129">Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.</span><span class="sxs-lookup"><span data-stu-id="2c435-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="2c435-130">Sie möchten von der Offlinezahlung zur Onlinezahlungsmethode wechseln.</span><span class="sxs-lookup"><span data-stu-id="2c435-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="2c435-131">Sie müssen die ursprüngliche Bestellung und den ursprünglichen Wiederkauf mithilfe der bevorzugten Zahlungsmethode stornieren.</span><span class="sxs-lookup"><span data-stu-id="2c435-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="2c435-132">So stornieren Sie einen Auftrag:</span><span class="sxs-lookup"><span data-stu-id="2c435-132">To cancel an order:</span></span>

1. <span data-ttu-id="2c435-133">Wählen Sie **im Dashboard die** Registerkarte Mitgliedschaftsangebote aus.</span><span class="sxs-lookup"><span data-stu-id="2c435-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="2c435-134">Wählen Sie **Bestellung stornieren aus.**</span><span class="sxs-lookup"><span data-stu-id="2c435-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="2c435-135">Ein Bestätigungsfenster wird angezeigt, und Sie müssen bestätigen, um die erste Bestellung zu stornieren.</span><span class="sxs-lookup"><span data-stu-id="2c435-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2c435-136">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2c435-136">Next steps</span></span>

- [<span data-ttu-id="2c435-137">Verwalten des Partner Center-Kontos</span><span class="sxs-lookup"><span data-stu-id="2c435-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="2c435-138">Lesen Ihrer Rechnung und Abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="2c435-138">How to read your bill and recon file</span></span>](read-your-bill.md)
