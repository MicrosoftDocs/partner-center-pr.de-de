---
title: Migrieren von Dynamics 365 Business Edition bietet auf neuere Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 Business Edition-Abonnements können nicht mehr erneuert werden.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Verlängern Sie Dynamics 365 bietet, Angebote, neue Dynamics 365-SKUs
ms.openlocfilehash: ca1823c4055e2d89edc5c49e900a1c255a94f59a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584623"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrieren von Dynamics 365 Business Edition-Angeboten zu neueren Versionen 

**Gilt für**

- Partner Center

Effektive 1. Januar 2019, Kunden in Dynamics 365 Business Edition-Abonnements können nicht mehr in älteren Angebote verlängern; vorhandene Abonnements werden nicht automatisch verlängert werden, wenn diese ablaufen. Auf der Detailseite des Abonnements ändert der Abonnementstatus zu "Läuft ab am [Datum]" sich von "erneuert automatisch am [Datum]".

Zur Sicherstellung der Kontinuität für Kunden, sollten Sie mit dem abgelaufene Abonnements für eine unterstützte Option, die unten aufgeführten übergehen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen.

Wenn Sie die API (CREST oder Partner Center) verwenden, finden Sie Verlängerung von ablaufenden Abonnements durch die das Enddatum des Abonnements sowie die automatische Auswertung = "false"-Eigenschaft. Die betreffenden Abonnements auf auto festgelegt erneuern = False auf 1. Januar 2019. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Die Dynamics 365 Business Editionen eingestellt

- Dynamics 365 für Finance and Operations, Business edition
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - der neue Dynamics 365 Business Edition-Angebote

Mit den neuen Dynamics Business Central bietet können Ihre Kunden verbinden ihre Finanzen, Vertrieb, Service und Vorgänge Geschäftsprozesse zu optimieren, Kundeninteraktionen verbessern und bessere Entscheidungen treffen. Dynamics 365 Business Central ist Cloud-basierten und Programmpartner nur Cloud Solution Provider (CSP) erhältlich.
Dynamics 365, die Business Edition-Kunden erhalten reduzierte Übergang die Preise für die neue Business Central berechtigt sind, bietet bis zum 30 Juni 2020.

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

 Verschieben von Kunden aus deaktivierten SKUs in neuere erfordert die folgenden Schritte aus, in der folgenden Reihenfolge:

- Kauf des neuen Abonnements
- Neuzuweisen der aktuellen Benutzerlizenzen
- Stornieren des alten Abonnements

## <a name="purchase-the-new-plan-for-your-customer"></a>Den neuen Plan für Ihre Kunden erwerben

1. Wählen Sie **Kunden** aus den linken Navigationsbereich, und wählen Sie dann den Kunden, die Sie in das neue Abonnement verschieben möchten.
2. Wählen Sie **-Abonnement hinzufügen**.
3. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus. 

Ihre Kunden haben jetzt sowohl das alte Abonnement und den neuen Wert. Der nächste Schritt ist für die neuzuweisung von Lizenzen, um den Kunden eines Benutzers.

1. Wählen Sie **Kunden** aus den linken Navigationsbereich, und wählen Sie dann den Kunden möchten verschieben.
2. Wählen Sie **Benutzer und Lizenzen**.
3. Um eine Lizenz zu einem Benutzer neu zuweisen möchten, wählen Sie den Benutzer aus, und wählen Sie dann **Verwalten von Lizenzen**. 
4. Auf der **Verwalten von Lizenzen** Seite, deaktivieren Sie die Dynamics 365 for Sales / Customer Engagement-Plan von Basic (qualifizierter bieten) lizenzieren Sie das Kontrollkästchen, und wählen Sie einen neuen Dienstplan für das Abonnement des Kunden auf verschoben wurde. 
5. Wählen Sie **Übermitteln** aus. Sie werden für jeden Benutzer so vorgehen, die die neue Lizenz benötigt. 

Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement Abbrechen. 

1. Wählen Sie **Kunden** aus den linken Navigationsbereich, und wählen Sie dann den Kunden möchten verschieben.
2. Legen Sie auf der Detailseite des Abonnements, auf das alte Abonnement **Suspended** , und wählen Sie **senden**.

Das alte Abonnement ist jetzt angehalten, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Ihre Kunden fallen keine zusätzlichen Kosten für das alte Abonnement auf.