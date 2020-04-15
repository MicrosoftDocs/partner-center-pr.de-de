---
title: Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag | Partner Center
ms.topic: article
ms.date: 04/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahre, wie du bestätigst, dass ein Kunde der Microsoft-Kundenvereinbarung zugestimmt hat. Dies kann erforderlich sein, um Microsoft-Produkte und -Dienste für Kunden zu bestellen.
author: LauraBrenner
ms.author: labrenne
keywords: Kunde, Kunden, Zustimmung, MCA, Microsoft-Kundenvereinbarung, Vorlagen für Kundenvereinbarungen
ms.localizationpriority: high
ms.openlocfilehash: 2223a8e05a9df4c2d6ac377fc6f6b5a06944adc9
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123325"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung

**Zielgruppe**
-  Partner Center

**Geeignete Rollen**

- Administrator-Agent
- Vertriebsbeauftragter

> [!NOTE]
> Die Vertragsressource wird zurzeit von Partner Center nur in der Microsoft Public Cloud unterstützt. Gilt nicht für:
> * Partner Center-Betreiber ist 21Vianet
> * Partner Center für Microsoft-Cloud Deutschland
> * Partner Center für Microsoft Cloud for US Government

>[!NOTE]
>Ab dem 31. Januar 2020 müssen alle Kunden (vorhandene Kunden und Neukunden) die neue Microsoft-Kundenvereinbarung signieren. Weitere Informationen finden Sie unter [Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung](confirm-customer-agreement.md).

Als Partner müssen Sie die Zustimmung Ihres Kunden zur Microsoft-Kundenvereinbarung einholen, bevor Sie Microsoft-Produkte und -Dienste für diesen Kunden bestellen können. Um Partner bei der Einhaltung von Complianceanforderungen zu unterstützen, bittet Microsoft die Partner, die Zustimmung durch Bereitstellung der folgenden Details zu der Person, die dem Vertrag zugestimmt hat, zu bestätigen:

- Vorname

- Nachname

- E-Mail-Adresse

- Telefonnummer (optional)

- Datum der Zustimmung

Direct-Bill-Partner und indirekte Anbieter müssen die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung bestätigen, wenn sie über Partner Center oder die Partner Center-API Transaktionen ausführen. Die Bestätigung ist *obligatorisch*.

Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:

-    Können Sie für diesen Kunden keine neuen Aufträge erstellen.

-    Können Sie die Anzahl der Arbeitsplätze vorhandener arbeitsplatzbasierter Abonnements für diesen Kunden nicht ändern.

Die Bestätigung der Zustimmung des Kunden kann über das Partner Center oder die Partner Center-API erfolgen. Um dies über die Partner Center-API zu erledigen, lesen Sie die folgenden Themen: 

-   [Abrufen der Bestätigung der Zustimmung des Kunden](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Abrufen von Vertragsmetadaten](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Bestätigen der Zustimmung des Kunden](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Dies gilt für Produktions- und Sandboxumgebungen.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Bestätigen der Zustimmung des Kunden im Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Bestätigen der Kundenzustimmung für einen neuen Kunden

Verwenden Sie das folgende Verfahren, um die Zustimmung des Kunden zu bestätigen, während Sie einen neuen Kundenmandanten im Partner Center erstellen. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus, und klicken Sie anschließend auf **Kontoinformationen**.
2. Geben Sie die Informationen zum **Unternehmen** und zum **Primären Kontakt** ein.

![Unternehmensinformationen](images/mca/mca1.png)

3. Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Der Kunde hat die neueste Microsoft-Kundenvereinbarung akzeptiert** aus.
4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.
5. Geben Sie die Details des Benutzers ein, der die Zustimmung bereitgestellt hat.

![Hinzufügen eines Annahmedatums](images/mca/MCA3.png)

Standardmäßig werden die Informationen des primären Kontakts angezeigt. Wenn diese nicht richtig sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer* (optional) der Person ein, die der Vereinbarung zugestimmt hat.

6. Wählen Sie **Weiter** aus, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Bestätigen der Kundenzustimmung für einen vorhandenen Kunden

Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.
2. Wählen Sie **Kontoinformationen** aus.
3. Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Aktualisieren** aus.

![Update/Aktualisieren](images/mca/mca4.png)

4. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.
5. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.
6. Wählen Sie **Speichern und fortfahren** aus.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Bestätigen der Kundenzustimmung beim Erstellen eines neuen Auftrags für einen vorhandenen Kunden

Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen. Führen Sie dazu die nachfolgend aufgeführten Schritte aus.

1. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.
2. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.
3. Wählen Sie **Speichern und fortfahren** aus.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Abrufen der Bestätigung der Kundenzustimmung für einen vorhandenen Kunden

Sie können die Bestätigung der Zustimmung für einen vorhandenen Kunden abrufen, den Sie zuvor mit dem nachstehenden Verfahren angegeben haben. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.
2. Wählen Sie **Kontoinformationen** aus.
3. Unter **Microsoft-Kundenvereinbarung** sehen Sie, ob für diesen Kunden eine Bestätigung bereitgestellt wurde.
