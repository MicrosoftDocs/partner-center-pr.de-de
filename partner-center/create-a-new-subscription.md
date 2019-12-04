---
title: Erstellen, Aussetzen oder Stornieren von Kundenabonnements | Partner Center
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Ihre Kunden Abonnements an Produkte im Katalog verkaufen, nachdem Sie einen Kundendaten Satz in Partner Center erstellt haben.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
Keywords: Abonnement, neu erstellen, Abonnement hinzufügen, anhalten, Abbrechen, aussetzen, anhalten, Saas, Lizenz, ISV, Drittanbieter
ms.localizationpriority: medium
ms.openlocfilehash: 05df57bc744263fd0bbd0eb52411a6e9368926f4
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721721"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Erstellen, Aussetzen oder Stornieren von Kundenabonnements

**Zielgruppe**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government
-  CSP-Partner

**Geeignete Rollen**

- Administratoragent
- Abrechnungsadministrator
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter

Nachdem Sie für Ihre Kunden einen Datensatz im Partner Center erstellt haben, können Sie ihnen Abonnements für Produkte im Katalog verkaufen. Dies schließt sowohl von Microsoft veröffentlichte Produkte als auch SaaS-Produkte (Software-as-a-Service) ein, die von unabhängigen Softwareanbietern (ISVs) von Drittanbietern im [kommerziellen Marketplace](https://azuremarketplace.microsoft.com/marketplace)veröffentlicht wurden. 

Bitte beachten Sie, dass bestimmte Angebote auf ein Abonnement pro Kunde beschränkt sind. Eine Liste der eingeschränkten Angebote finden Sie im Partner Center auf der Seite für Preise und Angebote.

>[!IMPORTANT]
Als Partner im CSP-Programm können Sie nur **Lizenz basierte Saas-** Abonnements von ISV-Verlegern innerhalb von Partner Center erwerben. Dies bedeutet, dass Sie alle **lizenzbasierten Saas-** Angebote erwerben können, die der ISV-Verleger Ihnen zur Verfügung gestellt hat, einschließlich [exklusiver Angebote](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , auf die Sie Zugriff haben. Zum Erwerb oder zur Verwaltung anderer kommerzieller Marketplace-Angebote von ISVs (z. b. **nutzungsbasierte**, gemessene oder Verbrauchs basierte Angebote mit Azure-Anwendungen, Containern oder VMS) müssen Sie das [Azure-Verwaltungs Portal](https://portal.azure.com/)aufrufen. Weitere Informationen finden Sie unter [erwerben kommerzieller Marketplace-Produkte](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Erstellen eines neuen Abonnements

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie **Abonnement hinzufügen**. Auf der Registerkarte **Online Dienste** werden alle verfügbaren Marketplace-SaaS-Angebote angezeigt.

4. Um nur bestimmte Arten von Abonnements anzuzeigen, treffen Sie eine Auswahl bei den verfügbaren Filter:
   - **Herausgeber**: Wählen Sie **Microsoft** aus, um nur Angebote von Microsoft oder **Partnern** anzuzeigen, um kommerzielle Marketplace-Produkte anzuzeigen, die von ISVs veröffentlicht werden.
   - **Abrechnungstyp**: Wählen Sie den Typ der Abonnement Abrechnung aus, den Sie verwenden möchten: **Lizenz** oder **Nutzung**. Unter [Häufig gestellte Fragen zu neuen Abrechnungsfunktionen](faq-about-new-billing-features.md) finden Sie Informationen, die Ihnen bei der Wahl zwischen monatlichem und jährlichem Abrechnungsintervall helfen.
   - **Kategorie**: Wählen Sie **Enterprise**, **Small Business**oder **Testversion**aus. Informationen zu Testabonnements finden Sie unter [Testversionen von Microsoft-Produkten anbieten](offer-your-customers-trials-of-microsoft-products.md).

5. Wählen Sie die Produkt Abonnements aus, die Sie für Ihren Kunden erwerben möchten. Welche Produkte Sie sehen, hängt vom Typ des Kunden Segments (Education, Government usw.) und den von Ihnen angewendeten Filtern ab. Einige Angebote, die auf dem Marketplace angezeigt werden, sind möglicherweise nicht immer für einen bestimmten Kunden oder einen bestimmten CSP-Partner verfügbar. Dies kann folgende Ursache haben:

    - Der Kunde hat bereits ein Abonnement für dieses Produkt und ist nur eins zulässig.

    - Das Abonnement des Kunden wurde möglicherweise angehalten (in diesem Fall können Sie das Abonnement reaktivieren, anstatt ein neues zu erwerben).
    
    - Für ISV-SaaS-Angebote gibt es möglicherweise einige Gründe, warum das Angebot nicht erworben werden kann: der ISV unterstützt das Abrechnungs Land oder die Region des Kunden möglicherweise nicht. der ISV hat möglicherweise entschieden, das Angebot nicht über das CSP-Programm verfügbar zu machen. oder der ISV hat das Angebot möglicherweise nur für bestimmte CSP-Partner [exklusiv](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gestaltet. Das ISV-Angebot kann auch nicht über das Partner Center (z. b. Container oder einige Verwendungs basierte Angebote) übertragen werden.  

6. Geben Sie für jedes Abonnement, das Sie hinzufügen möchten, die Anzahl der Lizenzen (falls erforderlich) ein, und wählen Sie **zum Warenkorb hinzufügen**aus.

7. Nachdem Sie Abonnements hinzugefügt haben, wählen Sie **überprüfen** aus, und überprüfen Sie Ihre Bestellung.

8. Nachdem Sie Ihre Bestellungen überprüft haben und bereit sind, diese Abonnements zu erwerben, wählen Sie **kaufen**aus.

9. Wenn Sie ein Abonnement für einen Kunden erworben haben, tritt Folgendes auf:

    - Sie können das Abonnement überprüfen oder bearbeiten, indem Sie den Abonnement Namen **auf der Abonnementseite des** Kunden auswählen. Dort können Sie Add-On-Lizenzen auswählen, falls verfügbar, die Menge der Lizenzen ändern oder das Abonnement aussetzen.

    **Für ISV Saas-Abonnements (Lizenz basiert):**
    - Sie erhalten einen Link zur Website des ISV-Verlegers. Dieser Link soll Ihnen helfen, die Bereitstellung oder das Konto für das Abonnement des Kunden abzuschließen. (Beachten Sie, dass weder Sie noch Ihr Kunde eine e-Mail mit Anweisungen zum Abschließen der Konto Einrichtung und-Bereitstellung für diese Art von ISV-Abonnement erhalten.)
    
    - Wenn Ihr Abonnement eine 30-tägige kostenlose Testversion enthält, wird der kostenlose Testzeitraum automatisch angewendet. Als Partner im CSP-Programm können Sie den kostenlosen Testzeitraum für Angebote, die Sie für Kunden erwerben, nicht aufheben. Sobald der kostenlose Testzeitraum endet, beginnt die Abonnement Laufzeit, und das Abonnement wird in "bezahlt" konvertiert. Das Abonnement wird dann nach dem gleichen Zeitplan automatisch erneuert.

## <a name="suspend-or-cancel-a-subscription"></a>Aussetzen oder Stornieren eines Abonnements

Partner können ein Abonnement auf Anforderung des Kunden, bei Nichtbezahlung oder bei Betrug aussetzen oder kündigen.

### <a name="suspend-a-subscription"></a>Aussetzen eines Abonnements

Wenn Sie den Status eines Abonnements zu **Ausgesetzt** ändern, können sich Benutzer nicht anmelden oder auf Dienste zugreifen.

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie das Abonnement aus, das Sie verwalten möchten.

4. Wählen Sie im Abschnitt **Status** den Eintrag **Ausgesetzt** aus. **Übermitteln** Sie dann Ihre Änderungen.

5. Alle Daten werden gelöscht, solange das Abonnement nicht innerhalb von 90 Tagen oder 90 Tagen zuzüglich der Anzahl der Tage zwischen der Eröffnung des Kontos und dem ersten Abrechnungszeitraum (maximal 120 Tage) reaktiviert wird.

Wenn Sie ein Abonnement aussetzen, gibt das Datum, das unterhalb der Schaltfläche **Ausgesetzt** angezeigt wird, an, wann das Abonnement automatisch ablaufen würde, wenn Sie es nicht erneut aktivieren. Weitere Informationen finden Sie unter Häufig gestellte [Fragen zu neuen Abrechnungs Features](faq-about-new-billing-features.md).

### <a name="cancel-a-subscription"></a>Stornieren eines Abonnements

Sie haben die Möglichkeit, Lizenz basierte Saas-Abonnements von Drittanbieter-ISV-Verlegern innerhalb des [kommerziellen Marketplace](csp-commercial-marketplace-overview.md)von Partner Center abzubrechen. Solange Sie innerhalb des Abbruch Zeitraums abbrechen, erhalten Sie eine vollständige Rückerstattung.

Für ISV-Angebote, die monatlich abgerechnet werden:

- Wenn Sie weniger als 24 Stunden abbrechen, nachdem Sie die Bestellung aufgegeben haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.

- Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 24 Stunden einen Abbruch durchführen, wird der Abbruch für die Verlängerung geplant.

Für Angebote, die jährlich abgerechnet werden:

- Wenn Sie weniger als 14 Tage abbrechen, nachdem Sie die Bestellung durchgeführt haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.

- Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 14 Tagen abbrechen, wird der Abbruch für die Verlängerung geplant.

Nach Ablauf dieser Zeiträume wird die Option zum Abbrechen des Abonnements nicht mehr angezeigt.

> [!NOTE]
> Nutzungsbasierte und gemessene ISV-Dienste von Drittanbietern (die beispielsweise virtuelle Computer oder Container verwenden) sind nicht für die Rückgabe berechtigt. Verwendungs basierte Dienste können als Abbruch Methode deaktiviert werden. Da Gebühren nach der Verwendung abgerechnet werden, sind diese Dienste nicht für eine Rückerstattung berechtigt.

Gehen Sie folgendermaßen vor, um ein Lizenz basiertes Saas-Abonnement von einem ISV-Verleger abzubrechen:

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Suchen Sie das Abonnement, das Sie abbrechen möchten.

4. Wählen Sie in der Spalte **Status** den Wert **Abbrechen**aus. **Übermitteln** Sie dann Ihre Änderungen.

5. Wenn ein Dialogfeld angezeigt wird, füllen Sie alle relevanten Details aus, und wählen Sie dann **senden**aus.

6. Um den Abbruch zu bestätigen, wählen Sie **Ja, Abbrechen**aus.

> [!NOTE]
> Sie haben auch die Möglichkeit, ein Azure Marketplace Abonnement mithilfe von APIs abzubrechen. Informationen hierzu finden Sie unter [Abbrechen eines Azure Marketplace Abonnements](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Auswählen, ob ein Abonnement des kommerziellen Marketplace automatisch verlängert werden soll

Standardmäßig werden aktive Abonnements auf automatische Verlängerung festgelegt, wenn der Abonnementzeitraum abläuft. Bei [Abonnements von Produkten des kommerziellen Marketplace](csp-commercial-marketplace-overview.md) können Sie optional auswählen, dass das Abonnement nicht automatisch verlängert wird.

So beenden Sie das automatische Erneuern eines aktiven Marketplace-Abonnements:

1. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3.  Wählen Sie **Abonnements**aus. Dadurch werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.

4.  Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.

5. Suchen Sie auf der Seite Abonnement Details den Abschnitt **Status** , und deaktivieren Sie das Kontrollkästchen **Automatische Verlängerung** . 

6. Wählen Sie **Übermitteln** aus.

## <a name="see-also"></a>Weitere Informationen:

- [Erwerben Sie kommerzielle Marketplace-Produkte für Ihre Kunden](csp-commercial-marketplace-purchase.md)
- [Verwalten Sie kommerzielle Marketplace-Produkte für Ihre Kunden](csp-commercial-marketplace-manage.md)
- [Übersicht über den kommerziellen Marketplace](csp-commercial-marketplace-overview.md)


