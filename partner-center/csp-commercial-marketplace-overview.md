---
title: 'Übersicht: CSP-Marketplace'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Kunden Abonnements für SaaS-Angebote (Software-as-a-Service) von unabhängigen Softwareanbietern (ISVs) im Marketplace verkaufen.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c8d64167261fe9f425a1430ac0c109b446b50913
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038828"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>Übersicht über den kommerziellen Marketplace im Partner Center

**Zielgruppe**

- Partner Center
- Partner im CSP-Programm

Wenn Sie ein Partner im CSP-Programm (Cloud Solution Provider) sind, können Sie Microsoft-Produkte zusammen mit Lösungen bündeln und verkaufen, die von Drittanbietern, unabhängigen Software Anbietern (Independent Software Providers, ISVs) veröffentlicht werden. Wenn Sie Lösungen auf diese Weise bündeln können, können Sie Endkunden besser bedienen und Ihr CSP-Dienst Geschäft steigern.

Als Partner im CSP-Programm können Sie Partner Center verwenden, um viele ISV-Lösungen über den kommerziellen Marketplace von Microsoft zu erwerben. Dadurch erhalten Sie und ihre Kunden einige wichtige Vorteile:

- Zugriff auf einen Katalog mit Softwarelösungen, die für Microsoft-Technologien und-Umgebungen optimiert sind.
- Vereinfachtes Vertrags-und verkürztes Beschaffungs Zyklen.
- Eine einzelne Integration in Partner Center-APIs. (Durch eine solche Integration wird der Zugriff auf einen Katalog von ISV-Lösungen ermöglicht, die Kosten für Betrieb und Engineering werden gesenkt, und die Verwaltung mehrerer Anbieter Abonnements und die Abrechnung erfolgt über einen einzelnen Anbieter.)
- Optimierte Bereitstellung und Bereitstellung im Azure-Mandanten des Kunden (für auf virtuellen Computern basierende Lösungen).
- Hierdurch werden potenzielle Herausforderungen bei direkten ISV-Käufen oder-Verträgen, bei der Konfiguration und Integration von Microsoft-Lösungen sowie bei der Notwendigkeit zum Verwalten oder Konsolidieren von periodischen Rechnungen von mehreren Anbietern reduziert

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>Übersicht über CSP-Angebote im kommerziellen Marketplace

Wenn Sie Partner im CSP-Programm sind, gibt es viele kommerzielle Marketplace-Aktivitäten, die Sie möglicherweise in Bezug auf ISV-Angebote durchführen möchten. Weitere Informationen zu den einzelnen Aktivitäten finden Sie in der folgenden Tabelle.

|**Zweck**  |**Lesen**   |
|:------------------------------------|:------------------|
|Erfahren Sie, wie Sie verfügbare Angebote, Preise, Produktdetails oder Kontaktinformationen des Herausgebers anzeigen oder suchen. | [Angebote entdecken](csp-commercial-marketplace-discover.md) | 
|Erfahren Sie, wie Sie ein Angebot erwerben und bereitstellen.   | [Kaufangebote](csp-commercial-marketplace-purchase.md)   | 
|Erfahren Sie, wie Sie ein Abonnement kündigen oder erneuern oder Lizenzen hinzufügen oder entfernen.  | [Verwalten von Angeboten](csp-commercial-marketplace-manage.md) |
|Erfahren Sie, wie die Abrechnung für kommerzielle Marketplace-Käufe funktioniert. | [Grundlegendes zur Abrechnung](csp-commercial-marketplace-billing.md) |
|Erfahren Sie, wer für welche Arten von Unterstützung für ISV-Käufe zuständig ist. | [Unterstützung](csp-commercial-marketplace-support.md) |
|Erfahren Sie mehr über Verträge und Zuständigkeiten von CSP-Partnern und ISVs im kommerziellen Marketplace | [Grundlegendes zum Vertrag](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> In dieser Übersicht wird beschrieben, wie Partner im CSP-Programm bestimmte kommerzielle Marketplace-Features in Partner Center verwenden können. Im Gegensatz zu Partnern im CSP-Programm haben ISV-Verleger eine andere Marketplace-Rolle. Außerdem verfügen Sie über verschiedene kommerzielle Marketplace-Features, die Ihnen innerhalb von Partner Center zur Verfügung stehen. Weitere Informationen zur Rolle von ISV-Verlegern finden Sie in der [Übersicht über den kommerziellen Marketplace in Azure](/azure/marketplace/partner-center-portal/commercial-marketplace-overview).

## <a name="where-to-complete-commercial-marketplace-activities"></a>Informationen zum Abschluss kommerzieller Marketplace-Aktivitäten

Als Partner im CSP-Programm können Sie viele kommerzielle Marketplace-Aktivitäten für ISV SaaS-Angebote direkt über das Partner Center- [Dashboard](https://partner.microsoft.com/dashboard) oder mithilfe von [Partner Center-APIs](/partner-center/develop/)durchführen. Zum Ausführen anderer Marketplace-Aktivitäten müssen Sie jedoch möglicherweise Folgendes aufrufen:

- Das [Microsoft Azure Verwaltungs Portal](https://portal.azure.com/)

    oder

- System oder Website eines Drittanbieter-ISV-Verlegers

Ein Großteil der Aktivitäten, die Sie zu den abgeschlossenen Aktivitäten machen, beginnt mit dem gewählten Angebotstyp. Partner im CSP-Programm können derzeit zwei Arten von angeboten mit ISV-Verlegern von Drittanbietern durcharbeiten:

1. Lizenz basierte SaaS-Angebote  
2. Nutzungsbasierte Angebote (einschließlich angeboten, die auf virtuellen Computern, Containern oder Azure-Anwendungen basieren)

Besuchen Sie die [Grundlagen der Abrechnung](billing-basics.md) , um mehr darüber zu erfahren, wie sich die Abrechnung zwischen lizenzbasierten angeboten und nutzungsbasierten angeboten unterscheidet.  

In den folgenden Tabellen erfahren Sie, wo Sie eine bestimmte Marketplace-Aktivität für Lizenz basierte oder nutzungsbasierte ISV-Angebote durchführen können.

|**Für Lizenz basierte oder getaktete SaaS-Angebote von ISVs**  |**Verwenden Sie**  |
|:------------------------------------|:------------------|
|So finden Sie verfügbare Angebote und suchen nach verfügbaren angeboten  | Partner Center-Dashboard oder Partner Center-APIs  |
|So erwerben Sie ein Angebot  | Partner Center-Dashboard oder Partner Center-APIs  |
|So stellen Sie ein erworbenes Angebot bereit (Konto Einrichtung, Software Verwaltung oder Bereitstellung im Aad-Mandanten des Kunden)  | System oder Website des ISV-Verlegers  |
|So können Sie Angebots Abonnements Abbrechen/erneuern oder Lizenzen hinzufügen/entfernen | Partner Center-Dashboard oder Partner Center-APIs  |
|So erstellen Sie Benutzer oder verwalten Berechtigungen  | System oder Website des ISV-Verlegers  |

|**Für nutzungsbasierte Angebote von ISVs**  |**Verwenden Sie**  |
|:------------------------------------|:------------------|
|So finden Sie verfügbare Angebote und suchen nach verfügbaren angeboten  | Partner Center-Dashboard, Partner Center-APIs oder Azure-Portal  |
|So erwerben Sie ein Angebot  | Azure-Portal  |
|So stellen Sie ein erworbenes Angebot bereit (Konto Einrichtung, Software Verwaltung oder Bereitstellung im Aad-Mandanten des Kunden)  | Azure-Portal  |
|So können Sie Angebots Abonnements Abbrechen/erneuern oder Lizenzen hinzufügen/entfernen | Azure-Portal  |
|So erstellen Sie Benutzer oder verwalten Berechtigungen  | Azure-Portal  |

## <a name="next-steps"></a>Nächste Schritte

- [Entdecken oder anzeigen kommerzieller Marketplace-Angebote](csp-commercial-marketplace-discover.md)
- [Erwerben kommerzieller Marketplace-Angebote](csp-commercial-marketplace-purchase.md)