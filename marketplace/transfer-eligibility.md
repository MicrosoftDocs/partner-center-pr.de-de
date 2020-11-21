---
title: Übertragungs Berechtigung – Richtlinien für die Übertragung eines Abonnements zwischen Abrechnungskonten, Azure Marketplace
description: Richtlinien für kommerzielle Überprüfungen vor der Übertragung eines Abonnements zwischen Abrechnungskonten in der Azure-Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007222"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Übertragungs Berechtigung für ein Abonnement zwischen Abrechnungskonten

Sie können [ein Abonnement](/azure/cost-management-billing/understand/subscription-transfer) im Abrechnungs Abschnitt des Azure-Portal von einem Abrechnungskonto in ein anderes Konto übertragen. Vor der Übertragung wird das Abonnement auf Produkte von Drittanbietern überprüft. Die Übertragung ist nur zulässig, wenn *alle* Produkte für die Übertragung gelöscht werden (siehe nachfolgende [Kriterien](#criteria-for-transfer-approval-or-denial) ). Das System generiert relevante Fehlermeldungen für die apps, die nicht gelöscht werden konnten, um Sie bei der Ermittlung der nächsten Schritte zu unterstützen.

> [!NOTE]
> Dieser Artikel gilt nicht für SaaS-Angebote, da SaaS-Ressourcen an einen Mandanten, nicht an ein Abonnement angefügt sind. Saas-Ressourcen sind von einem Abrechnungskonto auf ein anderes übertragbar, dies erfolgt jedoch pro Ressource und Azure-Support als Supportanfrage.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kriterien für die Übertragung oder Ablehnung

Ein Abonnement kann nicht übertragen werden, wenn eine der Drittanbieter-apps eines der folgenden Kriterien erfüllt:

- Das Zielkonto ist kommerziell, und die APP ist für den Verkauf über Partner deaktiviert.
- Die APP ist für ausgewählte Partner aktiviert, und das Zielkonto ist nicht in der Zulassungsliste enthalten.
- Das Angebot war in der Vergangenheit ein Vorschau Angebot für ausgewählte Abonnements oder ein privates Angebot, und das Abonnement ist nicht mehr in der Zulassungsliste enthalten.
- Das neue Abrechnungskonto befindet sich in einer Region, von der das Angebot verkauft wird, und das Angebot wird nicht in dieser Region verkauft.

Eine blockierte Übertragung bleibt wirksam, bis Sie die Ressource aus dem Abonnement entfernen. Anschließend können Sie die Übertragung erneut versuchen.

## <a name="next-steps"></a>Nächste Schritte

[Unterstützung für Microsoft AppSource und Azure Marketplace](get-support.md)

