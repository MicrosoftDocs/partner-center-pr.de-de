---
title: Problembehandlung beim Einrichten Ihres Partner Center-Kontos oder der MPN-Erneuerungs Probleme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Beheben von Problemen bei der Anmeldung in Partner Center
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1d850663224469f24d5d4442e33cc17c1bb6704
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220238"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="7ee82-103">Behandeln von Problemen mit der Konto Einrichtung oder der MPN-Erneuerung</span><span class="sxs-lookup"><span data-stu-id="7ee82-103">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="7ee82-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="7ee82-104">**Applies to**</span></span>

- <span data-ttu-id="7ee82-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="7ee82-105">Partner Center</span></span>
 
<span data-ttu-id="7ee82-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="7ee82-106">**Appropriate roles**</span></span>

- <span data-ttu-id="7ee82-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7ee82-107">Global admin</span></span>
- <span data-ttu-id="7ee82-108">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="7ee82-108">MPN partner admin</span></span> 
 
<span data-ttu-id="7ee82-109">Hier finden Sie einige Vorschläge zur Problembehandlung bei häufigen Problemen, die beim Einrichten Ihres Partner Center-Kontos auftreten.</span><span class="sxs-lookup"><span data-stu-id="7ee82-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="7ee82-110">Was geschieht, wenn Sie vom Partner Mitgliedschafts Center migrieren und keine Firmen Informationsfelder bearbeiten können.</span><span class="sxs-lookup"><span data-stu-id="7ee82-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="7ee82-111">Dies tritt auf, wenn Ihr Unternehmen bereits in Partner Center (z. –. CSP-Konto) vorhanden ist Ihnen wird ein Schreib geschützter Bildschirm angezeigt, auf dem alle Informationen zu Ihrem Unternehmen angezeigt werden, wie es im Partner Center vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="7ee82-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="7ee82-112">Die Details auf diesem Bildschirm können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7ee82-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="7ee82-113">Dies ist Entwurfs bedingt und kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="7ee82-113">This is by design and not an error.</span></span>

<span data-ttu-id="7ee82-114">Wählen Sie **annehmen** und **fort** fahren aus.</span><span class="sxs-lookup"><span data-stu-id="7ee82-114">Select **Accept** and **Continue** to proceed.</span></span>

## <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="7ee82-115">Sie versuchen, sich zu registrieren oder aus dem Partner Membership Center zu migrieren, und Sie erhalten eine Fehlermeldung, die besagt, dass die IT-Abteilung die Registrierung **für Partner Center**ausgeschaltet hat.</span><span class="sxs-lookup"><span data-stu-id="7ee82-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="7ee82-116">Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder die virale Registrierung für den Azure AD Mandanten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="7ee82-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="7ee82-117">Der globale Administrator für Ihr Azure AD Konto kann erforderliche Features aktivieren, indem Sie den folgenden PowerShell-Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="7ee82-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="7ee82-118">**Set-msolcompanysettings-zustellwemailverifiedusers $true-allowadhocabonnements $true**</span><span class="sxs-lookup"><span data-stu-id="7ee82-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="7ee82-119">Weitere Informationen finden Sie [unter Self-Service](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) -Registrierung.</span><span class="sxs-lookup"><span data-stu-id="7ee82-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="7ee82-120">Sie haben Ihr Kennwort vergessen.</span><span class="sxs-lookup"><span data-stu-id="7ee82-120">You forgot your password</span></span>

<span data-ttu-id="7ee82-121">Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link **kein Zugriff auf Ihr Konto?** aus, um Ihr Kennwort zurückzusetzen, oder bitten Sie Ihren globalen Administrator, Ihnen neue Anmelde Informationen zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="7ee82-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="7ee82-122">Auf dem Bildschirm "erzählen Sie uns von Ihrem Unternehmen" erhalten Sie den Fehler "ein Fehler ist aufgetreten".</span><span class="sxs-lookup"><span data-stu-id="7ee82-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="7ee82-123">Dies geschieht normalerweise, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercode in der Telefonnummer Ihres Unternehmens verwenden.</span><span class="sxs-lookup"><span data-stu-id="7ee82-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="7ee82-124">Der im Feld für die Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="7ee82-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

## <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="7ee82-125">Sie versuchen, den Kauf über die Kreditkarte abzuschließen, aber Sie erhalten eine Fehlermeldung mit dem Hinweis, dass die Bestellung abgelehnt wurde.</span><span class="sxs-lookup"><span data-stu-id="7ee82-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="7ee82-126">Überprüfen Sie Ihre Informationen "</span><span class="sxs-lookup"><span data-stu-id="7ee82-126">Please verify your information”</span></span>

<span data-ttu-id="7ee82-127">Sie sollten immer die Adresse Ihrer Kreditkarte einfügen, die ihrer juristischen Person nicht entspricht.</span><span class="sxs-lookup"><span data-stu-id="7ee82-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="7ee82-128">Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.</span><span class="sxs-lookup"><span data-stu-id="7ee82-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="7ee82-129">Sie möchten von der Offline Zahlung zur Online Zahlungsmethode wechseln.</span><span class="sxs-lookup"><span data-stu-id="7ee82-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="7ee82-130">Sie müssen die ursprüngliche Bestellung abbrechen und mithilfe der bevorzugten Zahlungsmethode erneut erwerben.</span><span class="sxs-lookup"><span data-stu-id="7ee82-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="7ee82-131">So brechen Sie eine Bestellung ab</span><span class="sxs-lookup"><span data-stu-id="7ee82-131">To cancel an order:</span></span>

1. <span data-ttu-id="7ee82-132">Wählen Sie im Dashboard die Registerkarte **mitgliedschaftsangebote** aus.</span><span class="sxs-lookup"><span data-stu-id="7ee82-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="7ee82-133">Select- **Reihenfolge Abbrechen**</span><span class="sxs-lookup"><span data-stu-id="7ee82-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="7ee82-134">Es wird ein Bestätigungsfenster angezeigt, das Sie bestätigen müssen, um die anfängliche Reihenfolge abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="7ee82-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
