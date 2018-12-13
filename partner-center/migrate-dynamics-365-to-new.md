---
title: Migrieren von Dynamics 365 Business-Edition bietet zu neueren Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 Business-Edition-Abonnements können nicht mehr verlängert werden.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: 11f0d9262856d28adb4d67871503d86f2d4945ac
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968283"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrieren von Dynamics 365 Business-Edition bietet zu neueren Versionen 

**Betrifft:**

- Partner Center

Effektive am 1. Januar 2019 Kunden mit Dynamics 365 Business-Edition-Abonnements können nicht mehr in diese älteren Angebote verlängern; vorhandene Abonnements werden bei Ablauf nicht automatisch verlängert. Auf der Detailseite des Abonnements wird der Abonnementstatus von "Datum der automatischen [Datum]" in "Gültig bis [Datum]" ändern.

Um Kontinuität für Kunden zu gewährleisten, sollten Sie diese mit ablaufenden Abonnements auf eine unterstützte Option, die unten aufgeführten übertragen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen.

Wenn Sie die API (CREST oder Partner Center) verwenden, finden Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie die automatische Verlängerung Eigenschaft "false". Die betreffenden Abonnements werden auf auto festgelegt werden verlängern = "false" am 1. Januar 2019. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Die Dynamics 365 Business-Editionen wird eingestellt

- Dynamics 365 for Finance and Operations, Unternehmen-edition
- Dynamics 365 for Team Members, Unternehmen-edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Unternehmen zentralen - die neue Angebote für Dynamics 365 Business-Edition

Mit der neuen Dynamics Unternehmen zentralen Angebote können Ihre Kunden verbinden ihre Financials, Vertrieb, Service und Vorgänge Unternehmen Prozesse optimieren, die Interaktion mit Kunden zu verbessern und eine bessere Entscheidungen treffen. Dynamics 365 Business zentralen ist Cloud-basierten und über nur Partner im Cloud Solution Provider (CSP) Programm verfügbar.
Dynamics 365, Business Edition-Kunden erhalten Übergang ermäßigte Preise für neue Unternehmen zentralen, bietet bis zu 30 Juni 2020.

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

 Wechseln von Kunden von eingestellte SKUs zu neueren erfordert die folgenden Schritte in der folgenden Reihenfolge:

- Kauf des neuen Abonnements
- Neuzuweisen der aktuellen Benutzerlizenzen
- Stornieren des alten Abonnements

## <a name="purchase-the-new-plan-for-your-customer"></a>Den neuen Plan für Ihre Kunden erwerben

1. Wählen Sie **Kunden** aus der linken Navigationsbereich, und wählen Sie dann den Kunden, die, den Sie dem neuen Abonnement verschieben möchten.
2. Wählen Sie das **Abonnement hinzufügen**.
3. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus. 

Ihr Kunde wird nun das alte Abonnement und die neue Aufgabe besitzen. Im nächste Schritt werden Lizenzen für Benutzer des Kunden neu zugewiesen.

1. Wählen Sie **Kunden** aus der linken Navigationsbereich, und wählen Sie dann den Kunden, die, den Sie verschieben.
2. Wählen Sie **Benutzer und Lizenzen**.
3. Um eine Lizenz für einen Benutzer erneut zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie dann die **Lizenzen verwalten**. 
4. Auf der Seite " **Lizenzen verwalten** " deaktivieren Sie die Dynamics 365 for Sales / Customer Engagement Plan aus Basic (qualifizierten anbieten), Kontrollkästchen, und wählen Sie einen neuen Serviceplan für das Abonnement aus, die der Kunde in verschoben wird. 
5. Wählen Sie **Übermitteln** aus. Sie werden für jeden Benutzer dazu, die neue Lizenz benötigt. 

Nachdem Sie die Lizenzen für das neue Abonnement verschoben haben, können Sie das alte Abonnement stornieren. 

1. Wählen Sie **Kunden** aus der linken Navigationsbereich, und wählen Sie dann den Kunden, die, den Sie verschieben.
2. Klicken Sie auf der Detailseite des Abonnements legen Sie das alte Abonnement auf **angehalten** , und wählen Sie **übermitteln**.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120Tagen automatisch aufgehoben. Ihre Kunden fallen für das alte Abonnement keine zusätzlichen Kosten.