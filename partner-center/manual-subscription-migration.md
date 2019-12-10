---
title: Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierte Angebote) zu neueren Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie ein neues Abonnement erwerben können, bevor die vorhandenen ablaufen, Benutzerlizenzen neu zuweisen und dann das alte Abonnement kündigen.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365-Angebote, Angebote verlängern, neue Dynamics 365-SKUs
ms.openlocfilehash: bbb7480264a2d3d5ae6ed1f50e0f32b5ebc1c16e
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943353"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierte Angebote) zu neueren Versionen

**Zielgruppe**

-  Partner Center

Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 for Sales/Customer Engagement Plan von Basic (qualifizierte Angebote)-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen. Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]". 


Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.). Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln. Die betreffenden Abonnements werden am 1. Januar 2019 auf „auto renew=False“ festgelegt. Sie können Kunden jederzeit zu einem neuen Plan migrieren. 

### <a name="the-dynamics-365-offers-being-retired"></a>Die folgenden Dynamics 365-Angebote werden eingestellt

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten
- Dynamics 365 for Sales Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal
- Dynamics 365 for Sales Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten
- Dynamics 365 for Sales Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Studenten
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Ersatzpläne für Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot)

**Eingestellte Angebote**   

- Dynamics 365 for Sales from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)
- Dynamics 365 Customer Engagement Plan from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)

**Ersatzoptionen**
- Dynamics 365 for Sales Professional (NEU)
- Dynamics 365 for Sales Professional (NEU)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement Plan oder
- Dynamics 365 Team Members



## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:

- Kauf des neuen Abonnements
- Neuzuweisen aktueller Benutzerlizenzen
- Stornieren des alten Abonnements

## <a name="purchase-the-new-plan-for-your-customer"></a>Kaufen des neuen Plans für Ihre Kunden

1. Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.
2. Wählen Sie **Abonnement hinzufügen** aus.
3. Wählen Sie im Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die gewünschte Anzahl von Lizenzen ein, und wählen Sie anschließend **Übermitteln** aus. 

Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement. Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.

1. Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.
2. Wählen Sie **Benutzer und Lizenzen**.
3. Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus. 
4. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird. 
5. Wählen Sie **Übermitteln** aus. Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen. 

Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement stornieren. 

1. Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.
2. Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.
 

 



