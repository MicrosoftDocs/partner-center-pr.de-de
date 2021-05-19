---
title: Verwalten von Marketplace-Produkten & Angeboten
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: In Partner Center erfahren Sie, wie Cloudlösungsanbieter ISV-Angebote von Drittanbietern verwalten können, die für Kunden über den kommerziellen Marketplace erworben wurden.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147903"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Verwalten von Produkten und Angeboten im kommerziellen Marketplace für Ihre Kunden


**Geeignete Rollen:** globale | Administrator-Agent

Partner im CSP-Programm (Cloud Solution Provider) können das Partner Center-Portal verwenden, um viele ISV-SaaS-Angebote oder -Abonnements für ihre Kunden über den kommerziellen Marketplace zu erwerben. Nachdem Sie ein Angebot erworben haben, haben Sie verschiedene Möglichkeiten, es zu verwalten.

## <a name="view-or-edit-a-subscription"></a>Anzeigen oder Bearbeiten eines Abonnements

Nachdem Sie ein Abonnement von einem ISV-Herausgeber eines Drittanbieters erworben haben, können Sie es wie folgt überprüfen oder bearbeiten:

1. Melden Sie sich beim Partner Center [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü **Kunden** aus.

2. Wählen Sie einen geeigneten Kunden und dann **Abonnements** aus. Hier werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.

3. Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie anzeigen oder bearbeiten möchten. Dadurch erhalten Sie weitere Informationen zum Einrichten oder Bereitstellen des Angebots. (Wenn weitere Aktionen für das Angebot erforderlich sind, wird möglicherweise auch der Status "Aktion erforderlich" in der Spalte Status angezeigt. Dies kann auch durch einen Link zur Website des ISV-Herausgebers begleitet werden.)

4. Nachdem Sie das Abonnement ausgewählt haben, das Sie anzeigen oder bearbeiten möchten, können Sie auf der Seite mit den Abonnementdetails das Abonnement bearbeiten und beispielsweise Folgendes tun:

    - Ändern des Abonnementspitznamens

    - Hinzufügen/Verringern der Anzahl von Lizenzen im Abonnement

    - Kündigen des Abonnements

    - Automatische Verlängerung deaktivieren

    - Fügen Sie ggf. eine MPN-ID für indirekte Vertriebspartner hinzu.

> [!NOTE]
> Möglicherweise müssen Sie bestimmte Vom ISV-Herausgeber definierte Schritte ausführen, bevor Sie einige Änderungen an einem Abonnement vornehmen können, z. B. das Kündigen eines Abonnements.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Zuweisen von Lizenzen und Aktivieren eines Abonnements im Auftrag eines Kunden

Wenn Sie ein SaaS-Angebot (Software-as-a-Service) erwerben, das von einem Herausgeber eines unabhängigen Softwareanbieters (Independent Software Vendor, ISV) im kommerziellen Marketplace bereitgestellt wird, hilft der ISV-Herausgeber dabei, den Prozess der Zuweisung von Lizenzen und die Aktivierung des Abonnements im Auftrag Ihres Kunden zu verwalten.

Der Herausgeber sollte Ihnen einen personalisierten Link und einen Autorisierungscode zur Verfügung stellen, der Ihren spezifischen Kauf identifiziert.

1. Sie finden diesen personalisierten Link vom ISV-Herausgeber auf verschiedene Arten:

   - Sie sehen den Link auf der Bestätigungsseite, der nach dem Kauf eines ISV-SaaS-Angebots angezeigt wird. Um diesen Link auf der Seite zu finden, suchen Sie nach , und wählen Sie **Go to publisher es site (Zur Website des Herausgebers wechseln) aus.**

   - Sie können den Link auf der Seite Abonnements eines bestimmten Kunden anzeigen. Dieser Herausgeberlink wird in der Zeile angezeigt, die dem ISV-Angebot oder -Abonnement zugeordnet ist, das bzw. das für den Kunden erworben wurde.

   - Sie können [den Link mithilfe Partner Center APIs abrufen.](/partner-center/develop/get-activation-link-by-order-line-item)

   > [!NOTE]
   > Um dies im Namen Ihres Kunden zu tun, müssen Sie möglicherweise den personalisierten Link kopieren, ihn in einen privaten Browser einfügen und die Anmeldeinformationen des Kunden eingeben.

2. Sobald Sie sich auf der Website oder im System des ISV-Herausgebers befinden, werden Sie vom Herausgeber über alle zusätzlichen Schritte informieren, die Sie zum Abschließen des Kundeneinrichtungsprozesses und zum Bereitstellen oder Zuweisen von Lizenzen ausführen müssen.

3. Als Partner im CSP-Programm, der im Auftrag Ihres Kunden arbeitet, sind Sie für die Folgenden verantwortlich:

    - Übermitteln Sie alle erforderlichen Informationen an den Herausgeber.

    - Senden Sie alle erforderlichen URLs direkt an Ihren Kunden (oder teilen Sie Ihrem Kunden auf andere Weise Details zu diesem Abonnement direkt mit).

4. Nachdem Sie dem Herausgeber die erforderlichen Informationen bereitgestellt haben, stellt der Herausgeber die entsprechenden Lizenzen zur Verfügung und weist sie zu. Die Abonnementabrechnung beginnt erst, wenn die folgenden Ereignisse auftreten:

    - Der ISV-Herausgeber hat erfolgreich entsprechende Lizenzen zugewiesen.

    - Der ISV-Herausgeber hat Microsoft (über eine separate SaaS-Fulfillment-API) bestätigt, dass die Kontoeinrichtung erfolgreich abgeschlossen wurde.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Kündigen eines lizenzbasierten SaaS-Abonnements von einem ISV-Herausgeber

Wenn Sie ein lizenzbasiertes SaaS-Produkt abonnieren, das von einem ISV-Herausgeber im kommerziellen Marketplace angeboten wird, haben Sie die Möglichkeit, das Abonnement innerhalb des festgelegten Kündigungszeitraums zu kündigen. Dieser Kündigungszeitraum ändert sich abhängig davon, ob Sie über ein monatliches oder jährliches Abonnement verfügen. Sie können auch auswählen, ob Sie das Abonnement automatisch verlängern möchten.

Weitere Informationen zu geltenden Kündigungszeiträumen, zum Kündigen oder zum automatischen Verlängern eines Abonnements finden Sie unter:

- [Kündigen eines Abonnements](create-a-new-subscription.md#cancel-a-subscription)

- [Automatische Verlängerung eines Abonnements für den kommerziellen Marketplace](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Hinzufügen oder Entfernen von Lizenzen für ein SaaS-Abonnement

Für Angebote im kommerziellen SaaS-Marketplace können Sie Benutzerlizenzen für ein Kundenabonnement hinzufügen oder entfernen.

1. Melden Sie sich beim Partner Center [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Navigationsmenü **Kunden** aus.

2. Wählen Sie einen geeigneten Kunden und dann **Abonnements** aus. Hier werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.

3. Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.

4. Suchen Sie auf der Seite mit den Abonnementdetails nach dem Feld **Menge.** Hier können Sie die Anzahl der Lizenzen erhöhen oder verringern.

5. Ändern Sie die Menge, und wählen Sie dann **Übermitteln** aus.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Verwalten von Abonnements mithilfe von Partner Center-APIs

Sie können auch Partner Center-APIs verwenden, um die Lebenszyklusverwaltung durchzuführen und Rechnungen für Ihre Abonnements zu verwalten. Weitere Informationen finden Sie unter [Erstellen eines Abonnements für kommerzielle Marketplace-Produkte.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Nächste Schritte

- [Erwerben von Angeboten im kommerziellen Marketplace](csp-commercial-marketplace-purchase.md)
- [Erfahren Sie mehr über die Abrechnung im kommerziellen Marketplace.](csp-commercial-marketplace-billing.md)