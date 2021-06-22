---
title: Behandeln von Problemen beim Einrichten Ihres Partner Center kontos oder der MPN-Verlängerung
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Behandeln von Problemen beim Versuch, sich bei einem Partner Center. Antworten auf Herausforderungen bei Zahlungsmethoden, das Vergessen von Kennwörtern und mehr.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431749"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="d0927-104">Behandeln von Problemen bei der Kontoeinrichtung oder MPN-Verlängerung</span><span class="sxs-lookup"><span data-stu-id="d0927-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="d0927-105">**Geeignete Rollen:** Globale Administratorrechte | MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="d0927-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="d0927-106">Hier finden Sie einige Vorschläge zur Behandlung häufiger Probleme, die beim Einrichten Ihres Kontos Partner Center auftreten.</span><span class="sxs-lookup"><span data-stu-id="d0927-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="d0927-107">Was geschieht, wenn Sie von einem Partner Membership Center und keine Felder für Unternehmensinformationen bearbeiten können?</span><span class="sxs-lookup"><span data-stu-id="d0927-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="d0927-108">In Fällen, in denen Ihr Unternehmen bereits in Partner Center (z. B. einem Cloud Solution Provider-Konto (CSP)) vorhanden ist, wird ihnen ein schreibgeschützter Bildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d0927-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="d0927-109">Auf diesem Bildschirm werden alle Informationen zu Ihrem Unternehmen angezeigt, wie es in der Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0927-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="d0927-110">Sie können die Details auf diesem Bildschirm nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="d0927-110">You can't change the details on this screen.</span></span> <span data-ttu-id="d0927-111">Dies ist entwurfsweise und kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="d0927-111">This is by design and not an error.</span></span>

<span data-ttu-id="d0927-112">Um fortzufahren, wählen **Sie Akzeptieren** und dann **Weiter aus.**</span><span class="sxs-lookup"><span data-stu-id="d0927-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="d0927-113">Wenn die IT-Abteilung die Anmeldung für die **Partner Center**</span><span class="sxs-lookup"><span data-stu-id="d0927-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="d0927-114">Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder weil die virale Anmeldung auf dem Azure Active Directory-Mandanten (AD) deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d0927-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="d0927-115">Der globale Administrator für Ihr Azure AD-Konto kann erforderliche Features aktivieren, indem er den folgenden PowerShell-Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="d0927-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="d0927-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="d0927-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="d0927-117">Weitere Informationen finden Sie unter [Self-Service-Anmeldung.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="d0927-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="d0927-118">Sie haben Ihr Kennwort vergessen.</span><span class="sxs-lookup"><span data-stu-id="d0927-118">You forgot your password</span></span>

<span data-ttu-id="d0927-119">Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite Die Option **Kann nicht auf Ihr Konto zugreifen? aus.**</span><span class="sxs-lookup"><span data-stu-id="d0927-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="d0927-120">Mit dieser Option können Sie Ihr Kennwort zurücksetzen oder Ihren globalen Administrator bitten, Ihnen neue Anmeldeinformationen zu zuweisen.</span><span class="sxs-lookup"><span data-stu-id="d0927-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="d0927-121">Auf dem Bildschirm "Informieren Sie uns über Ihr Unternehmen" wird der Fehler "Es ist ein Fehler aufgetreten" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d0927-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="d0927-122">Diese Fehlermeldung wird normalerweise angezeigt, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercodes in Ihrer Unternehmenstelefonnummer verwenden.</span><span class="sxs-lookup"><span data-stu-id="d0927-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="d0927-123">Der im Feld Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="d0927-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="d0927-124">Für Ihren Kreditkartenkauf wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihre Bestellung abgelehnt wurde.</span><span class="sxs-lookup"><span data-stu-id="d0927-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="d0927-125">Überprüfen Sie Ihre Informationen."</span><span class="sxs-lookup"><span data-stu-id="d0927-125">Please verify your information”</span></span>


<span data-ttu-id="d0927-126">Verwenden Sie immer die Adresse, die Ihrer Kreditkarte und nicht Ihrer juristischen Person entspricht.</span><span class="sxs-lookup"><span data-stu-id="d0927-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="d0927-127">Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.</span><span class="sxs-lookup"><span data-stu-id="d0927-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="d0927-128">Sie möchten von der Offlinezahlung zur Onlinezahlungsmethode wechseln.</span><span class="sxs-lookup"><span data-stu-id="d0927-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="d0927-129">Sie müssen die ursprüngliche Bestellung und den ursprünglichen Wiederkauf mithilfe der bevorzugten Zahlungsmethode stornieren.</span><span class="sxs-lookup"><span data-stu-id="d0927-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="d0927-130">So stornieren Sie eine Bestellung:</span><span class="sxs-lookup"><span data-stu-id="d0927-130">To cancel an order:</span></span>

1. <span data-ttu-id="d0927-131">Wählen Sie Partner Center Dashboard die Registerkarte **Mitgliedschaftsangebote** aus.</span><span class="sxs-lookup"><span data-stu-id="d0927-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="d0927-132">Wählen Sie **Bestellung stornieren aus.**</span><span class="sxs-lookup"><span data-stu-id="d0927-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="d0927-133">Ein Bestätigungsfenster wird angezeigt, und Sie müssen bestätigen, um die erste Bestellung zu stornieren.</span><span class="sxs-lookup"><span data-stu-id="d0927-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0927-134">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d0927-134">Next steps</span></span>

- [<span data-ttu-id="d0927-135">Verwalten des Partner Center-Kontos</span><span class="sxs-lookup"><span data-stu-id="d0927-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="d0927-136">Lesen Ihrer Rechnung und Abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="d0927-136">How to read your bill and recon file</span></span>](read-your-bill.md)
