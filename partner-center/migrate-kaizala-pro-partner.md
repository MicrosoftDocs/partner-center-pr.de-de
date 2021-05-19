---
title: Migrieren von Kaizala Pro-Abonnements zu Microsoft 365
description: Erfahren Sie, wie Sie Kaizala Pro-Abonnements zu Microsoft 365- oder Office 365-Versionen migrieren. Weitere Informationen zum Übergang Ihrer Kunden finden Sie in diesem Artikel.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146424"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrieren eigenständiger Kaizala Pro-Abonnements zu Microsoft 365- oder Office 365-Versionen

**Geeignete Rollen:** Vertriebs-Agent

Ab dem 1. Juli 2020 beendet Microsoft den Umsatz des eigenständigen Kaizala Pro-Diensts. Kunden können nach diesem Datum keine neuen Kaizala Pro-Abonnements mehr erwerben, und vorhandene Kaizala Pro-Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.

Um die Kontinuität für Kunden sicherzustellen, sollten Sie Kunden mit ablaufenden eigenständigen Kaizala Pro-Abonnements auf eine unterstützte SKU-Option umsteigen, die unten aufgeführt ist. Es wird empfohlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienstausfälle für Kunden zu vermeiden.

Wenn Sie die API verwenden (entweder DIE API oder Partner Center), können Sie ablaufende Abonnements ermitteln, indem Sie das Enddatum des Abonnements zusammen mit der Eigenschaft für die automatische Verlängerung auf FALSE festlegen: `auto renew = False` .

Die E4-Abonnements werden `auto renew=False` am 1. Juli 2020 auf festgelegt. Sie können Kunden jederzeit in einen neuen Plan verschieben.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro – eigenständige Ersetzungspläne

Mit den neuen Plänen können Ihre Kunden neuere Features und Funktionen in Microsoft 365 nutzen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.

- [**Microsoft 365 für Unternehmen,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)einschließlich:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 für Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)einschließlich:
   - Microsoft 365 F3 (ehemals Microsoft 365 F1) und Office 365 F3
    
- [**Microsoft 365 für Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)einschließlich: 
   - Office 365 E1
   - Microsoft 365 E3 and Office 365 E3
   - Microsoft 365 E5 und Office 365 E5

- [**Microsoft 365 für Bildungseinrichtungen,**](https://www.microsoft.com/education/buy-license/microsoft365)einschließlich: 
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

1. Um das neue Abonnement zu erwerben, wählen Sie im **Menü Partner Center** die Option **Kunden** aus, wählen Sie den Kunden aus, den Sie verschieben möchten, und wählen Sie dann **Abonnements hinzufügen** aus.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.

Ihr Kunde sollte nun sowohl über alte als auch über neue Abonnements, das alte eigenständige Kaizala Pro-Abonnement und das neue Zielabonnement verfügen, z. B. Option 1 – Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Neuzuweisen der aktuellen Benutzerlizenzen

1. Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen des Kunden im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Benutzer und Lizenzen** aus. Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.

2. Um die Benutzerlizenz neu zuzuweisen, wählen Sie den neu zuzuweisenden Benutzer und dann **Lizenzen verwalten** aus.

3. Aktivieren Sie **auf der Seite** Lizenzen verwalten das Kontrollkästchen Kaizala Pro Standalone license (Kaizala Pro Standalone-Lizenz), und wählen Sie einen neuen Serviceplan für das Abonnement aus, in das der Kunde um zieht.

4.  Klicken Sie auf **Submit** (Senden). Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt. Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.

### <a name="c-cancel-old-subscription"></a>C. Stornieren des alten Abonnements

Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

1.  Wählen Sie **Partner Center** Menü Kunden **aus.** Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.

2.  Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.

3.  Klicken Sie auf **Submit** (Senden).

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.
