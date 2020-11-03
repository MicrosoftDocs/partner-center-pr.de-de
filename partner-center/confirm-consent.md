---
title: Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung
description: Erfahre, wie du bestätigst, dass ein Kunde der Microsoft-Kundenvereinbarung zugestimmt hat. Dies kann erforderlich sein, um Microsoft-Produkte und -Dienste für Kunden zu bestellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333916"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Aktualisierte Methode zur Bestätigung der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung

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

Direct-Bill-Partner und indirekte Anbieter müssen die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung bestätigen, wenn sie über Partner Center oder die Partner Center-API Transaktionen ausführen. Die Bestätigung ist *obligatorisch* .

Wenn für einen bestimmten Kunden keine Bestätigung bereitgestellt wird:

- Können Sie für diesen Kunden keine neuen Aufträge erstellen.

- Können Sie die Anzahl der Lizenzen vorhandener lizenzbasierter Abonnements für diesen Kunden nicht ändern.

Die Bestätigung der Zustimmung des Kunden kann über das Partner Center oder die Partner Center-API erfolgen. Um dies über die Partner Center-API zu erledigen, lesen Sie die folgenden Themen:

- [Abrufen der Bestätigung der Zustimmung des Kunden](/partner-center/develop/get-confirmation-of-customer-consent)

- [Abrufen von Vertragsmetadaten](/partner-center/develop/get-agreement-metadata)

- [Bestätigen der Zustimmung des Kunden](/partner-center/develop/confirm-customer-consent)

Dies gilt für Produktions- und Sandboxumgebungen.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Bestätigen der Kundenzustimmung für einen neuen Kunden

Verwenden Sie das folgende Verfahren, um die Zustimmung des Kunden zu bestätigen, während Sie einen neuen Kundenmandanten im Partner Center erstellen. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus, und klicken Sie anschließend auf **Kontoinformationen** .

2. Geben Sie die Informationen zum **Unternehmen** und zum **Primären Kontakt** ein.

   :::image type="content" source="images/mca/mca1.png" alt-text="Unternehmensinformationen":::

3. Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Der Kunde hat die neueste Microsoft-Kundenvereinbarung akzeptiert** aus.

4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Geben Sie die Details des Benutzers ein, der die Zustimmung bereitgestellt hat.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Unternehmensinformationen":::

   Standardmäßig werden die Informationen des primären Kontakts angezeigt. Wenn diese nicht richtig sind, wählen Sie **Aktualisieren** aus, und geben Sie dann **Vorname** , **Nachname** , **E-Mail-Adresse** und * *Telefonnummer* (optional) der Person ein, die der Vereinbarung zugestimmt hat.

6. Wählen Sie **Weiter** aus, um mit den verbleibenden Schritten zum Erstellen des Kundenmandanten fortzufahren.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Bestätigen der Kundenzustimmung für einen vorhandenen Kunden

Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Wählen Sie unter **Microsoft-Kundenvereinbarung** die Option **Aktualisieren** aus.

   :::image type="content" source="images/mca/mca4.png" alt-text="Unternehmensinformationen":::

4. Geben Sie **Vorname** , **Nachname** , **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.

5. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

6. Wählen Sie **Speichern und fortfahren** aus.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Bestätigen der Kundenzustimmung beim Erstellen eines neuen Auftrags für einen vorhandenen Kunden

Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen. Führen Sie dazu die nachfolgend aufgeführten Schritte aus.

1. Geben Sie **Vorname** , **Nachname** , **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.

2. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

3. Wählen Sie **Speichern und fortfahren** aus.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Abrufen der Bestätigung der Kundenzustimmung für einen vorhandenen Kunden

Sie können die Bestätigung der Zustimmung für einen vorhandenen Kunden abrufen, den Sie zuvor mit dem nachstehenden Verfahren angegeben haben. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Unter **Microsoft-Kundenvereinbarung** sehen Sie, ob für diesen Kunden eine Bestätigung bereitgestellt wurde.

## <a name="next-steps"></a>Nächste Schritte

- [Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung im CSP-Partnerprogramm](confirm-customer-agreement.md)

- [Bestätigen der Zustimmung zur Microsoft-Kundenvereinbarung im Namen Ihres Kunden](attest-acceptance-customer-agreement.md)