---
title: Migrieren von kaizala pro-Abonnements zu Microsoft365
description: Erfahren Sie, wie Sie kaizala pro-Abonnements zu Microsoft365-oder Office 365-Versionen migrieren. Lesen Sie diesen Artikel, um weitere Informationen zum Übergang ihrer Kunden zu erhalten.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175175"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Migrieren von eigenständigen kaizala pro-Abonnements zu Microsoft365-oder Office 365-Versionen

Ab dem 1. Juli 2020 beendet Microsoft den Umsatz des eigenständigen kaizala pro-Dienstanbieter. Kunden können nach diesem Datum keine neuen kaizala pro-Abonnements mehr erwerben, und vorhandene kaizala pro-Abonnements werden nicht automatisch erneuert, wenn Sie ablaufen.

Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit abgelaufenen, eigenständigen kaizala pro-Abonnements auf eine unterstützte SKU-Option umstellen, die unten aufgeführt ist. Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.

Wenn Sie die API (entweder "Kamm" oder "Partner Center") verwenden, können Sie ablaufende Abonnements ermitteln, indem Sie das Enddatum des Abonnements und die Eigenschaft "automatisch erneuern" auf "false" festlegen `auto renew = False` .

Die E4-Abonnements werden auf den `auto renew=False` 1. Juli 2020 festgelegt. Sie können Kunden jederzeit in einen neuen Plan verschieben.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Eigenständige "kaizala pro"-Ersetzungs Pläne

Mit den neuen Plänen können Ihre Kunden in Microsoft 365 neuere Features und Funktionen nutzen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.

- [**Microsoft 365 für Unternehmen**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), einschließlich:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 für Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), einschließlich:
   - Microsoft 365 F3 (ehemals Microsoft 365 F1) und Office 365 F3
    
- [**Microsoft 365 für Unternehmen**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), einschließlich: 
   - Office 365 E1
   - Microsoft 365 E3 and Office 365 E3
   - Microsoft 365 E5 und Office 365 E5

- [**Microsoft 365 für Bildungseinrichtungen**](https://www.microsoft.com/education/buy-license/microsoft365), einschließlich: 
    - Microsoft 365 A1 und Office 365 A1
    - Microsoft 365 A3 und Office 365 A3
    - Microsoft 365 A5 und Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:

A. Kauf des neuen Abonnements

B. Neuzuweisen der aktuellen Benutzerlizenzen

C. Stornieren des alten Abonnements


## <a name="migrate-your-customers-to-new-plans"></a>Migrieren Ihrer Kunden zu neuen Plänen

### <a name="a-purchase-the-new-subscription"></a>A. Kauf des neuen Abonnements

1. Wenn Sie das neue Abonnement erwerben möchten, wählen Sie im **Partner Center** -Menü **Kunden**aus, wählen Sie den zu verschiebenden Kunden aus, und klicken Sie dann auf **Abonnements hinzufügen**.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.

Ihr Kunde sollte nun sowohl alte als auch neue Abonnements haben, das alte, eigenständige kaizala pro-Abonnement und das neue Abonnement "target", z. b. Option 1-Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Neuzuweisen der aktuellen Benutzerlizenzen

1. Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen des Kunden im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Benutzer und Lizenzen** aus. Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.

2. Um die Benutzerlizenz erneut zuzuweisen, wählen Sie den neu zuzuweisenden Benutzer aus, und wählen Sie dann **Lizenzen verwalten**aus.

3. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die eigenständige kaizala pro-Lizenz, und wählen Sie einen neuen Dienstplan für das Abonnement aus, zu dem der Kunde wechselt.

4.  Klicken Sie auf **Submit** (Senden). Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt. Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.

### <a name="c-cancel-old-subscription"></a>C. Stornieren des alten Abonnements

Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

1.  Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus. Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.

2.  Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.

3.  Klicken Sie auf **Submit** (Senden).

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.
