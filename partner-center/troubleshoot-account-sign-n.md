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
ms.openlocfilehash: 403899b73dda09dded582c94cabe4219ef56c568
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000614"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="bb129-103">Behandeln von Problemen mit der Konto Einrichtung oder der MPN-Erneuerung</span><span class="sxs-lookup"><span data-stu-id="bb129-103">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="bb129-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="bb129-104">**Applies to**</span></span>

- <span data-ttu-id="bb129-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="bb129-105">Partner Center</span></span>
 
<span data-ttu-id="bb129-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="bb129-106">**Appropriate roles**</span></span>

- <span data-ttu-id="bb129-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="bb129-107">Global admin</span></span>
- <span data-ttu-id="bb129-108">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="bb129-108">MPN partner admin</span></span> 
 
<span data-ttu-id="bb129-109">Hier finden Sie einige Vorschläge zur Problembehandlung bei häufigen Problemen, die beim Einrichten Ihres Partner Center-Kontos auftreten.</span><span class="sxs-lookup"><span data-stu-id="bb129-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="bb129-110">Was geschieht, wenn Sie vom Partner Mitgliedschafts Center migrieren und keine Firmen Informationsfelder bearbeiten können.</span><span class="sxs-lookup"><span data-stu-id="bb129-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="bb129-111">In Fällen, in denen Ihr Unternehmen bereits in Partner Center (z. –. CSP-Konto) vorhanden ist, wird Ihnen ein Schreib geschützter Bildschirm angezeigt, auf dem alle Informationen zu Ihrem Unternehmen angezeigt werden, wie es im Partner Center vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="bb129-111">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="bb129-112">Die Details auf diesem Bildschirm können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bb129-112">You can't change the details on this screen.</span></span> <span data-ttu-id="bb129-113">Dies ist Entwurfs bedingt und kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="bb129-113">This is by design and not an error.</span></span>

<span data-ttu-id="bb129-114">Wählen Sie **annehmen** und **fort** fahren aus.</span><span class="sxs-lookup"><span data-stu-id="bb129-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="bb129-115">, Wenn die IT-Abteilung die **Anmeldung für Partner Center**ausgeschaltet hat.</span><span class="sxs-lookup"><span data-stu-id="bb129-115">If the IT department has turned off **sign up for Partner Center**.</span></span>


<span data-ttu-id="bb129-116">Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder die virale Registrierung für den Azure AD Mandanten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="bb129-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="bb129-117">Der globale Administrator für Ihr Azure AD Konto kann erforderliche Features aktivieren, indem Sie den folgenden PowerShell-Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="bb129-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="bb129-118">**Set-msolcompanysettings-zustellwemailverifiedusers $true-allowadhocabonnements $true**</span><span class="sxs-lookup"><span data-stu-id="bb129-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="bb129-119">Weitere Informationen finden Sie [unter Self-Service](/azure/active-directory/users-groups-roles/directory-self-service-signup) -Registrierung.</span><span class="sxs-lookup"><span data-stu-id="bb129-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="bb129-120">Sie haben Ihr Kennwort vergessen.</span><span class="sxs-lookup"><span data-stu-id="bb129-120">You forgot your password</span></span>

<span data-ttu-id="bb129-121">Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link **kein Zugriff auf Ihr Konto?** aus, um Ihr Kennwort zurückzusetzen, oder bitten Sie Ihren globalen Administrator, Ihnen neue Anmelde Informationen zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="bb129-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="bb129-122">Auf dem Bildschirm "erzählen Sie uns von Ihrem Unternehmen" erhalten Sie den Fehler "ein Fehler ist aufgetreten".</span><span class="sxs-lookup"><span data-stu-id="bb129-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="bb129-123">Diese Fehlermeldung wird normalerweise angezeigt, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercode in der Telefonnummer Ihres Unternehmens verwenden.</span><span class="sxs-lookup"><span data-stu-id="bb129-123">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="bb129-124">Der im Feld für die Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="bb129-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="bb129-125">Ihr Kreditkarten Erwerb erhält eine Fehlermeldung, die besagt, dass Ihre Bestellung abgelehnt wurde.</span><span class="sxs-lookup"><span data-stu-id="bb129-125">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="bb129-126">Überprüfen Sie Ihre Informationen "</span><span class="sxs-lookup"><span data-stu-id="bb129-126">Please verify your information”</span></span>


<span data-ttu-id="bb129-127">Verwenden Sie immer die Adresse, die Ihrer Kreditkarte entspricht, anstelle ihrer juristischen Person.</span><span class="sxs-lookup"><span data-stu-id="bb129-127">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="bb129-128">Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.</span><span class="sxs-lookup"><span data-stu-id="bb129-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="bb129-129">Sie möchten von der Offline Zahlung zur Online Zahlungsmethode wechseln.</span><span class="sxs-lookup"><span data-stu-id="bb129-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="bb129-130">Sie müssen die ursprüngliche Bestellung abbrechen und mithilfe der bevorzugten Zahlungsmethode erneut erwerben.</span><span class="sxs-lookup"><span data-stu-id="bb129-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="bb129-131">So brechen Sie eine Bestellung ab</span><span class="sxs-lookup"><span data-stu-id="bb129-131">To cancel an order:</span></span>

1. <span data-ttu-id="bb129-132">Wählen Sie im Dashboard die Registerkarte **mitgliedschaftsangebote** aus.</span><span class="sxs-lookup"><span data-stu-id="bb129-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="bb129-133">Select- **Reihenfolge Abbrechen**</span><span class="sxs-lookup"><span data-stu-id="bb129-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="bb129-134">Es wird ein Bestätigungsfenster angezeigt, das Sie bestätigen müssen, um die anfängliche Reihenfolge abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="bb129-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bb129-135">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="bb129-135">Next steps</span></span>

- [<span data-ttu-id="bb129-136">Verwalten des Partner Center-Kontos</span><span class="sxs-lookup"><span data-stu-id="bb129-136">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="bb129-137">So lesen Sie Ihre Rechnung und die Datei "Reconnaissance"</span><span class="sxs-lookup"><span data-stu-id="bb129-137">How to read your bill and recon file</span></span>](read-your-bill.md)