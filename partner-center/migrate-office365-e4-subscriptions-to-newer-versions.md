---
title: Migrieren von Office365 E4-Abonnements zu neueren Versionen von Office365 | Partner Center
description: Microsoft Office365 Enterprise E4 Edition ist seit 7.April2017 eingestellt. Hier erfahren Sie, wie Sie Ihre Kundenabonnements zu neueren Versionen von Office365 migrieren.
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 545cfa5c635c9093cd0261bf35e01ba2823571ef
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876930"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrieren von Abonnements für Office365 E4 zu neueren Versionen von Office365

**Betrifft:**

-  Partner Center

Der Office 365 Enterprise E4-Plan wird ab 7. April 2017 eingestellt. Sie können keine neuen Office365 E4-Abonnements mehr nach diesem Datum kaufen und vorhandene E4-Abonnements werden bei Ablauf nicht automatisch verlängert.

Wenn E4-Abonnements enden, werden sie storniert. Um Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden E4-Abonnements auf eine unterstützte SKU-Option (nachfolgend aufgeführt) übertragen. Es wird empfohlen, Kunden auf neue Abonnements vor dem jährlichen Enddatum des Abonnements umzustellen, um Dienstausfälle für Kunden zu vermeiden. 

>**Hinweis:** Sowohl kommerzielle SKUs als auch Behörden-SKUs für Office365 Enterprise E4 werden eingestellt.
 
Auf der Detailseite des Abonnements wurde der E4-Abonnementstatus von "Datum der automatischen Verlängerung: [Datum]" in "Gültig bis [Datum]" geändert. 

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft "False" für die automatische Verlängerung ermitteln. 

Für die E4-Abonnements wird die automatische Verlängerung am 7.April2017 automatisch auf "False" festgelegt. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office365 Enterprise E4 Edition-Ersatzpläne

Sie können festlegen, dass bei E4 die gleiche Funktionalität beibehalten wird, oder Ihre Kunden neuere Features und Funktionen in Office365 und Skype for Business Online nutzen lassen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center. Secure Product Enterprise E3 oder Secure Productive Enterprise E5 werden unter Umständen jeweils in den folgenden Optionen für Office 365 Enterprise E3 oder Office 365 Enterprise E5 ersetzt.

- Option 1: Office 365 Enterprise E5

- Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (gleiche Preise und Funktionen wie E4)

- Option 4: Office 365 Enterprise E3


| Funktion | Option1 | Option2 | Option3 | Option4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Erhalten Sie alle in Office365 Enterprise E4 enthaltenen Funktionen? | Ja. | Ja | Ja | Nein. |
| Werden Telefonnummern in Office365 verwaltet? | Ja. | Ja | Nein | Nein. |
| Werden Telefonnummern sowohl lokal als auch in Office365 (Hybridbereitstellung) verwaltet? | Ja. | Ja | Nein | Nein. |
| Ist eine Option zum Hinzufügen eines PSTN-Sprachanrufplans enthalten? | Ja. | Ja | Nein | Nein. |
| PSTN-Konferenzen? | Ja. | Nein | Nein | Nein. |
| Erweiterte Tools für die Zusammenarbeit, Analysen und Sicherheit? | Ja. | Nein | Nein | Nein. |
| Interaktive Berichte, Dashboards und Datenvisualisierungen? | Ja. | Nein | Nein | Nein. | 
| Mehr Kontrolle über die Datensicherheit und -kompatibilität mit integriertem Datenschutz, Transparenz und optimierten Benutzersteuerelementen? | Ja. | Nein | Nein | Nein. | 

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste aktualisieren oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden von eingestellten SKUs zu neueren SKUs muss mit diesen Schritten erfolgen:

-   Kauf des neuen Abonnements
-   Neuzuweisen der aktuellen Benutzerlizenzen
-   Stornieren des alten Abonnements

Führen Sie die folgenden Schritteaus, um das Office365 Enterprise E4-Abonnements eines Kunden zu einer der Optionen in der Tabelle oben zu migrieren.

### <a name="step-1---purchase-the-new-subscription"></a>Schritt 1: Kauf des neuen Abonnements

1. Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend **Abonnements hinzufügen** aus.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.

   Ihr Kunde sollte nun sowohl alte als auch neue Abonnements besitzen, das alte Office 365 Enterprise E4-Abonnement und das neue Zielabonnement, z.B. Option 1: Office365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Schritt2: Neuzuweisen der Benutzerlizenzen des Kunden

1. Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend **Benutzer und Lizenzen** aus. Die Seite mit Benutzern und Lizenzen des Kunden wird geöffnet.

2. Um Benutzerlizenzen neu zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen**.

3. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen **Office 365 Enterprise E4**, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.

4. Wählen Sie **Übermitteln** aus. Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.

5. Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.

Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

### <a name="step-3---cancel-the-old-subscription"></a>Schritt 3: Stornieren des alten Abonnements

1. Wählen Sie im Menü **Dashboard** die Option **Kunden** aus. Wählen Sie den Kunden aus, den Sie verschieben möchten, und wählen Sie das Abonnement, das Sie stornieren möchten.

2. Legen Sie auf der Seite für Abonnementdetails den Abonnementstatus auf **Ausgesetzt** fest.

3. Wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.



 



