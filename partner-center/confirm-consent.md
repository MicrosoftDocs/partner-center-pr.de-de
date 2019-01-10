---
title: Bestätigen Sie Kunden Abnahme der Vereinbarung für Microsoft Cloud | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: Kunden, die Kunden, die Zustimmung
ms.localizationpriority: medium
ms.openlocfilehash: 356782420046cb8b49ac4e05981becd253d7049a
ms.sourcegitcommit: dcc0517b2441c5577994b802c455fc726cc5cb35
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/10/2019
ms.locfileid: "9000030"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Bestätigen Sie Kunden zur Annahme von den Microsoft-Cloud-Vertrag

**Betrifft:**
-  Partner Center

Partner müssen Sie Ihre Kunden Abnahme der Vereinbarung für Microsoft Cloud zu erhalten, bevor Sie Microsoft-Produkte und Dienste für diesen Kunden bestellen können. Zum besseren erfüllen Partner Compliance-Anforderungen auffordert, Microsoft Partner bestätigen Annahme hierzu werden die folgenden Details in Bezug auf die Person, die den Vertrag akzeptiert: 

-   Vorname

-   Nachname

-   E-Mail-Adresse

-   Telefonnummer

-   Datum der Annahme

Weitere Informationen finden Sie in der [Microsoft Cloud Agreement Kunden Annahme Bestätigung häufig gestellte Fragen](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Zeitplan

**7 August 2018**

-   Online-Dienst-Partner und indirekte Anbieter können Kunden zur Annahme von der Microsoft Cloud Agreement überprüfen. Bestätigung ist *optional*.

-   Bestätigung der Annahme von Kunden über Partner Center oder Partner Center-API möglich.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


**7 November 2018**

-   Bestätigen Online-Dienst-Partner und indirekte Anbieter **müssen** Kunden zur Annahme von der Microsoft Cloud Agreement. Bestätigung ist *obligatorisch*.

-   Wenn Bestätigung nicht für einen bestimmten Kunden bereitgestellt wird:

    -   Nicht werden für diese Kunden neue Aufträge erstellt.

    -   Sie wird nicht die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierte Abonnements für diesen Kunden ändern können.

-   Bestätigung der Annahme von Kunden über Partner Center oder Partner Center-API möglich.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


## <a name="confirming-customer-acceptance-in-partner-center"></a>Bestätigen der Abnahme durch den Kunden im Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Vergewissern Sie sich für einen neuen Kunden Abnahme durch den Kunden

Verwenden Sie das folgende Verfahren, um Kunden Zustimmung zu bestätigen, während Sie einen neuen kundenmandanten für im Partner Center erstellen. Beachten Sie, dass Sie ein Administrator-Agent-Verkauf-Agent zu diesem Zweck sein müssen. 
1.  Wählen Sie **Kunden**, und klicken Sie dann auf **neuen Kunden** , und wählen Sie dann die **Kontoinformationen**.

2.  Geben Sie die Informationen zu dem **Unternehmen** und **Hauptansprechpartner**.

![Unternehmensinformationen](images/mca/mca1.png)

3.  Wählen Sie unter **Microsoft-Cloud-Vertrag** **der Kunde hat den neuesten Microsoft-Cloud-Vertrag akzeptiert**. 

4.  Geben Sie unter der **Vereinbarung Annahme Datum, an dem**das entsprechende Datum. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

5.  Geben Sie die Details des Benutzers, der die Annahme bereitgestellt. 

![Acceptance Datum hinzufügen](images/mca/MCA3.png)

Standardmäßig wird die primäre Kontakt Informationen angezeigt. Wenn dies nicht korrekt ist, wählen Sie **Aktualisieren** , und geben Sie dann die **Vorname**, **Nachname**, **E-Mail-Adresse**, und **Telefonnummer* (optional) der Person, die den Vertrag akzeptiert.


6.  Wählen Sie **Weiter** mit die verbleibenden Schritte zum Erstellen von kundenmandanten.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Vergewissern Sie sich für einen vorhandenen Kunden Abnahme durch den Kunden

Sie müssen ein Administrator-Agent oder Verkäufe Agent, zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  Wählen Sie die **Kontoinformationen**.

3.  Wählen Sie unter **Microsoft Cloud Agreement** **Update**.

![Update](images/mca/mca4.png)

4.  Geben Sie die **Vorname**, **Nachname**, **E-Mail-Adresse**und **Telefonnummer** (optional) des Benutzers, der den Vertrag akzeptiert.

5.  Geben Sie unter der **Vereinbarung Annahme Datum, an dem**das entsprechende Datum. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

6.  Wählen Sie **Speichern und weiter**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Vergewissern Sie sich beim Erstellen des neuen Auftrags für einen vorhandenen Kunden Abnahme durch den Kunden

Wenn Sie versuchen, eine neue Bestellung für einen vorhandenen Kunden erstellen, die Sie nicht vor dem bestätigt haben, erhalten Sie dazu aufgefordert, führen Sie die Bestätigung. Verwenden Sie hierzu das folgende Verfahren. 

1.  Geben Sie die **Vorname**, **Nachname**, **E-Mail-Adresse**und **Telefonnummer** (optional) des Benutzers, der den Vertrag akzeptiert.

2.  Geben Sie unter der **Vereinbarung Annahme Datum, an dem**das entsprechende Datum. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

3.  Wählen Sie **Speichern und weiter**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Abrufen der Bestätigung der Kunde Annahme für einen vorhandenen Kunden

Sie können die Bestätigung der Kunde Annahme für einen vorhandenen Kunden abrufen, die Sie zuvor mit dem folgenden Verfahren bereitgestellt haben. Sie müssen ein Administrator-Agent oder Verkäufe Agent, zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  Wählen Sie die **Kontoinformationen**.

3.  **Microsoft Cloud Agreement**sehen Sie sich, unabhängig davon, ob eine Bestätigung für diesen Kunden zur Verfügung gestellt.

