---
title: Dynamics 365 Business Edition migrieren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie qualifizierte Dynamics 365 Business Edition-Angebote zu neueren Versionen migrieren, bevor Sie ablaufen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132637"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrieren von Dynamics 365 Business Edition-Angeboten zu neueren Versionen

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Administrator-Agent
- Vertriebsbeauftragter

Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 Business Edition-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen. Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]".

Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.). Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln. Die fraglichen Abonnements werden am 1. Januar 2019 auf Auto Renew = false festgelegt. Sie können Kunden jederzeit in einen neuen Plan verschieben. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Die folgenden Dynamics 365 Business Editions werden eingestellt

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – die neuen Dynamics 365 Business Edition-Angebote

Mit den neuen Dynamics Business Central-Angeboten können Ihre Kunden Bereiche wie Finanzen, Vertrieb, Service und operatives Geschäft verbinden, um Geschäftsprozesse zu optimieren, die Kundeninteraktionen zu verbessern und bessere Entscheidungen zu treffen. Dynamics 365 Business Central ist cloudbasiert und nur über Cloud Solution Provider (CSP)-Partner erhältlich.
Dynamics 365 Business Edition-Kunden erhalten bis zum 30. Juni 2020 Migrationsrabatte für die neuen Business Central-Angebote.

## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen

 Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:

- Kauf des neuen Abonnements
- Neuzuweisen der aktuellen Benutzerlizenzen
- Stornieren des alten Abonnements

## <a name="purchase-the-new-plan-for-your-customer"></a>Kaufen des neuen Plans für Ihre Kunden

1. Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.
2. Wählen Sie **Abonnement hinzufügen** aus.
3. Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus. 

Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement. Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.

1. Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.
2. Wählen Sie **Benutzer und Lizenzen** aus.
3. Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus. 
4. Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird. 
5. Klicken Sie auf **Senden**. Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen. 

Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement kündigen. 

1. Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.
2. Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.
