---
title: Eingeschränkte Direktabrechnungsfunktionen
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Anforderungen Cloud Solution Provider (CSP) direkt abgerechneter Partner und darüber, wie Sie verhindern können, dass Funktionen eingeschränkt werden. Ermitteln Sie, ob Ihre Funktionen eingeschränkt wurden.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551417"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Eingeschränkte Funktionen für direkt abgerechnete Rechnungen und die Anforderungen, die für CSP-Partner mit direkter Abrechnung erforderlich sind

**Geeignete Rollen**: Globaler Administrator

## <a name="overview"></a>Übersicht

Partner mit direkter Abrechnung müssen die neuen [Anforderungen](direct-partner-new-requirements.md) erfüllen, um im CSP-Programm (Direct Bill Partner) Cloud Solution Provider zu bleiben. Andernfalls wird Ihr Zugriff auf die Funktionen der direkten Abrechnung schließlich eingeschränkt, und sie können bestimmte Aufgaben (z. B. die Durchführung neuer Käufe für Ihre Kunden) nicht mehr übernehmen.

> [!Note]
> Partner mit direkter Abrechnung, die die neuen Anforderungen für das CSP-Partnerprogramm für direkt abgerechnete Rechnungen nicht erfüllen, werden von Microsoft darüber informiert, wann ihre Funktionen für direkte Rechnungen eingeschränkt werden. Dies gilt für alle Direktabrechnungspartner, unabhängig davon, ob sie sich für den [Übergang vom Direktabrechnungspartner zu indirekten Handelspartnern](transition-direct-to-indirect.md) entschieden haben oder nicht.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Erfahren Sie, ob Ihre Funktionen für direkte Rechnungen eingeschränkt wurden.

Führen Sie die folgenden Schritte aus, um zu überprüfen, ob der Zugriff vom Direktabrechnungspartnermandanten auf Funktionen für direkte Rechnungen eingeschränkt wurde.

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wechseln Sie zu **Kontoeinstellungen**  >  **Rechtliches Profil**.

3. Suchen Sie unter **Programminformationen** nach **Microsoft Cloud Solution Provider Status**.

4. Wenn für den Programmstatus der Wert **eingeschränkt** ist, bedeutet dies, dass der Zugriff Ihres Partnermandanten für direkt abgerechnete Rechnungen auf Funktionen für direkte Rechnungen eingeschränkt wurde.

## <a name="affected-direct-bill-capabilities"></a>Betroffene Direktabrechnungsfunktionen

Wenn Ihre Funktionen für direkte Rechnungen eingeschränkt wurden, können Sie in Partner Center keine neuen Käufe mehr für Ihre Kunden tätigen. Diese Einschränkung umfasst Folgendes:

- Azure-Abonnements

- Lizenzbasierte Abonnements

- Fügen Sie vorhandenen lizenzbasierten Abonnements neue Add-Ons hinzu.

- Einmalige Käufe von Software- und Reservierungsprodukten (z. B. Softwareabonnements, unbefristete Software und Azure Reserved Virtual Machine-Instanzen).

Sie können auch das Angebot für [gemeinsame Azure-Partnerdienste](shared-services.md) im Rahmen des CSP-Programms nicht verwenden, um neue Azure-Abonnements für Ihre eigene Verwendung zu erwerben.

Vorhandene Direktabrechnungsabonnements sind nicht betroffen. Sie bleiben gültig und werden automatisch neu angepasst. Sie werden weiterhin direkt von Microsoft in Rechnung gestellt, bis sie storniert werden. Sie können vorhandene Abonnements weiterhin auf folgende Weise verwalten:

- Aussetzen vorhandener Abonnements

- Anpassen der Lizenzanzahl vorhandener lizenzbasierter Abonnements

- Anpassen der Lizenzanzahl vorhandener Add-Ons für ein Abonnement. 

    >[!Note]
    >Sie können vorhandenen Abonnements keine neuen Add-Ons hinzufügen, da sie als neuer Kauf behandelt werden.

- Bereitstellen neuer Azure-Ressourcen und Verwalten vorhandener Azure-Ressourcen unter vorhandenen Azure-Abonnements. Dies schließt Ressourcen ein, die über Azure Marketplace und Visual Studio Abonnements verfügbar sind.

Neben neuen Käufen haben Sie auch keinen Zugriff mehr auf folgende Direktabrechnungsfunktionen in Partner Center:

- Sie können keine neuen Kundenmandanten erstellen. Die Option **Kunde erstellen** auf der Seite **Kunden** in Partner Center ist nicht verfügbar.

- Sie können keine Einladung an den Kunden generieren, der eine direkte Handelspartnerbeziehung anfordert. Die Option **Vertriebspartnerbeziehung anfordern** auf der Seite **Kunden** in Partner Center ist nicht verfügbar.

    >[!NOTE]
    >Wenn Sie ihren Direktabrechnungspartner-Mandanten bereits als indirekter Wiederverkäufer registriert haben, können Sie im Rahmen des Wechsels vom Direktabrechnungspartner zum indirekten Vertriebspartner stattdessen eine Einladung an den Kunden generieren, der eine indirekte Vertriebspartnerschaft anfordert.

- Sie können keinen neuen Sandboxmandanten erstellen. Jeder Direktabrechnungspartnermandant kann einen Sandboxmandanten für die API-Integration mit direkter Abrechnung erstellen. Wenn Sie noch keines erstellt haben, können Sie dies nicht mehr tun, nachdem Ihre Partnerfunktion für direkt abgerechnete Rechnungen eingeschränkt wurde.  

## <a name="next-steps"></a>Nächste Schritte

- [Weitere Informationen zu den Anforderungen an indirekte Wiederverkäufer](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Neue Anforderungen für direkte CSP-Partner](direct-partner-new-requirements.md)
