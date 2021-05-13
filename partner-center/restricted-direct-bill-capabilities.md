---
title: Eingeschränkte Direktabrechnungsfunktionen
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Anforderungen von CSP-Direktabrechnungspartner und darüber, wie Sie eine Einschränkung von Funktionen vermeiden können. Finden Sie heraus, ob Ihre Funktionen eingeschränkt wurden.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855487"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Eingeschränkte Direktabrechnungsfunktionen und die Anforderungen, die für CSP-Partner mit direkter Abrechnung erforderlich sind

**Geeignete Rollen:** Globaler Administrator

## <a name="overview"></a>Überblick

Direktabrechnungspartner müssen die neuen Anforderungen [erfüllen, um](direct-partner-new-requirements.md) im CSP-Programm für Partner mit direkter Abrechnung verbleiben zu können. Andernfalls wird Ihr Zugriff auf die Funktionen der direkten Abrechnung schließlich eingeschränkt, und sie können bestimmte Aufgaben (z. B. die Durchführung neuer Käufe für Ihre Kunden) nicht mehr übernehmen.

> [!Note]
> Partner mit direkter Abrechnung, die die neuen Anforderungen für das CSP-Direktabrechnungspartnerprogramm nicht erfüllen, werden von Microsoft informiert, wenn ihre Funktionen für direkte Rechnungen eingeschränkt werden. Dies gilt für alle Direktabrechnungspartner, unabhängig davon, ob sie sich für den Übergang vom Direktabrechnungspartner zu indirekten [Handelspartnern entschieden](transition-direct-to-indirect.md) haben oder nicht.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>So erkennen Sie, ob Ihre Funktionen für direkte Rechnungen eingeschränkt wurden

Um zu überprüfen, ob der Zugriff vom Direktabrechnungspartner-Mandanten auf Direct Bill-Funktionen eingeschränkt wurde, führen Sie die folgenden Schritte aus.

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wechseln Sie zu **Kontoeinstellungen**  ->  **Rechtliches Profil.**

3. Suchen **Sie unter** Programminformationen nach Microsoft Cloud Solution Provider **Status**.

4. Wenn der Programmstatus den Wert **eingeschränkt hat,** bedeutet dies, dass der Zugriff Ihres Direktabrechnungspartner-Mandanten auf Direktabrechnungsfunktionen eingeschränkt wurde.

## <a name="affected-direct-bill-capabilities"></a>Betroffene Direktabrechnungsfunktionen

Wenn Ihre Funktionen für direkte Rechnungen eingeschränkt wurden, können Sie keine neuen Käufe mehr für Ihre Kunden in Partner Center. Diese Einschränkung umfasst Folgendes:

- Azure-Abonnements

- Lizenzbasierte Abonnements

- Fügen Sie vorhandenen lizenzbasierten Abonnements neue Add-Ons hinzu.

- Einmalige Käufe von Software und Reservierungsprodukten (z. B. Softwareabonnements, unbefristete Software und Azure Reserved Virtual Machine-Instanzen).

Sie können auch nicht das [Azure-Partnerangebot für gemeinsame Dienste](shared-services.md) im Rahmen des CSP-Programms verwenden, um neue Azure-Abonnements für Ihre eigene Verwendung zu erwerben.

Vorhandene Direktabrechnungsabonnements sind nicht betroffen. Sie bleiben weiterhin gültig und werden automatisch verlängert. Sie werden weiterhin direkt von Microsoft abgerechnet, bis sie storniert werden. Sie können vorhandene Abonnements weiterhin auf folgende Weise verwalten:

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
