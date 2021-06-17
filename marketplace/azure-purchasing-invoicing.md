---
title: Erwerb von Software und Lösungen Azure Marketplace
description: Erfahren Sie mehr über Tools, die Softwarekäufe und -verwaltung in Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: f747c11ef4bfc9abe1035ffb3f059da59b6572ac
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276500"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace Käufe

Azure Marketplace verfügt über zahlreiche Tools und Features, die den Prozess des Kaufs, der Rechnungsstellung und der Verwaltung von Kaufrichtlinien vereinfachen und optimieren.

## <a name="simplified-procurement"></a>Vereinfachte Beschaffung

Der Azure Marketplace hilft Ihnen durch verschiedene Kaufoptionen dabei, den Beschaffungsprozess zu vereinfachen. Wenn Sie Produkte mithilfe einer Kreditkarte erwerben, die Ihrem Azure-Konto zugeordnet ist, werden alle Käufe auf einer einzelnen Rechnung konsolidiert und der Kreditkarte Ihrer Wahl in Rechnung gestellt. Wenn Sie ein großer Kunde sind, können Sie mithilfe eines Enterprise Agreement. Bei einem EA sind alle Softwarekäufe automatisch in Ihrer Azure-Rechnung enthalten. Auf Ihrer Rechnung sind dann zuerst die Gebühren für die Nutzung von Azure aufgeführt und dann die Azure Marketplace-Gebühren.

Wenn Sie über Azure Marketplace erwerben, entfällt die Komplexität der Verwaltung einzelner Anbieterbeziehungen und Rechnungen. Sie erhalten eine einzelne konsolidierte monatliche Rechnung von Microsoft, die sowohl Ihre Azure Marketplace als auch Ihre Azure-Gebühren enthält.

## <a name="permission-to-purchase"></a>Kaufberechtigung

Nachdem Sie die richtige Softwareanwendung gefunden haben, ist der Kauf einfach. Sie benötigen jedoch geeignete Berechtigungen innerhalb des Azure-Abonnements. Da Azure auf einem RBAC-Modell [(Role Based Access Control)](/azure/role-based-access-control/overview)  arbeitet,  benötigt Ihr Konto Berechtigungen für Abonnementbesitzer oder Mitwirkende, um einen Kauf tätigen zu können.

Stellen Sie vor abschluss eines Kaufs sicher, dass der Benutzer über die richtige Konfiguration im Azure-Mandanten verfügt. Dies hilft, Fehler während des Kaufs zu vermeiden.

Suchen Sie Azure Marketplace im Azure-Portal die Anwendung, die Sie kaufen möchten,  und wählen Sie Erstellen oder **Einrichten + abonnieren aus.** Sie werden aufgefordert, einige Informationen zu vervollständigen, bevor Sie Ihre neue Lösung verwenden können.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Die Schaltfläche &quot;Erstellen&quot; des Angebots.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Die Schaltfläche Einrichten + abonnieren.":::

Wenn Sie eine Lösung aus dem Azure Marketplace-Onlineshop bereitstellen  möchten, wählen Sie auf der Produktbeschreibungsseite die Option Jetzt herunterladen aus, und melden Sie sich dann mit Ihren Azure-Kontoanmeldeinformationen an.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Das Azure Marketplace Anmeldedialogfeld.":::

Nach der Anmeldung werden Sie zum Produkt in der Liste weitergeleitet, um Azure-Portal Kauf abschließen zu können.

## <a name="purchase-policy-management"></a>Verwaltung von Kaufrichtlinien

Mit Microsoft können Sie Benutzerkäufe über Ihr Abrechnungsprofil als Azure-Abonnementadministrator verwalten. Wählen Sie zwischen drei Optionen aus:

- **Free + Paid :** Ermöglicht Benutzern das Erwerben beliebiger Azure Marketplace Softwareanwendung.
- **Free:** Ermöglicht Benutzern, nur kostenlose Software aus Azure Marketplace.
- **Nein:** Verhindert, dass Benutzer Software von einem Azure Marketplace.

Diese Einstellungen gelten für alle Benutzer mit Zugriff auf Ihr Azure-Abonnement, wodurch Sie die IT-Beschaffung über die Azure-Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Steuern der IT-Beschaffung über Azure-Portal.":::

## <a name="cost-management"></a>Kostenverwaltung

Wenn Sie Produkte von Azure Marketplace erwerben, möchten Sie Einblicke erhalten, die Ihnen beim Verwalten der Kosten helfen. Azure Cost Management ist ein kostenloses Tool zum Anzeigen von Informationen zu den produkten, die Sie erworben haben. Sie können Cost Management verwenden, um Details zu den Diensten anzuzeigen, für die Sie im Laufe der Zeit Geld ausgeben, und wie diese Kosten im Verhältnis zu den von Ihnen festgelegten Budgets nachverfolgt werden. Zusätzlich zum Festlegen von Budgets können Sie Berichte planen und Abonnementkosten analysieren. Erfahren Sie mehr über Azure Cost Management, indem Sie das Microsoft Learn-Modul unter Analysieren von Kosten und Erstellen von Budgets [mit Azure Cost Management.](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

Im Kostenanalysetool von Azure Cost Management können Sie Ihre Azure Marketplace-Gebühren und -Rechnungen anzeigen.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Verwenden Azure Cost Management, um Einblicke in Ihre erworbenen Produkte zu erhalten.":::

## <a name="purchase-validation-checks"></a>Überprüfungen der Kaufvalidierung

Der Kauf eines Angebots über Azure Marketplace kann aus verschiedenen Gründen fehlschlagen. Die Verwendung der Befehlszeilenschnittstelle (COMMAND-Line Interface, CLI) für einen Kauf verursacht wahrscheinlicher Fehler, da Sie möglicherweise versuchen, ein Angebot zu erwerben, das in der Anwendung nicht verfügbar oder Azure Marketplace. Im Folgenden finden Sie die Überprüfungen, die dazu führen können, dass ein Kauf fehlschlägt:

1. Das Abonnement gehört zu einem Enterprise Agreement (EA), und der EA-Administrator hat Azure Marketplace deaktiviert.
1. Der EA-Administrator hat Käufe nur für kostenlose Angebote aktiviert, und das Angebot ist ein kostenpflichtiges Angebot.
1. Das Angebot wurde im Marketplace nicht gefunden.
1. Der unabhängige Softwarehersteller (Independent Software Vendor, ISV) hat den Verkauf des Angebots beendet, zumindest in Ihrer Region.
1. Das abonnement, das Sie verwenden, gehört zu einem Abrechnungskonto in einer Region, in der das Angebot nicht verfügbar ist.
1. Das Abonnement-/Abrechnungskonto ist einem gültigen Zahlungsmittel (z. B. einer gültigen Kreditkarte) nicht zugeordnet.
1. Das Abonnement gehört zu einem Cloud Solution Provider (CSP), und der ISV hat den Verkauf über einen CSP abgelehnt.
1. Der private Marketplace ist für das Abonnement aktiviert, und das Angebot ist nicht in der Liste der zulässigen Angebote enthalten.
1. Das Angebot ist privat/Vorschau für bestimmte Kunden, und das Abonnement ist nicht in der Liste der zulässigen Kunden enthalten.

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Fakturierung](billing-invoicing.md)