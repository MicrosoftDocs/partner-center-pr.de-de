---
title: Durchsetzung des Kreditlimits
ms.topic: how-to
ms.date: 05/11/2021
description: Erfahren Sie mehr über Ihr Kreditlimit und seine Berechnung. Enthält häufig gestellte Fragen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819208"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="3c84a-104">Erzwingung von Kreditlimits (CREDIT Limit Enforcement, CLE)</span><span class="sxs-lookup"><span data-stu-id="3c84a-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="3c84a-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="3c84a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3c84a-106">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="3c84a-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="3c84a-107">Ihr Guthabenlimit und seine Funktionsweise</span><span class="sxs-lookup"><span data-stu-id="3c84a-107">Your credit limit and how it works</span></span>

<span data-ttu-id="3c84a-108">Ihr Guthabenlimit ist der maximale Betrag (in US-Dollar), den Sie als Partner für den Erwerb von Produkten oder Abonnements in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3c84a-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="3c84a-109">Wenn Sie Ihr Guthabenlimit überschreiten, können Sie erst dann neue Käufe tätigen, wenn eine ausreichende Zahlung erfolgt ist.</span><span class="sxs-lookup"><span data-stu-id="3c84a-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="3c84a-110">Ihre vorhandenen Abonnements bleiben ohne Unterbrechung erhalten.</span><span class="sxs-lookup"><span data-stu-id="3c84a-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="3c84a-111">Guthabenlimits gelten für Angebote in Azure-Plänen, Azure-Reservierungen, Software, Marketplace, Azure 145 P, Office und Dynamics-Produkten.</span><span class="sxs-lookup"><span data-stu-id="3c84a-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="3c84a-112">Guthabenlimits gelten nicht für Verlängerungen und den fortlaufenden Verbrauch.</span><span class="sxs-lookup"><span data-stu-id="3c84a-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="3c84a-113">Wir weisen Ihr Guthabenlimit während des Onboardingzeitraums auf Mandantenebene zu.</span><span class="sxs-lookup"><span data-stu-id="3c84a-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="3c84a-114">Wir stützen uns auf Ihren prognostizierten Umsatz, Ihre Kaufprognose und Ihren Zahlungsverlauf.</span><span class="sxs-lookup"><span data-stu-id="3c84a-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="3c84a-115">Anschließend verwenden wir die folgende Formel, um Ihren verfügbaren Saldo zu berechnen:</span><span class="sxs-lookup"><span data-stu-id="3c84a-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="3c84a-116">**[Kreditlimit – (Eingehender Kauf + ausstehende Rechnungen für Rechnungen und nicht berechnete Gebühren – Überzahlung)]**</span><span class="sxs-lookup"><span data-stu-id="3c84a-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="3c84a-117">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="3c84a-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="3c84a-118">Ist mein Guthabenlimit auf Mandanten- oder globaler Ebene festgelegt?</span><span class="sxs-lookup"><span data-stu-id="3c84a-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="3c84a-119">Die Mandantenebene.</span><span class="sxs-lookup"><span data-stu-id="3c84a-119">The tenant level.</span></span> <span data-ttu-id="3c84a-120">Angenommen, Sie arbeiten aus den USA, Kanada und Japan.</span><span class="sxs-lookup"><span data-stu-id="3c84a-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="3c84a-121">Wenn der kanadische Mandant sein Kreditlimit erreicht, erhält dieser Mandant eine Benachrichtigung, wenn er versucht, einen Kauf in einem Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3c84a-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="3c84a-122">Die anderen Mandanten sind nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="3c84a-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="3c84a-123">Kann ich bestehende Kunden und Abonnements mit Vollzugriff weiter warten, wenn ich mein Guthabenlimit überschreitet?</span><span class="sxs-lookup"><span data-stu-id="3c84a-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="3c84a-124">Ja.</span><span class="sxs-lookup"><span data-stu-id="3c84a-124">Yes.</span></span> <span data-ttu-id="3c84a-125">Die vorhandenen Abonnements Ihrer Kunden werden ohne Unterbrechung fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="3c84a-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="3c84a-126">Sie können jedoch keine neuen Abonnements für Ihre Kunden erwerben.</span><span class="sxs-lookup"><span data-stu-id="3c84a-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="3c84a-127">Gilt CLE sowohl für Partner mit direkter Abrechnung als auch für indirekte Anbieter?</span><span class="sxs-lookup"><span data-stu-id="3c84a-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="3c84a-128">Ja, dies gilt für beide.</span><span class="sxs-lookup"><span data-stu-id="3c84a-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="3c84a-129">Wann kann ich nach dem Übermitteln meiner Zahlung zur Wiederherstellung meines Kontos weitere Abonnements erwerben?</span><span class="sxs-lookup"><span data-stu-id="3c84a-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="3c84a-130">Sie sollten in der Lage sein, den Kauf innerhalb von 24 Stunden nach Ihrer Zahlung fortzusetzen, vorausgesetzt, Microsoft hat alle Anforderungen zum Fortsetzen des Kreditprüfungsprozesses erhalten.</span><span class="sxs-lookup"><span data-stu-id="3c84a-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="3c84a-131">Wie kann ich mein Guthabenlimit überprüfen?</span><span class="sxs-lookup"><span data-stu-id="3c84a-131">How can I check my credit limit?</span></span>

<span data-ttu-id="3c84a-132">Wenden Sie [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) sich an , um Ihr Guthabenlimit anzuzeigen und Informationen zu kürzlich erworbenen Käufen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="3c84a-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="3c84a-133">Werden rechnungen, die in Konflikt stehen, gegen das Guthabenlimit angerechnet?</span><span class="sxs-lookup"><span data-stu-id="3c84a-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="3c84a-134">Ja.</span><span class="sxs-lookup"><span data-stu-id="3c84a-134">Yes.</span></span> <span data-ttu-id="3c84a-135">Sie können sich jedoch unter an Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) wenden, um das Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="3c84a-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="3c84a-136">Wie schnell höre ich zurück, wenn ich in ucmwrcsp@microsoft.com schreibe?</span><span class="sxs-lookup"><span data-stu-id="3c84a-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="3c84a-137">Sie sollten in weniger als 24 Stunden eine Antwort erhalten.</span><span class="sxs-lookup"><span data-stu-id="3c84a-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="3c84a-138">Welche Kriterien verwendet Microsoft zum Festlegen des Kreditlimits eines Partners?</span><span class="sxs-lookup"><span data-stu-id="3c84a-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="3c84a-139">Wir bestimmen Ihr Kreditlimit basierend auf Ihren prognostizierten Umsätzen, kaufbezogenen Vorteilen und dem Zahlungsverlauf.</span><span class="sxs-lookup"><span data-stu-id="3c84a-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="3c84a-140">Wird das Guthabenlimit derzeit für die neue Commerce-Benutzeroberfläche erzwungen?</span><span class="sxs-lookup"><span data-stu-id="3c84a-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="3c84a-141">Ja.</span><span class="sxs-lookup"><span data-stu-id="3c84a-141">Yes.</span></span> <span data-ttu-id="3c84a-142">Guthabenlimits gelten für alle CSP-Programme und -Produkte in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3c84a-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="3c84a-143">Wer erhält die Benachrichtigung, wenn sich meine Organisation dem Kreditlimit nähert?</span><span class="sxs-lookup"><span data-stu-id="3c84a-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="3c84a-144">Die Benachrichtigung sollte vom Finanzkonto-Kontakt Ihrer Organisation empfangen werden.</span><span class="sxs-lookup"><span data-stu-id="3c84a-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3c84a-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="3c84a-145">Next steps</span></span>

[<span data-ttu-id="3c84a-146">Grundlagen zur Abrechnung</span><span class="sxs-lookup"><span data-stu-id="3c84a-146">Billing basics</span></span>](./billing-basics.md)
