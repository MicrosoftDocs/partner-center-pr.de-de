---
title: Erwerben eines SaaS-Angebots in Azure-Portal
description: Erfahren Sie, wie Sie ein SaaS-Angebot in Azure-Portal finden und erwerben.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: b73a9acb7b9cf9eee1151de1f8e45f6fd6ef256f
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373474"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Erwerben eines SaaS-Angebots in Azure-Portal

In diesem Artikel werden die verschiedenen Optionen und Anforderungen für das Suchen, Ausprobieren und Erwerben eines SaaS-Angebots (Software-as-a-Service) aus dem Azure-Portal erläutert.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS bietet Ermittlung in Azure-Portal

Sobald Sie sich in Azure-Portal befinden, gibt es einige Möglichkeiten, Ihre Suche einzugrenzen, um sich auf SaaS-Angebote zu konzentrieren.

### <a name="narrowing-your-search"></a>Eingrenzen der Suche

Wählen Sie auf der Startseite unter **Azure-Dienste** die Option **+ Ressource erstellen** oder **Marketplace** aus. Alternativ können Sie die Tastenkombination **G + N** an einer beliebigen Stelle auf der Plattform verwenden.

- Schränken Sie die Ergebnisse auf SaaS-Angebote ein, indem Sie den Filter **Angebotstyp** verwenden und dann **SaaS** auswählen.
- Verwenden Sie die globale Suche Leiste im oberen Navigationsbereich, um nach einem bestimmten SaaS-Angebot zu suchen.

Suchen Sie ein [privates SaaS-Angebot,](/marketplace/private-offers) indem Sie oben auf der **Marketplace-Startseite** auf das Banner klicken. Nicht alle Angebote oder Pläne sind in allen geografischen Regionen verfügbar, und einige werden möglicherweise nur für bestimmte Mandanten angezeigt.

Die gefilterte Ansicht zeigt jedes verfügbare SaaS-Angebot an, das durch einen Titel dargestellt wird. Wählen Sie einen Eintrag aus, um die Seite mit den Produktdetails anzuzeigen. Dies umfasst die folgenden Abschnitte:

- Übersicht: Details zu Dienst, Marketing und Lernmaterialien
- Pläne und Preise: Jedes Angebot enthält mindestens einen Plan mit unterschiedlichen Abrechnungsbedingungen und Preisen.
- Nutzungsinformationen und Support – einschließlich Herausgeber-ID, Angebots-ID und Plan-ID
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
    1. Unter **Plan** wird der ausgewählte Plan auf der Seite "Produktde detail" (PDP) angezeigt. Wenn Sie im PDP keine aktive Auswahl getroffen haben, wird der Standardplan angezeigt. Sie können Ihre Auswahl ändern, indem Sie den Link **Plan ändern** auswählen. Wählen Sie den relevanten Abrechnungszeitraum und dann einen anderen Plan aus. Möglicherweise können Sie den Plan nach dem Kauf ändern, wenn er vom Herausgeber unterstützt wird. Sie können die Laufzeit jedoch nicht von monatlich in jährlich oder von jährlich in monatlich ändern.
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

Um den Prozess abzuschließen und mit der Verwendung des SaaS zu beginnen, müssen Sie mit der Konfiguration Ihres Abonnements beginnen. Wenn Sie auf die Schaltfläche **Konto jetzt konfigurieren** klicken, werden Sie zur Website des Herausgebers umgeleitet.

Sie können ihren Abonnementstatus auch überprüfen, indem Sie rechts oben in der Kopfzeile auf das Glockensymbol klicken.

Wenn Sie den Konfigurationsprozess nicht innerhalb von *30 Tagen* abschließen, wird dieses SaaS-Abonnement automatisch *gelöscht.* Die Abrechnung beginnt, nachdem Ihr Konto auf der Website des Herausgebers konfiguriert wurde.

Fehlermeldungen, auf die Sie während des Prozesses stoßen können:

- Der *Planname des ausgewählten Plans* kann nicht in einem kostenlosen Abonnement erworben werden.
  - Weitere Informationen finden Sie unter Aktualisieren Ihres https://aka.ms/UpgradeFreeSub Kontos.

- Der Kauf ist fehlgeschlagen, weil wir weder eine gültige Kreditkarte noch eine Zahlungsmethode finden konnten, die Ihrem Azure-Abonnement zugeordnet ist.
  - Verwenden Sie ein anderes Azure-Abonnement, oder fügen Sie die aktuelle Kreditkarte oder Zahlungsmethode für dieses Abonnement hinzu/aktualisieren, und wiederholen Sie den Vorgang.

- Der *Planname des plans, der* vom *Angebotsnamen* nach Herausgeber *des Angebots* ausgewählt wurde, steht Ihnen gemäß den von Ihrem IT-Administrator festgelegten Regeln nicht zum Kauf zur Verfügung.
  - Wenden Sie sich an Ihren IT-Administrator.

- Der *Planname des plans, der* vom Herausgeber *des Angebots* *ausgewählt* wurde, steht Ihnen aufgrund privater Marketplace-Einstellungen, die vom IT-Administrator Ihres Mandanten vorgenommen wurden, nicht zum Kauf zur Verfügung.
  - Wenden Sie sich an Ihren IT-Administrator.

- Fehler beim Kauf, weil der angeforderte Abrechnungszeitraum leer oder ungültig ist.
  - Versuchen Sie, einen anderen Plan bzw. eine andere Abrechnungslaufzeit zu erwerben.

- Der Kauf ist fehlgeschlagen, weil wir Ihre Signatur bei einer rechtlichen Vereinbarung nicht überprüfen konnten.
  - Wiederholen. Wenn der Fehler weiterhin auftritt, versuchen Sie, den Kauf mit einem anderen Azure-Abonnement vorzunehmen, oder wenden Sie sich an den Support.

- Fehler beim Kauf des *Angebots offerID* nach *Herausgeber-ID.* Dieses Angebot ist derzeit nicht für den Kauf verfügbar.
  - Versuchen Sie es später noch einmal. Wenn sie nach einer Stunde weiterhin diese Fehlermeldung erhalten, wenden Sie sich an den Support.  

- Fehler beim Erwerb der *Planplan-ID* des Angebots *offerID* nach *Herausgeber-ID.* Dieser Plan ist derzeit nicht für den Kauf verfügbar.
  - Versuchen Sie es später noch einmal. Wenn sie nach einer Stunde weiterhin diese Fehlermeldung erhalten, wenden Sie sich an den Support. 

- Die *Client-E-Mail-Adresse* mit der Objekt-ID *ObjectID* verfügt nicht über die Autorisierung zum Ausführen der Aktion *DeploymentValidationAction* über den Bereich *ResourceGroup. DeploymentScope* oder der Bereich ist ungültig.  
  - Sie erhalten diese Meldung, wenn Sie nicht über die richtigen Berechtigungen für das Azure-Abonnement bzw. die Azure-Ressourcengruppe verfügen.  
    Wenn der Zugriff kürzlich gewährt wurde, aktualisieren Sie Ihre Anmeldeinformationen.  
    Zum Bereitstellen von Ressourcen in einer Ressourcengruppe benötigen Sie mindestens Zugriff auf Mitwirkender. Überprüfen Sie Ihren Zugriffsstatus unter **Ressourcengruppen,** und **Access Control** Sie dann . Dies zeigt, wer der "Besitzer" ist, wen Sie bitten können, Sie als "Mitwirkender" zuzuweisen.

- Das für diesen Kauf verwendete Abonnement lässt keine Marketplace-Käufe zu.  
  - Verwenden Sie ein anderes Abonnement, oder bitten Sie Ihren Administrator, die Definition für dieses Abonnement zu ändern, und wiederholen Sie den Vorgang.

## <a name="next-steps"></a>Nächste Schritte

- Wenn Sie Ihr Angebot über Microsoft verkaufen, lesen Sie [Hinzufügen einer Vorschauzielgruppe für Ihr SaaS-Angebot](/azure/marketplace/create-new-saas-offer-preview).
- Lesen Sie andernfalls [Verkaufen Ihres SaaS-Angebots](/azure/marketplace/create-new-saas-offer-marketing).
