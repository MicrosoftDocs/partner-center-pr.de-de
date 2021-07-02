---
title: Erwerben eines SaaS-Angebots in Azure-Portal
description: Erfahren Sie, wie Sie ein SaaS-Angebot in Azure-Portal suchen und erwerben.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221439"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Erwerben eines SaaS-Angebots in Azure-Portal

In diesem Artikel werden die verschiedenen Optionen und Anforderungen für das Suchen, Ausprobieren und Erwerben eines SaaS-Angebots (Software-as-a-Service) aus dem Azure-Portal erläutert.

## <a name="create-a-saas-subscription"></a>Erstellen eines SaaS-Abonnements

Um ein SaaS-Abonnement zu erwerben, benötigen Sie ein Azure-Benutzerkonto mit Zugriff auf ein entsprechendes Azure-Abonnement. Dieses Abonnement wird sowohl für die Abrechnung als auch für die Aufteilung Ihrer erworbenen Cloudressourcen verwendet. Weitere Informationen zu Azure-Abonnements finden Sie unter [Erstellen eines zusätzlichen Azure-Abonnements.](/azure/cost-management-billing/manage/create-subscription)

Wählen Sie im Azure-Portal im Abschnitt **Marketplace** das gewünschte SaaS-Angebot aus.

Ein Software-as-a-Service-Abonnement bietet das Recht, einen Dienst für einen bestimmten Zeitraum über ein Onlineabonnement anstelle der lokalen Installation auf einzelnen Computern zu verwenden. Ein Abonnement ist eine Vereinbarung zur Verwendung einer oder mehrerer Cloudplattformen oder Dienste, für die Gebühren entweder basierend auf einer Lizenzgebühr pro Benutzer oder auf dem cloudbasierten Ressourcenverbrauch anfallen. Eine Organisation kann über mehrere SaaS-Abonnements verfügen.

Folgende Einschränkungen gelten für SaaS-Abonnements:

- Keine Studentenabonnements.
- Kein Visual Studio Enterprise Abonnement.
- Keine Abonnements mit kostenlosem Guthaben.
- Für kostenpflichtige Angebote ist ein Zahlungsmittel erforderlich.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS bietet Ermittlung in Azure-Portal

Sobald Sie sich in Azure-Portal befinden, gibt es einige Möglichkeiten, Ihre Suche einzugrenzen, um sich auf SaaS-Angebote zu konzentrieren.

### <a name="narrowing-your-search"></a>Eingrenzen der Suche

Wählen Sie auf der Startseite unter **Azure-Dienste** die Option **+ Ressource erstellen** oder **Marketplace** aus. Alternativ können Sie die Tastenkombination **G + N** an einer beliebigen Stelle auf der Plattform verwenden.

- Schränken Sie die Ergebnisse auf SaaS-Angebote ein, indem Sie den Filter **Angebotstyp** verwenden und dann **SaaS** auswählen.
- Verwenden Sie die globale Suche-Leiste im oberen Navigationsbereich, um ein bestimmtes SaaS-Angebot zu finden.

Suchen Sie ein [privates SaaS-Angebot,](/marketplace/private-offers) indem Sie oben auf der **Marketplace-Startseite** auf das Banner klicken. Nicht alle Angebote oder Pläne sind in allen geografischen Regionen verfügbar, und einige werden möglicherweise nur für bestimmte Mandanten angezeigt.

Die gefilterte Ansicht zeigt jedes verfügbare SaaS-Angebot an, das durch einen Titel dargestellt wird. Wählen Sie einen Eintrag aus, um die Seite mit den Produktdetails anzuzeigen. Dies umfasst die folgenden Abschnitte:

- Übersicht: Details zum Dienst, zu Marketing- und Lernmaterialien
- Pläne und Preise: Jedes Angebot enthält mindestens einen Plan mit unterschiedlichen Abrechnungsbedingungen und Preisen.
- Nutzungsinformationen und Support – einschließlich Publisher-ID, Angebots-ID und Plan-ID
- Bewertung und Überprüfungen des spezifischen SaaS-Angebots

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Verfügbare Abrechnungsmodelle (Pläne/SKUs) für SaaS-Angebote

Jedes SaaS-Angebot hat mindestens einen Plan. Jedem Angebot ist ein Preismodell zugeordnet: Pauschalpreis oder pro Benutzer. Jeder Planpreis ist eine wiederkehrende Gebühr, die null Dollar betragen kann (alle aufgeführten Preise dienen nur zu Beispielzwecken und sind nicht dafür vorgesehen, die tatsächlichen Kosten widerzuspiegeln). Bei dieser Gebühr handelt es sich entweder um eine Pauschalgebühr oder um einen Preis pro Benutzer. Verfügbare Typen von Plänen:

- **Monatliche Pläne:** wiederkehrende monatliche Gebühr; Pauschalgebühr oder monatliche Gebühr pro Benutzer, die bei einer monatlichen Wiederholung bezahlt wird. Wenn die Laufzeit endet, wird der Plan automatisch erneuert.
- **Jährliche Pläne:** wiederkehrende jahresgebühr; Pauschalgebühr oder jahresgebühr pro Benutzer, die im Rahmen einer jährlichen Wiederholung gezahlt wird. Wenn die Laufzeit endet, wird der Plan automatisch erneuert.
- **Benutzerdefinierte Verbrauchszähler:** Zusammen mit den wiederkehrenden Gebühren kann ein Pauschalplan auch optionale benutzerdefinierte Gemessene Dimensionen für die Überschreitungsnutzung enthalten, die nicht in der Pauschalgebühr enthalten sind. Jede Dimension stellt eine abrechenbare Einheit dar. Dies sind variable Kosten, die sich je nach Nutzung der gemessenen Einheiten ändern, z. B. Bandbreite, Tickets oder verarbeitete E-Mails. Ihnen wird die Monatliche Nutzung dieser Dimensionen in Rechnung gestellt. Beachten Sie, dass der Überschreitungsverbrauch nur beginnt, wenn Sie alle gemessenen Einheiten verwendet haben, die in der Pauschalpreis enthalten sind.
- **Kostenlose Testversion:** In einigen Fällen umfasst der Plan einen Testzeitraum von einem Monat, in dem Sie die Software kostenlos verwenden können.  Sobald der Testzeitraum vorbei ist, werden Ihnen die Gebühren gemäß Ihrem Plan in Rechnung gestellt. Testangebote sind nicht mit benutzerdefinierten Zählern kompatibel.

Diese Preismodelle sind sowohl für öffentliche als auch für private Pläne verfügbar.

## <a name="saas-purchase-experience"></a>SaaS-Kauferfahrung

1. Wählen Sie auf der Produktseite einen Plan aus, der Ihren Anforderungen entspricht, und fahren Sie mit **dem Einrichten und Abonnieren** fort.
2. Im Rahmen des Kaufvorgangs werden Sie zur Registerkarte **Grundlagen** umgeleitet, und Sie müssen folgende Anforderungen haben:
    1. Definieren Sie, welches *Abonnement* Sie für die Abrechnung verwenden möchten. Für das azure-Abonnement, das Sie verwenden, sollte eine gültige Kaufmethode definiert sein. Sie sollten über die richtige Berechtigungsebene verfügen oder über eine Ressourcengruppe unter diesem Abonnement mit der richtigen Berechtigungsebene verfügen. Außerdem sollte das Abrechnungsland ein Land sein, in dem das Angebot zum Kauf verfügbar ist. Azure-Abonnements ohne gültige Zahlungsmethode (z. B. ein MSDN-Abonnement) können nur zum Erwerb kostenloser Pläne verwendet werden.
    1. Wählen Sie eine **-Ressourcengruppe* aus, zu der die SaaS-Ressource gehören soll, oder erstellen Sie sie.
    1. Geben Sie einen *Namen* für das SaaS-Abonnement ein, um ihn später leicht zu identifizieren. Nach dem Kauf können Sie den Namen nicht mehr ändern.
    1. Unter **Plan** sehen Sie den plan, den Sie auf der Seite "Produktde detail" (PDP) ausgewählt haben. Wenn Sie im PDP keine aktive Auswahl getroffen haben, wird der Standardplan angezeigt. Sie können Ihre Auswahl ändern, indem Sie den Link **Plan ändern** auswählen. Wählen Sie den relevanten Abrechnungszeitraum und dann einen anderen Plan aus. Möglicherweise können Sie den Plan nach dem Kauf ändern, wenn er vom Herausgeber unterstützt wird. Sie können die Laufzeit jedoch nicht von monatlich in jährlich oder von jährlich in monatlich ändern.
    1. In Fällen, in denen das Preismodell *pro Benutzer* festgelegt ist, müssen Sie möglicherweise die Anzahl der *Benutzer* angeben. Der angezeigte Preis ändert sich basierend auf dem Abonnement, dem Plan und der Laufzeit, die Sie ausgewählt haben.
3. Fahren Sie mit der Registerkarte **Tags** fort: *Tags* sind benutzerdefinierte Schlüssel-Wert-Paare, die direkt auf einer Ressource oder einer Ressourcengruppe platziert werden können. Sie können Tags verwenden, um Ihre SaaS-Ressource später einfach zu finden. Azure unterstützt derzeit bis zu 50 Tags pro Ressource und Ressourcengruppe. Tags können zum Zeitpunkt der Erstellung auf einer Ressource platziert werden oder zu einer vorhandenen Ressource hinzugefügt werden.
4. Fahren Sie mit **Überprüfen und Abonnieren** fort, um das Angebot und die Plandetails zu durchlaufen.
    1. Lesen Sie *Nutzungsbedingungen,* *Zusatzbestimmungen* und *Datenschutzrichtlinien* des Herausgebers sowie Azure Marketplace
    1. Möglicherweise werden Sie aufgefordert, Ihre Kontaktdetails hinzuzufügen.
    1. Überprüfen der *Details zu Grundlagen* und *Tags*
5. Wählen Sie nach der Bestätigung **Abonnieren** aus.

## <a name="saas-subscription-and-configuration"></a>SaaS-Abonnement und -Konfiguration

Wenn Sie abonnieren auswählen, wird in einer Meldung "Ihr SaaS-Abonnement wird ausgeführt" angezeigt. Dieser Vorgang sollte einige Minuten dauern. Schließen Sie das Fenster erst, wenn es abgeschlossen ist.

Sobald das Abonnement abgeschlossen ist, wird in einer Meldung darauf hingewiesen, dass Ihr SaaS-Abonnement abgeschlossen ist, und Sie sollten das Konto so konfigurieren, dass es mit dem Kauf beginnt. Sie erhalten auch eine E-Mail, in der Sie aufgefordert werden, das neue Abonnement zu aktivieren. Wenn Sie nicht der Benutzer sind, der das SaaS-Konto konfiguriert, leiten Sie diese E-Mail an die entsprechende Person weiter.

Um den Prozess abzuschließen und mit der Verwendung des SaaS zu beginnen, müssen Sie mit der Konfiguration Ihres Abonnements beginnen. Wenn Sie die Schaltfläche **Konto jetzt konfigurieren** auswählen, werden Sie zur Website des Herausgebers weitergeleitet.

Sie können ihren Abonnementstatus auch überprüfen, indem Sie rechts oben in der Kopfzeile auf das Glockensymbol klicken.

Wenn Sie den Konfigurationsprozess nicht innerhalb von *30 Tagen* abschließen, wird dieses SaaS-Abonnement automatisch *gelöscht.* Die Abrechnung beginnt, nachdem Ihr Konto auf der Website des Herausgebers konfiguriert wurde.

Fehlermeldungen, auf die Sie während des Prozesses stoßen können:

- Der *Planname des ausgewählten Plans* kann nicht in einem kostenlosen Abonnement erworben werden.
  - Weitere Informationen finden Sie unter Upgrade Ihres https://aka.ms/UpgradeFreeSub Kontos.

- Der Kauf ist fehlgeschlagen, weil wir weder eine gültige Kreditkarte noch eine Zahlungsmethode finden konnten, die Ihrem Azure-Abonnement zugeordnet ist.
  - Verwenden Sie ein anderes Azure-Abonnement, oder fügen Sie die aktuelle Kreditkarte oder Zahlungsmethode für dieses Abonnement hinzu/aktualisieren, und wiederholen Sie den Vorgang.

- Der *Planname des plans, der* vom *Angebotsnamen* nach Herausgeber *des Angebots* ausgewählt wurde, steht Ihnen gemäß den von Ihrem IT-Administrator festgelegten Regeln nicht zum Kauf zur Verfügung.
  - Wenden Sie sich an Ihren IT-Administrator.

- Der Vom Herausgeber des Angebots *ausgewählte Planname des* Vom Herausgeber *des Angebots* *ausgewählten* Plans steht Ihnen aufgrund privater Marketplace-Einstellungen, die vom IT-Administrator Ihres Mandanten vorgenommen wurden, nicht zum Kauf zur Verfügung.
  - Wenden Sie sich an Ihren IT-Administrator.

- Fehler beim Kauf, weil der angeforderte Abrechnungszeitraum leer oder ungültig ist.
  - Versuchen Sie, einen anderen Plan/abrechnungszeitraum zu erwerben.

- Fehler beim Kauf, weil wir Ihre Signatur nicht überprüfen konnten.
  - Wiederholen. Wenn der Fehler weiterhin auftritt, versuchen Sie, den Kauf mit einem anderen Azure-Abonnement zu tätigen, oder wenden Sie sich an den Support.

- Fehler beim Kauf der *Angebots-ID* nach Herausgeber *publisherID.* Dieses Angebot ist derzeit nicht zum Kauf verfügbar.
  - Versuchen Sie es später noch einmal. Wenn Sie nach einer Stunde weiterhin diese Fehlermeldung erhalten, wenden Sie sich an den Support.  

- Fehler beim Kauf der *Planplan-ID* des *Angebots offerID* nach Herausgeber *publisherID.* Dieser Plan ist derzeit nicht für den Kauf verfügbar.
  - Versuchen Sie es später noch einmal. Wenn Sie nach einer Stunde weiterhin diese Fehlermeldung erhalten, wenden Sie sich an den Support. 

- Die *Client-E-Mail-Adresse* mit der *Objekt-ID ObjectID* verfügt nicht über die Autorisierung zum Ausführen der *Aktion DeploymentValidationAction* über den Bereich *ResourceGroup. DeploymentScope* oder der Bereich ist ungültig.  
  - Sie erhalten diese Meldung, wenn Sie nicht über die richtigen Berechtigungen für das Azure-Abonnement bzw. die Ressourcengruppe verfügen.  
    Wenn der Zugriff vor Kurzem gewährt wurde, aktualisieren Sie Ihre Anmeldeinformationen.  
    Um Ressourcen in einer Ressourcengruppe bereitzustellen, müssen Sie mindestens über Zugriff als Mitwirkender verfügen. Überprüfen Sie ihren Zugriffsstatus unter **Ressourcengruppen,** und klicken Sie **Access Control**. Dies zeigt, wer der "Besitzer" ist, den Sie bitten können, Sie als "Mitwirkender" zu zuweisen.

- Das für diesen Kauf verwendete Abonnement lässt keine Marketplace-Käufe zu.  
  - Verwenden Sie ein anderes Abonnement, oder bitten Sie Ihren Administrator, die Definition für dieses Abonnement zu ändern und den Vorgang zu wiederholen.

## <a name="next-steps"></a>Nächste Schritte

- Wenn Sie bereits ein Angebot im Marketplace erworben haben, wechseln Sie zu [Abrechnung und Rechnungsstellung.](/marketplace/billing-invoicing)
- Sie können auch mehr über Optionen für [private Pläne](/marketplace/private-offers) erfahren.
