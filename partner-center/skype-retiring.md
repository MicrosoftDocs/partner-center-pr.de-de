---
title: Migrieren von Skype for Business Online Plan 1-Abonnements auf neuere Versionen von Office365 | Partner Center
Description: Skype for Business Online Plan 1 subscriptions is retiring.
Author: labrenne
keywords: Skype for Business-Pläne, Einstellung von Skype, Office365
ms.localizationpriority: medium
ms.openlocfilehash: 8d41ded7a2315cb8a69871f43d41bad391db9885
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489806"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrieren von Skype for Business Online Plan 1-Abonnements auf neuere Versionen von Office365

**Betrifft**

- Partner Center

Der Skype for Business Online Plan 1 wird zum 1. August 2018 eingestellt. Nach diesem Datum können Kunden keine neuen Skype for Business Plan 1-Abonnements mehr erwerben und bestehende Abonnements werden bei Ablauf nicht automatisch verlängert. Es steht außerdem keine Verlängerungsoption zur Verfügung. Auf der Detailseite des Abonnements wurde der Skype for Business Online Plan 1-Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert.  

Um Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Skype for Business Online Plan 1-Abonnements auf eine unterstützte SKU-Option (nachfolgend aufgeführt) übertragen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen. 

>[!NOTE]
>Sowohl kommerzielle als auch Behörden-SKUs für Skype for Business Online Plan 1 werden eingestellt.

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung ermitteln. Für Skype for Business Online Plan 1-Abonnements wird die automatische Verlängerung am 1.September2018 auf „False“ festgelegt. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Ersatzpläne für Skype for Business Online Plan 1

Mit den neuen Plänen können Ihre Kunden neuere Features und Funktionen in Office365 nutzen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center. 

- Option 1: Office 365 Enterprise F1
- Option 2: Microsoft 365 Enterprise F1
- Option 3: Andere Office365-Pläne

|**Feature**    |**Option1**   |**Option2**   |**Option3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Alle in Skype for Business Online Plan 1 enthaltenen Features|Ja   |Ja   |Ja   |
|Chatten und Anwesenheit |Ja   |Ja   |Ja   |
|Peer-zu-Peer-Audio und -Video über IP|Ja   |Ja   |Ja   
|Als authentifizierter Benutzer an Besprechungen teilnehmen| Ja   |Ja   |Ja   |

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste aktualisieren oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden von eingestellten SKUs zu neueren SKUs muss mit diesen Schritten erfolgen:

- Kauf des neuen Abonnements
- Neuzuweisen der aktuellen Benutzerlizenzen
- Stornieren des alten Abonnements

### <a name="migrate-your-customers-to-new-plans"></a>Migrieren Ihrer Kunden zu neuen Plänen

1. Um das neue Abonnement, aus dem **Menü "Partner Center"** erworben haben, wählen Sie **Kunden**, wählen Sie den Kunden, die, den Sie verschieben möchten, und wählen Sie dann **Abonnements hinzufügen**.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus. 

Ihr Kunde sollte nun sowohl alte als auch neue Abonnements besitzen, das alte Skype for Business Online Plan 1-Abonnement und das neue Zielabonnement, z.B. Option 1: Office365 Enterprise F1.

3. Zuweisen von Benutzern des Kunden Lizenzen, die **Partner Center** -Menü Wählen Sie **Kunden**aus, wählen Sie den Kunden, den Sie verschieben möchten, den und wählen Sie dann **Benutzer und Lizenzen**. Die Seite mit Benutzern und Lizenzen des Kunden wird geöffnet.

4. Um die Benutzerlizenzen erneut zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen.**

5. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für Skype for Business Online Plan 1, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.

6. Wählen Sie **Übermitteln** aus. Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt. Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.

Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

7. Wählen Sie im **Partner Center** -Menü **Kunden**aus. Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.

8. Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.

9. Wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.

