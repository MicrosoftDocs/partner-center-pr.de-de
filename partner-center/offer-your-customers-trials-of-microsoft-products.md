---
title: Anbieten von Testversionen von Microsoft-Produkten für Kunden | Partner Center
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ihre Kunden können Microsoft-Abonnementprodukte 30 Tage lang testen. Sie können sich für diese Testversionen im Katalog ebenso wie für viele andere Onlinedienste registrieren.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384832"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Anbieten von Testversionen von Microsoft-Produkten für Kunden

Betrifft

- Partner Center

Eine kostenlose 30-Tage-Testversion ist eine gute Möglichkeit, Kunden neue Microsoft-Produkte vorzustellen. Sie können sich für die Testversionen im Katalog ebenso wie für viele andere Onlinedienste registrieren. Alle Partner können daran teilnehmen.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. Sie können z. B. eine kostenlose Testversion für Office 365 Business Premium und eine kostenlose Testversion für Office 365 E3 erhalten. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

Kostenlose Testversionen sind für folgende Produkte verfügbar:

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Plan 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Wir bieten kostenlose Testversionen für diese Produkte an, da sie die umfassendsten und beliebtesten Angebote für Unternehmen sind. Wir werden in Zukunft möglicherweise weitere kostenlose Testversionen anbieten.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. Navigieren Sie im Partner Center unter **Verkaufen** zu **Katalog**. 
2. Klicken Sie im Katalog unter **Billing frequency** (Abrechnungshäufigkeit) auf **Trial offer** (Testangebot). Dadurch werden nur kostenlose Testversionen angezeigt und kostenpflichtige Angebote ausgeblendet. Testversionen werden im Katalog auf der Registerkarte **Testversionen** angezeigt.
3. Wählen Sie die kostenlose Testversion aus, die Sie anbieten möchten, und wählen Sie dann **Übermitteln** aus. Alle Testversionen gelten für 30 Tage, in denen keine Kosten in Rechnung gestellt werden. Sie können sie auch zu einem beliebigen Zeitpunkt während des Testzeitraums in ein kostenpflichtiges Abonnement umwandeln.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. Wählen Sie auf der Abonnementseite des Kunden die kostenlose Testversion aus.
2. Wählen Sie **Testabonnement auf kostenpflichtiges Abonnement umstellen** aus.
3. Geben Sie die gewünschte Anzahl von Lizenzen und die Abrechnungshäufigkeit ein, und wählen Sie **Übernehmen** aus.
4. Die Abrechnung für das kostenpflichtige Abonnement beginnt mit dem Datum der Umstellung, und das Abonnement wird automatisch zwölf Monate nach der Umstellung verlängert. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [Umwandeln eines Probeabonnements in ein kostenpflichtiges Abonnement](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Abrufen einer Liste der Wechselangebote für Probeabonnements](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. Sie sollten diese Datumsangaben regemäßig überprüfen, damit Sie zusammen mit dem Kunden die entsprechenden Folgeaktionen durchführen können, wenn eine Entscheidung getroffen werden muss.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>Abrechnung

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit jährlicher Abrechnung umgewandelt wird, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem Datum der Umwandlung. Wird die kostenlose Testversion in ein kostenpflichtiges Angebot mit monatlicher Abrechnung umgewandelt, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem auf das Datum der Umwandlung folgenden Abrechnungsdatum.

### <a name="invoices"></a>Rechnungen

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>Incentives

Free trials do not have an impact on incentives.

## <a name="support"></a>Support

For support on free trials, submit a service request through Partner Center.
