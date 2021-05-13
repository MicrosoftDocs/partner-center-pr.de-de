---
title: Festlegen eines Azure-Ausgabenbudgets für Kunden
ms.topic: how-to
ms.date: 03/17/2021
description: Erfahren Sie, wie Sie monatliche Azure-Ausgabenbudgets für Ihre Kunden festlegen oder entfernen sowie Azure-Ausgabendaten anzeigen und budgetbezogene Benachrichtigungen festlegen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855351"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Festlegen, Überprüfen oder Entfernen monatlicher Azure-Ausgabenbudgets für Kunden in Partner Center

**Geeignete Rollen:** Administrator-Agent

Sie können [ein monatliches Azure-Ausgabenbudget für Ihre Kunden](#set-azure-spending-budget) in Partner Center festlegen. Dies hilft Ihren Kunden bei der Verwaltung ihrer Azure-Ausgaben. Mit dieser Option können Sie die Azure-Ausgaben Ihrer Kunden mit dem Budget während des Monats vergleichen. Außerdem können Ihre Kunden ihre Azure-Ausgaben so planen, dass ihre monatliche Rechnung nicht höher als erwartet ist.

> [!NOTE]  
> Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.

Nachdem Sie [ein Azure-Ausgabenbudget für Ihre Kunden festgelegt](#set-azure-spending-budget)haben, können Sie die Kundennutzung auch wie folgt überprüfen. Diese Optionen können Ihnen helfen, falsch konfigurierte Dienste oder ungewöhnliche Trends zu erkennen, die auf Betrug hindeuten können. Anschließend können Sie mit Ihren Kunden zusammenarbeiten, um die Grundursache zu ermitteln und die Kosten zu verwalten. Bei Bedarf können Sie auch das Budget des Kunden in einen höheren Betrag [ändern.](#set-azure-spending-budget)

- [Überprüfen der aktuellen Azure-Ausgaben](#check-current-azure-spending)

- [Aktivieren von E-Mail-Benachrichtigungen für den Zeitpunkt, an dem sich die Ausgaben eines Kunden dem Budgetlimit nähern](#notifications-for-budget-limits)

- [Anzeigen der aufgeschlüsselten Kosten nach Dienst für nutzungsbasierte Abonnements](#itemized-costs-by-service)

Sie können auch [jederzeit ein Azure-Ausgabenbudget](#remove-azure-spending-budget) für Kunden entfernen.

## <a name="azure-spending-data"></a>Azure-Ausgabendaten

Die Azure-Ausgabendaten sind eine *Schätzung,* und *die tatsächlichen Abrechnungsbeträge können variieren.* Der Wert der Daten *spiegelt keine* Steuern, Gutschriften, Anpassungen oder andere Gebühren wider, die möglicherweise anfallen.

Die Ausgabendaten *werden einmal pro Tag aktualisiert.* Ihre Kunden können weiterhin Azure-Dienste und -Ressourcen verwenden (und dafür in Rechnung gestellt werden), es sei denn, Sie ändern ihre Kontoeinstellungen im Azure-Portal.

## <a name="set-azure-spending-budget"></a>Festlegen des Azure-Ausgabenbudgets

Sie können *ein monatliches Azure-Ausgabenbudget* für mehrere Kunden in Partner Center:

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im linken Menü unter **CSP** die Option **Azure-Ausgaben aus.**

3. Wählen Sie **auf der Seite Azure-Ausgaben** unter Kunden **Microsoft Azure** Abonnements die Kunden aus, für die Sie ein Budget festlegen möchten.

4. Geben Sie einen Wert für **Monatliches Budget ein.**

5. Wählen Sie **Übernehmen aus,** um Ihre Änderungen zu speichern.

Sie können auch *ein Budget für einen einzelnen Kunden* in den Abonnementeinstellungen festlegen:

1. Melden Sie sich beim Partner Center-Dashboard an.

2. Wählen Sie im linken Menü unter **CSP** die Option **Kunden aus.**

3. Wählen Sie **auf der** Seite Kunden den Firmennamen des **Kunden aus.**

4. Wählen Sie auf der Seite **Abonnements des** Kunden unter **Nutzungsbasiertes Abonnement** die Option Budget ändern **aus.**

5. Geben Sie einen Wert für das Budget ein.

6. Wählen Sie **Übernehmen aus,** um Ihre Änderungen zu speichern.

## <a name="remove-azure-spending-budget"></a>Entfernen des Azure-Ausgabenbudgets

Sie können *ein monatliches Azure-Ausgabenbudget* für Ihre Kunden in Partner Center:

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im linken Menü unter **CSP** die Option **Azure-Ausgaben aus.**

3. Wählen Sie **auf der Seite Azure-Ausgaben** unter **Kunden Microsoft Azure** Abonnements die Kunden aus, deren Budget Sie entfernen möchten.

4. Wählen Sie **Budget entfernen aus.**

## <a name="check-current-azure-spending"></a>Überprüfen der aktuellen Azure-Ausgaben

Sie können *die aktuellen Azure-Ausgaben und monatlichen* Budgets Ihrer Kunden jederzeit nachverfolgen:

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im linken Menü unter **CSP** die Option **Azure-Ausgaben aus.**

3. Auf der **Seite Azure-Ausgaben** finden Sie unter **Kunden mit Microsoft Azure Abonnements** eine Übersicht über die monatlichen Budgets der Kunden, aktuelle Ausgabenschätzungen und den Prozentsatz des verwendeten Budgets.

## <a name="notifications-for-budget-limits"></a>Benachrichtigungen zu Budgetlimits

Sie können *E-Mail-Benachrichtigungen aktivieren,* wenn sich die monatlichen Ausgaben Ihres Kunden dem Budgetlimit nähern. Wenn Sie diese Option aktivieren, werden Sie benachrichtigt, wenn Kunden 80 % oder mehr ihres monatlichen Budgets verwenden. Mit dieser Option können Sie Ihre Azure-Rechnung im Auge behalten. So konfigurieren Sie E-Mail-Benachrichtigungen:

1. Melden Sie sich bei Partner Center an.

2. Wechseln Sie zu **Einstellungen**.

3. Wählen Sie **Meine Einstellungen aus.**

4. Konfigurieren Sie ggf. eine bevorzugte E-Mail-Adresse.

5. Konfigurieren Sie die bevorzugte Sprache für die Benachrichtigung.

6. Wählen Sie im Abschnitt **Benachrichtigungseinstellungen** die Registerkarte **CSP** aus.

7. Aktivieren Sie die Option E-Mail für **Azure-Ausgabenbenachrichtigung,** und **speichern Sie**.


## <a name="itemized-costs-by-service"></a>Aufgeschlüsselte Kosten nach Dienst

Sie können *die nach Dienst aufgeschlüsselten Kosten (und die geschätzte Nutzung) für nutzungsbasierte Abonnements anzeigen:*

1. Melden Sie sich bei Partner Center an.

2. Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.

3. Wählen Sie auf der Seite **Kunden** den **Unternehmensnamen** des Kunden aus.

4. Wählen Sie auf der Seite **Abonnements** des Kunden unter **Nutzungsbasierte Abonnements** den Namen des **Abonnements** aus.

5. Auf der Seite des Abonnements können Sie die **Artikelkosten** nach Dienst und die **geschätzte Nutzung** für den aktuellen Monat überprüfen.


## <a name="next-steps"></a>Nächste Schritte

- [Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung](azure-plan-billing.md)
