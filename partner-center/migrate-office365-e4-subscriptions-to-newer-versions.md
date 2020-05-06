---
title: Migrieren von Abonnements für Office 365 E4 zu neueren Versionen von Office 365 | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Die Enterprise E4-Edition von Microsoft Office 365 wurde am 7. April 2017 eingestellt. Hier erfahren Sie, wie Sie Ihre Kundenabonnements zu neueren Versionen von Office 365 migrieren.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 02d383172595e09a4ab0bf9c6db34862fcc17204
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798876"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrieren von Abonnements für Office 365 E4 auf neuere Versionen von Office 365

**Zielgruppe**

-  Partner Center

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Administrator-Agent
-   Vertriebsbeauftragter

Der Enterprise E4-Plan für Office 365 wurde am 7. April 2017 eingestellt. Nach diesem Datum können keine neuen Office 365 E4-Abonnements mehr erworben werden, und bereits vorhandene E4-Abonnements werden bei Ablauf nicht automatisch verlängert.

Wenn E4-Abonnements enden, werden sie storniert. Zur Gewährleistung von Kontinuität für betroffene Kunden sollten Sie Kunden mit ablaufenden E4-Abonnements zu einer unterstützten SKU-Option (nachfolgend aufgeführt) migrieren. Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden. 

> [!NOTE]  
>  Sowohl kommerzielle SKUs als auch Behörden-SKUs für Office 365 Enterprise E4 wurden eingestellt.
 
Auf der Detailseite des Abonnements wurde der E4-Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert. 

Bei Verwendung der API (CREST oder Partner Center) können Sie ablaufende Abonnements anhand des Enddatums des Abonnements sowie anhand der Eigenschaft „auto renew = False“ erkennen. 

Für E4-Abonnements wird die automatische Verlängerung am 7. April 2017 automatisch auf „False“ festgelegt. Sie können Kunden jederzeit in einen neuen Plan verschieben. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Ersatzpläne für die Enterprise E4-Edition von Office 365

Sie können wählen, ob die gleichen Funktionen wie in E4 bereitgestellt werden oder ob Ihre Kunden in Office 365 und Skype for Business Online in den Genuss neuerer Features und Funktionen kommen sollen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center. Secure Productive Enterprise E3 bzw. Secure Productive Enterprise E5 kann durch die folgenden Optionen für Office 365 Enterprise E3 bzw. Office 365 Enterprise E5 ersetzt werden:

- Option 1: Office 365 Enterprise E5

- Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (Preis-und Funktionalitäts Parität mit E4)

- Option 4: Office 365 Enterprise E3


| Funktion | Option 1: | Option 2: | Option 3 | Option 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Alle in Office 365 Enterprise E4 enthaltenen Features verfügbar? | Ja | Ja | Ja | Nein |
| Verwaltung von Telefonnummern in Office 365? | Ja | Ja | Nein | Nein  |
| Verwaltung von Telefonnummern sowohl lokal als auch in Office 365 (Hybridbereitstellung)? | Ja | Ja | Nein | Nein  |
| Option zum Hinzufügen eines PSTN-Sprachanrufplans? | Ja | Ja | Nein | Nein  |
| PSTN-Konferenzen? | Ja | Nein | Nein  | Nein  |
| Erweiterte Tools für Zusammenarbeit, Analysen und Sicherheit? | Ja | Nein | Nein  | Nein  |
| Interaktive Berichte, Dashboards und Datenvisualisierungen? | Ja | Nein | Nein  | Nein  | 
| Mehr Kontrolle über die Datensicherheit und Compliance mit integriertem Datenschutz, Transparenz und optimierten Benutzersteuerelementen? | Ja | Nein | Nein  | Nein  | 

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:

-   Kauf des neuen Abonnements
-   Neuzuweisen der aktuellen Benutzerlizenzen
-   Stornieren des alten Abonnements.

Führen Sie diese Schritte aus, um das Office 365 Enterprise E4-Abonnement eines Kunden zu einer der Optionen in der obigen Tabelle zu migrieren.

### <a name="step-1---purchase-the-new-subscription"></a>Schritt 1: Kaufen des neuen Abonnements

1. Wählen Sie im Menü **Partner Center** die Option **Kunden** und anschließend den Kunden aus, den Sie migrieren möchten. Wählen Sie dann **Abonnements hinzufügen** aus.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.

   Ihr Kunde sollte nun sowohl alte als auch neue Abonnements haben, das alte Office 365 Enterprise E4-Abonnement und das neue Abonnement "target", z. b. Option 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Schritt 2: Neuzuweisen der Benutzerlizenzen des Kunden

1. Wählen Sie im Menü **Partner Center** die Option **Kunden** und anschließend den Kunden aus, den Sie migrieren möchten. Wählen Sie dann **Benutzer und Lizenzen** aus. Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.

2. Um Benutzerlizenzen neu zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen**.

3. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Lizenzkontrollkästchen für **Office 365 Enterprise E4**, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.

4. Klicken Sie auf **Submit** (Senden). Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.

5. Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.

Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

### <a name="step-3---cancel-the-old-subscription"></a>Schritt 3: Stornieren des alten Abonnements

1. Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus. Wählen Sie den Kunden aus, den Sie migrieren möchten, und wählen Sie anschließend das Abonnement aus, das Sie stornieren möchten.

2. Legen Sie auf der Seite mit den Abonnementdetails den Abonnementstatus auf **Ausgesetzt** fest.

3. Klicken Sie auf **Submit** (Senden).

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.



 



