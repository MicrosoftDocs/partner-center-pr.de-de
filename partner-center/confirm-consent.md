---
title: Bestätigen Sie Kunden zur Annahme von der Microsoft Cloud Agreement | Partner Center
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
keywords: Kunden, die Kunden, die Zustimmung
ms.localizationpriority: medium
ms.openlocfilehash: 0c3b3f63f0134793130d8358a1f52e3ed9d41908
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876220"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Bestätigen Sie Kunden zur Annahme von den Microsoft-Cloud-Vertrag

**Betrifft:**
-  Partner Center

Als Partner müssen Sie Ihre Kunden zur Annahme von der Microsoft Cloud Agreement zu erhalten, bevor Sie Microsoft-Produkte und Dienste für diesen Kunden bestellen können. Zum besseren erfüllen Partner Compliance-Anforderungen, Microsoft Partner fordert um zu bestätigen Acceptance hierzu werden die folgenden Details in Bezug auf die Person, die den Vertrag akzeptiert: 

-   Vorname

-   Nachname

-   E-Mail-Adresse

-   Telefonnummer

-   Datum der Annahme

Weitere Informationen hierzu finden Sie in der [Microsoft Cloud Agreement Kunden Acceptance Bestätigung häufig gestellte Fragen](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Zeitplan

**7 August 2018**

-   Online-Dienst-Partner und indirekte Anbieter können Kunden Zustimmung des Microsoft Cloud Agreement bestätigen. Bestätigung ist *optional*.

-   Bestätigung der Kunde Annahme kann über Partner Center-Dashboard oder Partner Center-API erfolgen.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


**7 November 2018**

-   Online-Dienst-Partner und indirekte Anbieter **müssen** bestätigen Kunden zur Annahme von der Microsoft Cloud Agreement. Bestätigung ist *obligatorisch*.

-   Wenn Bestätigung nicht für einen bestimmten Kunden bereitgestellt wird:

    -   Nicht werden neue Aufträge für diesen Kunden erstellt.

    -   Nicht werden die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierte Abonnements für diesen Kunden geändert.

-   Bestätigung der Kunde Annahme kann über Partner Center-Dashboard oder Partner Center-API erfolgen.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


## <a name="confirming-customer-acceptance-using-partner-center-dashboard"></a>Bestätigen der Abnahme durch den Kunden über Partner Center-Dashboard

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Vergewissern Sie sich für einen neuen Kunden Abnahme durch den Kunden

Gehen Sie folgendermaßen vor, um Kunden Zustimmung zu bestätigen, während Sie einen neuen kundenmandanten für im Partner Center-Dashboard erstellen. Beachten Sie, dass Sie ein Administrator-Agent-Verkäufe Agent zu diesem Zweck sein müssen. 
1.  Wählen Sie **Kunden**, und klicken Sie dann auf **neuen Kunden**.

2.  Geben Sie die Informationen über die **Unternehmen** und **Hauptansprechpartner**aus.

3.  Wählen Sie unter **Microsoft-Cloud-Vertrag** **der Kunde hat den neuesten Microsoft-Cloud-Vertrag akzeptiert**. 

4.  Geben Sie das entsprechende Datum, unter der **Annahmedatum der Vereinbarung**. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

5.  Geben Sie die Details des Benutzers, der die Annahme bereitgestellt. 

    Standardmäßig wird die primäre Kontakt Benutzerinformationen angezeigt. Wenn dies nicht korrekt ist, wählen Sie **Update** , und geben Sie dann die **Vorname**, **Nachname**, **E-Mail-Adresse**, und **Telefonnummer* (optional) der Person, die den Vertrag akzeptiert.

    **Hinweis:** Vor der Bestätigung der Kunde obligatorisch Annahme, Sie Bestätigung durch nicht auswählen die Option, die **der Kunde den neuesten Microsoft-Cloud-Vertrag angenommen hat**, und wählen Sie dann **Weiter**überspringen können.

6.  Wählen Sie **als Nächstes** die verbleibenden Schritte aus, um den kundenmandanten zu erstellen.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Vergewissern Sie sich für einen vorhandenen Kunden Abnahme durch den Kunden

Sie müssen ein Administrator-Agent oder Verkäufe-Agent zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  **Konto**auswählen.

3.  Wählen Sie unter **Microsoft Cloud Agreement** **Update**.

4.  Geben Sie die **Vorname**, **Nachname**, **E-Mail-Adresse**und **Telefonnummer** (optional) des Benutzers, der den Vertrag akzeptiert.

5.  Geben Sie das entsprechende Datum, unter der **Annahmedatum der Vereinbarung**. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

6.  Wählen Sie **Speichern und fortsetzen**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Vergewissern Sie sich beim Erstellen der neue Bestellung für einen vorhandenen Kunden Abnahme durch den Kunden

Wenn Sie versuchen, eine neue Bestellung für einen vorhandenen Kunden erstellen, die Sie nicht vor dem bestätigt haben, erhalten Sie dazu aufgefordert, führen Sie die Bestätigung. Gehen Sie folgendermaßen vor, zu diesem Zweck. 

1.  Geben Sie die **Vorname**, **Nachname**, **E-Mail-Adresse**und **Telefonnummer** (optional) des Benutzers, der den Vertrag akzeptiert.

2.  Geben Sie das entsprechende Datum, unter der **Annahmedatum der Vereinbarung**. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

3.  Wählen Sie **Speichern und fortsetzen**.

**Hinweis:** Vor der Bestätigung der Kunde Annahme obligatorisch ist, können Sie die Bestätigung überspringen, durch die Auswahl **Abbrechen**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Abrufen der Bestätigung der Kunde Annahme für einen vorhandenen Kunden

Sie können die Bestätigung der Kunde Annahme für einen vorhandenen Kunden abrufen, die Sie zuvor mit dem folgenden Verfahren bereitgestellt haben. Sie müssen ein Administrator-Agent oder Verkäufe-Agent zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  **Konto**auswählen.

3.  **Microsoft Cloud Agreement**sehen Sie sich, unabhängig davon, ob eine Bestätigung für diesen Kunden zur Verfügung gestellt.

