---
title: Festlegen eines Azure-Ausgabenbudgets für Kunden
ms.topic: how-to
ms.date: 03/17/2021
description: Erfahren Sie, wie Sie ein monatliches Azure-Ausgabenbudget für Ihre Kunden einrichten oder entfernen und wie Sie Azure-Ausgaben Daten anzeigen und Budget bezogene Benachrichtigungen festlegen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712748"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Festlegen, überprüfen oder Entfernen eines monatlichen Azure-Ausgabenbudgets für Kunden im Partner Center

**Geeignete Rollen**

- Administrator-Agent

Sie können [ein monatliches Azure-Ausgabenbudget für Ihre Kunden](#set-azure-spending-budget) im Partner Center festlegen. Dadurch können Ihre Kunden ihre Azure-Ausgaben verwalten. Mit dieser Option können Sie die Azure-Ausgaben ihrer Kunden mit dem Budget innerhalb des Monats vergleichen. Außerdem hilft es Ihren Kunden, ihre Azure-Ausgaben zu berechnen, sodass Ihre monatliche Rechnung nicht höher als erwartet ist.

> [!NOTE]  
> Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.

Nachdem Sie [ein Azure-Ausgabenbudget für Ihre Kunden festgelegt](#set-azure-spending-budget)haben, können Sie die Kundennutzung auf folgende Weise überprüfen. Mithilfe dieser Optionen können Sie falsch konfigurierte Dienste oder ungewöhnliche Trends erkennen, die möglicherweise einen Betrugsversuch vorschlagen. Sie können dann mit ihren Kunden zusammenarbeiten, um die Ursache zu ermitteln und die Kosten zu verwalten. Falls erforderlich, können Sie auch [das Budget des Kunden](#set-azure-spending-budget) in einen höheren Betrag ändern.

- [Überprüfen der aktuellen Azure-Ausgaben](#check-current-azure-spending)

- [E-Mail-Benachrichtigungen aktivieren, wenn die Ausgaben eines Kunden dem Budget Limit nähern](#notifications-for-budget-limits)

- [Anzeigen der aufgelisteten Kosten nach Dienst für nutzungsbasierte Abonnements](#itemized-costs-by-service)

Sie können auch [ein Azure-Ausgabenbudget](#remove-azure-spending-budget) für Kunden jederzeit entfernen.

## <a name="azure-spending-data"></a>Azure-Ausgaben Daten

Die Azure-Ausgaben Daten sind *geschätzt* , und die *tatsächlichen Abrechnungs Beträge können variieren*. Der Wert der Daten *spiegelt nicht* die Steuern, Gutschriften, Anpassungen oder andere Gebühren wider, die anfallen können.

Die Ausgaben Daten werden *einmal täglich aktualisiert*. Ihre Kunden können weiterhin Azure-Dienste und-Ressourcen nutzen (und dafür in Rechnung gestellt werden), es sei denn, Sie ändern die Kontoeinstellungen in der Azure-Portal.

## <a name="set-azure-spending-budget"></a>Festlegen des Azure-Ausgabenbudgets

Sie können *ein monatliches Azure-Ausgabenbudget* für mehrere Kunden im Partner Center festlegen:

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.

3. Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements** die Kunden aus, für die Sie ein Budget festlegen möchten.

4. Geben Sie einen Wert für **monatliches Budget** ein.

5. Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.

Sie können auch *ein Budget für einen einzelnen Kunden* in seinen Abonnement Einstellungen festlegen:

1. Melden Sie sich beim Partner Center-Dashboard an.

2. Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.

3. Wählen Sie auf der Seite **Kunden** den **Firmennamen** des Kunden aus.

4. Wählen Sie auf der Seite **Abonnements** des Kunden unter **Nutzungs basiertes Abonnement** die Option **Budget ändern** aus.

5. Geben Sie einen Wert für das Budget ein.

6. Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.

## <a name="remove-azure-spending-budget"></a>Azure-Ausgabenbudget entfernen

Sie können *ein monatliches Azure-Ausgabenbudget* für Ihre Kunden im Partner Center entfernen:

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.

3. Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements** die Kunden aus, deren Budget Sie entfernen möchten.

4. Wählen Sie **Budget entfernen** aus.

## <a name="check-current-azure-spending"></a>Überprüfen der aktuellen Azure-Ausgaben

Sie können *die aktuellen Azure-Ausgaben und monatlichen Budgets von Kunden* jederzeit nachverfolgen:

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.

3. Auf der **Azure-Ausgaben** Seite unter **Kunden mit Microsoft Azure-Abonnements** können Sie eine Übersicht über die monatlichen Budgets von Kunden, die aktuellen Ausgabenschätzungen und den Prozentsatz des verwendeten Budgets anzeigen.

## <a name="notifications-for-budget-limits"></a>Benachrichtigungen für Budget Limits

Sie können *e-Mail-Benachrichtigungen* aktivieren, wenn die monatlichen Ausgaben Ihres Kunden dem Budget Limit nähern. Wenn Sie diese Option aktivieren, werden Sie benachrichtigt, wenn Kunden mindestens 80% Ihres monatlichen Budgets verwenden. Mit dieser Option können Sie Ihre Azure-Rechnung überwachen. So konfigurieren Sie e-Mail-Benachrichtigungen

1. Melden Sie sich bei Partner Center an.

2. Wechseln Sie zu **Einstellungen**.

3. Wählen Sie **meine Einstellungen** aus.

4. Konfigurieren Sie ggf. eine bevorzugte e-Mail-Adresse.

5. Konfigurieren Sie die bevorzugte Sprache für die Benachrichtigung.

6. Wählen Sie im Abschnitt **Benachrichtigungseinstellungen** die Registerkarte **CSP** .

7. Aktivieren Sie die e-Mail-Option **Azure-Ausgaben** Benachrichtigung, und **Speichern** Sie Sie.


## <a name="itemized-costs-by-service"></a>Itemisierte Kosten nach Dienst

Sie können die *aufgelisteten Kosten (und die geschätzte Nutzung) nach Dienst für nutzungsbasierte Abonnements anzeigen*:

1. Melden Sie sich bei Partner Center an.

2. Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.

3. Wählen Sie auf der Seite **Kunden** den **Firmennamen** des Kunden aus.

4. Wählen Sie auf der Seite **Abonnements** des Kunden unter **nutzungsbasierte Abonnements** den Namen des **Abonnements** aus.

5. Auf der Seite des Abonnements können Sie die **aufgelisteten Kosten** nach Dienst und die **geschätzte Nutzung** des aktuellen Monats überprüfen.


## <a name="next-steps"></a>Nächste Schritte

- [Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung](azure-plan-billing.md)
