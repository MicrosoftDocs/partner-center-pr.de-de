---
title: Ankündigungen für Januar 2021
description: Ankündigungen für Januar 2021 zum Microsoft Partner Center, einschließlich neuer Funktionen, Promotionen, Angebote, Märkte oder Änderungen an bestehenden Angeboten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 01/15/2021
ms.openlocfilehash: 9b972354fb21dbdfa4780717cee54bac14acdb0e
ms.sourcegitcommit: 9bcccaf8864d8ee3c93e67691f773463f162b5f0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/19/2021
ms.locfileid: "98571668"
---
# <a name="january-2021-announcements"></a>Ankündigungen für Januar 2021

Auf dieser Seite finden Sie Informationen zu den Ankündigungen vom Januar 2021 für Microsoft Partner Center.

Ankündigungen für 2021: Januar

Ankündigungen für 2020: [Mai](2020-may.md) | [Juni](2020-june.md) | [Juli](2020-july.md) | [August](2020-august.md) | [September](2020-september.md) | [Oktober](2020-October.md) | [November](2020-november.md) | [Dezember](2020-december.md)  

________________
## <a name="perpetual-software-now-generally-available-for-the-cloud-solution-provider-program"></a><a name="11"></a> Unbefristete Software ist jetzt allgemein im Cloud Solution Provider-Programm verfügbar

### <a name="categories"></a>Kategorien

- Datum: 19.01.2021
- Umsatzsteigerung

### <a name="impacted-audience"></a>Zielgruppe

Alle CSP-Partner

### <a name="details"></a>Details

Wie heute [angekündigt](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/), freuen wir uns, Ihnen mitteilen zu können, dass kommerzielle, unbefristete Softwarelizenzen nun allen CSP-Partnern allgemein zum Verkauf zur Verfügung stehen. Die CSP-Preisliste für unbefristete Software im Partner Center wurde neu veröffentlicht und enthält jetzt weitere Produkte und geografische Regionen.

Beachten Sie auch, dass ab heute die Partner Center-Funktionen für Software und Lizenzschlüssel eingestellt werden und dass Partner und Kunden künftig das Microsoft 365 Admin Center für diesen Zweck verwenden sollten.
Weitere Informationen und die nächsten Schritte sind unten angegeben.

### <a name="next-steps"></a>Nächste Schritte

- Laden Sie die **CSP-Preisliste für unbefristete Software** im Abschnitt **Software** auf der Partner Center-Seite [Preise und Angebote](https://partnercenter.microsoft.com/en-us/pcv/sales) herunter. Eine Auflistung der neu hinzugefügten Produkte und geografischen Regionen finden Sie [hier](https://partner.microsoft.com/resources/detail/software-in-csp-new-products-geos-pdf).
- Lesen Sie die [Anleitung zum Herunterladen von unbefristeter Software und Lizenzschlüsseln im Microsoft 365 Admin Center](https://go.microsoft.com/fwlink/p/?linkid=2152525), und geben Sie diese Informationen an Ihre Kunden weiter, wenn sie zum Herunterladen ihrer Software und Lizenzschlüssel bereit sind.
- Sehen Sie sich die Readiness-Materialien für [unbefristete Software im Cloud Solution Provider-Programm](https://partner.microsoft.com/resources/collection/software-in-csp#/) an. Verwenden Sie diese [Readiness-Karte](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf), um schnell die richtigen Informationen für Ihre Rolle zu finden.

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.

_____________
## <a name="reminder-introducingapithrottlingtopartners-calling-partner-centerapis"></a><a name="10"></a> Erinnerung: Einführung einer API-Drosselung für Partner, die Partner Center-APIs aufrufen 

### <a name="categories"></a>Kategorien

- Datum: 19.01.2021
- Umsatzsteigerung

### <a name="summary"></a>Zusammenfassung

Microsoft implementiert eine API-Drosselung, um den Partnern, die Partner Center-APIs aufrufen, eine konsistentere Leistung innerhalb einer Zeitspanne zu ermöglichen.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen  

### <a name="details"></a>Details

Ab Februar 2021 implementiert Microsoft eine API-Drosselung, um den Partnern, die Partner Center-APIs aufrufen, eine konsistentere Leistung innerhalb einer Zeitspanne zu ermöglichen. Durch die Drosselung wird die Anzahl von Anforderungen für einen Dienst in einer Zeitspanne begrenzt, um eine übermäßige Nutzung von Ressourcen zu verhindern. Wenn ein Drosselungsschwellenwert überschritten wird, schränkt Partner Center alle weiteren Anforderungen von diesem Client für einen bestimmten Zeitraum ein.
  
**Partnervorteile:** Partner Center ist darauf ausgelegt, eine große Anzahl von Anforderungen zu verarbeiten. Wenn jedoch eine übergroße Anzahl von Anforderungen von einigen wenigen Partnern gestellt wird, kann durch eine Drosselung die optimale Leistung und Zuverlässigkeit für alle Partner aufrechterhalten werden.  

- Durch eine Drosselung werden minimale Ausfallzeiten sichergestellt.
- Eine Drosselung reduziert die Anzahl von Anforderungen mit hohem Volumen und sorgt so für eine konsistente Leistung für alle Partner.

**Zu drosselnde APIs:**

| Vorgang | Partner Center-Dokumentation |
| ------ | ------- |
|{baseURL}/v1/customers/{customer_id}/subscriptions  | [Abrufen aller Abonnements eines Kunden](/partner-center/develop/get-all-of-a-customer-s-subscriptions&data) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}  | [Abrufen eines Abonnements nach ID](/partner-center/develop/get-a-subscription-by-id) |
|{baseURL}/v1/customers/{customer_id}/orders  | [Abrufen aller Kundenaufträge](/partner-center/develop/get-all-of-a-customer-s-orders) |
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}  | [Abrufen eines Auftrags nach ID](/partner-center/develop/get-an-order-by-id) |
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}/provisioningstatus  | [Abrufen des Abonnementbereitstellungsstatus](/partner-center/develop/get-subscription-provisioning-status) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}  | [Verwalten von Aufträgen und Verwalten eines Abonnements](/partner-center/develop/manage-orders#manage-a-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/addons  | [Abrufen einer Liste von Add-Ons für ein Abonnement](/partner-center/develop/get-a-list-of-add-ons-for-a-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/azureEntitlements | [Abrufen einer Liste von Azure-Berechtigungen für ein Abonnement](/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/registrationstatus  | [Abrufen des Abonnementregistrierungsstatus](/partner-center/develop/get-subscription-registration-status) |
|{baseURL}/v1/customers/{customer-tenant-id}/transfers  | [Abrufen aller Übertragungen eines Kunden](/partner-center/develop/get-all-of-a-customer-s-transfers) |
|{baseURL}/v1/productUpgrades/{upgrade-id}/status  | [Abrufen des Status der Produktaktualisierung](/partner-center/develop/get-product-upgrade-status) |
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions   | [Abrufen einer Liste von Testwechselangeboten](/partner-center/develop/get-a-list-of-trial-conversion-offers) |
 
Partnern wird dringend empfohlen, die Aktivitätsprotokoll-API für mehr Effizienz und zur Vermeidung einer Drosselung zu verwenden. Weitere Informationen zu diesem Feature finden Sie  [hier](/partner-center/develop/api-throttling-guidance).  

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die [Ressourcen](/partner-center/develop/api-throttling-guidance)  zu diesem Thema an, und führen Sie die erforderlichen Schritte aus.  

_____________

## <a name="security-compliance-and-identity-sci-launches-coming-on-february-1-2021"></a><a name="9"></a>Einführung von SCI-Angeboten (Sicherheit, Compliance and Identität) am 1. Februar 2021 

### <a name="categories"></a>Kategorien

- Datum: 15.01.2021
- Angebote/Märkte

### <a name="summary"></a>Zusammenfassung

Mehrere neue Microsoft 365-Angebote werden in die Preislistenvorschau im Januar aufgenommen und sind ab dem 1. Februar 2021 verfügbar.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details

#### <a name="microsoft-365-g5-compliance-component-skus-for-government"></a>[SKUs für Microsoft 365 G5-Compliancekomponenten für Behörden](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance)

Wir führen drei neue Komponentenangebote für GCC- (Government Community Cloud) und GCC High-Kunden ein, die ab dem 1. Februar 2021 verfügbar sind. Diese SKUs entsprechen Microsoft 365 E5 Information Protection and Governance, Microsoft 365 E5 Insider Risk Management und Microsoft 365 E5 eDiscovery and Audit, die derzeit in Commercial verfügbar sind. 

   |**Angebotsname**|**Angebots-ID**|**Materialkennung**|
   |-------------------|:------|:------|
   |Microsoft 365 E5 Information Protection and Governance für GCC|9e5397ab-f309-4d90-97f3-6fb5d53074d6|8QL-00002|
   |Microsoft 365 E5 eDiscovery and Audit für GCC|5c9ef884-6307-47e7-a914-f5092feae51e|8RI-00002|
   |Microsoft 365 E5 Insider Risk Management für GCC|11ccfdb3-80cb-4c80-8146-c9775045df17|8RF-00002|
   |Microsoft 365 E5 Information Protection and DLP (Add-On) für GCC|911d3177-53a9-42ec-a0e9-3b73fce527f0|8QY-00002|

#### <a name="10-year-audit-log-retention-add-on"></a>[Add-On zur Aufbewahrung von Überwachungsprotokollen für 10 Jahre](/microsoft-365/compliance/)

Ein Add-On, das Microsoft 365 E5 zur Voraussetzung hat und Kunden ermöglicht, ihre Daten 10 Jahre lang aufzubewahren. 

   |**Angebotsname**|**Angebots-ID**|**Materialkennung**|
   |-------------------|:------|:------|
   |10-Year Audit Log Retention Add On für EDU|879b5e1a-eaa2-4ea9-a628-0b429b2e8732|8LC-00002|
   |10-Year Audit Log Retention Add On|e14ce8d1-09f4-42d2-9b5e-ee85f32e7be4|8LB-00003|
   
#### <a name="frontline-worker-add-ons"></a>Add-Ons für Mitarbeiter in Service und Produktion

Ab dem 1. Februar 2021 können Kunden drei neue programmatische Angebote für Sicherheit und Compliance für Mitarbeiter in Service und Produktion als Add-Ons zu den [Microsoft 365 F1- und F3-SKUs](https://www.microsoft.com/microsoft-365/firstline-workers) erwerben.

Diese programmatischen Angebote ersetzen die aktuelle Promotion für [Sicherheit und Compliance](https://microsoft.sharepoint.com/teams/M365LicensingNews/SitePages/Security-and-Compliance-Promotion-for-Firstline-Workers-Update.aspx), die am **28. Februar 2021** abläuft. Im Gegensatz zur aktuellen Promotion bieten die F5-Add-Ons den Kunden mehr Vorhersagbarkeit für Prognosen bei einer wachsenden Anzahl von Mitarbeitern in Service und Produktion.

   
   |**Angebotsname**|**Angebots-ID**|**Materialkennung**|
   |-------------------|:------|:------|
   |Microsoft 365 F5 Security|a8fba59e-1fc2-4658-8684-5f3d0c71c490|8RQ-00003|
   |Microsoft 365 F5 Compliance|6dc6cb1d-7bcb-4234-80cc-9c7a9cded044|8RL-00003|
   |Microsoft 365 F5 Security & Compliance|ad396924-ee4e-4059-b779-efe43dfa24d2|8RU-00003|
   
### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Preislistenvorschau an, und geben Sie diese an die entsprechenden Mitarbeiter in Ihrer Organisation weiter. Weitere Informationen finden Sie unter [Microsoft Security and Compliance: Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-security-and/ct-p/MicrosoftSecurityandCompliance).

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden. 

_____________ 

## <a name="docusign-migration-to-adobe-sign-for-partners-under-microsoft-partner-agreements-mpas"></a><a name="8"></a>DocuSign-Migration zu Adobe Sign für Partner mit Microsoft Partner-Vereinbarung (MPA) 

### <a name="categories"></a>Kategorien

- Datum: 15.01.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Microsoft stellt die gesamte elektronische Signaturverarbeitung von DocuSign auf Adobe Sign um.

### <a name="impacted-audience"></a>Zielgruppe

Vorhandene direkte und indirekte CSP-Partner (Cloud Solution Provider) unter MPA. Partner in der Ukraine, Russland und Kasachstan müssen Rider einmal pro Jahr physisch oder elektronisch neu signieren.

### <a name="details"></a>Details

Im Februar 2021 beginnt Microsoft mit der Umstellung der gesamten elektronischen Signaturverarbeitung für CSP-Partner von DocuSign auf Adobe Sign. 

Es ist davon auszugehen, dass die Umstellung reibungslos erfolgt. Nach der Migration erhalten Sie eine E-Mail von adobesign@adobesign.com anstelle von DocuSign, wann immer Ihre elektronische Signatur erforderlich ist. Diese E-Mail enthält einen Link zur Adobe Sign-Webseite, auf der Sie eine Signatur vornehmen müssen. Microsoft-Partner müssen vorhandene Vereinbarungen nicht neu signieren, sondern nur zukünftige Channel-Vereinbarungen. 

Ein Beispiel für eine E-Mail mit einer Adobe Sign-Signaturanforderung finden Sie im [Ressourcenkatalog](https://partner.microsoft.com/resources/detail/adobe-sign-signature-request-email-pdf). 

**Um eine optimale Funktion zu gewährleisten, führen Sie die folgenden Schritte aus:**

1. Fügen Sie adobesign@adobesign.com der Liste der sicheren Absender hinzu, um zu verhindern, dass E-Mails von diesem Konto direkt in Ihren Junk-E-Mail-Ordner verschoben werden.
2. Führen Sie folgende Aufgaben zusammen mit Ihrer IT-Abteilung aus:
   - Fügen Sie die E-Mail-Adresse adobesign@adobesign.com der Liste der sicheren Absender hinzu, um sicherzustellen, dass Sie nicht in einer vorkonfigurierten Phishingregel enthalten ist.
   - Aktualisieren Sie vorhandene Sicherheitsrichtlinien, um sicherzustellen, dass alle erforderlichen Empfänger die Dokumente unter der Adobe Sign-Unternehmenslizenz signieren können.

Adobe Sign ist die von Microsoft bevorzugte Lösung für elektronische Signatur (ESS). Die Umstellung auf Adobe Sign gewährleistet eine sichere und effiziente Umgebung für die elektronische Signatur, die unseren Kunden und Partnern einen größeren Nutzen bietet.

Weitere Informationen zum elektronischen Signieren von Dokumenten und Delegieren elektronischer Signaturen finden Sie in den folgenden **Tutorials**: 
- [Elektronisches Signieren eines Dokuments | Adobe Sign-Tutorials](https://helpx.adobe.com/sign/how-to/adobe-for-signers.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/continuinged/collection.ccx.js&ref=helpx.adobe.com)
- [Delegieren einer anderen Person zum Signieren eines Dokuments | Adobe Sign-Tutorials](https://helpx.adobe.com/sign/how-to/use-the-delegator-role.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/orientation/collection.ccx.js&ref=helpx.adobe.com)

### <a name="next-steps"></a>Nächste Schritte

Leiten Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrem Unternehmen weiter.

### <a name="questions"></a>Fragen?

Wenn Sie Fragen haben, wenden Sie sich über das [Call Logging Tool (CLT)](https://clt.partners.extranet.microsoft.com/CLT) oder über [Explore.ms](https://www.explore.ms/) an Ihr Regional Operations Center. Folgen Sie dem CLT-Standardprozess, damit wir Ihre Frage so schnell wie möglich beantworten können.

_____________ 

## <a name="commercial-pricing-update-for-norwegian-krone"></a><a name="7"></a>Aktualisierung der Handelspreise für die norwegische Krone 

### <a name="categories"></a>Kategorien

- Datum: 14.01.2021
- Angebote/Märkte

### <a name="impacted-audience"></a>Zielgruppe

Cloud Solution Provider-Partner, die die norwegische Krone verwenden

### <a name="details"></a>Details

Ab dem 1. März 2021 werden die Preise in norwegischen Kronen für kommerzielle lokale Software und Onlinedienste zur Anpassung an das geltende Preisniveau in der Region geändert.
Die vollständige Ankündigung ist nur für Microsoft-Partner verfügbar. [Melden Sie sich an, um auf die vollständige Ankündigung zuzugreifen](https://partner.microsoft.com/resources/detail/pricing-update-norway-partners-pdf).

_____________ 

## <a name="commercial-pricing-update-for-the-indian-rupee"></a><a name="6"></a>Aktualisierung der Handelspreise für die indische Rupie 

### <a name="categories"></a>Kategorien

- Datum: 08.01.2021
- Angebote/Märkte

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner, die in Indien Transaktionen ausführen

### <a name="details"></a>Details 

Microsoft nimmt Änderungen an der Preisliste für die indische Rupie vor, um die Preise für kommerzielle Software und Onlinedienste innerhalb Indiens und des asiatischen Raums anzugleichen.

Die vollständige Ankündigung ist nur für Microsoft-Partner verfügbar. [Melden Sie sich an, um auf die vollständige Ankündigung zuzugreifen](https://partner.microsoft.com/resources/detail/price-update-indian-rupee.pdf).

________________

## <a name="calling-plan-and-phone-system-updates-for-february-1-20201"></a><a name="5"></a>Aktualisierungen von Calling Plan und Phone System für den 1. Februar 2021

### <a name="categories"></a>Kategorien

- Datum: 08.01.2021
- Angebote/Märkte

### <a name="summary"></a>Zusammenfassung

Ein Add-On-Angebot für Microsoft 365, das Phone System und Domestic Calling Plan sowie einen eigenständigen Domestic Calling Plan umfasst, wird in Kürze für ausgewählte Länder bereitstehen.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details 

Das gebündelte Add-On-Angebot für Microsoft 365 E1-, E3-und E5-Angebote umfasst Phone System und Domestic Calling Plan. Außerdem wird ein neues eigenständiges Domestic Calling Plan-Angebot nur für E5 verfügbar sein. Die neuen Angebote stehen nur Kunden in den USA, Puerto Rico und Kanada zur Verfügung. Für alle anderen Länder und Gebiete bleiben die global bestehenden eigenständigen SKUs und Preise unverändert. 

Die folgenden Angebote sind für Geschäftskunden, Schüler/Studenten, Lehrkräfte, Government Community Cloud (GCC) und gemeinnützige Organisationen in den USA, Puerto Rico und Kanada verfügbar. Anrufpläne sind in keinem der anderen US-Gebiete verfügbar.

   |**Angebotsname**|**Angebots-ID**|**Materialkennung**|
   |-------------------|:------|:------|
   |Microsoft Teams Calling Essentials für USA und Kanada|1ee81de6-4d8b-4cf1-b926-2fd2a774a4ca|8N2-00010|
   |Microsoft Teams Calling Essentials für USA und Kanada (Preise für Personal in gemeinnützigen Organisationen)|0c2ece0d-39b7-40ec-8c08-87c2b6c75d62|8N2-00011|
   |Microsoft Teams Calling Essentials für USA und Kanada für Lehrkräfte|b8baa3b8-8cc2-4f26-a212-7fbeb28e7895|8N3-00003|
   |Microsoft Teams Calling Essentials für USA und Kanada für Schüler/Studenten|26956da8-eeb5-44e3-aa79-d36e0e42b930|8N3-00004|
   |Microsoft Teams Calling Essentials für USA und Kanada für GCC|7a2e2d5a-41b5-4b20-a0d1-0d06d34b5fe1|8N4-00002|
   |Microsoft 365 Domestic Calling Plan für USA und Kanada|60d2919e-427a-46c9-bd03-89cbad27d53f|TK2-00050|
   |Microsoft 365 Domestic Calling Plan für Lehrkräfte für USA und Kanada|602e7548-375b-4e01-bf79-a9a8b8ff16d4|LM7-00006|
   |Microsoft 365 Domestic Calling Plan für Schüler/Studenten für USA und Kanada|1f4b4375-3185-40cf-b044-117fe3b102c6|LM7-00007|
   |Microsoft 365 Domestic Calling Plan für GCC für USA und Kanada|594ed84e-ddf8-4e40-9726-76c04bd29e3b|LM9-00023|

### <a name="next-steps"></a>Nächste Schritte

- Leiten Sie diese Informationen an die zuständigen Mitarbeiter in Ihrem Unternehmen weiter, und informieren Sie sich über Upselling- und Cross-Selling-Möglichkeiten. 
- Lesen Sie den Abschnitt zu Ressourcen im [Partnerleitfaden für Microsoft Teams](https://aka.ms/teamscallingmeetingsguide).

_____________ 

## <a name="license-base-price-list-updates-for-january-2021"></a><a name="4"></a>Aktualisierungen der lizenzbasierten Preislisten für Januar 2021 

### <a name="categories"></a>Kategorien

- Datum: 08.01.2021
- Angebote/Märkte

### <a name="summary"></a>Zusammenfassung

Die Januar- und Februar-Preislisten für lizenzbasierte Angebote wurden aktualisiert, um bestimmte falsche Listenpreise zu korrigieren.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details 

Die lizenzbasierten Preislisten für Januar 2021 und Februar 2021 enthielten einige falsche Listenpreise. Die betroffenen Angebote und Währungen sind nachfolgend aufgeführt. Die korrekten Preise wurden aktualisiert und sind ab dem 7. Januar 2021 um 14:00 Uhr (Pacific Standard Time) verfügbar. 

   |**Angebotsname**|**Angebots-ID**|**Materialkennung**|
   |-------------------|:------|:------|
   |Microsoft 365 E3|2b3b8d2d-10aa-4be4-b5fd-7f2feb0c3091|AAA-35638| 
   |Microsoft 365 Business Basic|bd938f12-058f-4927-bba3-ae36b1d2501c|AAA-10624|

Betroffene Währungen: 

- Preisprobleme bei Microsoft 365 E3 waren ausschließlich auf folgende Währungen beschränkt: JPY (Japanischer Yen), GBP (Britisches Pfund), EUR (Euro), AUD (Australischer Dollar). 
- Probleme bei Microsoft 365 Business Basic waren ausschließlich auf USD (US-Dollar) beschränkt. 

Partner sollten den aktuell verfügbaren Vorschaupreislisten für Januar und Februar die korrekten Preise entnehmen. 

### <a name="next-steps"></a>Nächste Schritte

- Partner sollten die neuesten Preislistendateien aus dem Partner Center herunterladen, um die korrigierten Preise für Januar und Februar zu erhalten. 
- Globale Administratoren für betroffene Mandanten, die zwischen dem 1. Januar und dem 6. Januar Abonnements erworben haben, erhalten vor Ende Januar eine Partner Center-E-Mail mit weiteren Details. 

_____________ 

## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="3"></a> Änderung der Partnerabrechnungswährung für neue E-Commerce-Angebote in der EU/EFTA

### <a name="categories"></a>Kategorien

- Datum: 07.01.2021
- Funktionen

### <a name="impacted-audience"></a>Zielgruppe

- Alle Partner, die Transaktionen im Rahmen des Cloud Solution Provider-Programms in der EU/EFTA-Region ausführen 

### <a name="details"></a>Details

In der Region der Europäischen Union (EU)/Europäischen Freihandelszone (EFTA) wird für alle neuen E-Commerce-Angebote im Cloud Solution Provider-Programm der Abrechnungsstandort des Partners anstelle des Abrechnungsstandorts des Kunden verwendet. Somit basiert die Abrechnung für Partner von Microsoft auf der Währung am Standort des Partners und nicht auf der Währung am Standort des Kunden. Diese Änderung wird in zwei Phasen umgesetzt:

**Phase 1:**

- Neue Kunden, die ein neues E-Commerce-Angebot in CSP erwerben

- Bestandskunden, die erstmalig neue E-Commerce-Angebote erwerben und deren Mandant vor dem 11. Mai 2020 erstellt wurde

Ab dem 28. Januar 2021 werden Partnern mit neuen Kunden, die ein neues E-Commerce-Angebot erwerben, oder Bestandskunden, die erstmalig neue E-Commerce-Angebote erwerben und deren Mandanten vor dem 11. Mai 2020 erstellt wurden, diese Käufe in der Währung am Standort des Partners in Rechnung gestellt.  

Für Partner mit Bestandskunden, die bereits neue E-Commerce-Angebote in CSP erworben haben, erfolgt die Abrechnung in dieser Phase weiterhin in der Währung am Standort der Kunden. Darüber hinaus erfolgt die Abrechnung für Partner mit Bestandskunden, die erstmalig ein neues E-Commerce-Angebot erwerben und deren Mandanten am oder nach dem 11. Mai 2020 erstellt wurden, weiterhin in der Währung der Kunden.

**Phase 2:**

- Bestandskunden, die vor Phase 1 bereits ein neues E-Commerce-Angebot in CSP erworben haben
- Bestandskunden, die erstmalig neue E-Commerce-Angebote erwerben und deren Mandant am oder nach dem 11. Mai 2020 erstellt wurde

Im Anschluss an Phase 1 und während des Kalenderjahrs 2021 stellt Microsoft die Abrechnung neuer E-Commerce-Angebote für Partner mit Bestandskunden, die vor Phase 1 ein neues E-Commerce-Angebot in CSP erworben haben, sowie Kunden, deren Mandanten am oder nach dem 11. Mai 2020 erstellt wurden, von der Währung am Kundenstandort auf die Währung am Partnerstandort um. Partner werden rechtzeitig benachrichtigt, bevor diese Änderung implementiert wird.

Nach Phase 2 erfolgt die Abrechnung für Partner in der EU/EFTA-Region für alle Kunden und alle CSP-Käufe in der Währung am Standort des Partners.

>[!NOTE]
>Diese Änderung wirkt sich nur auf die Abrechnungswährung der Partner aus und nicht auf die Preise neuer E-Commerce-Angebote in CSP. Diese Änderung betrifft die folgenden neuen E-Commerce-Angebote: Azure-Abonnements, die Teil eines Azure-Plans sind, Azure-Reservierungen, Serverabonnements, unbefristete Software und Käufe im kommerziellen Microsoft-Marketplace im Rahmen des Cloud Solution Provider-Programms.


### <a name="partner-benefits"></a>Partnervorteile

Durch diese Neuerung werden Komplexität und Aufwand bei der Abrechnung mit mehreren Währungen in der EU/EFTA-Region für das neue E-Commerce-Verfahren reduziert.

- Partner erhalten eine konsolidierte Rechnung in einer einzigen Währung, und es wird keine Rechnung mehr für jede Kundenstandortwährung ausgestellt.
- Incentiveauszahlungen erfolgen in derselben Währung wie die Rechnung des Partners.
- Partner werden eine geringere Abrechnungskomplexität gegenüber der Rechnungsstellung mit mehreren Währungen feststellen, wodurch Zeit und Ressourcen gespart werden, die derzeit für den Abgleich von Konten aufgewendet werden.
- Für Partner, die noch keine neuen E-Commerce-Angebote übernommen haben, wird diese Änderung an das vorherige Partnerabrechnungsmodell angepasst und ermöglicht den Partnern einen leichteren Übergang zum neuen E-Commerce-Verfahren in CSP.

### <a name="next-steps"></a>Nächste Schritte

Lesen Sie die Informationen zu diesem Thema im [Ressourcenkatalog für Vorgänge](https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/) (Anmeldung erforderlich) auf der Microsoft-Partner-Website.  

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen im Zusammenhang mit dieser Benachrichtigung wenden Sie sich an den [Partner Center-Support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals) (Anmeldung erforderlich).

### <a name="change-log"></a>Änderungsprotokoll

- 17. November 2020: Erstveröffentlichung
- 7\. Januar 2021: Hinzufügung eines zusätzlichen Szenarios für Phase 1 und Phase 2


________________
## <a name="deprecation-and-retirement-of-existing-get-and-put-qualification-apis-for-the-education-customer-validation-process-by-the-end-of-february-2021"></a><a name="2"></a>Einstellung und Deaktivierung vorhandener GET- und PUT-Qualifizierungs-APIs für den Überprüfungsprozess für Kunden im Bildungswesen bis Ende Februar 2021

### <a name="impacted-audience"></a>Zielgruppe

Partner, die Angebote für Bildungseinrichtungen im Rahmen des Cloud Solution Provider-Programms über die Partner Center-API vertreiben

### <a name="details"></a>Details 

Dies ist eine Weiterführung zu den im Dezember 2020 veröffentlichten API-Erweiterungen. Im Dezember 2020 wurden neue GET- und POST-Qualifizierungs-APIs veröffentlicht. Infolgedessen werden die alten GET- und PUT-Qualifizierungs-APIs bis Ende Februar 2021 eingestellt. Ab diesem Zeitpunkt müssen Sie die neuen GET- und POST-APIs im Partner Center verwenden, um Angebote für Bildungseinrichtungen erwerben zu können. 

### <a name="next-steps"></a>Nächste Schritte

- Wenn Sie noch keine Aktualisierung auf die neuen APIs vorgenommen haben, führen Sie diese für eine erfolgreiche und rechtzeitige Umstellung aus.
- Informieren Sie sich über die neuen Änderungen der Partner Center-API, und lesen Sie die [Anleitungen in den Operations Readiness-Ressourcen:  Verbesserungen des Überprüfungsprozesses für Kunden im Bildungswesen im Partner Center](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).
- Leiten Sie diese Informationen an die entsprechenden Teams in Ihrer Organisation und Ihre Handelspartner weiter, um sie bei der Vorbereitung auf diese Änderungen zu unterstützen.

_____________

## <a name="dynamics-365-offers-for-february-2021"></a><a name="1"></a>Dynamics 365-Angebote für Februar 2021

### <a name="categories"></a>Kategorien

- Datum: 04.01.2021
- Angebote

### <a name="summary"></a>Zusammenfassung

Im Februar 2021 werden neue Änderungen der Dynamics 365-Angebote eingeführt.

### <a name="impacted-audience"></a>Zielgruppe

Partner in den Incentiveprogrammen für CSP-Partner mit direkter Abrechnung, indirekte Anbieter und indirekte Wiederverkäufer

### <a name="details"></a>Details

Microsoft kündigt anstehende neue Änderungen der Dynamics 365-Angebote an, die im Februar 2021 für Folgendes eingeführt werden:

- Dynamics 365 Customer Voice – Zusätzliche Antworten
- Dynamics 365 Customer Service Insights – Ende des Lebenszyklus
- Dynamics 365 Cloud – Änderung der AX-Migrationsangebots-IDs

**Dynamics 365 Customer Voice – Zusätzliche Antworten**

Am 1. Februar 2021 stellt Microsoft ein neues Angebot für zusätzliche Antworten (Additional Response) mit einer Berechtigung für 1.000 Antworten als Ersatz für das bestehende Angebot mit 2.000 Umfrageantworten bereit, dessen Verkauf am 1. Februar 2021 endet.

Details zur SKU können Sie dem Tabellenblatt „Customer Voice Addl Resp“ im Excel-Dokument für [Dynamics CSP-Angebote im Februar 2021](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-february-2021-xls) entnehmen. Weitere Informationen finden Sie auf der [Homepage zu Dynamics 365 Customer Voice](https://dynamics.microsoft.com/en-us/customer-voice/overview/).

**Dynamics 365 Customer Service Insights – Ende des Lebenszyklus**

Am 1. Februar 2021 werden die folgenden Produkte eingestellt:

- Dynamics 365 Customer Service Insights (einschließlich „Additional Cases“)
- Dynamics 365 Virtual Agent for Customer Service

Das eigenständige Produkt „Customer Service Insights“ wird in „Dynamics 365 Customer Service“ übernommen. Dort können Kunden dieselben Funktionen tief eingebettet in die Kundendienstumgebungen finden.  

Details zur SKU können Sie dem Tabellenblatt „Customer Service Insights“ im Excel-Dokument für [Dynamics CSP-Angebote im Februar 2021](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-february-2021-xls) entnehmen. Weitere Informationen finden Sie auf der [Homepage zu Microsoft Dynamics Customer Service](https://dynamics.microsoft.com/customer-service/overview/).

**Dynamics 365 Cloud – AX-Migrationsangebots-IDs**

Diese SKUs wurden aus der endgültigen Preisliste vom 1. Januar 2021 entfernt und können derzeit nicht bestellt werden. 

   |**Angebotsname**|**Angebots-ID**|
   |-------------------|:------|
   |Dynamics 365 Finance für AX-Migrationsprogramm|7fbd1115-a4c1-4cf9-b881-40c4187ca581|
   |Dynamics 365 Supply Chain Management für AX-Migrationsprogramm|a3c62c0e-4f8a-4fc9-a47e-dec3310529d0|
   |Dynamics 365 Commerce für AX-Migrationsprogramm|97e98de6-24a8-4282-bad6-9d1a874e90a4|
   |Dynamics 365 Finance Attach für qualifizierendes Dynamics 365-Basisangebot für AX-Migrationsprogramm|69d789e8-1e93-4dee-86b2-3ddfb03c08b9|
   |Dynamics 365 Supply Chain Management Attach für qualifizierendes Dynamics 365-Basisangebot für AX-Migrationsprogramm|c897adce-2964-4d24-abc3-7f7ad4b6a80d|
   |Dynamics 365 Commerce Attach für qualifizierendes Dynamics 365-Basisangebot für AX-Migrationsprogramm|ba1fe561-cfda-405a-a25d-ecda3bd3cba7|
   |Dynamics 365 Operations – Aktivität für AX-Migrationsprogramm|177e954e-1fff-4941-8967-55a47e36e1ce|
   |Dynamics 365 Operations – Gerät für AX-Migrationsprogramm|8c8b7c8f-cb3a-4737-8319-1752938c7be3|
   |Dynamics 365 Team Members für AX-Migrationsprogramm|1eb3ad0b-9de3-419d-8bfe-0d61bdd945b2|

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrem Unternehmen weiter. 

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.

________________
