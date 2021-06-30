---
title: Registrieren Ihrer Angebote
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wenn Sie ein Angebot registrieren, das Sie in Partner Center gewonnen haben, bietet Microsoft Ihnen in Zukunft mehr Möglichkeiten.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080661"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registrieren von Abschlüssen, die Sie in Partner Center

**Geeignete Rollen**: Empfehlungsadministrator

Sie können die von Ihnen im Partner Center gewonnenen Angebote registrieren, indem Sie zusätzliche Informationen zum Vertrag bereitstellen. Diese Informationen helfen uns, Ihnen in Zukunft weitere Möglichkeiten zu bieten.

Es gibt zwei Pfade, die zur Dealregistrierung führen:

- Sie haben im Abschnitt **Co-Selling-Verkaufschancen** einen neuen Deal erstellt, und Ihr Deal erfüllt die Kriterien für die Dealregistrierung.
- Sie möchten einen geschlossenen ISV Connect-Deal melden, der nicht zusammen mit Microsoft verkauft wurde.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registrieren eines Deals, der aus einer Co-Selling-Verkaufschance stammt

Wenn Sie ein Angebot registrieren möchten, das von einer Co-Selling-Verkaufschance stammt, muss Ihr Deal die folgenden Berechtigungsanforderungen erfüllen:

- Der Dealtyp ist entweder Co-Selling oder partnergeführt (Sie haben sich entschieden, Microsoft-Verkäufern das Anzeigen dieses Deals zu erlauben).
- Es gibt mindestens eine Incentive-berechtigte Lösung im Deal. Eine Lösung ist incentivefähig, wenn sie mindestens eines der folgenden Tags enthält:
  - Azure IP Co-Selling
  - Business Applications Premium
  - Business Applications Standard
- Der Status des Deals lautet "Won".
- Wenn der Dealtyp Co-Selling ist, muss Microsoft entweder die Einladung angenommen oder den Deal als gewonnen markiert haben. Sie können den Microsoft-Status anzeigen, indem Sie sich die Microsoft-Karte unterHalb Ihrer Dealdetails ansehen.

Wenn Sie die Berechtigungsanforderungen erfüllt haben, werden Sie automatisch aufgefordert, Ihren Deal mit der Schaltfläche **Jetzt registrieren** zu registrieren, die auf der Statusleiste des Abschlusses angezeigt wird:

:::image type="content" source="images/register-deals.png" alt-text="Screenshot der Statusanzeige für den Deal":::

> [!NOTE]
> Wenn das **Registrierungselement "Deal"** nicht in der Statusanzeige für den Deal angezeigt wird, erfüllt der Deal nicht alle Anforderungen für die Dealregistrierung.

Nachdem Sie auf **Jetzt registrieren** geklickt haben, werden Sie zur Seite Deal Registration (Dealregistrierung) weitergeleitet und aufgefordert, ein Formular auszufüllen, das vorab ausgefüllte Informationen für Ihren Kunden und Ihre Lösung enthält. Füllen Sie das Formular mithilfe der folgenden Anweisungen aus, und klicken Sie auf **Registrieren.**

Bei der Registrierung werden je nach Lösung ein oder zwei Datensätze für die Dealregistrierung erstellt.

- Wenn Ihre Lösung für ISV Connect geeignet ist, wird ein ISV Connect-Dealregistrierungsdatensatz erstellt. Dieser Datensatz für die Dealregistrierung wird für die Rechnungsstellung verwendet.
- Wenn Ihre Lösung für IP-Co-Selling-Incentives berechtigt ist, wird ein Registrierungsdatensatz für den IP-Co-Selling-Deal erstellt. Dieser Datensatz für die Dealregistrierung wird vom Co-Selling-Deal-Prüfungsteam überprüft und genehmigt oder abgelehnt.

## <a name="report-a-closed-isv-connect-deal"></a>Melden eines geschlossenen ISV Connect-Abschlusses

Um einen geschlossenen ISV Connect-Deal zu melden, wechseln Sie zur Registerkarte **Deal registration (Dealregistrierung),** und klicken Sie auf **+ Geschlossenen ISV Connect-Deal** melden. Füllen Sie die erforderlichen Felder aus, und klicken Sie auf **Registrieren.** Dieser Datensatz für die Dealregistrierung wird für die Rechnungsstellung verwendet.

## <a name="fill-out-the-deal-registration-form"></a>Ausfüllen des Formulars für die Dealregistrierung

> [!NOTE]
> Sie können Deals nach Kundenname, Status und Dealtyp filtern. Klicken Sie hierzu oben auf der Seite Deal Registration (Dealregistrierung) auf die Schaltfläche **Filter** .

Unabhängig davon, ob Sie die Registrierung über eine Co-Selling-Verkaufschance abgeschlossen haben oder einen geschlossenen ISV Connect-Deal melden, der nicht mit Microsoft gemeinsam verkauft wurde, werden Sie aufgefordert, die folgenden Felder im Formular für die Dealregistrierung auszufüllen.

- **Kundendetails:** Geben Sie den **Unternehmensnamen** für Ihren Kunden ein, und wählen Sie **das Land/die Region** aus. Geben Sie dann **Stadt** und **Bundesland/Kanton** ein.
- **Lösung:** Wählen Sie die Lösung aus, die für den Deal verwendet wird. Wenn die richtige Lösung nicht angezeigt wird, wenden Sie sich an den Support.
- **Vertragstyp:** Geben Sie an, ob es sich bei diesem Deal um einen **neuen** Vertrag oder um eine **Verlängerung** eines vorherigen Vertrags handelt.
- **Gesamtvertragswert:** Der erwartete Gesamtwert für die Einbindung. Dieser Wert sollte alle Software- und Dienstgebühren enthalten, jedoch keine Hardwarekosten. Achten Sie darauf, dass Sie die entsprechende Währung auswählen.
- **Lösungswert:** Der Gesamtwert der Cloudlösung, die für den Deal verwendet wird. Stellen Sie sicher, dass Sie alle Kosten im Zusammenhang mit Software- und Wartungskosten einschließen, jedoch keine erstattungsfähigen Posten, einmalige Anpassungsgebühren oder direkt damit verbundene CSP-Lizenzgebühren, die von Microsoft bezahlt werden.
- **Wird die Lösung in Azure bereitgestellt? Falls nicht, wählen Sie Andere aus:** Wählen Sie entweder **Azure** oder **Andere** aus.
- **Wird die Nutzung der Lösung auf dem Partnermandanten oder Kundenmandanten ausgeführt?**: Wählen Sie entweder den **Kundenmandanten** oder den **Partnermandanten** aus.
- **Startdatum** des Vertrags: Das Datum, an dem der Vertrag beginnt. Verwenden Sie für Nutzungsbasierte Bezahlung (Pay-As-You-Go, PAYG) das Datum der ersten Rechnung. Standardmäßig lässt Partner Center nicht zu, dass Sie ein Startdatum vor dem Vertragsabschlussdatum eingeben. Dies kann sich auf einige Deals auswirken, z. B. IP-Bereitstellungen, die vor dem Signierungsdatum beginnen. Um diese Deals erfolgreich einzugeben, verwenden Sie beim Übermitteln das Vertragsabschlussdatum sowohl für das Vorzeichen als **auch** für das Startdatum. (Der Vertrag sollte die Dauer des Geschäftsabschlusses explizit angeben, damit ACV ordnungsgemäß berechnet werden kann.)
- **Enddatum** des Vertrags: Wenn der Vertrag an einem bestimmten Datum endet, wählen Sie **Hat ein Enddatum** aus, und geben Sie dieses Datum an. Wenn der Vertrag kein bestimmtes Enddatum hat, wählen Sie **Unbefristet** aus. Verwenden Sie für Nutzungsbasierte Bezahlung (Pay-As-You-Go, PAYG) das Datum der letzten oder letzten Rechnung.
- **Vertragssigniertes Datum:** Das Datum, an dem der endgültige Vertrag von Ihrer Organisation und vom Kunden unterzeichnet wurde. Verwenden Sie für Nutzungsbasierte Bezahlung (Pay-As-You-Go, PAYG) das Datum der ersten Rechnung.
- **Registrierungskontakt:** **Vorname,** **Nachname,** Telefonnummer und **E-Mail-Adresse** für eine Person in Ihrer Organisation, an die wir uns wenden können, wenn wir weitere Details zu den hier bereitgestellten Informationen benötigen. 

Wenn Sie alle Abschnitte der Seite abgeschlossen haben, klicken Sie auf **Registrieren.**

- Wenn es sich bei dem Deal um einen ISV Connect-Deal handelt, werden Sie feststellen, dass der Status des Abschlusses "Übermittelt, Abgeschlossen" lautet. Für diesen Dealregistrierungsdatensatz ist keine weitere Aktion erforderlich. Dieser Datensatz wird für die Rechnungsstellung verwendet.
- Wenn es sich bei dem Deal um einen IP-Co-Selling-Deal handelt, werden Sie feststellen, dass der Status des Geschäfts "Übermittelt" lautet. Das Microsoft Co-Selling Deal Review-Team überprüft die Informationen, die Sie in diesem Datensatz für die Dealregistrierung angegeben haben. Das Überprüfungsteam fordert bei Bedarf weitere Maßnahmen von Ihnen an oder genehmigt/lehnt den Deal direkt ab.
- Wenn Sie einen Deal registrieren, der von einer Co-Selling-Verkaufschance stammt, und Sie sehen, dass zwei Datensätze für die Dealregistrierung erstellt wurden, bedeutet dies, dass die Lösung für Ihren Deal sowohl für ISV Connect als auch für DEN IP-Co-Selling geeignet ist. Der ISV Connect-Datensatz wird für die Rechnungsstellung verwendet. Der IP-Co-Selling-Datensatz wird vom Co-Selling-Dealvalidierungsteam überprüft.

