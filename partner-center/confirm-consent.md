---
title: Bestätigen Sie Kunden Abnahme der Vereinbarung für Microsoft Cloud | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: Kunden, die Kunden, die Zustimmung
ms.localizationpriority: medium
ms.openlocfilehash: baab5e0fb3ac01284b210a2059b006ee2e17f921
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795283"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Bestätigen Sie Abnahme der Vereinbarung für Microsoft Cloud durch den Kunden

**Betrifft:**
-  Partner Center

Als Partner müssen Sie Ihre Kunden Abnahme der Vereinbarung für Microsoft Cloud zu erhalten, bevor Sie Microsoft-Produkte und Dienste für diesen Kunden bestellen können. Zum besseren erfüllen Partner Compliance-Anforderungen, Microsoft Partner fordert bestätigen Annahme hierzu werden die folgenden Details in Bezug auf die Person, die den Vertrag akzeptiert: 

-   Vorname

-   Nachname

-   E-Mail-Adresse

-   Telefonnummer

-   Datum der Annahme

Weitere Informationen hierzu finden Sie in der [Microsoft Cloud Agreement Kunden Annahme Bestätigung häufig gestellte Fragen](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Zeitplan

**7 August 2018**

-   Online-Dienst Partner und indirekte Anbieter können Kunden Abnahme der Vereinbarung für Microsoft Cloud bestätigen. Bestätigung ist *optional*.

-   Bestätigung der Kunde Annahme kann über Partner Center oder Partner Center-API erfolgen.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


**7 November 2018**

-   Direkte Rechnung Partner und indirekte Anbieter **müssen** bestätigen Kunden Annahme von der Microsoft Cloud Agreement. Bestätigung ist *obligatorisch*.

-   Wenn Bestätigung nicht für einen bestimmten Kunden bereitgestellt wird:

    -   Nicht werden mehr neue Aufträge für diesen Kunden erstellt.

    -   Nicht werden mehr die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierte Abonnements für diesen Kunden geändert.

-   Bestätigung der Kunde Annahme kann über Partner Center oder Partner Center-API erfolgen.

-   Bestätigung der Kunde Annahme wird nur mit öffentlichen Cloud von Microsoft unterstützt.


## <a name="confirming-customer-acceptance-in-partner-center"></a>Bestätigen der Abnahme durch den Kunden im Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Vergewissern Sie sich für einen neuen Kunden Abnahme durch den Kunden

Gehen Sie folgendermaßen vor, um Abnahme durch den Kunden zu bestätigen, während Sie einen neuen kundenmandanten für im Partner Center erstellen. Beachten Sie, dass Sie ein Administrator-Agent oder Sales Agent zu diesem Zweck müssen. 
1.  Wählen Sie **Kunden**und dann **neuen Kunden**.

2.  Geben Sie die Informationen zu dem **Unternehmen** und **Hauptansprechpartner**.

3.  Wählen Sie unter **Microsoft Cloud Agreement** **der Kunde hat den neuesten Microsoft-Cloud-Vertrag akzeptiert**. 

4.  Geben Sie das entsprechende Datum, unter der **Annahmedatum der Vereinbarung**. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

5.  Geben Sie die Details des Benutzers, der die Annahme bereitgestellt. 

    Standardmäßig wird die primäre Kontakt Benutzerinformationen angezeigt. Wenn dies nicht korrekt ist, wählen Sie **Aktualisieren** , und geben Sie dann die **Vorname**, **Nachname**, **E-Mail-Adresse**, und **Telefonnummer* (optional) der Person, die den Vertrag akzeptiert.

    **Hinweis:** Vor der Bestätigung des Kunden obligatorisch Akzeptanz, Sie zur Bestätigung durch nicht auswählen der Option, die **der Kunde den neuesten Microsoft-Cloud-Vertrag angenommen hat**, und wählen dann **Weiter**überspringen können.

6.  Wählen Sie **als Nächstes** die verbleibenden Schritte aus, um den kundenmandanten zu erstellen.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Vergewissern Sie sich für einen vorhandenen Kunden Abnahme durch den Kunden

Sie müssen ein Administrator-Agent oder Sales Agent zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  Wählen Sie **Konto**.

3.  Wählen Sie unter **Microsoft Cloud Agreement**- **Update**.

4.  Geben Sie den **Vornamen**, **Nachnamen**, **E-Mail-Adresse**und **Telefonnummer** (optional des Benutzers, der den Vertrag akzeptiert).

5.  Geben Sie das entsprechende Datum, unter der **Annahmedatum der Vereinbarung**. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

6.  Wählen Sie **Speichern und fortsetzen**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Vergewissern Sie sich beim Erstellen des neuen Auftrags für einen vorhandenen Kunden Abnahme durch den Kunden

Wenn Sie versuchen, eine neue Bestellung für einen vorhandenen Kunden erstellen, die Sie nicht vor dem bestätigt haben, erhalten Sie eine Aufforderung zur Bestätigung abzuschließen. Gehen Sie folgendermaßen vor, um dies tun. 

1.  Geben Sie den **Vornamen**, **Nachnamen**, **E-Mail-Adresse**und **Telefonnummer** (optional des Benutzers, der den Vertrag akzeptiert).

2.  Geben Sie das entsprechende Datum, unter der **Annahmedatum der Vereinbarung**. Dies kann nicht zu einem späteren Zeitpunkt festgelegt werden.

3.  Wählen Sie **Speichern und fortsetzen**.

**Hinweis:** Vor der Bestätigung der Kunde Annahme obligatorisch ist, überspringen Sie zur Bestätigung, durch die Auswahl **Abbrechen**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Bestätigung der Kunde Annahme für einen vorhandenen Kunden abrufen

Sie können zur Bestätigung der Kunde Annahme für einen vorhandenen Kunden abrufen, die Sie zuvor mit dem folgenden Verfahren bereitgestellt haben. Sie müssen ein Administrator-Agent oder Sales Agent zu diesem Zweck sein. 

1.  Wählen Sie **Kunden**, und suchen Sie und wählen Sie den Kunden, die, den Sie anzeigen möchten. 

2.  Wählen Sie **Konto**.

3.  **Microsoft Cloud Agreement**sehen Sie, ob Bestätigung für diesen Kunden bereitgestellt wurde oder nicht.

