---
title: Bestätigen der Zustimmung des Kunden zum Microsoft Cloud-Vertrag | Partner Center
ms.topic: article
ms.date: 02/22/2019
Description: Als Partner müssen Sie die Zustimmung Ihres Kunden zum Microsoft Cloud-Vertrag einholen, bevor Sie Microsoft-Produkte und -Dienste für den Kunden bestellen können. Zur besseren Hilfe lernen Sie Partner konformitätsanforderungen, Microsoft Fragen von Partnern zum bestätigen, dass Sie durch die Bereitstellung von bestimmte Details in Bezug auf die Person, die die Vereinbarung akzeptiert.
author: LauraBrenner
ms.author: v-petand
keywords: Kunden, Kunden, damit einverstanden sind, MCA, Microsoft Cloud-Vertrag, Kunden vereinbarungsvorlagen
ms.localizationpriority: medium
ms.openlocfilehash: e8c4b66027eeb9e285bd09a4b77aaf9bb6574188
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587563"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Bestätigen der Zustimmung des Kunden zum Microsoft Cloud-Vertrag

**Gilt für**
-  Partner Center

Als Partner müssen Sie die Zustimmung Ihres Kunden zum Microsoft Cloud-Vertrag einholen, bevor Sie Microsoft-Produkte und -Dienste für den Kunden bestellen können. Um Partner bei der Einhaltung von Compliance-Anforderungen zu unterstützen, bittet Microsoft die Partner, die Zustimmung durch Bereitstellung der folgenden Details zu der Person, die den Vertrag akzeptiert hat, zu bestätigen: 

-   Vorname

-   Nachname

-   E-Mail-Adresse

-   Telefonnummer

-   Datum der Zustimmung

Weitere Informationen finden Sie unter den Vertrag zwischen Microsoft Cloud Customer Bestätigung [häufig gestellte Fragen](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Zeitplan

**7. August 2018**

-   Direct Bill-Partner und indirekte Anbieter können die Kundenzustimmung zum Microsoft Cloud-Vertrag bestätigen. Die Bestätigung ist *optional*.

-   Bestätigung der Kundenakzeptanz kann über Partner Center oder das Partner Center-API erfolgen.

-   Die Bestätigung der Zustimmung des Kunden wird nur für Microsoft Public Cloud unterstützt.


**7. November 2018**

-   Direkte Rechnung Partner und indirekte Anbieter **müssen** bestätigen, dass Kunden der Microsoft-Cloud-Vereinbarung beim Austausch von über Partner Center-Dashboard. Die Bestätigung ist *obligatorisch*.

-   Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:

    -   Sie können für diesen Kunden keine neuen Aufträge anlegen.

    -   Sie können die Anzahl der Arbeitsplätze bestehender arbeitsplatzbasierter Abonnements für diesen Kunden nicht ändern.

-   Bestätigung der Kundenakzeptanz kann über Partner Center oder das Partner Center-API erfolgen.

-   Die Bestätigung der Zustimmung des Kunden wird nur für Microsoft Public Cloud unterstützt.

-   Dies gilt für Produktions- und Sandbox-Umgebungen.

**11. März 2018**

- Online-Dienst-Partner und indirekte Providersmust bestätigen, dass Kunden der Microsoft-Cloud-Vereinbarung in CSP-sandboxumgebung beim Austausch von über Partner Center-API.
- Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:

    - Sie wird nicht zum Erstellen neuer Bestellungen für diesen Kunden, Partner Center-API verwenden können.
 
    - Sie wird nicht zum Ändern der Anzahl der Arbeitsplätze des vorhandenen arbeitsplatzbasis für diesen Kunden, Partner Center-API verwenden können.
- Die Bestätigung der Zustimmung des Kunden wird nur für Microsoft Public Cloud unterstützt. 

**22. März 12018**

- Online-Dienst-Partner und indirekte Providersmust bestätigen, dass Kunden der Microsoft-Cloud-Vereinbarung in CSP-produktionsumgebung beim Austausch von über Partner Center-API.

- Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:
  - Sie wird nicht zum Erstellen neuer Bestellungen für diesen Kunden, Partner Center-API verwenden können.

  - Sie wird nicht zum Ändern der Anzahl der Arbeitsplätze des vorhandenen arbeitsplatzbasis für diesen Kunden, Partner Center-API verwenden können.
-  Die Bestätigung der Zustimmung des Kunden wird nur für Microsoft Public Cloud unterstützt.







## <a name="confirming-customer-acceptance-in-partner-center"></a>Bestätigen die Kundenakzeptanz im Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Bestätigen der Kundenzustimmung für einen neuen Kunden

Verwenden Sie das folgende Verfahren, um die Kundenakzeptanz Vergewissern Sie sich beim Erstellen eines neuen Mandantenverwaltungs für Kunden im Partner Center. Beachten Sie, dass Sie dafür ein Administratoragent oder Vertriebsbeauftragter sein müssen.
 
1.  Wählen Sie **Kunden**, und klicken Sie dann **Neukunden** und wählen Sie dann **Kontoinformationen**.

2.  Geben Sie die Informationen zu dem **Unternehmen** und **primären Kontakt** ein.

![Unternehmensinformationen](images/mca/mca1.png)

3.  Wählen Sie unter **Microsoft Cloud-Vertrag** die Option **Der Kunde hat den neuesten Microsoft Cloud-Vertrag akzeptiert**. 

4.  Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein späteres Datum festgelegt werden.

5.  Geben Sie die Details des Benutzers ein, der die Zustimmung gegeben hat. 

![Annahmedatum hinzufügen](images/mca/MCA3.png)

Standardmäßig werden die Informationen des primären Kontakts angezeigt. Wenn diese nicht korrekt sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer* (optional) der Person ein, die den Vertrag akzeptiert hat.

6.  Wählen Sie **Weiter**, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Bestätigen der Kundenzustimmung für einen bestehenden Kunden

Beachten Sie, dass Sie dafür ein Administratoragent oder Vertriebsbeauftragter sein müssen. 

1.  Wählen Sie **Kunden**, und suchen Sie dann den Kunden, die Sie anzeigen möchten. Wählen Sie diesen aus. 

2.  Wählen Sie **Kontoinformationen**.

3.  Wählen Sie unter **Microsoft Cloud-Vertrag** die Option **Aktualisieren** aus.

![Update/Aktualisieren](images/mca/mca4.png)

4.  Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der den Vertrag akzeptiert hat.

5.  Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein späteres Datum festgelegt werden.

6.  Wählen Sie **Speichern und fortfahren** aus.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Bestätigen der Kundenzustimmung beim Erstellen eines neuen Auftrags für einen vorhandenen Kunden

Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen. Führen Sie dazu die nachfolgend aufgeführten Schritte aus. 

1.  Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der den Vertrag akzeptiert hat.

2.  Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein späteres Datum festgelegt werden.

3.  Wählen Sie **Speichern und fortfahren** aus.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Abrufen der Bestätigung der Kundenzustimmung für einen vorhandenen Kunden

Sie können die Bestätigung der Zustimmung für einen vorhandenen Kunden abrufen, den Sie zuvor mit dem nachstehenden Verfahren angegeben haben. Beachten Sie, dass Sie dafür ein Administratoragent oder Vertriebsbeauftragter sein müssen. 

1.  Wählen Sie **Kunden**, und suchen Sie dann den Kunden, die Sie anzeigen möchten. Wählen Sie diesen aus. 

2.  Wählen Sie **Kontoinformationen**.

3.  Unter **Microsoft Cloud-Vertrag** sehen Sie, ob für diesen Kunden eine Bestätigung bereitgestellt wurde oder nicht.

