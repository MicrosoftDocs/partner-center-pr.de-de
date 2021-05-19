---
title: Erzwingung des Kreditlimits
ms.topic: how-to
ms.date: 05/11/2021
description: Erfahren Sie mehr über Ihr Kreditlimit und seine Berechnung. Enthält häufig gestellte Fragen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148107"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="fb710-104">Erzwingung von Kreditlimits (CREDIT Limit Enforcement, CLE)</span><span class="sxs-lookup"><span data-stu-id="fb710-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="fb710-105">**Geeignete Rollen:** Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="fb710-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="fb710-106">Ihr Guthabenlimit und seine Funktionsweise</span><span class="sxs-lookup"><span data-stu-id="fb710-106">Your credit limit and how it works</span></span>

<span data-ttu-id="fb710-107">Ihr Guthabenlimit ist der maximale Betrag (in US-Dollar), den Sie als Partner für den Erwerb von Produkten oder Abonnements in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="fb710-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="fb710-108">Wenn Sie Ihr Guthabenlimit überschreiten, können Sie erst dann neue Käufe tätigen, wenn eine ausreichende Zahlung erfolgt ist.</span><span class="sxs-lookup"><span data-stu-id="fb710-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="fb710-109">Ihre vorhandenen Abonnements bleiben ohne Unterbrechung erhalten.</span><span class="sxs-lookup"><span data-stu-id="fb710-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="fb710-110">Guthabenlimits gelten für Angebote in Azure-Plänen, Azure-Reservierungen, Software, Marketplace, Azure 145 P, Office und Dynamics-Produkten.</span><span class="sxs-lookup"><span data-stu-id="fb710-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="fb710-111">Guthabenlimits gelten nicht für Verlängerungen und den laufenden Verbrauch.</span><span class="sxs-lookup"><span data-stu-id="fb710-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="fb710-112">Wir weisen Ihr Guthabenlimit während des Onboardingzeitraums auf Mandantenebene zu.</span><span class="sxs-lookup"><span data-stu-id="fb710-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="fb710-113">Wir stützen uns auf Ihren prognostizierten Umsatz, Ihre Kaufprognose und Ihren Zahlungsverlauf.</span><span class="sxs-lookup"><span data-stu-id="fb710-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="fb710-114">Anschließend verwenden wir die folgende Formel, um Ihren verfügbaren Saldo zu berechnen:</span><span class="sxs-lookup"><span data-stu-id="fb710-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="fb710-115">**[Kreditlimit – (Eingehender Kauf + ausstehende Rechnungen für Rechnungen und nicht berechnete Gebühren – Überzahlung)]**</span><span class="sxs-lookup"><span data-stu-id="fb710-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="fb710-116">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="fb710-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="fb710-117">Ist mein Guthabenlimit auf Mandanten- oder globaler Ebene festgelegt?</span><span class="sxs-lookup"><span data-stu-id="fb710-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="fb710-118">Die Mandantenebene.</span><span class="sxs-lookup"><span data-stu-id="fb710-118">The tenant level.</span></span> <span data-ttu-id="fb710-119">Angenommen, Sie arbeiten aus den USA, Kanada und Japan.</span><span class="sxs-lookup"><span data-stu-id="fb710-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="fb710-120">Wenn der kanadische Mandant sein Kreditlimit erreicht, erhält dieser Mandant eine Benachrichtigung, wenn er versucht, einen Kauf in einem Partner Center.</span><span class="sxs-lookup"><span data-stu-id="fb710-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="fb710-121">Die anderen Mandanten sind nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="fb710-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="fb710-122">Kann ich bestehende Kunden und Abonnements mit Vollzugriff weiter warten, wenn ich mein Guthabenlimit überschreitet?</span><span class="sxs-lookup"><span data-stu-id="fb710-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="fb710-123">Ja.</span><span class="sxs-lookup"><span data-stu-id="fb710-123">Yes.</span></span> <span data-ttu-id="fb710-124">Die vorhandenen Abonnements Ihrer Kunden werden ohne Unterbrechung fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="fb710-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="fb710-125">Sie können jedoch keine neuen Abonnements für Ihre Kunden erwerben.</span><span class="sxs-lookup"><span data-stu-id="fb710-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="fb710-126">Gilt CLE sowohl für Partner mit direkter Abrechnung als auch für indirekte Anbieter?</span><span class="sxs-lookup"><span data-stu-id="fb710-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="fb710-127">Ja, dies gilt für beide.</span><span class="sxs-lookup"><span data-stu-id="fb710-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="fb710-128">Wann kann ich nach dem Übermitteln meiner Zahlung zur Wiederherstellung meines Kontos weitere Abonnements erwerben?</span><span class="sxs-lookup"><span data-stu-id="fb710-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="fb710-129">Sie sollten in der Lage sein, den Kauf innerhalb von 24 Stunden nach Ihrer Zahlung fortzusetzen, vorausgesetzt, Microsoft hat alle Anforderungen zum Fortsetzen des Kreditprüfungsprozesses erhalten.</span><span class="sxs-lookup"><span data-stu-id="fb710-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="fb710-130">Wie kann ich mein Guthabenlimit überprüfen?</span><span class="sxs-lookup"><span data-stu-id="fb710-130">How can I check my credit limit?</span></span>

<span data-ttu-id="fb710-131">Wenden Sie [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) sich an , um Ihr Guthabenlimit anzuzeigen und Informationen zu kürzlich erworbenen Käufen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="fb710-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="fb710-132">Werden rechnungen, die in Konflikt stehen, gegen das Guthabenlimit angerechnet?</span><span class="sxs-lookup"><span data-stu-id="fb710-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="fb710-133">Ja.</span><span class="sxs-lookup"><span data-stu-id="fb710-133">Yes.</span></span> <span data-ttu-id="fb710-134">Sie können sich jedoch unter an Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) wenden, um das Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="fb710-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="fb710-135">Wie schnell höre ich zurück, wenn ich in ucmwrcsp@microsoft.com schreibe?</span><span class="sxs-lookup"><span data-stu-id="fb710-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="fb710-136">Sie sollten in weniger als 24 Stunden eine Antwort erhalten.</span><span class="sxs-lookup"><span data-stu-id="fb710-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="fb710-137">Welche Kriterien verwendet Microsoft zum Festlegen des Kreditlimits eines Partners?</span><span class="sxs-lookup"><span data-stu-id="fb710-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="fb710-138">Wir bestimmen Ihr Kreditlimit basierend auf Ihren prognostizierten Umsätzen, kaufbezogenen Vorteilen und dem Zahlungsverlauf.</span><span class="sxs-lookup"><span data-stu-id="fb710-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="fb710-139">Wird das Guthabenlimit derzeit für die neue Commerce-Benutzeroberfläche erzwungen?</span><span class="sxs-lookup"><span data-stu-id="fb710-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="fb710-140">Ja.</span><span class="sxs-lookup"><span data-stu-id="fb710-140">Yes.</span></span> <span data-ttu-id="fb710-141">Guthabenlimits gelten für alle CSP-Programme und -Produkte in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="fb710-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="fb710-142">Wer erhält die Benachrichtigung, wenn sich meine Organisation dem Kreditlimit nähert?</span><span class="sxs-lookup"><span data-stu-id="fb710-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="fb710-143">Die Benachrichtigung sollte vom Finanzkonto-Kontakt Ihrer Organisation empfangen werden.</span><span class="sxs-lookup"><span data-stu-id="fb710-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fb710-144">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="fb710-144">Next steps</span></span>

[<span data-ttu-id="fb710-145">Grundlagen zur Abrechnung</span><span class="sxs-lookup"><span data-stu-id="fb710-145">Billing basics</span></span>](./billing-basics.md)
