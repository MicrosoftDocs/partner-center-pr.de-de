---
title: Autorisieren von Kunden, eigene Dienste zu erwerben
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie CSP-Programmpartner Kunden ermöglichen können, eigene Dienste wie Azure-Reservierungen für ein für Sie erworbenes Abonnement zu erwerben.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: Abonnement, Self-Service-Erwerb, Self-Service-RI, Aktivieren von RI, Deaktivieren von RI, Self-Service, Kunden Erwerb, Kunden Berechtigungen, reservierte Instanz des Kunden Kauf, Kunden Kauf Azure-Reservierungen, Self-Service aktivieren, Self-Service ausschalten
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255469"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a>Erfahren Sie, wie Sie Kunden die Berechtigung zum erwerben ihrer eigenen Produkte oder Dienste erteilen.

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
- Sie können Kunden Berechtigungen mithilfe des Partner Center-Dashboards oder der [Partner Center-APIs](https://docs.microsoft.com/partner-center/develop/manage-customers)aktivieren (oder deaktivieren).
- Nachdem Sie die Berechtigungen für einen bestimmten Kunden aktiviert haben, sind Sie dafür verantwortlich, alle nachfolgenden Einkäufe dieses Kunden zu bezahlen. Wenn Kunden einen Erwerb austauschen, Abbrechen oder erneuern möchten, können Sie diesen Vorgang nicht selbst durchführen. Sie müssen Sie als Partner bitten, diese Käufe auszutauschen, abzubrechen oder zu erneuern.
- Nachdem Sie die Berechtigungen für einen bestimmten Kunden aktiviert haben, **werden Sie nicht** mehr über spätere Käufe des Kunden benachrichtigt.
- Spätere Käufe, die vom Kunden getätigt werden, werden zusammen mit den von Ihnen getätigten Käufen in Partner Center angezeigt. Diese Käufe finden Sie auf der Seite **Auftrags Verlauf** des Kunden, auf der Seite " **Reservierungen** " oder im [**Aktivitätsprotokoll**](activity-logs.md).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.

Azure-Reservierungen sind eine gute Möglichkeit, um Azure-Dienste zu einem reduzierten Preis zu erwerben. Weitere Informationen zu den Vorteilen von Azure-Reservierungen finden Sie unter [Was ist Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Nun haben Sie die Wahl, Azure-Reservierungen im Auftrag ihrer Kunden zu erwerben, da Sie dies möglicherweise bereits getan haben. Oder Sie können Kunden die Berechtigung erteilen, ihre eigenen Azure-Reservierungen zu erwerben.

>[!NOTE]
> Nachdem Sie den Kunden die Berechtigung zum erwerben ihrer eigenen Azure-Reservierungen erteilt haben, können Sie Ihnen helfen, die von Ihnen erworbenen Reservierungen zu verwalten. Beispielsweise möchten Kunden vielleicht wissen, wie Sie die Verwendung einer Reservierung optimieren oder den Bereich einer Reservierung ändern können. Weitere Informationen zu diesen Themen finden Sie in den Artikeln [Verwalten von Reservierungen für Azure-Ressourcen]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

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

5. Wenn Sie einem bestimmten Benutzer die Rolle " **Besitzer** " zuweisen möchten, führen Sie die folgenden Schritte aus, [um einen Benutzer als Administrator zuzuweisen](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Aktivieren oder deaktivieren Sie die Kunden Berechtigungen, um Ihre eigenen Azure-Reservierungen zu erwerben.

Nachdem Sie überprüft haben, ob der Kunde über ein vorhandenes Azure-Abonnement verfügt und Benutzern die Rolle " **Besitzer** " für dieses Abonnement zugewiesen ist, können Sie die Kunden Berechtigungen aktivieren (aktivieren). Mit diesen Schritten können Sie auch die Kunden Berechtigungen deaktivieren (deaktivieren). Sie können Kunden Berechtigungen entweder über das Partner Center-Dashboard oder die [Partner Center-APIs](https://docs.microsoft.com/partner-center/develop/manage-customers)aktivieren oder deaktivieren.

So aktivieren oder deaktivieren Sie Kunden Berechtigungen in Partner Center:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im linken Navigationsmenü **CSP**und dann **Kunden**aus. Eine Kundenliste wird angezeigt.

3. Wählen Sie einen bestimmten Kundennamen aus.

4. Wählen Sie im Menü Kunde die Option **Konto** aus. Die Seite Kunden **Konto** wird angezeigt.

5. Suchen Sie unten auf der Seite den Bereich **Kunden Berechtigungen** .

   ![Kunden Berechtigungen auf der Seite "Konto"](images/give-customers-permission-reservations.png)

6. Suchen Sie unter **Azure-Reservierungen**die Option **Kauf von Kunden gestatten** .

7. Um die Kunden Berechtigungen zu aktivieren, verschieben Sie den Schalter neben dieser Option in die Position an der Position **an** . Um die Kunden Berechtigungen zu deaktivieren, verschieben Sie den Schalter an die Position **aus** .

>[!NOTE]
> Informationen dazu, was sonst passiert, wenn Sie die Berechtigungen eines Kunden zum Erwerb ihrer eigenen Azure-Reservierungen aktivieren, finden Sie unter Übersicht über die [Kunden Berechtigungen in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center). Wenn Sie die Kunden Berechtigungen aktivieren (oder deaktivieren), zeichnet das Aktivitätsprotokoll jede Aktion auf. (Auf dieses Protokoll kann zugegriffen werden, wenn Sie das Zahnrad Symbol oben im Partner Center-Dashboard auswählen). Wenn Sie die Kunden Berechtigungen aktivieren oder deaktivieren, wird die Aktion entweder als **Create Customer Purchase-Berechtigungen** oder zum **Löschen von Customer Purchase** -Berechtigungen im Aktivitätsprotokoll angezeigt.

## <a name="see-also"></a>Weitere Informationen

- [Erwerben von Azure-Reservierungen im Namen Ihrer Kunden](azure-reservations-buying.md)
- [Partner Center: verkaufen von Microsoft-Reservierungen](azure-reservations.md)
- [Azure Reservations im Auftrag Ihrer Kunden verwalten](azure-reservations-manage.md) 