---
title: Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to confirm customer acceptance of the Microsoft Customer Agreement. This may be needed to order Microsoft products and services for customers.
author: LauraBrenner
ms.author: labrenne
keywords: Kunden, Kunden, Zustimmung, MCA, Microsoft Cloud-Vertrag, Microsoft-Kundenvertrag, Vorlagen für Kundenverträge
ms.localizationpriority: medium
ms.openlocfilehash: 9d362f581d0d318b1a457ba6a75db54713fce6bb
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252225"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirm customer acceptance of the Microsoft Customer Agreement

Currently, before a CSP partner can place order on a customer's behalf, the customer must accept and sign the applicable **Microsoft Cloud Agreement**. Anschließend muss der Partner seine Kundenzustimmung bestätigen, indem er Microsoft Informationen zum Signaturgeber zur Verfügung stellt. Wenn keine Bestätigung bereitgestellt wird:
- You won't be able to create new orders for this customer.
- You won't be able to change the seat count of existing seat-based subscriptions for this customer.

Weitere Informationen dazu, wie Sie die Zustimmung eines Kunden zum Microsoft Cloud-Vertrag über das Partner Center-Dashboard oder die entsprechende API bestätigen können, finden Sie unter [Bestätigen der Zustimmung des Kunden zum Microsoft Cloud-Vertrag](confirm-consent.md).

Am 1. Oktober 2019 stellt Microsoft den **Microsoft-Kundenvertrag** für das CSP-Programm vor, der den Microsoft Cloud-Vertrag ersetzt. Um die Migration von Partnern zum neuen Vertrag zu erleichtern, wird der aktuelle Microsoft Cloud-Vertrag noch bis zum 31. Januar 2020 im CSP-Programm unterstützt. Weitere Informationen zum zeitlichen Ablauf finden Sie in der folgenden Tabelle:

| Datum | Meilenstein | Details |
|------------|------------|--------------------------------|
|1\. August 2019|In Sandbox verfügbare UX-Vorschau|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center-Dashboard in der CSP-Sandboxumgebung bestätigen. Partner, die Zugriff auf die CSP-Sandboxumgebung haben, erhalten eine Vorschau auf die Änderungen bei der Benutzeroberfläche. Partner ohne Sandboxzugriff können sich in diesem Thema über die Änderungen informieren.|
|03. September 2019|In Sandbox verfügbare API-Vorschau|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über die Partner Center-API in der CSP-Sandboxumgebung bestätigen. API-Partner können diese Gelegenheit nutzen, um sich eine Vorschau der API-Änderungen anzusehen und mit der API-Integration zur Unterstützung des neuen Vertrags zu beginnen.|
|September 20, 2019|Vorschau des .NET SDK ist in Sandbox verfügbar.|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center .NET SDK in der CSP-Sandboxumgebung bestätigen. API-Partner können diese Gelegenheit nutzen, um sich eine Vorschau der Änderungen des .NET SDK anzusehen und mit der API-Integration zur Unterstützung des neuen Vertrags zu beginnen.|
|1\. Oktober 2019|Microsoft-Kundenvertrag in der Produktionsumgebung verfügbar|Microsoft stellt den Microsoft-Kundenvertrag für das CSP-Programm vor, der den Microsoft Cloud-Vertrag ersetzt. Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center-Dashboard und die entsprechende API in der Produktionsumgebung bestätigen. Der Microsoft Cloud-Vertrag wird innerhalb des CSP-Partnerprogramms weiterhin unterstützt. Partnern wird jedoch empfohlen, mit der Migration zum Microsoft-Kundenvertrag zu beginnen. Neue Käufe und Änderungen an der Anzahl der Arbeitsplätze für vorhandene Abonnements erfordern eine Bestätigung des Microsoft-Kundenvertrags oder des Microsoft Cloud-Vertrags durch den Partner. Bestimmte neue Angebote (z. B. der neue Azure-Plan) erfordern eine Bestätigung des Microsoft-Kundenvertrags.|
|31. Januar 2020|Microsoft Cloud-Vertrag aus der Produktionsumgebung entfernt|Der Microsoft Cloud-Vertrag wird innerhalb des CSP-Partnerprogramms nicht mehr akzeptiert. Neue Käufe und Änderungen an der Anzahl der Arbeitsplätze für vorhandene Abonnements erfordern eine Bestätigung des Microsoft-Kundenvertrags durch den Partner. Diese Anforderung gilt für neue Kunden und Bestandskunden, die möglicherweise zuvor den Microsoft Cloud-Vertrag angenommen haben.|

## <a name="access-microsoft-customer-agreement-template"></a>Access Microsoft Customer Agreement template
Partners can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement). Note that the Microsoft Customer Agreement is country-specific. When requesting for the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirm customer acceptance using Partner Center API/SDK
Partners can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement. For details on the API/SDK, please refer to:

- [Abrufen von Vertragsmetadaten für den Microsoft-Kundenvertrag](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Abrufen der Bestätigung der Zustimmung des Kunden zum Microsoft-Kundenvertrag](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Abrufen eines Downloadlinks für die Vorlage des Microsoft-Kundenvertrags](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>Bestätigen der Zustimmung des Kunden in Partner Center
Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new customers and existing customers.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Bestätigen der Kundenzustimmung für Neukunden

Wenn Sie in Partner Center einen Mandanten für einen Neukunden erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert hat. Um diese Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus.

2. Machen Sie unter **Kontoinformationen** Angaben zum Unternehmen und seinem primären Kontakt.

3. Wählen Sie unter **Microsoft-Vertrag** die Option **Microsoft-Kundenvertrag** aus.

4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind. Wenn diese nicht richtig sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat.

6. Wählen Sie **Weiter** aus, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.

![Neukunde](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Bestätigen der Kundenzustimmung für einen Bestandskunden

Um die folgenden Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein:

1. Wählen Sie **Kunden** aus. Suchen und wählen Sie den Kunden aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Wählen Sie unter **Microsoft-Kundenvertrag** die Option **Aktualisieren** aus.

4. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Wählen Sie **Speichern und fortfahren** aus.

![Bestandskunde](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Abrufen der Bestätigung der Kundenzustimmung für einen Bestandskunden

Mithilfe der folgenden Schritte können Sie eine Bestätigung abrufen, dass ein Bestandskunde den Microsoft-Kundenvertrag akzeptiert hat. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Unter **Microsoft-Kundenvertrag** wird angezeigt, ob die Bestätigung durch diesen Kunden erfolgt ist.
