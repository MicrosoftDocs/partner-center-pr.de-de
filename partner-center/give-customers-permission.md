---
title: Kunden den Kauf eigener Dienste in CSP erlauben
description: Erfahren Sie, wie CSP-Programmpartner Es Kunden erlauben können, ihre eigenen Dienste wie Azure-Reservierungen für ein Abonnement zu erwerben, das sie in Partner Center erworben haben.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150759"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Erteilen sie Kunden die Berechtigung in Partner Center, ihre eigenen Produkte oder Dienste zu erwerben.

**Geeignete Rollen:** Administrator-Agent-| Vertriebsmitarbeiter

In diesem Artikel wird gezeigt, wie ein Partner im CSP-Programm (Cloud Solution Provider) einem Kunden die Berechtigung erteilen kann, einige seiner eigenen Dienste oder Ressourcen zu erwerben.

Partner im CSP-Programm verwenden häufig Partner Center und den kommerziellen Marketplace, um Lösungen und Dienste für ihre Kunden zu erwerben. Partner lassen dann zu, dass einige Kunden diese Dienste selbst direkt über die Azure-Portal bereitstellen.

Hier sehen Sie ein Beispiel. Angenommen, Sie erwerben ein Azure-Planabonnement für einen Kunden in Partner Center. Anschließend entscheiden Sie sich, diesem Abonnement im Namen des Kunden weitere Ressourcen oder Dienste hinzuzufügen. In diesem Fall können Sie dem Abonnement des Kunden Azure-Reservierungen hinzufügen (z. B. das Hinzufügen reservierter VM-Instanzen). Sie können dem Kunden dann erlauben, die Azure-Reservierungsressourcen selbst im Azure-Portal weiter zu bereitstellen.

Mit dem Feature **"Kundenberechtigungen"** erhalten Kunden jetzt mehr Self-Service-Optionen mit Azure-Ressourcen. Indem Sie Berechtigungen für den Kunden aktivieren, ermöglichen Sie Kunden den Erwerb eigener Ressourcen (z. B. den Erwerb eigener Azure-Reservierungen).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Übersicht über Kundenberechtigungen in Partner Center

Verwenden Sie die Seite **Kundenkonto,** um Kundenberechtigungen zu aktivieren (oder zu deaktivieren). Derzeit unterstützt dieses Feature:

- **Azure-Reservierungen:** Durch Aktivieren dieser Berechtigung kann der Kunde seine eigenen Azure-Reservierungen für ein bestimmtes Azure-Abonnement erwerben, das Sie für sie erworben haben.

Beachten Sie vor dem Aktivieren von Kundenberechtigungen die folgenden wichtigen Punkte:

- Standardmäßig werden Kundenberechtigungen in Partner Center automatisch deaktiviert (deaktiviert).

- Bevor Sie Berechtigungen für einen Kunden aktivieren (oder deaktivieren) können, muss Ihnen die Rolle Administrator-Agent in der Partner Center.

  Partner, die die Rolle "Vertriebs-Agent" oder "Helpdesk-Agent" zugewiesen haben, verfügen über schreibgeschützten Zugriff und können kundenspezifische Berechtigungen nicht aktivieren oder deaktivieren.

- Sie können Berechtigungen für jeden kundenspezifischen Kunden aktivieren (aktivieren).

- Sie können Kundenberechtigungen entweder mithilfe des Dashboards Partner Center oder mithilfe der Partner Center [deaktivieren.](/partner-center/develop/manage-customers)

- Nachdem Sie Berechtigungen für einen bestimmten Kunden aktiviert (aktivieren) haben, sind Sie für alle nachfolgenden Käufe dieses Kunden verantwortlich. Wenn Kunden einen von ihnen vorgenommenen Kauf umtauschen, stornieren oder verlängern möchten (oder den anfänglichen Bereich einer Reservierung ändern möchten), können sie dies nicht selbst tun. Sie müssen Sie als Partner bitten, Käufe umtauschen, stornieren und verlängern oder spätere Änderungen am Reservierungsbereich vornehmen zu können.  

- Nachdem Sie Die Berechtigungen für einen  bestimmten Kunden aktivieren, werden Sie nicht über spätere Käufe des Kunden benachrichtigt.

- Spätere vom Kunden getätigte Käufe werden in Partner Center von Ihnen getätigten Käufen angezeigt. Sie finden diese Käufe auf  der Seite  Bestellverlauf des Kunden, auf der Seite Reservierungen oder im [**Aktivitätsprotokoll.**](activity-logs.md)

>[!NOTE]
> Informationen zu den Preisen, die der Kunde bezahlen wird, und zur Unterstützung von Kunden bei der Verwaltung ihrer Käufe finden Sie unter Hilfe für Kunden beim Verwalten [von Reservierungen, die sie erwerben.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben

Azure-Reservierungen sind eine gute Möglichkeit, um Azure-Dienste zu einem reduzierten Preis zu erwerben. Weitere Informationen zu den Vorteilen von Azure-Reservierungen finden Sie unter [Was sind Azure-Reservierungen?.](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Jetzt haben Sie die Möglichkeit, Azure-Reservierungen im Auftrag Ihrer Kunden zu erwerben, wie sie es möglicherweise bereits tun. Oder Sie können Kunden die Berechtigung erteilen, ihre eigenen Azure-Reservierungen zu erwerben.

>[!NOTE]
> Nachdem Sie Kunden die Berechtigung erteilt haben, ihre eigenen Azure-Reservierungen zu erwerben, helfen Sie ihnen bei der Verwaltung von Reservierungen, die sie erwerben. Weitere Informationen finden Sie unter Unterstützen [von Kunden beim Verwalten von Reservierungen, die sie erwerben.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>So ermöglichen Sie Es Kunden, ihre eigenen Azure-Reservierungen zu erwerben

1. Vergewissern Sie sich, dass der Kunde über einen Azure-Plan oder ein globales Azure-Abonnement verfügt, das Sie in ihrem Namen erworben haben.

2. Vergewissern Sie sich, dass dem Kunden die Rolle **Besitzer** für dieses Abonnement zugewiesen wurde.

3. Aktivieren Sie Kundenberechtigungen (aktivieren Sie dieses **Feature),** um ihre eigenen Azure-Reservierungen zu erwerben.

Jeder Schritt wird unten angezeigt.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Überprüfen, ob der Kunde über ein vorhandenes Azure-Abonnement verfügt

Bevor Sie Kunden die Berechtigung zum Kauf ihrer eigenen Azure-Reservierungen erteilen, müssen Sie überprüfen, ob der Kunde über einen vorhandenen Azure-Plan oder ein globales Azure-Abonnement verfügt. Wenn der Kunde kein aktuelles Azure-Abonnement in Partner Center, müssen Sie ein Abonnement für den Kunden erwerben, bevor Sie seine Kundenberechtigungen aktivieren.

- Um zu sehen, ob ein Kunde bereits über ein Azure-Abonnement verfügt, melden Sie sich beim dashboard Partner Center an, und wählen Sie **dann CSP** gefolgt von **Customers aus.** Wählen Sie den jeweiligen Kunden aus der Liste aus. Wählen Sie dann **Abonnements aus,** und suchen Sie nach nutzungsbasierten Abonnements für Azure Plan oder Azure Global.

- Wenn ein Kunde noch kein Azure-Abonnement hat, können Sie ein Abonnement für ihn erwerben. Weitere Informationen [finden Sie unter Erwerben des Azure-Plans.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Vergewissern Sie sich, dass dem Kunden die richtige Rolle in Azure zugewiesen wurde.

Nachdem Sie überprüft haben, ob der Kunde über ein vorhandenes Azure-Abonnement verfügt,  müssen Sie auch überprüfen, ob den Schlüsselbenutzern, die Ihrem Kunden zugeordnet sind, die richtige Rolle Besitzer für dieses Azure-Abonnement zugewiesen wurde. Dies ist der rollenbasierte Zugriff (Role-Based Access, RBAC), den der Kunde benötigt, um Azure-Reservierungen für ein von Ihnen erworbenes Azure-Abonnement zu erwerben.

Einige Partner haben kunden,  die ihre eigenen Azure-Ressourcen aktiv verwalten und bereitstellen möchten, möglicherweise bereits die Rolle Besitzer zugewiesen. Wenn Sie einem Kunden bereits den **Besitzerstatus** zugewiesen haben, um vorherige Abonnements zu verwalten, die Sie für diesen erworben haben, können Sie diesen Schritt überspringen.  

> [!IMPORTANT]
> Wenn einem Kunden nicht die Rolle **Besitzer** zugewiesen wurde, wird ein Fehler in der Azure-Portal verhindert, dass er Azure-Reservierungen kaufen kann.

So überprüfen Sie, ob dem Kunden die Rolle **Besitzer** für ein Azure-Abonnement zugewiesen wurde:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie **CSP** und dann **Kunden** und dann den jeweiligen Kunden aus.

3. Wählen Sie **Abonnements** für diesen Kunden aus, und suchen Sie das jeweilige Azure-Abonnement.

4. Wählen Sie neben dem Abonnement des Kunden die Schaltfläche **Verwalten** aus. Dadurch wird die [Azure-Portal](https://portal.azure.com/)geöffnet.

5. Um einem bestimmten Benutzer die Rolle **Besitzer** zuzuweisen, führen Sie die folgenden Schritte [aus, um einen Benutzer als Administrator zuzuweisen.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Aktivieren oder Deaktivieren von Kundenberechtigungen zum Erwerb eigener Azure-Reservierungen

Nachdem Sie sich vergewissert haben, dass der Kunde über ein vorhandenes Azure-Abonnement verfügt und Benutzern die Rolle **Besitzer** für dieses Abonnement zugewiesen ist, können Sie Kundenberechtigungen aktivieren (aktivieren). Sie können diese Schritte auch zum Deaktivieren (Deaktivieren) von Kundenberechtigungen verwenden. Sie können Kundenberechtigungen entweder über das Partner Center-Dashboard oder [Partner Center-APIs](/partner-center/develop/manage-customers)aktivieren oder deaktivieren.

So aktivieren (oder deaktivieren Sie) Sie Kundenberechtigungen in Partner Center:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im linken Navigationsmenü **CSP** und dann **Kunden** aus. Eine Kundenliste wird angezeigt.

3. Wählen Sie einen bestimmten Kundennamen aus.

4. Wählen Sie im Menü **"Kunde"** die Option Konto aus. Die Seite **Kundenkonto** wird angezeigt.

5. Suchen Sie unten auf der Seite nach dem Bereich **Kundenberechtigungen.**

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Kundenberechtigungen auf der Seite &quot;Konto&quot;." border="true":::

6. Suchen Sie unter **Azure-Reservierungen** nach der Option **Allow customer to purchase (Kunden den Kauf erlauben).**

7. Um Kundenberechtigungen zu aktivieren, verschieben Sie den Schalter neben dieser Option auf die **Position Ein.** Um Kundenberechtigungen zu deaktivieren, verschieben Sie den Schalter auf die **Position Aus.**

>[!NOTE]
> Informationen dazu, was sonst noch geschieht, wenn Sie die Berechtigungen eines Kunden zum Erwerb eigener Azure-Reservierungen aktivieren, finden Sie unter Übersicht über Kundenberechtigungen [in Partner Center.](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
>Wenn Sie Kundenberechtigungen aktivieren (oder deaktivieren), zeichnet das Aktivitätsprotokoll jede Aktion auf. (Auf dieses Protokoll kann zugegriffen werden, wenn Sie oben im Dashboard auf das Zahnradsymbol Partner Center klicken).) Wenn Sie Kundenberechtigungen aktivieren oder deaktivieren, wird die Aktion entweder als Create **Customer Purchase Permissions** oder Delete Customer Purchase **Permissions** im Aktivitätsprotokoll angezeigt.

## <a name="help-customers-manage-reservations-they-purchase"></a>Unterstützen von Kunden beim Verwalten von Reservierungen, die sie erwerben

Nachdem Sie Kunden die Berechtigung erteilt haben, ihre eigenen Azure-Reservierungen zu erwerben, können Sie ihnen helfen, alle ressourcen, die sie erwerben, besser zu verwalten. Kunden können viele Aspekte von Azure-Reservierungen selbst direkt über [die](https://portal.azure.com/)Azure-Portal. Sie benötigen Ihre Hilfe bei der Verwaltung von einigen anderen Aspekten von Azure-Reservierungen, die sie in Ihrem CSP-Abonnement erwerben.  

Helfen Sie Kunden, mehr über die Verwaltung dieser Aspekte von Azure-Reservierungen zu erfahren:

- Preise, die Kunden für Azure-Reservierungen bezahlen
- Optimieren der Nutzung von Azure-Reservierungen durch Kunden
- Was geschieht, wenn Kunden Reservierungen mit einem gemeinsam genutzten Bereich erwerben?
- Was geschieht, wenn Kunden eine Reservierung ändern, stornieren und verlängern oder ihren Bereich ändern möchten?

**Preise, die Kunden für ihre Reservierungen bezahlen.** Ihr Kunde kauft Azure-Reservierungen basierend auf einem Abonnement, das Sie zuvor für sie in Ihrem CSP-Partnerabrechnungskonto erworben haben. Der Preis des Kunden für alle Azure-Reservierungen, die er basierend auf diesem Abonnement erwerbt, wird ebenfalls von Ihnen festgelegt. Dieser Preis kann sich vom Web Direct-Preis unterscheiden, den der Kunde in der Azure-Portal.

**Wie Kunden ihre Nutzung einer Reservierung optimieren können.** Einige Kunden profitieren möglicherweise davon, mehr darüber zu erfahren, wie sie ihre Nutzung einer Reservierung optimieren oder den anfänglichen Umfang einer Reservierung während des Kaufs zuweisen können. Weitere Informationen finden Sie unter [Verwalten von Reservierungen für Azure-Ressourcen.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Was geschieht, wenn ein Kunde eine Reservierung mit einem gemeinsam genutzten Bereich erwirbt?** Wenn Kunden eine Reservierung basierend auf einem früheren CSP-Abonnement erwerben und dieser Reservierung einen freigegebenen Bereich zuweisen, gelten alle Rabatte, die der Kunde vom CSP erhalten hat, für die übereinstimmende Nutzung für alle Abonnements, die der CSP-Partner für diesen Kunden erworben hat.

**Was sollten Kunden tun, wenn sie einen erworbenen Kauf umtauschen, stornieren oder verlängern oder den ursprünglichen Umfang einer Reservierung ändern möchten?** Kunden müssen ihren Partner bitten, den anfänglichen Umfang einer Reservierung zu ändern. Außerdem benötigen sie Hilfe eines Partners, um eine Reservierung umtauschen, stornieren oder verlängern zu können. Sie können diese Aufgaben nicht selbst mit Reservierungen ausführen, die auf Abonnements basieren, die von einem CSP-Partner für sie erworben wurden.

## <a name="next-steps"></a>Nächste Schritte

- [Erwerben von Azure-Reservierungen im Namen Ihrer Kunden](azure-reservations-buying.md)

- [Partner Center: Verkaufen von Microsoft-Reservierungen](azure-reservations.md)

- [Azure Reservations im Auftrag Ihrer Kunden verwalten](azure-reservations-manage.md)