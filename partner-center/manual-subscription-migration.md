---
title: Migrieren von Dynamics 365 und Customer Engagement Plan aus Basic (qualifizierten Angebote) zu neueren Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement Plan (qualifizierten bietet) Basic Abonnements können nicht mehr verlängert werden.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968270"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrieren von Dynamics 365 und Customer Engagement Plan aus Basic (qualifizierten Angebote) zu neueren Versionen

**Betrifft:**

-  Partner Center

Effektive am 1. Januar 2019 Kunden mit Dynamics 365 for Sales / Customer Engagement Plan (qualifizierten bietet) Basic Abonnements können nicht mehr erneuern, die diese älteren Angebote; vorhandene Abonnements werden bei Ablauf nicht automatisch verlängert. Auf der Detailseite des Abonnements wird der Abonnementstatus von "Datum der automatischen [Datum]" in "Gültig bis [Datum]" ändern. 


Um Kontinuität für Kunden zu gewährleisten, sollten Sie diese mit ablaufenden Abonnements auf eine unterstützte Option, die unten aufgeführten übertragen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen.

Wenn Sie die API (CREST oder Partner Center) verwenden, finden Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie die automatische Verlängerung Eigenschaft "false". Die betreffenden Abonnements werden auf auto festgelegt werden verlängern = "false" am 1. Januar 2019. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

### <a name="the-dynamics-365-offers-being-retired"></a>Die Dynamics 365 bietet eingestellt wird

- Dynamics 365 für Vertrieb Enterprise Edition CRMOL Basic (qualifizierten Angebot)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Lehrkräfte
- Dynamics 365 für Vertrieb Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Schüler und Studenten
- Dynamics 365 für Vertrieb Enterprise Edition (Behörden Preisgestaltung) CRMOL Basic (qualifizierten Angebot)
- Dynamics 365 for Sales Enterprise-Edition SA für CRM Basic (qualifizierten Angebot)
- Dynamics 365 for Sales Enterprise-Edition SA für CRM Basic (qualifizierten Angebot) für Lehrpersonal
- Dynamics 365 for Sales Enterprise-Edition SA für CRM Basic (qualifizierten Angebot) für Schüler und Studenten
- Dynamics 365 Sales Enterprise-Edition (Behörden Preisgestaltung) SA für CRM Basic (qualifizierten Angebot)
- Dynamics 365 for Sales Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot)
- Dynamics 365 for Sales Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Lehrpersonal
- Dynamics 365 for Sales Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Schüler und Studenten
- Dynamics 365 für Vertrieb Enterprise Edition (Behörden Preisgestaltung) Add-On für CRM Basic (qualifizierten Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierten Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Behörden Preisgestaltung) CRMOL Basic (qualifizierten Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Schüler und Studenten
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Lehrpersonal
- Dynamics 365 Customer Engagement Plan Enterprise-Edition von SA für CRM Basic (qualifizierten Angebot)
- Dynamics 365 Kunden Engagement Plan Enterprise-Edition (Behörden Preisgestaltung) von SA für CRM Basic (qualifizierten Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise-Edition von SA für CRM Basic (qualifizierten Angebot) für Schüler und Studenten
- Dynamics 365 Customer Engagement Plan Enterprise-Edition von SA für CRM Basic (qualifizierten Angebot) für Lehrkräfte
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot)
- Dynamics 365 Kunden Engagement Plan Enterprise Edition (Behörden Preisgestaltung) Add-On für CRM Basic (qualifizierten Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Schüler und Studenten
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Lehrkräfte



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / Customer Engagement Plan aus (qualifizierten bietet) Basic Ersatz-Pläne

**Eingestellte Angebote**   

- Dynamics 365 für den Verkauf von CRM Basic oder CRMOL Basic (qualifizierten Angebot)
- Dynamics 365 Customer Engagement Plan von CRM Basic oder CRMOL Basic (qualifizierten Angebot)

**Ersatz-Optionen**
- Dynamics 365 for Sales Professional (neu)
- Dynamics 365 for Sales Professional (neu)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement Plan oder
- Dynamics 365 Team Member



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
 

 



