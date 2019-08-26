---
title: Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag | Partner Center
ms.topic: article
ms.date: 04/16/2019
Description: Als Partner müssen Sie die Zustimmung Ihres Kunden zum Microsoft-Kundenvertrag einholen, bevor Sie Microsoft-Produkte und -Dienste für diesen Kunden bestellen können. Um Partner bei der Einhaltung von Complianceanforderungen zu unterstützen, bittet Microsoft die Partner, die Zustimmung durch Bereitstellung bestimmter Details zu der Person, die dem Vertrag zugestimmt hat, zu bestätigen.
author: LauraBrenner
ms.author: labrenne
keywords: Kunden, Kunden, Zustimmung, MCA, Microsoft Cloud-Vertrag, Microsoft-Kundenvertrag, Vorlagen für Kundenverträge
ms.localizationpriority: medium
ms.openlocfilehash: 295c997baa43dd087552315d71d726a0f28c6ed1
ms.sourcegitcommit: 0712e68734f0b3e53821b490a6c32a6c991a6e49
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2019
ms.locfileid: "69871775"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag (Vorschauphase)

Bevor ein CSP-Partner eine Bestellung im Auftrag eines Kunden aufgeben können, muss der Kunde derzeit den entsprechenden **Microsoft Cloud-Vertrag** akzeptieren und unterzeichnen. Anschließend muss der Partner seine Zustimmung bestätigen, indem er Microsoft Informationen über den Signaturgeber zur Verfügung stellt. Wenn ein Kunde seine Zustimmung zum Microsoft Cloud-Vertrag nicht bestätigt:
- Können Sie für diesen Kunden keine neuen Aufträge erstellen.
- Können Sie die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierter Abonnements für diesen Kunden nicht ändern.

Weitere Informationen dazu, wie Sie die Zustimmung eines Kunden zum Microsoft Cloud-Vertrag über das Partner Center-Dashboard oder die entsprechende API bestätigen können, finden Sie unter [Bestätigen der Zustimmung des Kunden zum Microsoft Cloud-Vertrag](confirm-consent.md).

Am 1. Oktober 2019 stellt Microsoft den **Microsoft-Kundenvertrag** für das CSP-Programm vor, der den Microsoft Cloud-Vertrag ersetzt. Um die Migration von Partnern zum neuen Vertrag zu erleichtern, wird der aktuelle Microsoft Cloud-Vertrag noch bis zum 31. Januar 2019 im CSP-Programm unterstützt. Weitere Informationen zum zeitlichen Ablauf finden Sie in der folgenden Tabelle:

| Datum | Meilenstein | Details |
|------------|------------|--------------------------------|
|1\. August 2019|In Sandbox verfügbare UX-Vorschau|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center-Dashboard in der CSP-Sandboxumgebung bestätigen. Partner, die Zugriff auf die CSP-Sandboxumgebung haben, erhalten eine Vorschau auf die Änderungen bei der Benutzeroberfläche. Partner ohne Sandboxzugriff können sich in diesem Thema über die Änderungen informieren.|
|2\. September 2019|In Sandbox verfügbare API-Vorschau|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über die Partner Center-API in der CSP-Sandboxumgebung bestätigen. API-Partner können diese Gelegenheit nutzen, um sich eine Vorschau der API-Änderungen anzusehen und mit der API-Integration zur Unterstützung des neuen Vertrags zu beginnen.|
|1\. Oktober 2019|Microsoft-Kundenvertrag in der Produktionsumgebung verfügbar|Microsoft stellt den Microsoft-Kundenvertrag für das CSP-Programm vor, der den Microsoft Cloud-Vertrag ersetzt. Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center-Dashboard und die entsprechende API in der Produktionsumgebung bestätigen. Der Microsoft Cloud-Vertrag wird innerhalb des CSP-Partnerprogramms weiterhin unterstützt. Partnern wird jedoch empfohlen, mit der Migration zum Microsoft-Kundenvertrag zu beginnen. Neue Käufe und Änderungen an der Anzahl der Arbeitsplätze für vorhandene Abonnements erfordern eine Bestätigung des Microsoft-Kundenvertrags oder des Microsoft Cloud-Vertrags durch den Partner. Bestimmte neue Angebote (z. B. der neue Azure-Plan) erfordern eine Bestätigung des Microsoft-Kundenvertrags.|
|31. Januar 2019|Microsoft Cloud-Vertrag aus der Produktionsumgebung entfernt|Der Microsoft Cloud-Vertrag wird innerhalb des CSP-Partnerprogramms nicht mehr akzeptiert. Neue Käufe und Änderungen an der Anzahl der Arbeitsplätze für vorhandene Abonnements erfordern eine Bestätigung des Microsoft-Kundenvertrags durch den Partner. Diese Anforderung gilt für neue Kunden und Bestandskunden, die möglicherweise zuvor den Microsoft Cloud-Vertrag angenommen haben.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Bestätigen der Kundenzustimmung für Neukunden

Wenn Sie in Partner Center einen Mandanten für einen Neukunden erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert hat. Um diese Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus.

2. Machen Sie unter **Kontoinformationen** Angaben zum Unternehmen und seinem primären Kontakt.

3. Wählen Sie unter **Microsoft-Vertrag** die Option **Microsoft-Kundenvertrag** aus.

4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind. Wenn diese nicht richtig sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat.

6. Wählen Sie **Weiter** aus, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.

![Neukunde](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Bestätigen der Kundenzustimmung für einen Bestandskunden

Um die folgenden Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein:

1. Wählen Sie **Kunden** aus. Suchen und wählen Sie den Kunden aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Wählen Sie unter **Microsoft-Kundenvertrag** die Option **Aktualisieren** aus.

4. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Wählen Sie **Speichern und fortfahren** aus.

![Bestandskunde](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Abrufen der Bestätigung der Kundenzustimmung für einen Bestandskunden

Mithilfe der folgenden Schritte können Sie eine Bestätigung abrufen, dass ein Bestandskunde den Microsoft-Kundenvertrag akzeptiert hat. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Unter **Microsoft-Kundenvertrag** wird angezeigt, ob die Bestätigung durch diesen Kunden erfolgt ist.


