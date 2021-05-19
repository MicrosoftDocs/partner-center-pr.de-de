---
title: Erwerben von Angeboten für den kommerziellen Marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie CSP-Programmpartner den Partner Center Marketplace verwenden können, um Kunden Käufe von SaaS-Angeboten von unabhängigen Softwareherstellern (INDEPENDENT Software Vendors, ISVs) zu tätigen.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147852"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Erwerben Sie Produkte im kommerziellen Marketplace für Ihre Partner Center


**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent

Als Partner im Cloud Solution Provider-Programm (CSP) können Sie den kommerziellen Marketplace verwenden, um Abonnements für Ihre Kunden für bestimmte SaaS-Produkte (Software-as-a-Service) zu erwerben, die von unabhängigen Softwareherstellern (Independent Software Vendors, ISVs) angeboten werden.

Indem Sie IHREN Kunden ISV-SaaS-Abonnements anbieten, können Sie Ihr Unternehmen unterscheiden. Sie können Kunden auch Zugriff auf Softwarepakete geben, die ihre spezifischen Geschäftsanforderungen erfüllen. Sie verwalten Lizenzen und Abonnements für diese Marketplace-SaaS-Produkte von ISV-Herausgebern genauso wie Lizenzen und Abonnements für Microsoft-Produkte.

Sie können entweder **lizenzbasierte SaaS-Abonnements** oder **nutzungsbasierte Abonnements** erwerben. Weitere Informationen zum Unterschied zwischen lizenzbasierter und nutzungsbasierter Abrechnung finden Sie unter [Grundlagen der Abrechnung.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Erwerben lizenzbasierter und gemessener SaaS-Abonnements in Partner Center

Sie erwerben Abonnements für lizenzbasierte oder gemessene SaaS-Produkte, die von ISV-Herausgebern angeboten werden, mit demselben Prozess, den Sie zum Erwerben von Abonnements für Microsoft-Produkte verwenden.

Informationen zum Erwerb eines lizenzbasierten oder gemessenen SaaS-Abonnements in Partner Center Sie unter Erstellen, Aussetzen oder Kündigen [von Kundenabonnements.](create-a-new-subscription.md#create-a-new-subscription)

Sie können auch [Partner Center-APIs](/partner-center/develop/) verwenden, um Abonnements für Ihre Kunden im kommerziellen Marketplace zu erstellen. (Weitere Informationen zur Verwendung von Partner Center-APIs finden Sie unter Erstellen eines Abonnements für Produkte [im kommerziellen Marketplace.)](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> Als Partner im CSP-Programm können Sie lizenzbasierte oder gemessene  SaaS-Abonnements von ISV-Herausgebern innerhalb Partner Center.  Dies bedeutet, dass Sie alle lizenzbasierten oder gemessenen  SaaS-Angebote [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) erwerben können, die der **ISV-Herausgeber** Ihnen zur Verfügung gestellt hat, einschließlich exklusiver Angebote, auf die Sie Zugriff haben. Um andere Angebote des kommerziellen Marketplace von ISVs zu erwerben oder zu verwalten (z. B. nutzungsbasierte Angebote mit Azure-Anwendungen, Containern oder VMs), müssen Sie zum [Azure-Portal](https://portal.azure.com/)wechseln.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Erwerben nutzungsbasierter Abonnements im Azure-Portal

Im Gegensatz zu lizenzbasierten SaaS-Abonnements von ISV-Herausgebern von Drittanbietern erfordern nutzungsbasierte Abonnements zunächst, dass ein Kunde über ein Azure-Abonnement verfügt. Abrechnung für den kommerziellen Marketplace: Nutzungsbasierte Ressourcen fallen unter das Azure-Abonnement des Kunden. Sobald Ihr Kunde über ein Azure-Abonnement verfügt, kann ein Partner im CSP-Programm die folgenden Schritte ausführen, um ein Abonnement für den kommerziellen Marketplace zu erwerben:

1. Melden Sie sich beim Partner Center [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann im linken Menü **Kunden** aus.

2. Wählen Sie den spezifischen Kunden und dann **Abonnements** aus.  

3. Wählen Sie unter **Nutzungsbasierte Abonnements** die Option **Alle Ressourcen** aus. Dadurch gelangen Sie zum Azure-Verwaltungsportal.

4. Wählen Sie im Azure-Verwaltungsportal im linken Menü Ressource **erstellen** aus.

5. Wählen Sie oben in der Liste Azure Marketplace alle **anzeigen** aus.

6. Um Ihre Liste einzugrenzen, verwenden Sie Filter oben in der Marketplace-Liste. Sie können z. B. **Microsoft** oder **Partner** aus der **Dropdownliste Herausgeber** auswählen, um nur Angebote von Microsoft oder von einem ISV-Herausgeber anzuzeigen.

7. Wählen Sie ein bestimmtes Angebot und dann **Erstellen** aus.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Angeboten im kommerziellen Marketplace](csp-commercial-marketplace-purchase.md)