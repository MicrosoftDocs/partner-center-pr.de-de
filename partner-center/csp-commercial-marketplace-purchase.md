---
title: Erwerben Sie kommerzielle Marketplace-Produkte oder-Angebote für Ihre Kunden | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie CSP-Programmpartner den Partner Center Marketplace nutzen können, um Kunden Käufe von SaaS-Angeboten von unabhängigen Software Anbietern (ISVs) zu tätigen.
author: MicheleHope
ms.author: v-mihope
keywords: Abonnements, Marketplace, kommerzieller Marketplace, Drittanbieter, ISV, SaaS-Angebote, Cloud Solution Provider-Programm, erwerben eines Angebots, erwerben eines Abonnements
ms.localizationpriority: medium
ms.openlocfilehash: 3dd3facf79e0e33a6dfc35a162c444a13a19b256
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253798"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Erwerben Sie kommerzielle Marketplace-Produkte für Ihre Kunden im Partner Center

**Gilt für**

- Partner Center
- Partner im CSP-Programm

**Geeignete Rollen**

- Globaler Administrator
- Administratoragent

Als Partner im CSP-Programm (Cloud Solution Provider) können Sie den kommerziellen Marketplace verwenden, um Abonnements für Ihre Kunden an bestimmte SaaS-Produkte (Software-as-a-Service) zu erwerben, die von unabhängigen Softwareanbietern (ISVs) angeboten werden. 

Wenn Sie Ihren Kunden ISV-Saas-Abonnements anbieten, können Sie Ihr Unternehmen unterscheiden. Sie können auch Ihren Kunden Zugriff auf Softwarepakete bieten, die Ihren speziellen Geschäftsanforderungen gerecht werden. Sie verwalten Lizenzen und Abonnements für diese Marketplace-SaaS-Produkte von ISV-Verlegern, genauso wie Sie Lizenzen und Abonnements für Microsoft-Produkte verwalten.

Sie können entweder **Lizenz basierte Saas-** Abonnements oder **nutzungsbasierte** Abonnements erwerben. Weitere Informationen zum Unterschied zwischen der lizenzbasierten und der nutzungsbasierten Abrechnung finden Sie unter [Grundlagen der Abrechnung](billing-basics.md).

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>Erwerben Sie Lizenz basierte Saas-Abonnements im Partner Center

Abonnements für Lizenz basierte SaaS-Produkte, die von ISV-Verlegern angeboten werden, werden mit demselben Prozess erworben, den Sie auch zum Erwerb von Abonnements für Microsoft-Produkte verwenden

Informationen zum Erwerb eines lizenzbasierten Saas-Abonnements im Partner Center finden Sie unter [erstellen, aussetzen oder Abbrechen von Kunden Abonnements](create-a-new-subscription.md#create-a-new-subscription).

Sie können auch [Partner Center-APIs](https://docs.microsoft.com/partner-center/develop/) verwenden, um Abonnements für Ihre Kunden im kommerziellen Marketplace zu erstellen. (Weitere Informationen zur Verwendung von Partner Center-APIs finden Sie unter [Erstellen eines Abonnements für kommerzielle Marketplace-Produkte](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Als Partner im CSP-Programm können Sie nur **Lizenz basierte Saas-** Abonnements von ISV-Verlegern innerhalb von Partner Center erwerben. Dies bedeutet, dass Sie alle **lizenzbasierten Saas-** Angebote erwerben können, die der ISV-Verleger Ihnen zur Verfügung gestellt hat, einschließlich [exklusiver Angebote](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , auf die Sie Zugriff haben. Zum Erwerb oder zur Verwaltung anderer kommerzieller Marketplace-Angebote von ISVs (z. b. **nutzungsbasierte**, gemessene oder Verbrauchs basierte Angebote mit Azure-Anwendungen, Containern oder VMS) müssen Sie das [Azure-Verwaltungs Portal](https://portal.azure.com/)aufrufen. Weitere Informationen finden Sie im folgenden Thema.

## <a name="purchase-usage-based-subscriptions-in-the-azure-management-portal"></a>Erwerben von nutzungsbasierten Abonnements im Azure-Verwaltungs Portal

Im Gegensatz zu lizenzbasierten Saas-Abonnements von Drittanbieter-ISV-Verlegern erfordern nutzungsbasierte Abonnements zunächst, dass ein Kunde über ein Azure-Abonnement verfügt. Abrechnung für kommerziellen Marketplace, nutzungsbasierte Ressourcen fallen unter das Azure-Abonnement des Kunden. Sobald Ihr Kunde über ein Azure-Abonnement verfügt, kann ein Partner im CSP-Programm die folgenden Schritte ausführen, um ein kommerzielles Marketplace-Abonnement für Sie zu erwerben:

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie im Menü auf der linken Seite die Option **Kunden** aus.

2. Wählen Sie den jeweiligen Kunden aus, und wählen Sie dann **Abonnements**aus.  

3. Wählen Sie unter **nutzungsbasierte Abonnements**die Option **alle Ressourcen**aus. Dadurch gelangen Sie zum Azure-Verwaltungs Portal.

4. Wählen Sie im Azure-Verwaltungs Portal im Menü auf der linken Seite **Ressource erstellen** aus.

5. Wählen Sie oben in der Liste Azure Marketplace die Option **alle** anzeigen aus.

6. Um die Liste einzugrenzen, verwenden Sie oben in der Marketplace-Liste Filter. Sie können z. b. **Microsoft** oder **Partner** in der Dropdown Liste **Herausgeber** auswählen, um nur Angebote von Microsoft oder von einem ISV-Verleger anzuzeigen.

7. Wählen Sie ein bestimmtes Angebot aus, und wählen Sie dann **Erstellen**aus.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten kommerzieller Marketplace-Angebote](csp-commercial-marketplace-purchase.md)