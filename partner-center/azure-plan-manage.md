---
title: Verwalten von Abonnements und Ressourcen in einem Azure-Plan | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Partner mithilfe der verschiedenen Optionen für die rollenbasierte Zugriffssteuerung (Role-Based Access Control, RBAC) die operative Kontrolle über und die Verwaltung für die Azure-Ressourcen eines Kunden erhalten.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 15d1fd3bdff078e752f3b3acb9b200300dc2e64b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253276"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Verwalten von Abonnements und Ressourcen in einem Azure-Plan

Wenn Sie einen Kunden auf den Azure-Plan umstellen, werden Ihnen standardmäßig privilegierte Administratorrechte in Azure zugewiesen (Abonnementbesitzerrechte im Auftrag, die durch den Administrator wahrgenommen werden).

 > [!NOTE]
 > Die Administratorrechte für das Azure-Abonnement können vom Kunden auf Abonnement-, Ressourcengruppen- oder Workloadebene entfernt werden. 

 Partner können die operative Kontrolle und Verwaltung der Azure-Ressourcen eines Kunden in CSP rund um die Uhr (24/7) erreichen, indem sie verschiedene Optionen verwenden, die über die Funktion zur rollenbasierten Zugriffsteuerung (RBAC) zur Verfügung gestellt werden. 

- **Administrator im Auftrag von (Admin on Behalf Of, AOBO)** : Mit [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) hat jeder Benutzer mit der Rolle „Administrator-Agent“ im Partnermandanten RBAC-Besitzerzugriff auf Azure-Abonnements, die du im Rahmen des CSP-Programms erstellst.

- **Azure Lighthouse**: AOBO bietet nicht die Flexibilität, verschiedene, getrennte Gruppen zu erstellen, die mit verschiedenen Kunden zusammenarbeiten, oder für Gruppen und Benutzer verschiedene Rollen zu aktivieren. Mithilfe von Azure Lighthouse können Sie verschiedene Gruppen verschiedenen Kunden oder Rollen zuweisen. Da Benutzer in Form der delegierten Ressourcenverwaltung von Azure über eine geeignete Zugriffsebene verfügen, können Sie die Anzahl der Benutzer verringern, die über die Rolle „Administrator-Agent“ verfügen (und daher vollständigen AOBO-Zugriff besitzen). Dies hilft, die Sicherheit zu verbessern, indem unnötiger Zugriff auf die Ressourcen deiner Kunden vermieden wird. Außerdem erhalten Sie mehr Flexibilität beim Verwalten mehrerer Kunden in großem Maßstab. Weitere Informationen finden Sie unter [Azure Lighthouse und das Programm für Cloud-Lösungsanbieter](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider).

-  **Verzeichnis- oder Gastbenutzer oder [Dienstprinzipale](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)** : Sie können den Zugriff auf CSP-Abonnements im Detail delegieren, indem Sie Benutzer im Kundenverzeichnis hinzufügen oder Gastbenutzer hinzufügen und ihnen spezifische RBAC-Rollen zuweisen. 

Microsoft empfiehlt als Sicherheitsmaßnahme, dass Benutzer nur über die Minimalberechtigungen verfügen, die sie zum Durchführen ihrer Arbeit benötigen. Weitere Informationen erhalten Sie unter [Ressourcen für das Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure). 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Verknüpfen Sie Ihre Partner-ID (MPN ID) mit Ihren Anmeldeinformationen, um die Azure-Ressourcen von Kunden zu verwalten

Die folgende Tabelle zeigt die Methoden. die verwendet werden, um Ihre Partner-ID den verschiedenen RBAC-Zugriffsoptionen zuzuordnen.

|**Kategorie**   |**Szenario**   |**MPN ID-Zuordnung**|
|-----------------|:------------------------|:------------------|
|AOBO   |Ein direkter CSP-Partner oder ein indirekter Anbieter erstellt das Abonnement für den Kunden und macht dabei den direkten CSP-Partner oder den indirekten Anbieter mithilfe von AOBO zum Standardbesitzer des Abonnements. Direkte CSP-Partner oder indirekte Anbieter erteilen indirekten Zugriff auf das Abonnement für Wiederverkäufer mithilfe von AOBO.|Automatisch (keine Aktion vom Partner erforderlich)|
|Azure Lighthouse|Partner erstellt ein neues [Angebot für verwaltete Dienste in Marketplace](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers). Dieses Angebot wird im CSP-Abonnement angenommen, und der Partner erhält Zugriff auf das CSP-Abonnement.|Automatisch (keine Aktion vom Partner erforderlich)|
|Azure Lighthouse|Der Partner stellt eine [ARM-Vorlage](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer) im Azure-Abonnement bereit|Der Partner muss die MPN-ID im Partnermandanten dem Benutzer oder Dienstprinzipal zuordnen. Weitere Informationen findest du unter [Verknüpfung mit Partner-ID](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|
|Verzeichnis- oder Gastbenutzer|Der Partner erstellt im Kundenverzeichnis einen neuen Benutzer oder Dienstprinzipal und erteilt dem Benutzer Zugriff auf das CSP-Abonnement. Der Partner erstellt im Kundenverzeichnis einen neuen Benutzer oder Dienstprinzipal. Der Partner fügt den Benutzer einer Gruppe hinzu, und erteilt der Gruppe Zugriff auf das CSP-Abonnement.|Der Partner muss im Kundenmandanten die MPN-ID dem Benutzer oder Dienstprinzipal zuordnen. Weitere Informationen findest du unter [Verknüpfung mit Partner-ID](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Überprüfen Sie, ob Sie über Administratorzugriff verfügen

Sie benötigen Administratorzugriff, um die Dienste Ihres Kunden zu verwalten und um erworbene Guthaben zu empfangen. Detaillierte Informationen zu erworbenen Guthaben finden Sie unter [Vom Partner erworbene Guthaben](partner-earned-credit.md). Sie können auf zweierlei Weise feststellen, ob Sie Administratorzugriff besitzen.

- Überprüfen der täglichen Nutzungsdatei: Dies kann so erfolgen, dass der Einzelpreis und der effektive Preis pro Einheit in der täglichen Nutzungsdatei verglichen werden und überprüft wird, ob ein Rabatt angewendet wird. Wenn Sie den Rabatt empfangen, sind Sie der Administrator.

- Erstellen einer Azure Monitor-Warnmeldung: Sie können eine [Warnmeldung](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) des Azure Monitor-Aktivitätsprotokolls erstellen, damit Sie benachrichtigt werden, wenn Ihr RBAC-Zugriff aus dem CSP-Abonnement entfernt wird.

### <a name="create-an-azure-monitor-alert"></a>Erstellen einer Azure Monitor-Warnmeldung

1. Erstellen einer Warnmeldung.

![Azure-Warnmeldung](images/azure/azurealert1.png)

2. Wählen Sie die Art der Aktion aus, die die Warnmeldung ausführen soll. Wenn Sie beispielsweise angeben, dass Sie eine E-Mail erhalten möchten, empfangen Sie eine E-Mail, die Sie benachrichtigt, falls Löschungen von Rollenzuweisungen auftreten.

![Konfigurieren der Warnmeldung](images/azure/azureconfigurealert2.png)

### <a name="aobo-removal"></a>AOBO-Entfernung

Kunden können den Zugriff auf ihre Abonnements verwalten, indem sie im Azure-Portal zu **Zugriffssteuerung** navigieren. Auf der Registerkarte **Rollenzuweisungen** wählen sie **Zugriff entfernen** aus. Wenn dies geschieht, haben Sie die folgenden Möglichkeiten:

- Setzen Sie sich mit Ihrem Kunden in Verbindung, um herauszufinden, ob der Administratorzugriff wiederhergestellt werden kann.
- Verwenden Sie den Zugriff, der durch die [rollenbasierte Zugriffssteuerung (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview) zur Verfügung steht.
- Verwenden Sie den Zugriff, der durch [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) zur Verfügung steht.

Der rollenbasierte Zugriff unterscheidet sich vom Administratorzugriff. Rollen grenzen präzise ein, was Sie ausführen können und was nicht. Der Administratorzugriff ist breiter.

Um die Rollen zu sehen, die zum Erwerb von PEC berechtigt sind, lesen Sie [Roles and permissions for the partner earned credit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2) (Rollen und Berechtigungen für vom Partner erworbenes Guthaben).




**Weitere Informationen**

- [Wiederrufen und Reaktivieren von Administratorrechten für Azure CSP-Abonnements](revoke-reinstate-csp.md)

- [Vom Partner erworbenes Guthaben – Übersicht](partner-earned-credit.md)

- [Vom Partner erworbenes Guthaben für verwaltete Dienste](partner-earned-credit-explanation.md)