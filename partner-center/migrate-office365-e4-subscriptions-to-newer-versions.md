---
title: Migrieren von Office 365 E4-Abonnements zu neueren Versionen von Office 365 | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Microsoft Office 365 Enterprise E4 Edition ist seit 7. April 2017 eingestellt. Hier erfahren Sie, wie Sie Ihre Kundenabonnements zu neueren Versionen von Office 365 migrieren.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e14ffbfaeaec64e8ccf3612cba9ed0f27aa31968
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134380"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrieren von Abonnements für Office 365 E4 auf neuere Versionen von Office 365

**Gilt für**

-  Partner Center

Der Office 365 Enterprise E4-Plan wird ab 7. April 2017 eingestellt. Sie können keine neuen Office 365 E4-Abonnements mehr nach diesem Datum kaufen und vorhandene E4-Abonnements werden bei Ablauf nicht automatisch verlängert.

Wenn E4-Abonnements enden, werden sie storniert. Um Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden E4-Abonnements auf eine unterstützte SKU-Option (nachfolgend aufgeführt) übertragen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen. 

> [!NOTE]  
>  Sowohl Office 365 Enterprise E4 kommerzielle und Government-SKUs werden zurückgezogen.
 
Auf der Detailseite des Abonnements wurde der E4-Abonnementstatus von "Datum der automatischen Verlängerung: [Datum]" in "Gültig bis [Datum]" geändert. 

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft "False" für die automatische Verlängerung ermitteln. 

Für die E4-Abonnements wird die automatische Verlängerung am 7. April 2017 automatisch auf "False" festgelegt. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4 Edition-Ersatzpläne

Sie können festlegen, dass bei E4 die gleiche Funktionalität beibehalten wird, oder Ihre Kunden neuere Features und Funktionen in Office 365 und Skype for Business Online nutzen lassen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center. Secure Product Enterprise E3 oder Secure Productive Enterprise E5 werden unter Umständen jeweils in den folgenden Optionen für Office 365 Enterprise E3 oder Office 365 Enterprise E5 ersetzt.

- Option 1: Office 365 Enterprise E5

- Option 2: Office 365 Enterprise E3 und Skype für Business-Cloud PBX

- Option 3: Office 365 Enterprise E3 und Skype for Business sowie CAL (Preise und Funktionen Parität mit E4)

- Option 4: Office 365 Enterprise E3


| Feature | Option 1 | Option 2 | Option 3 | Option 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Erhalten Sie alle in Office 365 Enterprise E4 enthaltenen Funktionen? | Ja | Ja | Ja | Nein |
| Werden Telefonnummern in Office 365 verwaltet? | Ja | Ja | Nein | Nein |
| Werden Telefonnummern sowohl lokal als auch in Office 365 (Hybridbereitstellung) verwaltet? | Ja | Ja | Nein | Nein |
| Ist eine Option zum Hinzufügen eines PSTN-Sprachanrufplans enthalten? | Ja | Ja | Nein | Nein |
| PSTN-Konferenzen? | Ja | Nein | Nein | Nein |
| Erweiterte Tools für die Zusammenarbeit, Analysen und Sicherheit? | Ja | Nein | Nein | Nein |
| Interaktive Berichte, Dashboards und Datenvisualisierungen? | Ja | Nein | Nein | Nein | 
| Mehr Kontrolle über die Datensicherheit und -kompatibilität mit integriertem Datenschutz, Transparenz und optimierten Benutzersteuerelementen? | Ja | Nein | Nein | Nein | 

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste aktualisieren oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden von eingestellten SKUs zu neueren SKUs muss mit diesen Schritten erfolgen:

-   Kauf des neuen Abonnements
-   Neuzuweisen der aktuellen Benutzerlizenzen
-   Stornieren des alten Abonnements.

Führen Sie die folgenden Schritte aus, um das Office 365 Enterprise E4-Abonnements eines Kunden zu einer der Optionen in der Tabelle oben zu migrieren.

### <a name="step-1---purchase-the-new-subscription"></a>Schritt 1: Kauf des neuen Abonnements

1. Von der **Partner Center** , wählen Sie im Menü **Kunden**, wählen Sie den Kunden, die Sie verwenden möchten, verschieben, und wählen Sie dann **Abonnements hinzufügen**.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.

   Ihr Kunde sollte nun sowohl alte als auch neue Abonnements besitzen, das alte Office 365 Enterprise E4-Abonnement und das neue Zielabonnement, z. B. Option 1: Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Schritt 2: Neuzuweisen der Benutzerlizenzen des Kunden

1. Von der **Partner Center** , wählen Sie im Menü **Kunden**, wählen Sie den Kunden, die Sie verwenden möchten, verschieben, und wählen Sie dann **Benutzer und Lizenzen**. Die Seite mit Benutzern und Lizenzen des Kunden wird geöffnet.

2. Um Benutzerlizenzen neu zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen**.

3. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen **Office 365 Enterprise E4**, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.

4. Wählen Sie **Übermitteln** aus. Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.

5. Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.

Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

### <a name="step-3---cancel-the-old-subscription"></a>Schritt 3: Stornieren des alten Abonnements

1. Von der **Partner Center** , wählen Sie im Menü **Kunden**. Wählen Sie den Kunden aus, den Sie verschieben möchten, und wählen Sie das Abonnement, das Sie stornieren möchten.

2. Legen Sie auf der Seite für Abonnementdetails den Abonnementstatus auf **Ausgesetzt** fest.

3. Wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.



 



