---
title: Verwalten von Marketplace-Produkten & angeboten
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Mithilfe von Partner Center erfahren Sie, wie cloudlösungsanbieter ISV-Angebote von Drittanbietern verwalten können, die für Kunden aus dem kommerziellen Marketplace erworben wurden.
author: rbars
ms.author: rbars
keywords: Abonnements, Marketplace, Drittanbieter, ISV, SaaS-Angebote, cloudlösungsanbieter-Programm, Verwalten eines Angebots, Verwalten eines Abonnements, Lizenzen, kündigen eines Abonnements, Arbeitsplätze, Deaktivieren der automatischen Verlängerung, indirekte Reseller-MPN-ID
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a2d64a18410ac5a668d7ace8f236716df21eb2bc
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947756"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Verwalten Sie kommerzielle Marketplace-Produkte und-Angebote für Ihre Kunden

**Zielgruppe**

- Partner Center
- Partner im CSP-Programm

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent

Partner im CSP-Programm (Cloud Solution Provider) können das Partner Center-Portal verwenden, um zahlreiche ISV-SaaS-Angebote oder-Abonnements für Ihre Kunden über den kommerziellen Marketplace zu erwerben. Nachdem Sie ein Angebot erworben haben, haben Sie verschiedene Möglichkeiten, es zu verwalten.

## <a name="view-or-edit-a-subscription"></a>Anzeigen oder Bearbeiten eines Abonnements

Nachdem Sie ein Abonnement von einem Drittanbieter-ISV-Verleger erworben haben, können Sie es wie folgt überprüfen oder bearbeiten:

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü die Option **Kunden** aus.

2. Wählen Sie einen geeigneten Kunden aus, und klicken Sie dann auf **Abonnements**. Dadurch werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.

3. Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie anzeigen oder bearbeiten möchten. Dadurch erhalten Sie weitere Informationen zum Einrichten oder Bereitstellen des Angebots. (Wenn mehr Aktionen für das Angebot erforderlich sind, wird möglicherweise auch der Status "Aktion erforderlich" in der Spalte Status angezeigt. Dies kann auch von einem Link zur Website des ISV-Verlegers begleitet werden.)

4. Nachdem Sie das Abonnement ausgewählt haben, das Sie anzeigen oder bearbeiten möchten, können Sie auf der Seite mit den Abonnement Details das Abonnement bearbeiten und folgende Aktionen ausführen:

    - Ändern des Abonnement namens

    - Hinzufügen/verringern der Anzahl von Arbeitsplätzen (Lizenzen) im Abonnement

    - Kündigen des Abonnements

    - Automatische Verlängerung deaktivieren

    - Fügen Sie ggf. eine indirekte Reseller-MPN-ID hinzu.

> [!NOTE]
> Möglicherweise müssen Sie bestimmte Schritte durchführen, die vom ISV-Verleger definiert werden, bevor Sie einige Änderungen an einem Abonnement ausführen können, z. b. das Abbrechen eines Abonnements.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Zuweisen von Lizenzen und Aktivieren eines Abonnements im Auftrag eines Kunden

Wenn Sie ein SaaS-Angebot (Software-as-a-Service) erwerben, das von einem ISV-Herausgeber (Independent Software Vendor) im kommerziellen Marketplace bereitgestellt wird, hilft der ISV-Verleger dabei, das Zuweisen von Lizenzen und das Aktivieren des Abonnements im Auftrag Ihres Kunden zu verwalten.

Der Herausgeber sollte Ihnen einen personalisierten Link und einen Autorisierungs Code bereitstellen, der ihren jeweiligen Erwerb identifiziert.

1. Sie finden diesen personalisierten Link auf dem ISV-Verleger auf verschiedene Arten:

   - Sie können den Link auf der Bestätigungsseite sehen, der angezeigt wird, nachdem Sie ein ISV SaaS-Angebot erworben haben. Um diesen Link auf der Seite zu finden, suchen Sie nach, und wählen Sie **dann zu Verleger Website**wechseln aus.

   - Sie können den Link auf der Seite Abonnements eines bestimmten Kunden anzeigen. Dieser Verleger Link wird in der Zeile angezeigt, die dem für den Kunden erworbenen ISV-Angebot oder-Abonnement zugeordnet ist.

   - Sie können [den Link mithilfe der Partner Center-APIs abrufen](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Um dies im Auftrag Ihres Kunden zu tun, müssen Sie möglicherweise den personalisierten Link kopieren, ihn in einen privaten Browser einfügen und die Anmelde Informationen des Kunden eingeben.

2. Wenn Sie sich auf der Website oder dem System des ISV-Verlegers befinden, werden Sie vom Herausgeber über alle zusätzlichen Schritte informiert, die Sie durchführen müssen, um den Kunden Setup Vorgang abzuschließen und Lizenzen bereitzustellen oder zuzuweisen.

3. Als Partner im CSP-Programm, das im Auftrag Ihres Kunden arbeitet, sind Sie dafür verantwortlich, die folgenden Aufgaben auszuführen:

    - Übermitteln Sie alle erforderlichen Informationen an den Verleger.

    - Senden Sie jede erforderliche URL direkt an Ihren Kunden (oder übermitteln Sie Details zu diesem Abonnement direkt an Ihren Kunden).

4. Nachdem Sie die erforderlichen Informationen für den Verleger bereitgestellt haben, werden die entsprechenden Lizenzen vom Verleger bereitgestellt und zugewiesen. Die Abonnement Abrechnung wird erst gestartet, nachdem die folgenden Ereignisse eintreten:

    - Der ISV-Verleger hat erfolgreich geeignete Lizenzen zugewiesen.

    - Der ISV-Verleger hat Microsoft (über eine separate Saas-Erfüllungs-API) bestätigt, dass das Konto Setup erfolgreich abgeschlossen wurde.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Abbrechen eines lizenzbasierten Saas-Abonnements von einem ISV-Verleger

Wenn Sie ein Lizenz basiertes Saas-Produkt abonnieren, das von einem ISV-Verleger innerhalb des kommerziellen Marketplace angeboten wird, haben Sie die Möglichkeit, das Abonnement innerhalb des festgelegten Abbruch Zeitraums abzubrechen. Dieser Abbruch Zeitraum ändert sich abhängig davon, ob Sie über ein monatliches oder ein Jahresabonnement verfügen. Sie können auch auswählen, ob Sie das Abonnement automatisch verlängern möchten.

Weitere Informationen zu abbruchzeiten, die angewendet werden, zum Abbrechen oder zum automatischen erneuern eines Abonnements finden Sie unter:

- [Kündigen eines Abonnements](create-a-new-subscription.md#cancel-a-subscription)

- [Automatisches erneuern eines kommerziellen Marketplace-Abonnements](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Hinzufügen oder Entfernen von Lizenzen für ein SaaS-Abonnement

Für Angebote des kommerziellen Marketplace in Saas können Sie Benutzerlizenzen für ein Kunden Abonnement hinzufügen oder entfernen.

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü die Option **Kunden** aus.

2. Wählen Sie einen geeigneten Kunden aus, und klicken Sie dann auf **Abonnements**. Dadurch werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.

3. Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.

4. Suchen Sie auf der Seite Abonnement Details das Feld **Menge** . An dieser Stelle können Sie die Anzahl der Lizenzen erhöhen oder verringern.

5. Ändern Sie die Menge, und wählen Sie dann **senden**aus.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Verwalten von Abonnements mithilfe von Partner Center-APIs

Sie können auch Partner Center-APIs verwenden, um die Lebenszyklus Verwaltung durchzuführen und Rechnungen für Ihre Abonnements zu verwalten. Weitere Informationen finden Sie unter [Erstellen eines Abonnements für kommerzielle Marketplace-Produkte](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Nächste Schritte

- [Erwerben kommerzieller Marketplace-Angebote](csp-commercial-marketplace-purchase.md)
- [Weitere Informationen zur Abrechnung im kommerziellen Marketplace](csp-commercial-marketplace-billing.md)