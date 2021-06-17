---
title: Integration von Azure Marketplace-Partnerlösungen
description: Erfahren Sie mehr über Azure Marketplace Lösungen, die in Ihre Azure-Umgebung integriert werden können, und erhalten Sie einen Link zu Bereitstellungsanleitungen von Microsoft-Partnern.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276483"
---
# <a name="azure-marketplace-partner-integrations"></a>Integration von Azure Marketplace-Partnerlösungen

Erfahren Sie, wie Sie Partnerlösungen in Ihre Azure-Umgebung integrieren. Dieser Artikel bietet eine Übersicht über die einzelnen Lösungen und Links zu detaillierten Bereitstellungshandbüchern. Lösungen werden in alphabetischer Reihenfolge aufgeführt. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka in Confluent Cloud

![Confluent Cloud.](./media/partners/confluent-cloud.png)

Mit Azure können Sie zusätzlich zu Ihren Cloudanwendungen auch in Confluent Cloud integrieren. Confluent-Kunden navigieren häufig zwischen Azure-Portal und Confluent Cloud. Sobald ein Benutzer beispielsweise ein Confluent Cloud-Angebot in Azure Marketplace erwirbt, wird davon ausgegangen, dass er ein Konto bei Confluent Cloud eingibt. Dieser Prozess erhöht die Komplexität und die Zeit und erfordert, dass Benutzer die Konfiguration und Ressourcen zwischen den beiden Portalen verwalten. Um die Verwaltungslast plattformübergreifend zu reduzieren, hat Microsoft in Zusammenarbeit mit Confluent Cloud eine integrierte Bereitstellungsebene von Azure in Confluent Cloud erstellt. Die Lösung ist in Azure Marketplace verfügbar und bietet eine nahtlose Benutzeroberfläche für die Verwendung des Confluent Cloud-Angebots in Azure.

Die Lösung verwendet einen in Azure aktivierten Ressourcenanbieter zum Bereitstellen von Confluent Cloud-Ressourcen. Dadurch können Benutzer über die Azure-Portal, Azure CLI und Azure SDKs auf Echtzeitereignisstreaming zugreifen. Confluent Cloud besitzt und führt die SaaS-Anwendung aus, die Umgebungen, Cluster, Themen, API-Schlüssel und verwaltete Connectors umfasst.

Die umfassende Integration in Confluent Cloud ermöglicht die folgenden Funktionen:

- Bereitstellen einer neuen Confluent Cloud-Organisationsressource mit vollständig verwalteter Infrastruktur über das Azure-Portal.
- Optimieren des einmaligen Anmeldens von Azure bei Confluent Cloud mit Azure Active Directory keine separate Authentifizierung über das Confluent Cloud-Portal erforderlich.
- Erhalten Sie eine einheitliche Abrechnung der Confluent Cloud-Verbrauchsgebühren über die Rechnungsstellung von Azure-Abonnements.
- Verwalten Sie Confluent Cloud-Ressourcen über die Azure-Portal, und verfolgen Sie sie neben Ihren Azure-Ressourcen auf der Seite **Alle Ressourcen** nach.

[Leitfäden zur Confluent Cloud-Bereitstellung](https://docs.confluent.io/current/cloud/marketplace/index.html)

Wenn Sie Probleme im Zusammenhang mit Confluent in Azure haben, wechseln Sie zu [https://support.confluent.io](https://support.confluent.io) . Wenn Sie ein erstmaliger Benutzer sind, setzen Sie Ihr Kennwort zurück, bevor Sie sich beim Confluent-Supportportal anmelden. Wenn Sie kein Konto bei Confluent haben, senden Sie eine E-Mail an [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![DataDog-Logo.](./media/partners/datadog.png)

Datadog bietet Azure-Benutzern Überwachungs- und Sicherheitstools, um die Integrität und Leistung ihrer Anwendungen in Hybrid- und Multi-Cloud-Umgebungen zu verstehen. Zum Konfigurieren der erforderlichen Integrationen ist jedoch häufig das Navigieren zwischen dem Azure-Portal und Datadog erforderlich. Um die Konfiguration und Ressourcenverwaltung portalübergreifend zu vereinfachen, hat Microsoft mit Datadog zusammengearbeitet, um eine integrierte Datadog-Lösung in Azure zu erstellen. Diese Lösung ist über die Azure Marketplace verfügbar und bietet Azure-Kunden eine nahtlose Benutzeroberfläche für die Verwendung der Cloudüberwachungslösung von Datadog.

Weitere Informationen zu dieser Lösung und zur Registrierung für die öffentliche Vorschau finden Sie in der [Azure Monitor-Dokumentation.](/azure/azure-monitor/platform/partners#datadog)

## <a name="next-steps"></a>Nächste Schritte

- [Azure Marketplace Onlineshop](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Erstellen eines Azure-Kontos](/learn/modules/create-an-azure-account/)
