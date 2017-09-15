---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. Im Rahmen des neuen Produkts führt Microsoft am 1.November2016 neue Microsoft Dynamics-Abonnementpläne für Kunden ein, die den aktuellen Plänen zwar ähnlich, jedoch nicht mit diesen identisch sind.

Die Anweisungen in diesem Dokument beschrieben, wie indirekte Anbieter vorhandene Microsoft Dynamics AX- und Microsoft Dymanics CRM Online-Abonnements von Kunden zum neuen Microsoft Dynamics365 migrieren können. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

Die Microsoft Dynamics CRM Online und AX-Pläne werden deaktiviert.  Ab dem 1.Juli2017 können die älteren Pläne nicht mehr verlängert werden. Auch bestehende E4-Abonnements werden nicht automatisch verlängert.

Wenn CRM Online und AX-Abonnements enden, werden sie storniert. Um Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements auf eine unterstützte SKU-Option (nachfolgend aufgeführt) übertragen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen. 

Auf der Detailseite des Abonnements wurde der Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert. 

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung ermitteln. Die Abonnements wurden für den 1. Juli 2017 auf „renew=False“ gesetzt. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

**Änderungen für die Microsoft Dynamics AX-Lizenzierung**

Die Microsoft Dynamics AX-Produktlinie wird mit Wirkung vom 1.November2016 eingestellt. Weitere Informationen zu den neuen Lizenzierungsoptionen für Dynamics365 finden Sie im [Lizenzierungshandbuch](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf), das in Kürze veröffentlicht wird.

 Die folgende Tabelle enthält Details zur Lizenzzuordnung:

|**Veraltete SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Microsoft Dynamics 365 for Unified Operations oder Microsoft Dynamics 365 Plan |
|Aufgabe|Microsoft Dynamics 365 for Sales
|Aufgabe/Self-Service|Microsoft Dynamics 365 for Team Members|
|Gerät|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Microsoft Dynamics CRM Online-Lizenzierungsänderungen 

**Microsoft Dynamics CRM Online**

Der aktuelle Microsoft Dynamics CRM Online-Plan wird mit Wirkung vom 1.November2016 eingestellt. Weitere Informationen zu den neuen Lizenzierungsoptionen für Microsoft Dynamics365 finden Sie im [Lizenzierungshandbuch](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Weitere Informationen zu neuen Lizenzierungsoptionen finden Sie unter [Wichtige Informationen für CRM Online-Kunden](https://go.microsoft.com/fwlink/?linkid=831667).

Die folgende Tabelle enthält Details zur Lizenzzuordnung:

|**Veraltete SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Dynamics 365 Enterprise Customer Engagement Plan |
|Professional|Dynamics 365 Enterprise Customer Engagement Plan, Dynamics 365 for Sales oder Dynamics 365 for Customer Service|
|Basic|Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service oder Dynamics 365 Enterprise Customer Engagement Plan|
|Unentbehrlich|Dynamics 365 for Team Member|
|Field Service-Add-On|Dynamics 365 Enterprise Customer Engagement Plan oder Dynamics 365 for Field Service|
|Projekt Service Authomation-Add-On|Dynamics 365 Customer Engagement Plan oder Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [Stornieren des alten Abonnements](#manual-subscription-migration-cancelsubscriptions).

Mit den folgenden Verfahren migrieren Sie einen Kunden von Microsoft Dynamics AX oder CRM Online zu Dynamics365.

Der Wiederverkäufer muss einen Kunden mit einem vorhandenen Dynamics AX Enterprise-Abonnement zu Dynamics365 for Operations migrieren. Der erste Schritt besteht im Kauf von Dynamics365 for Operations.  Wiederholen Sie diese Schrittefür einen CRM Online-Kunden zum Wechsel zu Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Kauf des neuen Abonnements**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



