---
title: Erwerben von Software und Lösungen aus Azure Marketplace
description: Erfahren Sie mehr über Tools, die den Erwerb und die Verwaltung von Software in Azure Marketplace vereinfachen und optimieren.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: de58fad7af7dd2cd6b8c98e5763557d54cc776a2
ms.sourcegitcommit: c46658f4d70004596e758fe4cd8671b6e9dadeab
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/20/2021
ms.locfileid: "98584196"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace Einkauf

Azure Marketplace verfügt über zahlreiche Tools und Features, die den Erwerb, die Rechnungsstellung und die Verwaltung der Kauf Richtlinien vereinfachen und optimieren.

## <a name="simplified-procurement"></a>Vereinfachte Beschaffung

Der Azure Marketplace hilft Ihnen durch verschiedene Kaufoptionen dabei, den Beschaffungsprozess zu vereinfachen. Wenn Sie Produkte mit einer Kreditkarte kaufen, die Ihrem Azure-Konto zugeordnet ist, werden alle Käufe in einer einzelnen Rechnung konsolidiert und der Kreditkarte Ihrer Wahl in Rechnung gestellt. Wenn Sie ein großer Kunde sind, können Sie ihn mit einem Konzernvertrag erwerben. Bei einem EA werden alle Software Käufe automatisch in ihrer Azure-Rechnung aufgeführt. Auf Ihrer Rechnung sind dann zuerst die Gebühren für die Nutzung von Azure aufgeführt und dann die Azure Marketplace-Gebühren.

Wenn Sie über Azure Marketplace erwerben, entfällt die Komplexität der Verwaltung einzelner Hersteller Beziehungen und-Rechnungen. Sie erhalten eine einzelne, konsolidierte monatliche Rechnung von Microsoft, die sowohl Ihre Azure Marketplace Käufe als auch Ihre Azure-Gebühren umfasst.

## <a name="permission-to-purchase"></a>Kauf Berechtigung

Nachdem Sie die richtige Software Anwendung gefunden haben, ist es einfach, den Kauf abzuschließen. Sie benötigen jedoch entsprechende Berechtigungen innerhalb des Azure-Abonnements. Da in Azure ein [rollenbasiertes Access Control](/azure/role-based-access-control/overview) -Modell (RBAC) betrieben wird, benötigt Ihr Konto **Abonnement Besitzer** oder **Mitwirkender** -Berechtigungen, um einen Kauf zu tätigen.

Vergewissern Sie sich vor Abschluss des Kaufs, dass der Benutzer über die richtige Konfiguration im Azure-Mandanten verfügt. Dadurch werden Fehler beim Kauf verhindert.

Suchen Sie im Azure Marketplace im Azure-Portal nach der Anwendung, die Sie kaufen möchten, und wählen Sie **Erstellen** oder **Einrichten + abonnieren** aus. Sie werden aufgefordert, einige Informationen abzuschließen, bevor Sie Ihre neue Lösung verwenden können.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Die Schaltfläche zum Erstellen des Angebots.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Die Schaltfläche &quot;einrichten + abonnieren&quot;.":::

Wenn Sie eine Lösung aus dem Azure Marketplace Online Store bereitstellen möchten, klicken Sie auf der Seite Produktbeschreibung auf **jetzt starten** , und melden Sie sich mit den Anmelde Informationen Ihres Azure-Kontos an.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Das Dialogfeld Azure Marketplace anmelden.":::

Nachdem Sie sich angemeldet haben, werden Sie an das Produkt im Azure-Portal umgeleitet, um den Kauf abzuschließen.

## <a name="purchase-policy-management"></a>Kauf Richtlinien Verwaltung

Microsoft ermöglicht Ihnen die Verwaltung von Benutzer Käufen über Ihr Abrechnungs Profil als Azure-Abonnement Administrator. Wählen Sie zwischen drei Optionen aus:

- **Free + bezahlt** – ermöglicht Benutzern das Abrufen beliebiger Azure Marketplace Softwareanwendungen.
- **Free** – ermöglicht es Benutzern, nur kostenlose Software aus Azure Marketplace bereitzustellen.
- **Nein** – verhindert, dass Benutzer Software aus Azure Marketplace bereitstellen.

Diese Einstellungen gelten für alle Benutzer mit Zugriff auf Ihr Azure-Abonnement, das Ihnen die Möglichkeit bietet, die IT-Beschaffung über den Azure-Portal zu steuern.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Steuern der IT-Beschaffung durch die Azure-Portal":::

## <a name="cost-management"></a>Kostenverwaltung

Wenn Sie Produkte aus Azure Marketplace erwerben, erhalten Sie Einblicke, die Ihnen bei der Verwaltung der Kosten helfen. Azure Cost Management ist ein kostenloses Tool zum Anzeigen von Informationen zu den Produkten, die Sie gekauft haben. Mit Cost Management können Sie die Details der Dienste anzeigen, für die Sie im Laufe der Zeit Geld aufwenden, und wie diese Kosten gegen das von Ihnen festgelegte Budget nachverfolgt werden. Zusätzlich zum Festlegen von Budgets können Sie Berichte planen und die Abonnementkosten analysieren. Weitere Informationen zu Azure Cost Management finden Sie im Microsoft Learn-Modul unter [Analysieren von Kosten und Erstellen von Budgets mit Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Im Kostenanalysetool von Azure Cost Management können Sie Ihre Azure Marketplace-Gebühren und -Rechnungen anzeigen.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Verwenden Sie Azure Cost Management, um Einblicke in Ihre erworbenen Produkte zu erhalten.":::

## <a name="purchase-validation-checks"></a>Kauf überprüfungsprüfungen

Der Erwerb eines Angebots über Azure Marketplace kann aus unterschiedlichen Gründen fehlschlagen. Das Verwenden der Befehlszeilenschnittstelle (Command-Line Interface, CLI) für einen Einkauf führt wahrscheinlich zu Fehlern, da Sie möglicherweise versuchen, ein Angebot zu erwerben, das in Azure Marketplace nicht verfügbar oder nicht sichtbar ist. Im folgenden finden Sie die Überprüfungen, die einen Kauf Fehler verursachen können:

1. Das Abonnement gehört zu einem Konzernvertrag (EA), und der EA-Administrator ist Azure Marketplace Käufe deaktiviert.
1. Der EA-Administrator hat Käufe nur für kostenlose Angebote aktiviert, und das Angebot ist ein kostenpflichtiges Angebot.
1. Das Angebot wurde im Marketplace nicht gefunden.
1. Der unabhängige Software Hersteller (Independent Software Vendor, ISV) hat das Angebot, zumindest in Ihrer Region, nicht mehr verkauft.
1. Das von Ihnen verwendete Abonnement gehört zu einem Abrechnungskonto in einer Region, in der das Angebot nicht verfügbar ist.
1. Das Abonnement-/Abrechnungs Konto ist keinem gültigen Zahlungsinstrument (z. b. eine gültige Kreditkarte) zugeordnet.
1. Das Abonnement gehört zu einem cloudlösungsanbieter (Cloud Solution Provider, CSP), und der ISV lehnt den Verkauf über einen CSP ab.
1. Der private Marketplace ist für das Abonnement aktiviert, und das Angebot ist nicht in der Liste der zulässigen Angebote enthalten.
1. Das Angebot ist für bestimmte Kunden privat/Vorschau, und das Abonnement ist nicht in der Liste der zulässigen Kunden enthalten.

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Fakturierung](billing-invoicing.md)