---
title: Kunden ermöglichen, eigene Dienste im CSP zu erwerben
description: Erfahren Sie, wie CSP-Programmpartner Kunden ihre eigenen Dienste (z. b. Azure-Reservierungen) für ein Abonnement erwerben können, das Sie im Partner Center erworben haben.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19f86ec5353abc21e14a3a8ac2ef17dd17924cfe
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000464"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Erteilen Sie Kunden eine Berechtigung im Partner Center, um Ihre eigenen Produkte oder Dienste zu erwerben.

**Zielgruppe**

- Partner Center
- Partner im CSP-Programm

**Geeignete Rollen**

- Administrator-Agent
- Vertriebsbeauftragter

In diesem Artikel wird gezeigt, wie ein Partner im Cloud Solution Provider-Programm (CSP) einem Kunden die Berechtigung zum Erwerb einiger eigener Dienste oder Ressourcen erteilen kann.

Partner im CSP-Programm nutzen häufig Partner Center und ihren kommerziellen Marketplace, um Lösungen und Dienste für Ihre Kunden zu erwerben. Partner ermöglichen es einigen Kunden dann, diese Dienste selbst direkt aus dem Azure-Portal bereitzustellen.

Hier sehen Sie ein Beispiel. Nehmen wir an, dass Sie ein Azure-Plan Abonnement für einen Kunden im Partner Center erwerben. Anschließend legen Sie im Auftrag des Kunden weitere Ressourcen oder Dienste zu diesem Abonnement hinzu. In diesem Fall können Sie Azure-Reservierungen dem Abonnement des Kunden hinzufügen (z. b. durch Hinzufügen reservierter Instanzen virtueller Computer). Sie können dem Kunden dann gestatten, die Azure-Reservierungs Ressourcen selbst in der Azure-Portal bereitzustellen.

Mit dem Feature " **Kunden Berechtigungen** " bieten Sie den Kunden nun mehr Self-Service-Optionen für Azure-Ressourcen. Durch Aktivieren der Berechtigungen für den Kunden gestatten Sie Kunden, ihre eigenen Ressourcen zu erwerben (z. b., um Ihre eigenen Azure-Reservierungen zu erwerben).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Übersicht über Kunden Berechtigungen in Partner Center

Verwenden Sie die Seite Kunden **Konto** , um die Kunden Berechtigungen zu aktivieren (oder zu deaktivieren). Diese Funktion unterstützt derzeit Folgendes:

- **Azure-Reservierungen:** Wenn Sie diese Berechtigung aktivieren, kann der Kunde seine eigenen Azure-Reservierungen für ein bestimmtes Azure-Abonnement erwerben, das Sie für Sie erworben haben.

Bevor Sie die Kunden Berechtigungen aktivieren, beachten Sie die folgenden wichtigen Punkte:

- Standardmäßig werden Kunden Berechtigungen im Partner Center automatisch deaktiviert (ausgeschaltet).

- Bevor Sie Berechtigungen für einen Kunden aktivieren (oder deaktivieren) können, muss Ihnen in Partner Center die Rolle admin Agent zugewiesen sein.

  Partner, denen die Rolle "Sales Agent" oder "Help Desk Agent" zugewiesen ist, haben schreibgeschützten Zugriff und können die Kunden Berechtigungen nicht aktivieren oder deaktivieren.

- Sie können Berechtigungen für jeden von Ihnen ausgewählten Kunden aktivieren (aktivieren).

- Sie können Kunden Berechtigungen mithilfe des Partner Center-Dashboards oder der [Partner Center-APIs](/partner-center/develop/manage-customers)aktivieren (oder deaktivieren).

- Nachdem Sie die Berechtigungen für einen bestimmten Kunden aktiviert haben, sind Sie dafür verantwortlich, alle nachfolgenden Einkäufe dieses Kunden zu bezahlen. Wenn Kunden einen Erwerb austauschen, Abbrechen oder erneuern möchten (oder den anfänglichen Bereich einer Reservierung ändern möchten), können Sie dies nicht selbst tun. Sie müssen Sie als Partner bitten, Sie beim austauschen, Abbrechen und erneuern von Käufen zu unterstützen oder spätere Änderungen am Bereich einer Reservierung vorzunehmen.  

- Nachdem Sie die Berechtigungen für einen bestimmten Kunden aktiviert haben, **werden Sie nicht** mehr über spätere Käufe des Kunden benachrichtigt.

- Spätere Käufe, die vom Kunden getätigt werden, werden zusammen mit den von Ihnen getätigten Käufen in Partner Center angezeigt. Diese Käufe finden Sie auf der Seite **Auftrags Verlauf** des Kunden, auf der Seite " **Reservierungen** " oder im [**Aktivitätsprotokoll**](activity-logs.md).

>[!NOTE]
> Informationen zu den Preisen, die der Kunde bezahlen wird, und zum unterstützen der Kunden bei der Verwaltung Ihrer Käufe finden Sie unter unter [stützen von Kunden bei der Verwaltung von Reservierungen](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.

Azure-Reservierungen sind eine gute Möglichkeit, um Azure-Dienste zu einem reduzierten Preis zu erwerben. Weitere Informationen zu den Vorteilen von Azure-Reservierungen finden Sie unter [Was ist Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Nun haben Sie die Wahl, Azure-Reservierungen im Auftrag ihrer Kunden zu erwerben, da Sie dies möglicherweise bereits getan haben. Oder Sie können Kunden die Berechtigung erteilen, ihre eigenen Azure-Reservierungen zu erwerben.

>[!NOTE]
> Nachdem Sie den Kunden die Berechtigung zum Erwerb ihrer eigenen Azure-Reservierungen erteilt haben, helfen Sie Ihnen, die von Ihnen erworbenen Reservierungen zu verwalten. Weitere Informationen finden Sie unter unter [stützen von Kunden beim Verwalten von Reservierungen, die Sie erwerben](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>So aktivieren Sie Kunden die Möglichkeit, ihre eigenen Azure-Reservierungen zu erwerben

1. Vergewissern Sie sich, dass der Kunde über einen vorhandenen Azure-Plan oder ein globales Azure-Abonnement verfügt, das Sie in seinem

2. Vergewissern Sie sich, dass dem Kunden die Rolle " **Besitzer** " für dieses Abonnement zugewiesen wurde.

3. Aktivieren Sie Kunden Berechtigungen (aktivieren Sie **Diese Funktion)**, um Ihre eigenen Azure-Reservierungen zu erwerben.

Jeder Schritt wird unten angezeigt.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Überprüfen, ob der Kunde über ein Azure-Abonnement verfügt

Bevor Sie Kunden die Berechtigung zum Erwerb ihrer eigenen Azure-Reservierungen erteilen, müssen Sie sicherstellen, dass der Kunde über einen Azure-Plan oder ein globales Azure-Abonnement verfügt. Wenn der Kunde kein Aktuelles Azure-Abonnement in Partner Center anzeigt, müssen Sie ein Abonnement für diese erwerben, bevor Sie seine Kunden Berechtigungen aktivieren.

- Um festzustellen, ob ein Kunde bereits ein Azure-Abonnement hat, melden Sie sich beim Partner Center-Dashboard an, und wählen Sie dann **CSP** , gefolgt von **Kunden**. Wählen Sie den jeweiligen Kunden aus der Liste aus. Wählen Sie dann **Abonnements** aus, und suchen Sie nach nutzungsbasierten Abonnements für Azure-Plan oder Azure Global.

- Wenn ein Kunde über kein vorhandenes Azure-Abonnement verfügt, können Sie ein Abonnement für diese erwerben. Weitere Informationen finden Sie [unter Azure-Plan erwerben](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Vergewissern Sie sich, dass dem Kunden in Azure die richtige Rolle zugewiesen wurde.

Nachdem Sie überprüft haben, ob der Kunde über ein vorhandenes Azure-Abonnement verfügt, müssen Sie auch überprüfen, ob die Schlüssel Benutzer, die Ihrem Kunden zugeordnet sind, der richtigen **Besitzer** Rolle für dieses Azure-Abonnement zugewiesen wurden. Dies ist der rollenbasierte Zugriff (RBAC), den der Kunde benötigt, um Azure-Reservierungen für ein Azure-Abonnement zu erwerben, das Sie erworben haben.

Einige Partner haben möglicherweise bereits der Rolle " **Besitzer** " für Kunden zugewiesen, die ihre eigenen Azure-Ressourcen aktiv verwalten und bereitstellen möchten. Wenn Sie einem Kunden bereits einen **Besitzer** Status zugewiesen haben, um vorherige Abonnements zu verwalten, die Sie für Sie erworben haben, können Sie diesen Schritt überspringen.  

> [!IMPORTANT]
> Wenn einem Kunden nicht die Rolle " **Besitzer** " zugewiesen wurde, erhalten Sie einen Fehler in der Azure-Portal die den Kauf von Azure-Reservierungen verhindert.

So überprüfen Sie, ob dem Kunden die Rolle " **Besitzer** " für ein Azure-Abonnement zugewiesen wurde:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie **CSP**und dann **Kunden** aus, und wählen Sie den Kunden aus.

3. Wählen Sie **Abonnements** für diesen Kunden aus, und suchen Sie nach dem jeweiligen Azure-Abonnement.

4. Wählen Sie neben dem Abonnement des Kunden die Schaltfläche **Verwalten** aus. Dadurch wird die [Azure-Portal](https://portal.azure.com/)geöffnet.

5. Wenn Sie einem bestimmten Benutzer die Rolle " **Besitzer** " zuweisen möchten, führen Sie die folgenden Schritte aus, [um einen Benutzer als Administrator zuzuweisen](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Aktivieren oder deaktivieren Sie die Kunden Berechtigungen, um Ihre eigenen Azure-Reservierungen zu erwerben.

Nachdem Sie überprüft haben, ob der Kunde über ein vorhandenes Azure-Abonnement verfügt und Benutzern die Rolle " **Besitzer** " für dieses Abonnement zugewiesen ist, können Sie die Kunden Berechtigungen aktivieren (aktivieren). Mit diesen Schritten können Sie auch die Kunden Berechtigungen deaktivieren (deaktivieren). Sie können Kunden Berechtigungen entweder über das Partner Center-Dashboard oder die [Partner Center-APIs](/partner-center/develop/manage-customers)aktivieren oder deaktivieren.

So aktivieren oder deaktivieren Sie Kunden Berechtigungen in Partner Center:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im linken Navigationsmenü **CSP**und dann **Kunden**aus. Eine Kundenliste wird angezeigt.

3. Wählen Sie einen bestimmten Kundennamen aus.

4. Wählen Sie im Menü Kunde die Option **Konto** aus. Die Seite Kunden **Konto** wird angezeigt.

5. Suchen Sie unten auf der Seite den Bereich **Kunden Berechtigungen** .

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Kunden Berechtigungen auf der Seite Konto." border="true":::

6. Suchen Sie unter **Azure-Reservierungen**die Option **Kauf von Kunden gestatten** .

7. Um die Kunden Berechtigungen zu aktivieren, verschieben Sie den Schalter neben dieser Option in die Position an der Position **an** . Um die Kunden Berechtigungen zu deaktivieren, verschieben Sie den Schalter an die Position **aus** .

>[!NOTE]
> Informationen dazu, was sonst passiert, wenn Sie die Berechtigungen eines Kunden zum Erwerb ihrer eigenen Azure-Reservierungen aktivieren, finden Sie unter Übersicht über die [Kunden Berechtigungen in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Wenn Sie die Kunden Berechtigungen aktivieren (oder deaktivieren), zeichnet das Aktivitätsprotokoll jede Aktion auf. (Auf dieses Protokoll kann zugegriffen werden, wenn Sie das Zahnrad Symbol oben im Partner Center-Dashboard auswählen). Wenn Sie die Kunden Berechtigungen aktivieren oder deaktivieren, wird die Aktion entweder als **Create Customer Purchase-Berechtigungen** oder zum **Löschen von Customer Purchase** -Berechtigungen im Aktivitätsprotokoll angezeigt.

## <a name="help-customers-manage-reservations-they-purchase"></a>Helfen Sie Kunden bei der Verwaltung von Reservierungen

Nachdem Sie den Kunden die Berechtigung zum Erwerb ihrer eigenen Azure-Reservierungen erteilt haben, können Sie Ihnen helfen, die von Ihnen erworbenen Ressourcen besser zu verwalten. Kunden können zahlreiche Aspekte von Azure-Reservierungen selbst direkt aus dem [Azure-Portal](https://portal.azure.com/)verwalten. Sie benötigen Ihre Hilfe bei der Verwaltung einiger anderer Aspekte von Azure-Reservierungen, die Sie in Ihrem CSP-Abonnement erwerben.  

Helfen Sie Kunden, mehr über die Verwaltung dieser Aspekte von Azure-Reservierungen zu erfahren:

- Preise, die Kunden für Azure-Reservierungen bezahlen
- Wie Kunden die Nutzung von Azure-Reservierungen optimieren können
- Was geschieht, wenn Kunden Reservierungen mit einem freigegebenen Bereich erwerben?
- Was geschieht, wenn Kunden eine Reservierung ändern, stornieren und erneuern oder Ihren Bereich ändern möchten?

**Preise, die Kunden für Ihre Reservierungen bezahlen.** Ihr Kunde kauft Azure-Reservierungen auf der Grundlage eines Abonnements, das Sie zuvor für Sie in Ihrem CSP-Partner Abrechnungskonto erworben haben. Der Preis des Kunden für alle Azure-Reservierungen, die basierend auf diesem Abonnement erworben werden, wird ebenfalls von Ihnen festgelegt. Dieser Preis unterscheidet sich möglicherweise vom direkten Web-Preis, der dem Kunden in der Azure-Portal angezeigt wird.

**Wie Kunden ihre Verwendung einer Reservierung optimieren können.** Einige Kunden können davon profitieren, dass Sie mehr darüber erfahren, wie Sie die Verwendung einer Reservierung optimieren oder den anfänglichen Bereich einer Reservierung während des Kaufs zuweisen. Wenn Sie weitere Informationen wünschen, bitten Sie Kunden, sich mit der [Verwaltung von Reservierungen für Azure-Ressourcen](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Was geschieht, wenn ein Kunde eine Reservierung mit einem freigegebenen Bereich erwirbt?** Wenn Kunden eine Reservierung basierend auf einem früheren CSP-Abonnement erwerben und dieser Reservierung einen freigegebenen Bereich zuweisen, gelten alle Rabatte, die der Kunde vom CSP erhalten hat, für die übereinstimmende Nutzung aller Abonnements, die der CSP-Partner für diesen Kunden erworben hat.

**Was sollten Kunden tun, wenn Sie einen von Ihnen vorgenommenen Erwerb austauschen, Abbrechen oder erneuern oder den anfänglichen Bereich einer Reservierung ändern möchten?** Kunden müssen sich an Ihren Partner wenden, um Sie bei der Änderung des Anfangs Bereichs einer Reservierung zu unterstützen. Außerdem benötigen Sie eine Partner Hilfe zum austauschen, Abbrechen oder Erneuern einer Reservierung. Diese Aufgaben können nicht mit Reservierungen auf der Grundlage von Abonnements ausgeführt werden, die von einem CSP-Partner für Sie erworben wurden.

## <a name="next-steps"></a>Nächste Schritte

- [Erwerben von Azure-Reservierungen im Namen Ihrer Kunden](azure-reservations-buying.md)

- [Partner Center: verkaufen von Microsoft-Reservierungen](azure-reservations.md)

- [Azure Reservations im Auftrag Ihrer Kunden verwalten](azure-reservations-manage.md)
