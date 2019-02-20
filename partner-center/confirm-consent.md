---
title: Bestätigen Sie Kunden Abnahme der Vereinbarung für Microsoft Cloud | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: Kunden, Kunden, erklären, MCA, Microsoft Cloud Agreement, Vorlagen für kundenverträge
ms.localizationpriority: medium
ms.openlocfilehash: 0cadf9462152786fd5cb5c70f7bd787caf85658b
ms.sourcegitcommit: 17066c1f254bb514f3d43eb1a8819e6f064bc180
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/20/2019
ms.locfileid: "9083193"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Bestätigen Sie Kunden zur Annahme von den Microsoft-Cloud-Vertrag

**Betrifft:**
-  Partner Center

Als Partner müssen Sie Ihr Kunde Abnahme der Vereinbarung für Microsoft Cloud zu erhalten, bevor Sie Microsoft-Produkte und Dienste für diesen Kunden bestellen können. Zum besseren erfüllen Partner Compliance-Anforderungen, Microsoft Partner fordert bestätigen Annahme hierzu werden die folgenden Details in Bezug auf die Person, die den Vertrag akzeptiert: 

-   Vorname

-   Nachname

-   E-Mail-Adresse

-   Telefonnummer

-   Datum der Annahme

Weitere Informationen hierzu finden Sie in der Microsoft Cloud Agreement Kunden Annahme Bestätigungs [Häufig gestellte Fragen](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Zeitplan

**7. August 2018**

-   Online-Dienst-Partner und indirekte Anbieter können Kunden Zustimmung des Microsoft Cloud Agreement bestätigen. Bestätigung ist *optional*.

-   Bestätigung der Kunde Annahme kann über Partner Center oder Partner Center-API erfolgen.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


**7. November 2018**

-   Online-Dienst-Partner und indirekte Anbieter **müssen** bestätigen Kunden zur Annahme von der Microsoft Cloud Agreement. Bestätigung ist *obligatorisch*.

-   Wenn Bestätigung nicht für einen bestimmten Kunden bereitgestellt wird:

    -   Nicht werden mehr neue Aufträge für diesen Kunden erstellt.

    -   Nicht werden mehr die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierte Abonnements für diesen Kunden geändert.

-   Bestätigung der Kunde Annahme kann über Partner Center oder Partner Center-API erfolgen.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


## <a name="confirming-customer-acceptance-in-partner-center"></a>Bestätigen der Abnahme durch den Kunden im Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Vergewissern Sie sich für einen neuen Kunden Abnahme durch den Kunden

Verwenden Sie das folgende Verfahren, um Kunden Zustimmung zu bestätigen, während Sie einen neuen kundenmandanten im Partner Center erstellen. Beachten Sie, dass Sie ein Administrator-Agent-Verkauf-Agent zu diesem Zweck sein müssen.
 
1.  Wählen Sie **Kunden**, und klicken Sie dann auf **neuen Kunden** , und wählen Sie dann die **Kontoinformationen**.

2.  Geben Sie die Informationen zu dem **Unternehmen** und **Hauptansprechpartner**.

![Unternehmensinformationen](images/mca/mca1.png)

3.  Wählen Sie unter **Microsoft-Cloud-Vertrag** **der Kunde hat den neuesten Microsoft-Cloud-Vertrag akzeptiert**ein. 

4.  Geben Sie das entsprechende Datum, unter der **Annahme-Datum der Vereinbarung**. Dies kann nicht auf ein späteres Datum festgelegt werden.

5.  Geben Sie die Details des Benutzers, der die Annahme bereitgestellt. 

![Annahmedatum hinzufügen](images/mca/MCA3.png)

Standardmäßig wird die primäre Kontakt Benutzerinformationen angezeigt. Wenn dies nicht korrekt ist, wählen Sie **Aktualisieren** , und geben Sie dann die **Vorname**, **Nachname**, **E-Mail-Adresse**und **Telefonnummer* (optional) der Person, die den Vertrag akzeptiert.

6.  Wählen Sie **als Nächstes** die verbleibenden Schritte aus, um den kundenmandanten zu erstellen.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Vergewissern Sie sich für einen vorhandenen Kunden Abnahme durch den Kunden

Sie müssen ein Administrator-Agent oder Sales-Agent zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  Wählen Sie die **Kontoinformationen**.

3.  Wählen Sie unter **Microsoft Cloud Agreement** **Update**.

![Update](images/mca/mca4.png)

4.  Geben Sie den **Vornamen**, **Nachnamen**, **E-Mail-Adresse**und **Telefonnummer** (optional) des Benutzers, der den Vertrag akzeptiert.

5.  Geben Sie das entsprechende Datum, unter der **Annahme-Datum der Vereinbarung**. Dies kann nicht auf ein späteres Datum festgelegt werden.

6.  Wählen Sie **Speichern und fortsetzen**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Vergewissern Sie sich beim Erstellen der neuen Auftrags für einen vorhandenen Kunden Abnahme durch den Kunden

Wenn Sie versuchen, eine neue Bestellung für einen vorhandenen Kunden erstellen, die Sie nicht vor dem bestätigt haben, erhalten Sie eine Aufforderung, führen Sie die Bestätigung. Verwenden Sie hierzu das folgende Verfahren. 

1.  Geben Sie den **Vornamen**, **Nachnamen**, **E-Mail-Adresse**und **Telefonnummer** (optional) des Benutzers, der den Vertrag akzeptiert.

2.  Geben Sie das entsprechende Datum, unter der **Annahme-Datum der Vereinbarung**. Dies kann nicht auf ein späteres Datum festgelegt werden.

3.  Wählen Sie **Speichern und fortsetzen**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Bestätigung der Kunde Annahme für einen vorhandenen Kunden abrufen

Sie können die Bestätigung der Kunde Annahme für einen vorhandenen Kunden abrufen, die Sie zuvor mit dem folgenden Verfahren bereitgestellt haben. Sie müssen ein Administrator-Agent oder Sales-Agent zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  Wählen Sie die **Kontoinformationen**.

3.  **Microsoft Cloud Agreement**sehen Sie sich, unabhängig davon, ob eine Bestätigung für diesen Kunden zur Verfügung gestellt.

