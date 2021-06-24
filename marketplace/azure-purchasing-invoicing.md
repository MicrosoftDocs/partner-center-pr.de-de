---
title: Erwerb von Software und Lösungen von Azure Marketplace
description: Erfahren Sie mehr über Tools, die Softwarekäufe und -verwaltung in Azure Marketplace vereinfachen und optimieren.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 0e79674825f8ab28fa4b0e68dd01c9c1b7e8c27a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565184"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace Kauf

Azure Marketplace verfügt über zahlreiche Tools und Features, die den Kaufprozess, die Rechnungsstellung und die Verwaltung von Kaufrichtlinien vereinfachen und optimieren.

## <a name="simplified-procurement"></a>Vereinfachte Beschaffung

Der Azure Marketplace hilft Ihnen durch verschiedene Kaufoptionen dabei, den Beschaffungsprozess zu vereinfachen. Wenn Sie Produkte mithilfe einer Kreditkarte erwerben, die Ihrem Azure-Konto zugeordnet ist, werden alle Käufe auf einer einzigen Rechnung konsolidiert und der Kreditkarte Ihrer Wahl in Rechnung gestellt. Wenn Sie ein großer Kunde sind, können Sie mit einem Enterprise Agreement erwerben. Bei einem EA sind alle Softwarekäufe automatisch in Ihrer Azure-Rechnung enthalten. Auf Ihrer Rechnung sind dann zuerst die Gebühren für die Nutzung von Azure aufgeführt und dann die Azure Marketplace-Gebühren.

Wenn Sie über Azure Marketplace erwerben, entfällt die Komplexität der Verwaltung einzelner Anbieterbeziehungen und Rechnungen. Sie erhalten eine einzelne konsolidierte monatliche Rechnung von Microsoft, die sowohl Ihre Azure Marketplace als auch Ihre Azure-Gebühren enthält.

## <a name="permission-to-purchase"></a>Berechtigung zum Kauf

Nachdem Sie die richtige Softwareanwendung gefunden haben, ist der Kauf einfach. Sie benötigen jedoch geeignete Berechtigungen innerhalb des Azure-Abonnements. Da Azure auf einem [rollenbasierten Access Control-Modell](/azure/role-based-access-control/overview) (Role Based Access Control, RBAC) basiert, benötigt Ihr Konto Berechtigungen vom **Typ "Abonnementbesitzer"** oder **"Mitwirkender",** um einen Kauf tätigen zu können.

Bevor Sie einen Kauf abschließen, stellen Sie sicher, dass der Benutzer über die richtige Konfiguration im Azure-Mandanten verfügt. Dadurch können Fehler während des Kaufs verhindert werden.

Suchen Sie auf der Azure Marketplace im Azure-Portal nach der Anwendung, die Sie kaufen möchten, und wählen **Sie Erstellen** oder Einrichten **+ Abonnieren** aus. Sie werden aufgefordert, einige Informationen zu machen, bevor Sie Ihre neue Lösung verwenden können.

> [!CAUTION]
> Die Genehmigung im privaten Marketplace weist nicht auf die Beschaffung einer Lösung hin.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Die Schaltfläche &quot;Erstellen&quot; des Angebots.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Die Schaltfläche Einrichten + Abonnieren.":::

Wenn Sie eine Lösung aus dem Azure Marketplace Onlineshop bereitstellen möchten, wählen Sie auf der Seite mit der Produktbeschreibung die Option **Jetzt** abrufen aus, und melden Sie sich dann mit den Anmeldeinformationen Ihres Azure-Kontos an.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Das Dialogfeld für die Azure Marketplace Anmeldung.":::

Nachdem Sie sich angemeldet haben, werden Sie auf das Produkt im Azure-Portal umgeleitet, um Ihren Kauf abzuschließen.

## <a name="purchase-policy-management"></a>Verwaltung von Kaufrichtlinien

Mit Microsoft können Sie Benutzerkäufe über Ihr Abrechnungsprofil als Azure-Abonnementadministrator verwalten. Wählen Sie zwischen drei Optionen aus:

- **Free + Paid** : Ermöglicht Benutzern das Erwerben Azure Marketplace Softwareanwendung.
- **Free:** Ermöglicht Benutzern, nur kostenlose Software aus Azure Marketplace bereitzustellen.
- **Nein:** Verhindert, dass Benutzer Software von Azure Marketplace bereitstellen.

Diese Einstellungen gelten für alle Benutzer mit Zugriff auf Ihr Azure-Abonnement, wodurch Sie die IT-Beschaffung über die Azure-Portal steuern können.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Steuern der IT-Beschaffung über die Azure-Portal.":::

## <a name="cost-management"></a>Kostenverwaltung

Wenn Sie Produkte von Azure Marketplace erwerben, möchten Sie Erkenntnisse gewinnen, die Ihnen beim Verwalten der Kosten helfen. Azure Cost Management ist ein kostenloses Tool zum Anzeigen von Informationen zu den erworbenen Produkten. Sie können Cost Management verwenden, um Details darüber anzuzeigen, für welche Dienste Sie im Laufe der Zeit Geld ausgeben und wie diese Kosten im Vergleich zu den von Ihnen festgelegten Budgets nachverfolgt werden. Zusätzlich zum Festlegen von Budgets können Sie Berichte planen und Abonnementkosten analysieren. Weitere Informationen zu Azure Cost Management finden Sie im modul Microsoft Learn unter Analysieren von [Kosten und Erstellen von Budgets mit Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Im Kostenanalysetool von Azure Cost Management können Sie Ihre Azure Marketplace-Gebühren und -Rechnungen anzeigen.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Verwenden Sie Azure Cost Management, um Einblicke in Ihre erworbenen Produkte zu erhalten.":::

## <a name="purchase-validation-checks"></a>Überprüfungen der Kaufvalidierung

Der Erwerb eines Angebots über Azure Marketplace kann aus verschiedenen Gründen fehlschlagen. Die Verwendung der Befehlszeilenschnittstelle (COMMAND-Line Interface, CLI) für einen Kauf führt wahrscheinlicher zu Fehlern, da Sie möglicherweise versuchen, ein Angebot zu erwerben, das in Azure Marketplace nicht verfügbar oder sichtbar ist. Im Folgenden finden Sie die Überprüfungen, die dazu führen können, dass ein Kauf fehlschlägt:

1. Das Abonnement gehört zu einem Enterprise Agreement (EA), und der EA-Administrator hat Azure Marketplace Käufe deaktiviert.
1. Der EA-Administrator hat Käufe nur für kostenlose Angebote aktiviert, und das Angebot ist ein kostenpflichtiges Angebot.
1. Das Angebot befindet sich nicht im Marketplace.
1. Der unabhängige Softwarehersteller (Independent Software Vendor, ISV) hat den Verkauf des Angebots beendet, zumindest in Ihrer Region.
1. Das von Ihnen verwendete Abonnement gehört zu einem Abrechnungskonto in einer Region, in der das Angebot nicht verfügbar ist.
1. Das Abonnement-/Abrechnungskonto ist keinem gültigen Zahlungsmittel (z. B. einer gültigen Kreditkarte) zugeordnet.
1. Das Abonnement gehört zu einem Cloud Solution Provider (CSP), und der ISV hat den Verkauf über einen CSP abgelehnt.
1. Der private Marketplace ist für das Abonnement aktiviert, und das Angebot ist nicht in der Liste der zulässigen Angebote enthalten.
1. Das Angebot ist privat/Vorschau für bestimmte Kunden, und das Abonnement ist nicht in der Liste der zulässigen Kunden enthalten.

Der Erwerb von Marketplace-Angeboten schlägt möglicherweise fehl, wenn ein Konflikt mit der vom Azure-Administrator in Ihrer Organisation definierten Azure Policy besteht. Beispielsweise können Sie Microsoft.SaaS nicht erwerben, wenn es nicht in der **Liste der zulässigen** Dateien Ihrer Organisation enthalten ist. Weitere Informationen finden Sie in [der Azure Policy-Dokumentation.](/azure/governance/policy/)

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Fakturierung](billing-invoicing.md)