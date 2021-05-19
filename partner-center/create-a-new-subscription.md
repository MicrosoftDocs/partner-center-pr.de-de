---
title: Erstellen von Kundenabonnements in Partner Center
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Abonnements für von Microsoft veröffentlichte Produkte und SaaS-Produkte, die von ISVs von Drittanbietern veröffentlicht werden, an Ihre Kunden verkaufen.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148196"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Erstellen, Aussetzen oder Stornieren von Kundenabonnements

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Administrator-Agent| Abrechnungsadministrator| Globale Administratorrechte | Helpdesk-| Vertriebs-Agent

Nachdem Sie für Ihre Kunden einen Datensatz im Partner Center erstellt haben, können Sie ihnen Abonnements für Produkte im Katalog verkaufen. Dies schließt Produkte ein, die von Microsoft veröffentlicht werden, sowie SaaS-Produkte (Software-as-a-Service), die von unabhängigen Softwareherstellern (Independent Software Vendors, ISVs) von Drittanbietern im [kommerziellen Marketplace veröffentlicht werden.](https://azuremarketplace.microsoft.com/marketplace)

Einige Angebote sind auf ein Abonnement pro Kunde beschränkt. Eine Liste der eingeschränkten Angebote finden Sie im Partner Center auf der Seite für Preise und Angebote.

>[!IMPORTANT]
> Als Partner im CSP-Programm können Sie lizenzbasierte oder gemessene  SaaS-Abonnements von ISV-Herausgebern innerhalb Partner Center.  Dies bedeutet, dass Sie alle lizenzbasierten oder gemessenen  SaaS-Angebote [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) erwerben können, die der **ISV-Herausgeber** Ihnen zur Verfügung gestellt hat, einschließlich exklusiver Angebote, auf die Sie Zugriff haben. Um andere, kommerzielle Marketplace-Angebote von ISVs zu erwerben oder zu verwalten (z. B. nutzungsbasierte Angebote mit Azure-Anwendungen, Containern oder virtuellen [Azure-Portal).](https://portal.azure.com/)

## <a name="create-a-new-subscription"></a>Erstellen eines neuen Abonnements

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie **Abonnement hinzufügen** aus. Auf **der Registerkarte Onlinedienste** werden alle verfügbaren Marketplace-SaaS-Angebote angezeigt.

4. Um nur bestimmte Arten von Abonnements anzuzeigen, treffen Sie eine Auswahl bei den verfügbaren Filter:
   - **Herausgeber:** Wählen Sie **Microsoft** aus, um nur Angebote von Microsoft oder **Partner** zu sehen, um von ISVs veröffentlichte Produkte aus dem kommerziellen Marketplace zu sehen.
   - **Abrechnungstyp:** Wählen Sie den Typ der Abonnementabrechnung aus, den Sie verwenden möchten: **Lizenz** oder **Nutzung**. Informationen [zur Entscheidung zwischen monatlicher](license-based-billing.md) und jährlicher Abrechnungshäufigkeit finden Sie unter Lizenzbasierte Abrechnung.
   - **Kategorie:** Wählen Sie **Enterprise,** **Small Business** oder **Trial aus.** Informationen zu Testabonnements finden Sie unter [Testversionen von Microsoft-Produkten anbieten](offer-your-customers-trials-of-microsoft-products.md).

5. Wählen Sie die Produktabonnements aus, die Sie für Ihren Kunden erwerben möchten. Welche Produkte Sie sehen, hängt von der Art des Kundensegments (Bildung, Regierung usw.) und den angewendeten Filtern ab. Einige angebote, die im Marketplace angezeigt werden, sind möglicherweise nicht immer für einen bestimmten Kunden oder einen bestimmten CSP-Partner verfügbar. Dies kann sein, weil:

   - Der Kunde verfügt bereits über ein Abonnement für dieses Produkt und ist nur eines zulässig.

   - Das Abonnement des Kunden wurde möglicherweise ausgesetzt (in diesem Fall können Sie das Abonnement reaktivieren, anstatt ein neues zu erwerben).)

   - Für ISV-SaaS-Angebote gibt es möglicherweise einige Gründe, warum das Angebot nicht zum Kauf verfügbar ist: Der ISV unterstützt das Abrechnungsland oder die Region des Kunden möglicherweise nicht. der ISV hat sich möglicherweise dafür entschieden, das Angebot nicht über das CSP-Programm verfügbar zu machen. oder der ISV hat das Angebot möglicherweise nur für bestimmte CSP-Partner [exklusiv](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gemacht. Das ISV-Angebot ist möglicherweise auch nicht über die Partner Center transaktionsfähig (z. B. Container oder einige nutzungsbasierte Angebote).  

6. Geben Sie für jedes Abonnement, das Sie hinzufügen möchten, die Anzahl der Lizenzen ein (falls erforderlich), und wählen **Sie Zum Warenkorb hinzufügen** aus.

7. Wenn Sie mit dem Hinzufügen von Abonnements fertig sind, wählen Sie **Überprüfen** aus, und überprüfen Sie Ihre Bestellung.

8. Nachdem Sie Ihre Bestellungen überprüft haben und bereit sind, diese Abonnements zu erwerben, wählen Sie **Kaufen** aus.

9. Nachdem Sie ein Abonnement für einen Kunden gekauft haben, geschieht Folgendes:

    - Sie können das Abonnement überprüfen oder bearbeiten, indem Sie auf der Seite **Abonnements** des Kunden den Abonnementnamen auswählen. Dort können Sie Add-On-Lizenzen auswählen, falls verfügbar, die Menge der Lizenzen ändern oder das Abonnement aussetzen.

    **Für ISV-SaaS-Abonnements (lizenzbasiert und gemessen):**
    - Sie erhalten einen Link zur Website des ISV-Herausgebers. Dieser Link sollte Ihnen helfen, die Bereitstellung oder Kontoeinrichtung des Kundenabonnements abzuschließen.
      
    >[!NOTE]
    > Weder Sie noch Ihr Kunde erhalten eine E-Mail mit Anweisungen zum Abschließen der Kontoset up/provisioning für diese Art von ISV-Abonnement.)

    - Wenn Ihr Abonnement eine 30-tägige kostenlose Testversion enthält, wird der kostenlose Testzeitraum automatisch angewendet. Als Partner im CSP-Programm können Sie nicht auf den kostenlosen Testzeitraum für Angebote verzichten, die Sie für Kunden erwerben. Sobald der kostenlose Testzeitraum endet, beginnt die Abonnementlaufzeit, und das Abonnement wird in den kostenpflichtigen Status konvertiert. Das Abonnement wird dann automatisch gemäß demselben Zeitplan verlängert.
   
## <a name="update-subscriptions-with-add-ons"></a>Aktualisieren von Abonnements mit Add-Ons 

Um ein Add-On zu erwerben, muss der Kunde zunächst über ein aktives Basisabonnement verfügen.  Sie können über den Katalog keine Add-Ons erwerben.

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie das Abonnement aus, das Sie verwalten möchten.

4. Unterhalb **des Abschnitts** Status finden Sie eine Liste der verfügbaren Add-Ons für das Abonnement.  

5. Aktualisieren Sie die Anzahl der Lizenzen für jedes erforderliche Add-On. Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.

Die Möglichkeit, Add-Ons über Partner Center zu erwerben, steht nur direkten Abrechnungsanbietern und indirekten Anbietern zur Verfügung.
Nur geeignete Add-Ons werden basierend auf den Basisanforderungen und der regionalen Verfügbarkeit angezeigt. Weitere Informationen zu Preisen und Angeboten finden Sie in der Cloud Reseller-Angebotsmatrix. Wenn die Ausführung des Basisabonnements angehalten wird, werden auch alle zugehörigen Add-Ons angehalten.

Das Startdatum für Add-Ons richtet sich nach dem Basisabonnement, und die Gebühren werden anhand des entsprechenden Start- und Enddatums berechnet. Die erste Rechnung enthält die anteiligen Gebühren. Weitere Informationen finden Sie unter [Lizenzbasierte Abrechnung.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Aussetzen oder Stornieren eines Abonnements

Partner können ein Abonnement auf Anforderung des Kunden, bei Nichtbezahlung oder bei Betrug aussetzen oder kündigen.

### <a name="suspend-a-subscription"></a>Aussetzen eines Abonnements

Wenn Sie den Status eines Abonnements zu **Ausgesetzt** ändern, können sich Benutzer nicht anmelden oder auf Dienste zugreifen.

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie das Abonnement aus, das Sie verwalten möchten.

4. Wählen Sie im Abschnitt **Status** die Option **Ausgesetzt** aus. Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.

5. Alle Daten werden gelöscht, solange das Abonnement nicht innerhalb von 90 Tagen oder 90 Tagen zuzüglich der Anzahl der Tage zwischen der Eröffnung des Kontos und dem ersten Abrechnungszeitraum (maximal 120 Tage) reaktiviert wird.

Wenn Sie ein Abonnement aussetzen, gibt das Datum, das unterhalb der Schaltfläche **Ausgesetzt** angezeigt wird, an, wann das Abonnement automatisch ablaufen würde, wenn Sie es nicht erneut aktivieren. 

>[!NOTE]
>CSP-Abonnements haben keinen abgelaufenen Zeitraum (wie web-direct-Abonnements), in dem die Dienste weiterhin funktionieren, das Abonnement jedoch keine Abrechnungsgebühren generiert. CSP-Abonnements sind entweder aktiv oder angehalten (oder vollständig gelöscht).

### <a name="cancel-a-subscription"></a>Kündigen eines Abonnements

Sie können lizenzbasierte SaaS-Abonnements von ISV-Herausgebern von Drittanbietern im Partner Center [Marketplace kündigen.](csp-commercial-marketplace-overview.md) Solange Sie innerhalb des Kündigungszeitraums kündigen, erhalten Sie eine vollständige Rückerstattung.

Für ISV-Angebote, die monatlich abgerechnet werden:

- Wenn Sie weniger als 24 Stunden nach der Bestellung stornieren, erhalten Sie auf der nächsten Rechnung eine vollständige Gutschrift.

- Wenn Sie später als 24 Stunden nach der Bestellung stornieren, wird die Kündigung bei der Verlängerung geplant.

Für jährlich abgerechnete Angebote:

- Wenn Sie weniger als 14 Tage nach der Bestellung stornieren, erhalten Sie auf der nächsten Rechnung eine vollständige Gutschrift.

- Wenn Sie später als 14 Tage nach der Bestellung stornieren, wird die Kündigung bei der Verlängerung geplant.

Nachdem diese Zeiträume beendet sind, wird ihnen die Option zum Kündigen des Abonnements nicht mehr zur Auswahl stehen.

> [!NOTE]
> Nutzungsbasierte und gemessene ISV-Dienste von Drittanbietern (die z. B. virtuelle Computer oder Container verwenden) sind nicht zur Rückgabe berechtigt. Nutzungsbasierte Dienste können als Abbruchmethode aufgehoben werden. Da Gebühren nach der Nutzung in Rechnung gestellt werden, sind diese Dienste nicht für eine Rückerstattung berechtigt.

Gehen Sie zum Kündigen eines lizenzbasierten SaaS-Abonnements eines ISV-Herausgebers wie folgt vor:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Suchen Sie das Abonnement, das Sie kündigen möchten.

4. Wählen Sie in der Spalte **Status** die Option **Abbrechen** aus. Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.

5. Wenn ein Dialogfeld angezeigt wird, geben Sie alle relevanten Details ein, und wählen Sie dann **Senden** aus.

6. Um den Abbruch zu bestätigen, wählen Sie **Ja, abbrechen** aus.

> [!NOTE]
> Sie können auch ein Azure Marketplace Abonnement mithilfe von APIs kündigen. Informationen hierzu finden Sie unter [Kündigen eines Azure Marketplace Abonnements.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Auswählen, ob ein Abonnement des kommerziellen Marketplace automatisch verlängert werden soll

Standardmäßig sind aktive Abonnements so festgelegt, dass sie automatisch erneuert werden, wenn der Abonnementzeitraum abläuft. Für [Abonnements von Produkten des kommerziellen Marketplace](csp-commercial-marketplace-overview.md)können Sie optional festlegen, dass das Abonnement nicht automatisch verlängert wird.

So beenden Sie die automatische Verlängerung eines aktiven Abonnements für den kommerziellen Marketplace:

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie **Abonnements**. Hier werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.

4. Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.

5. Navigieren Sie auf der Seite mit den Abonnementdetails zum Abschnitt **Status,** und deaktivieren Sie das Kontrollkästchen **Automatische Verlängerung.**

6. Klicken Sie auf **Submit** (Senden).

## <a name="next-steps"></a>Nächste Schritte

- [Kaufen von Produkten des kommerziellen Marketplace für Ihre Kunden](csp-commercial-marketplace-purchase.md)

- [Verwalten kommerzieller Marketplace-Produkte für Ihre Kunden](csp-commercial-marketplace-manage.md)

- [Übersicht über den kommerziellen Marketplace](csp-commercial-marketplace-overview.md)