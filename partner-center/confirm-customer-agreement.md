---
title: Bestätigen Sie die kundenannahme des Microsoft-Kunden Vertrags | Partner Center
ms.topic: article
ms.date: 04/16/2019
Description: Als Partner müssen Sie die Zustimmung Ihres Kunden zum Microsoft-Kundenvertrag einholen, bevor Sie Microsoft-Produkte und-Dienste für diesen Kunden bestellen können. Um Partner bei der Einhaltung von Complianceanforderungen zu unterstützen, bittet Microsoft die Partner, die Zustimmung durch Bereitstellung bestimmter Details zu der Person, die dem Vertrag zugestimmt hat, zu bestätigen.
author: LauraBrenner
ms.author: labrenne
keywords: Kunde, Kunden, Zustimmung, MCA, Microsoft Cloud Vereinbarung, Microsoft-Kunden Vereinbarung, Kunden Vertrags Vorlagen
ms.localizationpriority: medium
ms.openlocfilehash: 6ca8eb3acdee0114f01dbd5952e9c092859147a2
ms.sourcegitcommit: ee722dc2b9d82557d273738b64cec6d8cb435084
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/31/2019
ms.locfileid: "68681756"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Bestätigen der kundenannahme des Microsoft-Kunden Vertrags (Vorschau)

Derzeit muss der Kunde die anwendbare **Microsoft Cloud Vereinbarung**annehmen und signieren, bevor ein CSP-Partner die Bestellung im Auftrag eines Kunden platzieren kann. Anschließend muss der Partner seine Zustimmung bestätigen, indem er Informationen über den Signatur Geber für Microsoft bereitstellt. Wenn ein Kunde seine Zustimmung zur Microsoft Cloud Vereinbarung nicht bestätigt:
- Sie können für diesen Kunden keine neuen Aufträge anlegen.
- Sie können die Anzahl der Arbeitsplätze bestehender arbeitsplatzbasierter Abonnements für diesen Kunden nicht ändern.

Ausführliche Informationen dazu, wie Sie die Zustimmung eines Kunden zum Microsoft Cloud Vertrag mithilfe des Partner Center-Dashboards oder der API bestätigen, finden Sie unter [bestätigen der kundenannahme des Microsoft Cloud Vertrags](confirm-consent.md).

Am 1. Oktober 2019 stellt Microsoft den **Microsoft-Kundenvertrag** für das CSP-Programm vor, um die Microsoft Cloud Vereinbarung zu ersetzen. Um die Migration von Partnern zum neuen Vertrag zu vereinfachen, wird die aktuelle Microsoft Cloud Vereinbarung bis zum 31. Januar 2019 im CSP-Programm unterstützt. Weitere Zeitachsen Details finden Sie in der folgenden Tabelle:

| date | Meilenstein | Details |
|------------|------------|--------------------------------|
|01. August, 2019|In Sandbox verfügbare UX-Vorschau|Partner können die Kunden Zustimmung des Microsoft-Kunden Vertrags über das Partner Center-Dashboard in der CSP-Sandbox-Umgebung bestätigen. Partner, die Zugriff auf die CSP-Sandkasten Umgebung haben, werden geändert. Partner ohne Sandbox-Zugriff können sich über die Änderungen in diesem Thema informieren.|
|2\. September, 2019|API Preview ist in Sandbox verfügbar.|Der Partner kann die Kundenakzeptanz des Microsoft-Kunden Vertrags mithilfe der Partner Center-API in der CSP-Sandkasten Umgebung bestätigen. API-Partner können diese Gelegenheit nutzen, um eine Vorschau der API-Änderungen anzuzeigen und mit der API-Integration zu beginnen, um den neuen Vertrag zu unterstützen|
|01. Oktober, 2019|Microsoft-Kunden Vereinbarung in der Produktion verfügbar|Microsoft führt den Microsoft-Kundenvertrag für das CSP-Programm ein, um die Microsoft Cloud Vereinbarung zu ersetzen. Partner können die Kundenakzeptanz des Microsoft-Kunden Vertrags über das Partner Center-Dashboard und die API in der Produktionsumgebung bestätigen. Die Microsoft Cloud Vereinbarung wird innerhalb des CSP-Partnerprogramms weiterhin unterstützt. Partner werden jedoch empfohlen, mit der Migration zum Microsoft-Kundenvertrag zu beginnen. Neue Käufe und Arbeitsplatz Anzahl Änderungen an vorhandenen Abonnements erfordern eine Partner Bestätigung des Microsoft-Kunden Vertrags oder der Microsoft Cloud Vereinbarung. Bestimmte neue Angebote (z. b. der neue Azure-Plan) erfordern eine Bestätigung des Microsoft-Kunden Vertrags.|
|31. Januar 2019|Microsoft Cloud Vereinbarung aus der Produktionsumgebung entfernt|Die Microsoft Cloud Vereinbarung wird innerhalb des CSP-Partnerprogramms nicht mehr akzeptiert. Bei neuen Käufen und Arbeitsplatz Anzahl Änderungen an vorhandenen Abonnements muss der Partner eine Bestätigung des Microsoft-Kunden Vertrags bereitstellen. Diese Anforderung gilt für neue Kunden und Bestandskunden, die die Microsoft Cloud Vereinbarung möglicherweise bereits angenommen haben.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Kundenakzeptanz für neue Kunden bestätigen

Wenn Sie einen neuen Kunden Mandanten in Partner Center erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert. Zum Ausführen dieser Schritte müssen Sie Administrator-Agent oder Sales Agent sein.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus.

2. Geben Sie unter **Konto Info**Informationen für das Unternehmen und seinen primären Kontakt ein.

3. Wählen Sie unter **Microsoft Agreement**den **Microsoft-Kundenvertrag**aus.

4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein späteres Datum festgelegt werden.

5. Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind. Wenn dies nicht richtig ist, wählen Sie **Aktualisieren** aus, und geben Sie **Vorname,** **Nachname**, **e-Mail-Adresse**und **Telefonnummer** (optional) der Person ein, die die Vereinbarung akzeptiert hat.

6. Wählen Sie **Weiter**, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.

![Neuer Kunde](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Bestätigen der Kundenakzeptanz für vorhandene Kunden

Hierfür müssen Sie Administrator-Agent oder Vertriebs-Agent sein:

1. Wählen Sie **Kunden**aus. Suchen und wählen Sie den Kunden aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Wählen Sie unter **Microsoft-Kunden Vereinbarung**die Option **Aktualisieren**aus.

4. Geben Sie **Vorname**, **Nachname**, **e-Mail-Adresse**und **Telefonnummer** (optional) der Person ein, die die Vereinbarung akzeptiert hat. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein späteres Datum festgelegt werden.

5. Wählen Sie **Speichern** und Fortfahren aus.

![Vorhandener Kunde](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Bestätigung der Kundenakzeptanz abrufen

Mithilfe der folgenden Schritte können Sie bestätigen, dass ein vorhandener Kunde den Microsoft-Kundenvertrag akzeptiert hat. Beachten Sie, dass Sie dafür ein Administratoragent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Zeigen Sie unter **Microsoft-cloudvertrag**an, ob die Bestätigung von diesem Kunden bestätigt oder noch nicht bereitgestellt wurde.


