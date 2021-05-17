---
title: Ankündigungen für April 2021
description: Ankündigungen für April 2021 zum Microsoft Partner Center, einschließlich neuer Funktionen, Promotions, Angebote, Märkte oder Änderungen an bestehenden Angeboten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702823"
---
# <a name="april-2021-announcements"></a>Ankündigungen für April 2021

Auf dieser Seite finden Sie die Ankündigungen vom April 2021 für Microsoft Partner Center.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Bereitschaft: Aktualisierte API zur Überprüfung von Kundenadressen im CSP-Programm geht im Juni online; Testfunktion jetzt verfügbar

### <a name="categories"></a>Kategorien

- Datum: 30.04.2021
- Bereitschaft

### <a name="summary"></a>Zusammenfassung

Damit Partner und Kunden ihre Geschäfte auf Vertrauensbasis tätigen können, laden wir Partner ein, Änderungen an der Adressüberprüfungs-API für alle Länder weltweit zu testen.

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner mit direkter Abrechnung und indirekte Anbieter, die neue Adressdetails für Kunden erstellen oder bestehende Details aktualisieren

### <a name="details"></a>Details

Microsoft setzt auf Vertrauen. Wir haben uns verpflichtet, eine kompatible und sichere Methode der Überprüfung von Kundenadressen zur Abwicklung von Kundenabonnements im CSP-Programm bereitzustellen. Ab dem 31. März 2021 haben wir Änderungen an der Adressüberprüfungs-API eingeführt. Wir laden Partner ein, die API vor der Liveschaltung Ende Juni 2021 zu testen. 

Beachten Sie, dass diese Änderungen nur die Adressüberprüfungs-API betreffen. Die APIs zum Erstellen von Kunden und Aktualisieren von Abrechnungsprofilen sind nicht betroffen. Obwohl die vorgeschlagene Adresse derzeit nicht in der API zum Erstellen von Kunden verwendet werden muss, wird dies dringend empfohlen.

Die Antwort gibt eine der folgenden Statusmeldungen zurück:

| Status     | Beschreibung |    Anzahl der zurückgegebenen vorgeschlagenen Adressen |
|-------|---------------|-------------------|
|Versandfähigkeit überprüft | Die Adresse ist überprüft und für den Versand geeignet. | Eine |
|Überprüft | Die Adresse ist überprüft. | Eine |
|Interaktion erforderlich | Die vorgeschlagene Adresse wurde erheblich geändert und muss vom Benutzer bestätigt werden. | Eine |
|Straße unvollständig | Die angegebene Straße in der Adresse ist unvollständig und erfordert weitere Informationen. | Mehrere – maximal drei |
|Räumlichkeiten unvollständig | Die angegebenen Räumlichkeiten (Gebäudenummer, Suitenummer und andere) sind unvollständig und erfordern weitere Informationen. | Mehrere – maximal drei |
|Mehrere | Mehrere Felder in der Adresse sind unvollständig (möglicherweise einschließlich der Felder für Straße und Räumlichkeiten). | Mehrere – maximal drei |
|Keine | Die Adresse ist falsch. | Keine |
|Nicht überprüft | Die Adresse konnte den Überprüfungsprozess nicht durchlaufen. | Keine |

Bei US-Postleitzahlen werden zusätzlich vier Ziffern und ein Bindestrich zurückgegeben, z. B. 12345-6789.

### <a name="next-steps"></a>Nächste Schritte

- Ausführlichere Anleitungen finden Sie in der technischen Dokumentation und unter den häufig gestellten Fragen in der [jeweiligen Sammlung für Partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).
- Bereiten Sie die Einbindung der Änderungen mithilfe der Partner Center-API und der Webbenutzeroberfläche vor. 
- Teilen Sie dem Fachexperten (Ali Khaki) Ihre Sandbox-Mandanten-ID mit, damit Sie in die Testphase einbezogen werden und mit der Vorbereitung für die Aktualisierung beginnen können. 
- Wenden Sie sich an Ihren CPV (Control Panel Vendor), wenn Sie eine CPV-Lösung verwenden.

### <a name="questions"></a>Fragen?

Wenn Sie Unterstützung hinsichtlich des Geschäftsbetriebs mit Microsoft benötigen, wenden Sie sich an Ihre Yammer-Gruppe beim Partner-Support oder erstellen Sie eine [Serviceanfrage](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Neuer Speicherort für Dokumentation zu Partner Center-API-Swagger

### <a name="categories"></a>Kategorien

- Datum: 26.04.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Die Dokumente zu Partner Center-API-Swagger wurden von der [vorherigen Swagger-Dokumentationswebsite](https://apidocs.microsoft.com/services/partnercenter) zu einer [neuen Swagger-Dokumentationswebsite](https://docs.microsoft.com/rest/api/partner-center-rest/) migriert.

### <a name="impacted-audience"></a>Zielgruppe

Partner mit direkter Abrechnung und indirekte Anbieter, die am CSP-Programm (Cloud Solution Provider) teilnehmen und die Partner Center-APIs verwenden

### <a name="details"></a>Details

Ab dem 26. April 2021 befindet sich die Dokumentation zu Partner Center-API-Swagger, einschließlich der REST-API-Inhalte, auf einer [neuen Website](https://docs.microsoft.com/rest/api/partner-center-rest/). Auf die alte Website kann nach einigen Wochen nicht mehr zugegriffen werden.

### <a name="benefits"></a>Vorteile

Die Dokumentation zu Partner Center-API-Swagger umfasst eine **Testen**-Funktion. Um diese Funktion zu nutzen, benötigen Sie ein Bearertoken, das Sie mithilfe der unter [Partner Center-Authentifizierung](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication) aufgeführten Schritte generieren können.

### <a name="next-steps"></a>Nächste Schritte

Leiten Sie diese Informationen an das geeignete Team in Ihrem Unternehmen weiter, damit es seine Prozesse überprüfen und aktualisieren kann.

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Hinweis zur Richtlinie für den Rückgabezeitraum für Software im CSP-Programm (Cloud Solution Provider) und zum Ablauf des Downloadlinks

### <a name="categories"></a>Kategorien

- Datum: 21.04.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Es gibt Änderungen bei der Richtlinie für den Rückgabezeitraum für Software in CSP und dem Ablauf des Downloadlinks.

### <a name="impacted-audience"></a>Zielgruppe

Partner, die Transaktionen für Angebote für unbefristete Software oder Softwareabonnements in CSP durchführen

### <a name="details"></a>Details

Beachten Sie die folgenden wichtigen Mitteilungen zum Kauf von unbefristeter Software und Softwareabonnements über Partner Center:

#### <a name="software-return-period-policy"></a>Richtlinie für den Rückgabezeitraum für Software

Ab dem 1. Juni 2021 ändert sich der Rückgabezeitraum für Softwareangebote in CSP, wie in der Microsoft Partner-Vereinbarung (MPA) festgelegt, von 60 Tagen ab Bestelldatum in 30 Tage ab Bestelldatum.

Nachdem eine Bestellung für ein Softwareangebot übermittelt wurde, haben Partner 30 Tage ab dem Bestelldatum Zeit, Änderungen an einer solchen Bestellung einzureichen:

- Jede unbefristete Softwarelizenz, die innerhalb des 30-tägigen Rückgabezeitraums zurückgegeben wird, erhält eine vollständige Gutschrift des gezahlten Kaufpreises.

- Jedes Softwareabonnementprodukt, das innerhalb des 30-tägigen Rückgabezeitraums zurückgegeben wird, erhält eine anteilige Gutschrift des gezahlten Kaufpreises.

Diese Benachrichtigung ist eine Fortführung unserer E-Mail-Mitteilungen, die im Dezember 2020 und April 2021 an alle CSP-Partner gesendet wurden und Informationen zum Rückgabezeitraum und anderen Aktualisierungen der MPA enthielten. In diesen Mitteilungen finden Sie ausführliche Informationen zu Änderungen, die sich auf die MPA auswirken.

#### <a name="software-download-link-expiry"></a>Ablauf des Downloadlinks für Software

Ab dem 3. Juni 2021 weisen die Downloadlinks für unbefristete Software und Softwareabonnementprodukte, die über Partner Center erworben wurden, ein Ablaufdatum von fünf Tagen nach dem ersten Download auf. Der Ablaufzeitraum gilt für alle Käufe vor dem 3. Juni 2021 sowie am oder nach dem 3. Juni 2021.

### <a name="next-steps"></a>Nächste Schritte

Lesen Sie die [häufig gestellten Fragen zum Rückgabezeitraum in CSP und dem Ablauf des Downloadlinks](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), und informieren Sie alle entsprechenden Teams in Ihrer Organisation über diese Änderungen:

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Open Licensing-Programm: Umstellung von Handelspartnern auf das CSP-Programm (Cloud Solution Provider)

### <a name="categories"></a>Kategorien

- Datum: 19.04.2021
- Umsatzsteigerung

### <a name="summary"></a>Zusammenfassung

In dieser Mitteilung wird erläutert, wie Sie sich auf die Änderungen vorbereiten, die demnächst für das Open Licensing-Programm anstehen.

### <a name="impacted-audience"></a>Zielgruppe

CSP- und Open License-Partner

### <a name="details"></a>Details

Im Jahr 2020 [kündigte Microsoft an](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/), dass unbefristete Softwarelizenzen für Partner und Kunden über das CSP-Programm (Cloud Solution Provider) allgemein verfügbar sein werden. Der erste Meilenstein wurde im Januar 2021 erreicht, als Angebote für kommerzielle, unbefristete Softwarelizenzen verfügbar wurden. Der nächste wichtige Meilenstein wird im Juli 2021 folgen, wenn Angebote für den [öffentlichen Sektor](https://aka.ms/openlicensepublicsector) verfügbar werden. Es wurde außerdem [mitgeteilt](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/), dass ab dem 1. Januar 2022 keine neuen Softwarelizenzkäufe oder Verlängerungen von Software Assurance oder Onlinediensten über das Open License-Programm vorgenommen werden können.

Durch den Übergang unbefristeter Software zum CSP-Programm im neuen E-Commerce-Verfahren können Partner ihre Möglichkeiten zum Anbieten verschiedener Lösungen und verwalteter Dienste weiter ausbauen. Dies beschleunigt auch den Übergang von Kunden in die Cloud.  Um einen reibungslosen Übergang für unsere Partner und Kunden sicherzustellen, haben wir die folgenden Anpassungen vorgenommen und Materialien erstellt, um diese digitale Transformation zu beschleunigen:

#### <a name="april-2021"></a>April 2021

[Jetzt verfügbar](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Materialen zum Übergang von Open License zu CSP für Handelspartner

#### <a name="july-2021"></a>Juli 2021

##### <a name="csp"></a>CSP

- 1\. Juli: Unbefristete Softwarelizenzen für Kunden im öffentlichen Sektor verfügbar

- 7\. Juli: Unbefristete Softwarelizenzen für Visual Studio Pro und Get Genuine Windows Agreement für alle Segmente verfügbar

##### <a name="open-value"></a>Open Value

- 1\. Juli: Zusätzliche SKUs im Open Value-Programm für Bildungseinrichtungen und gemeinnützige Organisationen verfügbar, Bereitstellung ähnlicher Angebote für das Open License-Programm

##### <a name="open-license"></a>Open License

- 1\. Juli: Microsoft führt keine neuen Angebote mehr im Open License-Programm ein.

#### <a name="january-2022"></a>Januar 2022

- 1\. Januar: Es können keine neuen Käufe oder Verlängerungen über das Open License-Programm getätigt werden.

### <a name="next-steps"></a>Nächste Schritte

#### <a name="csp-indirect-providers"></a>Indirekte CSP-Anbieter

Nutzen Sie die nächsten Monate, um Open License-Handelspartnern bei der Orientierung im CSP-Programm zu helfen. Nehmen Sie dazu an Veranstaltungen der Partnercommunity teil, und nutzen Sie die Materialen zum Übergang von Open License zu CSP für Handelspartner:

- [Materialen zum Übergang von Open License zu CSP für Handelspartner](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Anpassbare Übersichtspräsentation, E-Mail-Vorlage, Leitfaden für das Onboarding indirekter CSP-Vertriebspartner und vieles mehr, um die Akzeptanz bei Ihren Handelspartnern im großen Stil zu fördern.

- [Veranstaltungen der CSP-Partnercommunity](https://globalpbocomm.eventbuilder.com/GlobalCSP), die von Microsoft Business Operations veranstaltet werden.  Nehmen Sie an den verschiedenen Sitzungen teil, um sich mit den Grundlagen von CSP (CSP Fundamentals) vertraut zu machen oder auf dem Laufenden zu bleiben und um Fragen zu Software in CSP zu stellen (Q&A Sessions).

- (Bald verfügbar) Auf indirekte CSP-Vertriebspartner ausgerichtete Schulungssitzung, die von Microsoft Business Operations veranstaltet wird.

#### <a name="open-license-resellers"></a>Open License-Handelspartner

- Wenn Ihre Organisation derzeit nicht für das CSP-Programm registriert ist, wenden Sie sich an Ihren Vertriebspartner, um Informationen zu den ersten Schritte zu erhalten. [Hier](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider) finden Sie einen indirekten Anbieter.

- Wenn Ihre Organisation bereits für das CSP-Programm registriert ist, können Sie [hier](https://partner.microsoft.com/resources/collection/software-in-csp) mehr über unbefristete Software in CSP erfahren.

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Jetzt verfügbar: Readiness-Leitfaden für globale Promotions

### <a name="categories"></a>Kategorien

- Datum: 16.04.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Launch Readiness hat einen neuen [Readiness-Leitfaden für globale Promotions](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) im Operations Readiness-Ressourcenkatalog veröffentlicht. Dieser Leitfaden bietet eine konsolidierte Ansicht aller aktiven [globalen Promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner für Volumenlizenzierung (VL), Dynamics-Preisliste (DPL) und Cloud Solution Provider (CSP)

### <a name="details"></a>Details

Microsoft-Partner haben uns mitgeteilt, dass sie eine konsolidierte Ansicht aller globalen Promotions mit unterstützenden Details benötigen. Sie möchten durch diesen konsolidierten Leitfaden bei Promotions die Gewissheit haben, dass alle verfügbaren Informationen an einem zentralen und leicht zugänglichen Ort verfügbar sind.

Ab April 2021 aktualisiert Microsoft diesen Leitfaden monatlich und stellt ihn in einer dedizierten Sammlung für den Readiness-Leitfaden für globale Promotions im Operations Readiness-Ressourcenkatalog bereit.

Links zu diesem Leitfaden sind auch in den folgenden Sammlungen enthalten:

- [Sammlung für den Produkteinführungskalender](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/): Diese bietet eine zentrale Übersicht über bevorstehenden Produktänderungen und -einführungen.

- [Communitysammlungen](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/): Diese enthalten unterstützendes Material für unsere monatlichen Partner Calls und weisen auf bevorstehende Änderungen und aktuelle Themen von betrieblichem Interesse hin.

- [Partner-Newsletter](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), z. B. das monatliche CSP-Update.

Als monatliche Erinnerung veröffentlichen wir auch eine Partner Center-Ankündigung mit dem jeweils neuen Thema im Readiness-Leitfaden für globale Promotions.

### <a name="next-steps"></a>Nächste Schritte

Zu Beginn jedes Monats finden Sie den aktuellen [Readiness-Leitfaden für globale Promotions](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) im [Operations Readiness-Ressourcenkatalog](https://partner.microsoft.com/resources).

Leiten Sie diese Informationen an alle zuständigen Mitarbeiter in Ihrer Organisation weiter, und teilen Sie uns über die Schaltfläche „War diese Seite hilfreich?“ am Ende jeder Seite mit, wie hilfreich dieser Leitfaden für Sie ist.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Aktualisierungen und Erinnerungen der CSP-Community (Cloud Solution Provider) im April

### <a name="categories"></a>Kategorien

- Datum: 16.04.2021
- Community | Einladungen und Erinnerungen

### <a name="summary"></a>Zusammenfassung

CSP-Communityressourcen sind bei Bedarf verfügbar und werden monatlich aktualisiert, um Sie auf dem Laufenden zu halten und auf Änderungen im CSP-Programm vorzubereiten.

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner mit direkter Abrechnung und indirekte Anbieter

### <a name="details"></a>Details

In diesem Monat enthalten die Ressourcen die folgenden wichtigen Themen:

- [Neuerungen bei der Weiterentwicklung des CSP-Programms und Änderungen des Open License-Programms](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Änderungen der Anforderungen für das Onboarding von Kunden im CSP-Programm in bestimmten Regionen](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Neues Format für die PDF-Rechnung beim neuen E-Commerce-Verfahren im CSP-Programm](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

In der [CSP-Communitysammlung](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/) finden Sie Folgendes:

- Den herunterladbaren [Newsletter mit dem monatlichen CSP-Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), der neueste CSP-Ankündigungen, Aktualisierungen, Ereignisse und Erinnerungen in einem leicht lesbaren Dokument zusammenfasst.

- Den [CSP-Ankündigungskalender](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), der eine zeitliche Übersicht über bevorstehende Änderungen bietet, die sich auf das Programm auswirken.

- Den neuen [Produkteinführungskalender](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), in dem bevorstehende Produkteinführungen und -angebote angezeigt werden.

- [Ressourcen für Aktualisierungen der CSP-Einführung](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) mit leicht nutzbaren Inhalten zu wichtigen betrieblichen Änderungen.

- [Aktualisierungen und Erinnerungen](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) zu wichtigen CSP-Themen, für die Interesse besteht und Anfragen eingegangen sind.

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

CSP Community Call Q&As sind verfügbar, um Sie bei Fragen im Zusammenhang mit bevorstehenden Änderungen zu unterstützen. Registrieren Sie sich jetzt für CSP Community Call Q&As, die im April, Mai und Juni stattfinden. Diese konzentrieren sich auf die neuesten Einführungen, wichtige Aktualisierungen und Erinnerungen.

[Registrieren Sie sich hier](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Communityressourcen an, und registrieren Sie sich für Community Call Q&A.

Um sicherzustellen, dass Sie optimal von Community Call Q&A profitieren, sehen Sie sich die On-Demand-Communityinhalte an, und reichen Sie Ihre Fragen bis zu 48 Stunden vorher ein.

### <a name="questions"></a>Haben Sie Fragen?

Das monatliche CSP Community Call Q&A ist der beste Ort für Fragen im Bezug auf Änderungen im CSP-Programm. Sehen Sie sich jeden Monat das Material an, und senden Sie Ihre Fragen vorab, damit wir in der Sitzung die Themen behandeln können, die für Sie am wichtigsten sind.

Wenden Sie sich an den [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp), um weitere Informationen zu erhalten.

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Letzte Erinnerung: Einstellung der GET-Qualifizierung am 6. Mai 2021

### <a name="categories"></a>Kategorien

- Datum: 04.05.2021

- Funktionen

### <a name="impacted-audience"></a>Zielgruppe

Partner, die Angebote für Bildungseinrichtungen, gemeinnützige Organisationen und GCC (Government Community Cloud) im Rahmen des Cloud Solution Provider-Programms über die Partner Center-API vertreiben

### <a name="details"></a>Details

Diese Ankündigung ist eine Weiterführung zu den [im Dezember veröffentlichten Verbesserungen](https://docs.microsoft.com/partner-center/announcements/2020-december#1) in Partner Center. Im Rahmen dieser Veröffentlichung wurden neue GET- und POST-Qualifizierungs-APIs bereitgestellt. Infolgedessen wird **die vorhandene GET-Qualifizierung am 6. Mai 2021 eingestellt**. Zu diesem Zeitpunkt müssen Sie auf die Verwendung der neuen POST-APIs in Partner Center umgestellt haben. Mit den neuen POST-APIs können Sie Angebote für Bildungseinrichtungen erwerben, während Sie mit den neuen GET-APIs vorab qualifizierte Angebote für gemeinnützige Organisationen und GCC erwerben können.

### <a name="next-steps"></a>Nächste Schritte

- Führen Sie für eine erfolgreiche und rechtzeitige Umstellung eine **Aktualisierung auf die neuen APIs** durch.

- **Informieren Sie sich über die neuen Änderungen der Partner Center-API, und lesen Sie die Anleitungen** in den Operations Readiness-Ressourcen: [Verbesserungen des Überprüfungsprozesses für Kunden im Bildungswesen in Partner Center](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Leiten Sie diese Informationen an die entsprechenden Teams in Ihrer Organisation und Ihre Handelspartner weiter, um sie bei der Vorbereitung auf diese Änderungen zu unterstützen.

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen im Zusammenhang mit dieser Benachrichtigung wenden Sie sich an den [Partner Center-Support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).

### <a name="change-log"></a>Änderungsprotokoll

- 4\. Mai 2021: Letzte Erinnerung an die anstehende Einstellung der GET-Qualifizierung

- 9\. April 2021: Erinnerung an die anstehende Einstellung der GET-Qualifizierung 

- Februar: Aktualisierte Zeitpläne für die Einstellung von GET- und PUT-Qualifizierungen

- Januar: Erinnerung an die anstehende Einstellung von GET- und PUT-Qualifizierungen

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Neues Format für die PDF-Rechnung beim neuen E-Commerce-Verfahren in CSP

### <a name="categories"></a>Kategorien

- Datum: 05.04.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Microsoft führt ein neues Format für die PDF-Rechnung beim neuen E-Commerce-Verfahren im CSP-Programm (Cloud Solution Provider) ein, um Abrechnungsdetails nach Produktdetail anstelle der SKU-Beschreibung anzuzeigen.

### <a name="impacted-audience"></a>Zielgruppe

Partner, die Transaktionen im Rahmen des CSP-Programms durchführen

### <a name="details"></a>Details

Ab Mai 2021 führt Microsoft ein neues Format für die PDF-Rechnung beim neuen E-Commerce-Verfahren im CSP-Programm ein, um Abrechnungsdetails nach Produktdetail anstelle der SKU-Beschreibung anzuzeigen. Bei dieser neuen Aktualisierung werden die Positionen nach Produkttyp aggregiert, wobei jedes Produkt in einer einzelnen Zeile angezeigt wird.

Partner werden diese Änderung zum ersten Mal bei ihrer Rechnung im Mai für den Abrechnungszeitraum zwischen dem 1. April 2021 und dem 30. April 2021 bemerken. Die betroffenen Angebote sind reservierte Microsoft Azure-Instanzen, Azure-Abonnements (Azure-Plan) und Marketplace.

Alle Anforderungen einer Gutschrift/Neuberechnung, die nach der Aktualisierung des Rechnungsformats erfolgen, werden im neuen Format generiert.

#### <a name="partner-benefits"></a>Partnervorteile

Diese Aktualisierung bietet Partnern die folgenden Verbesserungen hinsichtlich der Rechnungsstellung:

- Geringere Rechnungsgröße unter Beibehaltung wichtiger Daten

- Anpassung des Formats an Branchenstandards für kompakte und benutzerfreundliche Rechnungen 

Die folgenden Elemente sind nicht betroffen:

- Abrechnungszusammenfassung in der Rechnungs-PDF

- Vorhandene Abrechnungs-APIs

- Abstimmungsdateien (können zum Abrufen präziser Daten verwendet werden) 

- Rechnungen für nutzungs- und lizenzbasierte Gebühren

### <a name="next-steps"></a>Nächste Schritte

Lesen Sie die Informationen zu diesem Thema im [Operations Readiness-Ressourcenkatalog](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) auf der Microsoft-Partner-Website. Weitere Informationen zu Abrechnungs- und Steuerthemen, einschließlich Abrechnungsressourcen, Rechnungen, CSP-Abrechnung und Steuern, finden Sie im [Abschnitt „Abrechnung“](https://docs.microsoft.com/partner-center/billing) in Partner Center.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Änderungen der Anforderungen für das Onboarding von Kunden im CSP-Programm (Cloud Solution Provider)

### <a name="categories"></a>Kategorien

- Datum: 02.04.2021
- Angebote/Märkte

### <a name="summary"></a>Zusammenfassung

Im Rahmen unserer Verpflichtung, Partner und Kunden bei der Ausführung ihrer Geschäfte auf Vertrauensbasis zu unterstützen, werden wir ab dem 25. März 2021 zusätzliche Kundeninformationen anfordern.

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner mit direkter Abrechnung und indirekte Anbieter mit neuen Kunden oder Bestandskunden in den im nächsten Abschnitt aufgeführten Ländern

### <a name="details"></a>Details

Microsoft setzt auf Vertrauen. Wir haben uns verpflichtet, eine kompatible und sichere Methode der Kundenüberprüfung zur Abwicklung von Kundenabonnements im CSP-Programm bereitzustellen. Am 25. März 2021 werden wir Verbesserungen der Partner Center-API und -Benutzeroberfläche (UI) einführen, die sich auf Partner auswirken, die die beiden folgenden Kriterien erfüllen:

- Der Partner hat eine direkte Abrechnungsbeziehung mit Microsoft (das heißt, er ist ein Partner mit direkter Abrechnung oder ein indirekter Anbieter).

- Der Partner tätigt Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern:

    - Thailand
    - Vietnam
    - Türkei
    - Polen
    - Südafrika
    - Indien
    - Brasilien
    - Irak
    - Myanmar
    - Südsudan
    - Saudi-Arabien
    - Vereinigte Arabische Emirate
    - Venezuela

Partner, die diese Kriterien erfüllen, müssen bei der nächsten Aktualisierung oder Abonnementerstellung für einen Kunden dessen Firmenregistrierungs-ID (auch als Organisations-INN des Kunden bezeichnet) und Telefonnummer angeben. Diese Partner können auch einen optionalen zweiten Vornamen für den Kunden eingeben.

Beachten Sie, dass Sie beim Hinzufügen Ihrer Firmenregistrierungs-ID Ihre Unternehmenssteuer-ID und nicht die persönliche ID des Kunden verwenden sollten.

Für Partner, die Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern tätigen, erfolgte bereits ein Onboarding mit einer früheren Version im November 2020.

- Armenien
- Aserbaidschan
- Belarus
- Ungarn
- Kasachstan
- Kirgisistan
- Moldawien
- Russland
- Tadschikistan
- Ukraine
- Usbekistan

Partner mit Kunden in anderen Ländern weltweit haben Ende März 2021 die Möglichkeit, die Firmenregistrierungs-ID, die Telefonnummer und den zweiten Vornamen für Kunden als optionale Details einzugeben.

### <a name="next-steps"></a>Nächste Schritte

- Ausführlichere Anleitungen finden Sie in der technischen Dokumentation und unter den häufig gestellten Fragen in der jeweiligen [Sammlung für Partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).
- Bereiten Sie die Einbindung der Änderungen mithilfe der Partner Center-API und der Webbenutzeroberfläche vor. API/SDKs werden zu Testzwecken bereitgestellt.
- Stellen Sie sicher, dass Sie beim Onboarding neuer Kunden oder beim Ändern von Bestandskundendetails die zusätzlichen Daten übermitteln.
- Wenden Sie sich an Ihren CPV (Control Panel Vendor), wenn Sie eine CPV-Lösung verwenden.

### <a name="questions"></a>Fragen?

Wenn Sie Fragen in Bezug auf die Firmenregistrierungs-ID (auch INN oder TIN genannt) haben, wenden Sie sich an Ihren Steuerberater oder das örtliche Finanzamt. Microsoft kann in Steuerfragen keine Hilfestellung bieten.

Wenn Sie Unterstützung hinsichtlich des Geschäftsbetriebs mit Microsoft benötigen, erstellen Sie eine [Serviceanfrage](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Anzeige der Produkteinführungen und -angebote in diesem Monat

### <a name="categories"></a>Kategorien

- Datum: 01.04.2021
- Funktionen
 
### <a name="summary"></a>Zusammenfassung

Der Produkteinführungskalender für April 2021 wurde jetzt veröffentlicht.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details

Der [Produkteinführungskalender](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) für April 2021 ist jetzt im Operations Readiness-Ressourcenkatalog verfügbar. Sehen Sie sich die kommenden Produkteinführungen und -angebote hier an.

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich den [Produkteinführungskalender](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) an, und geben Sie die Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.  

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.
