---
title: Migrieren einiger Skype for Business-Abonnements
description: Erfahren Sie, wie und wann bestimmte Kunden mit abgeschalteten Skype for Business Online Plan 1-Abonnements zu neuen Office 365-Versionen migriert werden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854824"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrieren von Skype for Business Online Plan 1-Abonnements zu neueren Versionen von Office 365

**Geeignete Rollen:** Vertriebs-Agent

Der Skype for Business Online-Plan 1 wird am 1. August 2018 zurückgezogen. Nach diesem Datum können Kunden keine neuen Skype for Business Plan 1-Abonnements mehr erwerben, und bestehende Abonnements werden bei Ablauf nicht automatisch verlängert. Es steht außerdem keine Verlängerungsoption zur Verfügung. Auf der Detailseite des Abonnements wurde der Skype for Business Online Plan 1-Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert.  

Um Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Skype for Business Online Plan 1-Abonnements auf eine unterstützte SKU-Option (nachfolgend aufgeführt) übertragen. Es wird empfohlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienstausfälle für Kunden zu vermeiden. 

>[!NOTE]
>Sowohl kommerzielle als auch Behörden-SKUs für Skype for Business Online Plan 1 werden eingestellt.

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln. Für Skype for Business Online Plan 1-Abonnements wird die automatische Verlängerung (auto renew) am 1. September 2018 auf „False“ festgelegt. Sie können Kunden jederzeit in einen neuen Plan verschieben. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Ersatzpläne für Skype for Business Online Plan 1

Mit den neuen Plänen können Ihre Kunden neuere Features und Funktionen in Office 365 nutzen. Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center. 

- Option 1: Office 365 Enterprise F1
- Option 2: Microsoft 365 Enterprise F1
- Option 3: Andere Office 365-Pläne

|**Feature**    |**Option 1:**   |**Option 2:**   |**Option 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Alle in Skype for Business Online Plan 1 enthaltenen Features|Ja   |Ja   |Ja   |
|Chatten und Anwesenheit |Ja   |Ja   |Ja   |
|Peer-zu-Peer-Audio und -Video über IP|Ja   |Ja   |Ja   
|Als authentifizierter Benutzer an Besprechungen teilnehmen| Ja   |Ja   |Ja   |

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:

- Kauf des neuen Abonnements
- Neuzuweisen der aktuellen Benutzerlizenzen
- Stornieren des alten Abonnements

### <a name="migrate-your-customers-to-new-plans"></a>Migrieren Ihrer Kunden zu neuen Plänen

1. Wählen Sie zum Erwerben eines neuen Abonnements im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Abonnements hinzufügen** aus.

2. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus. 

Ihr Kunde sollte jetzt sowohl über alte als auch über neue Abonnements verfügen, das alte Skype for Business Online Plan 1-Abonnement und das neue Zielabonnement, z. B. Option 1 – Office 365 Enterprise F1.

3. Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen des Kunden im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Benutzer und Lizenzen** aus. Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.

4. Um die Benutzerlizenzen erneut zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Lizenzen verwalten**.

5. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für Skype for Business Online Plan 1, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.

6. Klicken Sie auf **Submit** (Senden). Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt. Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.

Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

7. Wählen Sie **Partner Center** Menü Kunden **aus.** Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.

8. Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.

9. Wählen Sie **Senden aus.**

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.

## <a name="next-steps"></a>Nächste Schritte

- [Advisors: Erstellen und Senden einer Testeinladung für Clients zum Testen von Office 365](advisors-create-a-trial-invitation.md)
- [Advisors: Erstellen Ihrer Clientbasis mit Office 365-Testeinladungen und Kaufangeboten](advisors-build-your-business.md)
- [Advisors: Erstellen eines Kaufangebots](advisor-create-a-purchase-offer.md)
