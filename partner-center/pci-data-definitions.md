---
title: Insights-Datendefinitionen
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Das Dokument listet verschiedene Berichte und deren Datendefinitionen auf, die Sie von der Berichtsseite Insights Download herunterladen können.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686346"
---
# <a name="export--data-definitions"></a>Export – Datendefinitionen 

**Geeignete Rollen** 

- Berichtleser
- Executive Report-Leser

## <a name="introduction"></a>Einführung 

Mithilfe des Hubs Berichte herunterladen im Insights-Dashboard können Sie die unformatierten Datasets exportieren. 

Die verschiedenen Berichte, die Sie zusammen mit ihren Datendefinitionen herunterladen können, sind in den folgenden Tabellen aufgeführt: 

### <a name="partner-profile-report"></a>**Partnerprofilbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPNId | Bezeichner des Microsoft Partner Network (MPN) | 
| PartnerName | Name des Partners | 
| PGA_MPNId | Bezeichner des globalen Partnerkonto-MPN | 
| PGA_PartnerName | Name des globalen Partnerkontos | 
| City | Ort des Partners | 
| Land | Länderstandort des Partners | 
| HierarchyLevel | Gibt an, ob es sich um eine globale MPN-ID oder eine STANDORT-MPN-ID (Location MPN ID) | 

### <a name="customer-details-report"></a>**Bericht "Kundendetails"**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | Bezeichner des Kundenmandanten | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| CustomerSegment | Kundensegment | 
| CustomerMarket | Geografischer Markt des Kunden | 
| CustomerStatus | Kundenstatus (Aktiv oder Inaktiv) | 
| Produkt | Das Produkt, das vom MPN an den Kunden verkauft wird: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI oder Microsoft Azure | 
| SKU | Produkt-SKU | 
| Month | Monat, für den Nutzung und Umsatz gemeldet werden | 
| MPNId | Bezeichner Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp des Partners | 
| SalesChannel | Vertriebskanal | 
| AvailableSeats | Verfügbare Stellen | 
| RevenueUSD | Umsatz in US-Dollar | 

### <a name="reseller-performance-report"></a>**Reseller Performance Report (Bericht zur Resellerleistung)**

> [!Note]
> Umsatz- und ACR-Daten sind nur für Benutzer verfügbar, die Berichts-Viewer der Geschäftsleitung sind.

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| ResellerMPNid | Reseller Microsoft Partner Network Identifier | 
| ResellerName | Name des Handelspartners | 
| ResellerMarket | Handelspartnerland des Markts | 
| IndirectProviderMPNId | Bezeichner des indirekten Anbieters Microsoft Partner Network | 
| IndirectProviderName | Indirekter Anbietername | 
| Month | Monat, für den Nutzung und Umsatz gemeldet werden | 
| Produkt | Produktname | 
| SubscriptionID | Bezeichner des Abonnements | 
| AvailableSeats | Anzahl verfügbarer Arbeitsplätze | 
| AssignedSeats | Anzahl zugewiesener Arbeitsplätze | 
| BilledRevenueUSD | Abgerechneter Umsatz in US-Dollar | 
| CustomerName | Name des Kunden | 
| CustomerTPid | Bezeichner des obersten übergeordneten Kunden | 
| CustomerSegment | Kundensegment | 
| CustomerMarket | Geografischer Markt des Kunden | 
| ResellerStatus | Status des Wiederverkäufers | 

### <a name="subscription-details-report"></a>**Bericht "Abonnementdetails"**

>[!Note]
>Umsatz- und ACR-Daten sind nur für Benutzer verfügbar, die Berichts-Viewer von Führungskräften sind.

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Startdatum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionState | Status des Abonnements (Aktiv oder Änderung) | 
| Month | Monat, für den Nutzung und Umsatz gemeldet werden | 
| IsAutoRenew | Gibt an, ob das Abonnement neu ist (Ja oder Nein). | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden | 
| CustomerTpid | Oberster übergeordneter Bezeichner des Kunden | 
| CustomerSegment | Segment des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| Produkt | Vom Partner an den Kunden verkauftes Produkt | 
| SKU | SKU des Produkts | 
| MPNId | Microsoft Partner Network-ID des Partners | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp für das Abonnement | 
| SalesChannel | Vertriebskanal – Direkt, CSP (Cloud Solution Provider) usw. | 
| AvailableSeats | Aktueller verfügbarer Platz | 
| RevenueUSD | Umsatz in US-Dollar | 
| Registrierungs-ID | Registrierungs-ID des Abonnements | 

### <a name="azure-usage-report"></a>**Azure-Nutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Das Datum des Beginns des Abonnements | 
| SubscriptionEndDate | Das Datum des Endes des Abonnements | 
| SubscriptionState | Aktueller Status des Abonnements (Offen, Geschlossen, Aktiv oder In Toleranzperiode) | 
| Month | Nach Monat aggregiertes Datum | 
| Dienstname | Name des Azure-Diensts | 
| MeterCategory | Name der Verbrauchsmessungskategorie | 
| UsageUnits | Die Anzahl der Einheiten, die während des Abrechnungszyklus verwendet werden | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Übergeordnete ID des Kunden | 
| CustomerSegment | Segment des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| MPNId | Microsoft Partner Network-ID des Kunden | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp des Partners | 
| SalesChannel | Vertriebskanal (Direct/CSP, Indirect/CSP, Direct usw.) | 
| ACR_USD | Von Azure verbrauchter Umsatz (ACR) in US-Dollar | 
| Registrierungs-ID | Registrierungs-ID des Azure-Abonnements | 

### <a name="office-365-license-usage-report"></a>**Office 365-Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Oberste übergeordnete Kunden-ID | 
| WorkloadName | Skype for Business, Teams, Exchange Online | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| PaidAvailableUnits | Anzahl der kostenpflichtigen verfügbaren Einheiten | 
| MonthlyActiveUsers | Anzahl der monatlich aktiven Benutzer | 
| CustomerName | Name des Kunden | 
| CustomerMarket | Geografischer Standort des Markts des Kunden | 
| CustomerSegment | Kundensegment | 
| MPNId | Bezeichner Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp des Partners | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility-Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Übergeordnete ID des Kunden | 
| WorkloadName | Name der ENTERPRISE MOBILITY + SECURITY -Workload (EMS) | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| PaidAvailableUnits | Anzahl der kostenpflichtigen verfügbaren Einheiten | 
| MonthlyActiveUsers | Anzahl der monatlich aktiven Benutzer | 
| CustomerName | Name des Kunden | 
| CustomerMarket | Geografischer Standort des Markts des Kunden | 
| CustomerSegment | Kundensegment | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp des Partners | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365-Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Startdatum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionStatus | Status des Abonnements | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| RevSumDivisionName | Name der Revisionssummendivision | 
| RevSumCategoryName | Name der Summenkategorie "Rev" | 
| SKU | SKU des Produkts | 
| SKUId | SKU-ID des Produkts | 
| FreeVsPaidSKU | Gibt an, ob es sich um eine kostenlose oder kostenpflichtige SKU | 
| SalesModel | Vertriebskanal, der zum Verkaufen des Abonnements verwendet wird | 
| DetailedSalesModel | Detailliertes Verkaufsmodell für das Abonnement | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden mandanten | 
| CustomerTpid | Oberster übergeordneter Bezeichner des Kunden | 
| CustomerSegment | Segment des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| MPNId | Bezeichner Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttachType | Zuordnungstyp für das Abonnement | 
| AvailableSeats | Aktueller verfügbarer Platz | 
| AssignedSeats | Aktuell zugewiesener Platz | 
| ActiveSeats | Aktuelle aktive Arbeitsplätze | 
| BereitstellungOpportunity | Aktuelle Bereitstellungschance | 
| ActiveUsagePercent | Prozentsatz der aktuellen aktiven Nutzung | 

### <a name="power-bi-license-usage-report"></a>**Power BI Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Startdatum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionStatus | Status des Abonnements (Aktiv, Inaktiv oder In Karenzzeit) | 
| Month | Nach Monat aggregiertes Datum | 
| SKU | SKU des Produkts | 
| SKUId | SKU-ID des Produkts | 
| FreeVsPaidSKU | Free- oder paid-SKU-Differentiator | 
| SalesModel | Vertriebsmodell, das zum Verkaufen des Abonnements verwendet wird | 
| DetailedSalesModel | Detailliertes Verkaufsmodell für das Abonnement | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden mandanten | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| CustomerSegment | Segment des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| MPNId | Bezeichner Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttachType | Zuordnungstyp für das Abonnement | 
| AvailableSeats | Aktuell verfügbare Arbeitsplätze | 
| AssignedSeats | Aktuell zugewiesene Arbeitsplätze | 
| ActiveSeats | Aktuelle aktive Arbeitsplätze | 
| BereitstellungOpportunity | Aktuelle Bereitstellungschance | 
| ActiveUsagePercent | Prozentsatz der aktuellen aktiven Nutzung | 

### <a name="teams-meetings-and-calls-report"></a>**Bericht zu Teams-Besprechungen und -Anrufen**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| Subworkload | Unterarbeitslast, für die die Nutzung gemeldet wird (Besprechungen, Anrufe oder Telefonsysteme) | 
| Anzahl von Besprechungen | Anzahl von Besprechungen | 
| Besprechungsdauer | Gesamtdauer der Besprechung in Stunden | 

### <a name="teams-monthly-usage-report"></a>**Bericht zur monatlichen Nutzung von Teams**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| Unterworkload | Unterauslastung, für die Nutzung gemeldet wird (Besprechungen, Anrufe oder Telefonsysteme) | 
| Desktopbenutzer | Anzahl der Benutzer, die Teams auf dem Desktop verwenden | 
| Mobile Benutzer | Anzahl der Benutzer, die Teams auf mobilgeräten verwenden | 
| Webbenutzer | Anzahl der Benutzer, die Teams im Web verwenden | 
| AllUpParticipants | Anzahl eindeutiger Benutzer von Teams für den Monat | 

### <a name="teams-usage-3p-apps-report"></a>**Bericht zu 3P-Apps für die Teams-Nutzung**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Übergeordnete ID des Kunden | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| 3P-App-Name | Name der Teams-App | 
| Benutzeranzahl | Anzahl der Benutzer für die App | 


### <a name="training-details-report"></a>**Bericht "Trainingsdetails"**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| TrainingActivityId | Bezeichner des Trainings | 
| TrainingTitle | Titel des Trainings | 
| TrainingType | Trainingstyp (Zertifizierung oder Prüfung) | 
| IndividualFirstName | Vorname des Kunden | 
| IndividualLastName | Nachname des Kunden | 
| E-Mail | Persönliche E-Mail-ID des Kunden | 
| CorpEmail | Office-E-Mail-ID des Kunden | 
| TrainingCompletionDate | Abschlussdatum des Trainings | 
| Month | Monat, für den die Daten gemeldet werden | 
| IcMCP | Gibt an, ob der Benutzer ein Microsoft Certified Professional (MCP) ist. | 
| MCPID | MCP-ID des Benutzers | 
| MPNId | Bezeichner Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerCityLocation | Geografischer Ort des Partners | 
| PartnerCountryLocation | Geografischer Standort des Partners | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| UserName | Name des Benutzers | 
| UserId | GUID des Benutzers | 
| TrainingName | Name des Trainings | 
| TrainingType | Trainingstyp (Modul oder Lernpfad) | 
| Produkte | Produkt, für das das Lernmodul anwendbar ist | 
| Rollen | Anwendbare Rollen des Trainings | 
| CompletionDate | Datum des Abschlusses des Trainings | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Land | Geografischer Standort des Partners | 

### <a name="competency-summary-and-history-report"></a>**Kompetenzzusammenfassung und Verlaufsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CompetencyName | Name der Kompetenz | 
| CompetencyLevel | Kompetenzebene (Gold oder Silber) | 
| CompetencyStatus | Aktueller Status der Kompetenz (Aktiv, Inaktiv oder In Karenzzeit) | 
| CompetencyStartDate | Startdatum der Kompetenz | 
| CompetencyEndDate | Enddatum der Kompetenz | 

### <a name="competency-performance-report"></a>**Kompetenzleistungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CompetencyName | Name der Kompetenz | 
| CompetencyAttainmentOptionName | Name der Option für die Kompetenzerreichung | 
| Month | Monat, für den die Metriken gemeldet werden | 
| MetricName | Name der Metrik, die für die Kompetenz relevant ist | 
| MetricMonthlyContribution | Monatlicher Beitrag der Metrik | 
| TTMAggregate | Aggregierte Metrik für die folgenden 12 Monate | 
| AnniversaryYearAggregate | Aggregierte Metrik für das aktuelle Jahrestag | 
| GoldThreshold | Leistungsanforderung zur Erfüllung der Gold-Kompetenz | 
| SilverThreshold | Leistungsanforderung zur Erfüllung der Silver-Kompetenz | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent – Microsoft 365 Propensity-Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Bezeichnernummer des Kunden | 
| DUNS-Nummer | Die Dun & Brad sinus (D&B) des Kunden, der aufgrund der Neigung bewertet wird | 
| Account Name | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche, zu der die Organisation gehört | 
| Vertical | Die Vertikale des Kunden, der für die Neigung bewertet wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert. | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, dessen Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, dessen Neigung bewertet wird | 
| City | Geografischer Ort der Organisation | 
| State | Geografischer Standort der Organisation | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Standort der Organisation | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Markt" | 
| SMC-Typzusammenfassung | SMC-Typ | 
| Top Unmanaged – Compute-Basis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Nicht verwaltet – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob es sich bei der Organisation um eine gemeinnützige Organisation handelt (Ja oder Nein). | 
| Aktivieren von Remotearbeit – Exchange Online-Ziel | Kunden, die über ein aktives Exchange Online-Abonnement verfügen, werden an Microsoft 365 | 
| Aktivieren von Remotearbeit – lokale Übernahme (aktuelle Version) mit Cloud Ascent-Propensität – +10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt. Das heißt, die Clientversion ist höher als eine EOL-Version (End of Life). Der Kunde verfügt über 10 oder mehr Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Aktivieren von RemoteArbeit – lokale Übernahme (aktuelle Version) mit Cloud Ascent-Propensity – <10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine Version höher als EOL). Der Kunde verfügt über weniger als 10 Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Remotearbeit aktivieren – lokale Übernahme (aktuelle Version) ohne Cloud Ascent-Neigung – +10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine Version höher als EOL). Der Kunde verfügt über 10 oder mehr Lizenzen. Der Kunde hat keine Voraussetzungsbewertung. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (aktuelle Version) ohne Cloud Ascent-Propensität – <10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat keine Voraussetzungsbewertung. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (EOL-Version) mit Cloud Ascent-Vorteilen – +10 Lizenzen | Kunde, der über einen lokalen EOL-Office- oder Windows-Client verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über 10 oder mehr Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (EOL-Version) mit Cloud Ascent-Propensität – <10 Lizenzen | Kunde, der über einen lokalen EOL-Office- oder Windows-Client verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (EOL-Version) ohne Cloud Ascent-Propensität – +10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über 10 oder mehr Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Aktivieren von RemoteArbeit – lokale Übernahme (EOL-Version) ohne Cloud Ascent-Propensity – <10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Aktivieren von Remotearbeit – Hohe Propensity-Perspektive für Microsoft 365 (Act NowithEvaluate) | Kunden mit hoher Kundenzufriedenheit für Microsoft 365 | 
| Aktivieren von Remotearbeit – Wettbewerb (Zoom) mit Microsoft 365 | Kunde mit Zoom und Microsoft 365 für die Konvertierung in Teams | 
| Aktivieren von Remotearbeit – Wettbewerb (Zoom) ohne Microsoft 365 | Kunde mit Zoom, Ziel für die Konvertierung in Teams | 
| Reduzieren von Kosten und Verwalten– Microsoft 365 E3 für Microsoft 365 E5 | Vorhandener Kunde mit Microsoft 365 E3, Ziel für Microsoft 365 E5 | 
| Reduzieren von Kosten und Verwalten: Microsoft 365 Business Basic- und Business Standard-Kunden für Microsoft 365 Business Premium | Vorhandene Microsoft 365 Business Basic- und Business Standard-Kunden für Microsoft 365 Business Premium | 
| Transform Organizational Productivity - Surface Propensity | Kunde zeigt eine Neigung für Surface an | 
| M365Cluster | Identifiziert die Bereitschaft eines Kunden, Microsoft 365 zu erwerben. Target Act Now und Evaluate clusters because they will will produce higher yield. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn nach Act Now und Evaluate-Kunden noch Kapazität vorhanden ist. | 
| M365Fit | Interne und externe Datenpunkte, die Firmografien definieren. Bei der Bewertung von Anpassungen wird ein lookalike-Modell für unsere besten kleinen oder mittelgroßen Unternehmen (SMBs) verwendet, um Kunden zu vergleichen und zu sehen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| M365Intent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird bei Anpassen überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| SurfaceCluster | Identifiziert die Bereitschaft eines Kunden, Surface zu erwerben, indem die Empfehlungen für Anpassung und Absicht in einem Cluster konsolidiert werden. Target Act Now und Evaluate clusters because they will will produce higher yield. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn nach Act Now und Evaluate-Kunden noch Kapazität vorhanden ist. | 
| SurfaceFit | Interne und externe Datenpunkte, die Firmografien definieren. Bei der Bewertung von Anpassungen wird ein lookalike-Modell für unsere besten SMBs verwendet, um Kunden zu vergleichen und zu prüfen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| SurfaceIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| O365Cluster | Gibt die Neigung des Kunden an, Office 365 zu erwerben. Target Act Now und Evaluate clusters because they'll produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Zielkunden nur dann zu pflegen und zu schulen, wenn nach "Jetzt handeln" und "Auswerten" noch Kapazität zur Verfügung steht. | 
| O365Fit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Anpassungsbewertung wird ein lookalike-Modell für unsere besten SMBs verwendet, um Kunden zu vergleichen und zu prüfen, ob sie sich für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| O365Intent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| M365UpsellCustomer | Gibt an, ob der Kunde upsell propensity for Microsoft 365 | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von Google-Produkten zeigt. | 
| Verfügt über AWS | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von AWS-Produkten (Amazon Web Services) anzeigt. | 
| Verfügt über EA | Gibt an, ob eine Verlängerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob eine Verlängerung eine Open- oder Open Value-Vereinbarung ist. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent – Dynamics 365-Propensity-Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Kundenbezeichnernummer | 
| DUNS-Nummer | Die Dun-& Brad number des Kunden, der aufgrund der Neigung bewertet wird. | 
| Account Name | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche, zu der die Organisation gehört | 
| Vertical | Die Vertikale des Kunden, der für die Neigung bewertet wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert.
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, dessen Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, dessen Neigung bewertet wird | 
| City | Geografischer Ort | 
| State | Standort des geografischen Bundesstaats | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Landstandort | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Market" | 
| Zusammenfassung des SMC-Typs | Die Kategorisierung eines Kunden: Die obersten nicht verwalteten Benutzerbasen sind Kunden mit mehr als 300 Mitarbeitern, die meisten nicht verwalteten Computebasen sind Kunden mit 10.000 US-Dollar im Azure-Drei-Jahres-Potenzial, mittlere Unternehmen sind Kunden mit mehr als 25 Mitarbeitern und kleine Unternehmen kunden mit weniger als 25 Mitarbeitern. | 
| Top Nicht verwaltet – Computebasis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Nicht verwaltet – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob es sich bei der Organisation um eine gemeinnützige Organisation handelt (Ja oder Nein). | 
| Aktivieren von Digital Selling – Microsoft 365 – Größe >= 25 Plätzen (SalesPro-Propensity-Modell) | Kunde ohne Dynamics 365. Größe des Platzes: 25+. Partner sollten für cross-sell von Dynamics 365 SalesPro als Ziel verwendet werden. | 
| Aktivieren von Digital Selling – Dynamics 365 SalesPro propensity (Jetzt handeln oder auswerten) | Kunden mit hoher Geschwindigkeit ohne Dynamics 365. Partner sollte dynamics 365 SalesPro als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base – Navision (Business Central propensity model) (Verwalten von Finanzrisiken &– Lokale Dynamics-Installationsbasis – Navision (Business Central-Propensity-Modell) | Bestehender Kunde mit lokalem Navision. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base – Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Bestehender Kunde mit einer lokalen AX. Partner sollten dynamics 365 Finance + Operations als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base – Great Plains (Business Central propensity model) (Verwalten von Finanzrisiko- und Betrugsversuchen – Lokale Dynamics-Installationsbasis – Great Plains (Business Central-Propensity-Modell)) | Bestehender Kunde mit lokalen Great Plains. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base ( Managing Financial Risk & Fraud – Dynamics on-premises install base – Soll (Business Central Propensity Model) | Bestehender Kunde mit lokalem System. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Verwalten von finanzrisiken & Betrugsversuchen – Lokale Dynamics-Installationsbasis – Andere (Business Central-Propensity-Modell) | Bestehender Kunde mit anderen lokalen Lösungen, die zuvor nicht aufgeführt wurden. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Erstellen von agilen Geschäftsprozessen – Dynamics lokal – Installationsbasis – AX/GP/SL/NAV/Other (Dynamics 365-Propensity-Modell) | Erstellen von agilen Geschäftsprozessen – Dynamics lokal – Installationsbasis – AX/GP/SL/NAV/Other (Dynamics 365-Propensity-Modell) | 
| Erstellen von agilen Geschäftsprozessen – Dynamics-Basis – Mendix/OutSystems/Salesforce (Dynamics 365-Propensity-Modell) | Erstellen agiler Geschäftsprozesse – Dynamics-Konkurrenzbasis – Mendix/OutSystems/Salesforce (Dynamics 365-Propensity-Modell) | 
| Erstellen von agilen Geschäftsprozessen– Dynamics 365 Finance + Operations-Installationsbasis | Vorhandene Dynamics 365 Finance + Operations-Kunden. Partner für Power Apps. | 
| Erstellen von agilen Geschäftsprozessen – Dynamics 365 Business Central-Installationsbasis | Vorhandene Dynamics 365 Business Central-Kunden. Partner für Power Apps. | 
| Erstellen von agilen Geschäftsprozessen– Dynamics 365 Customer Engagement-Installationsbasis | Vorhandene Dynamics 365 Customer Engagement-Kunden. Partner für Power Apps. | 
| Erstellen einer robusten Lieferkette – Windows und Aktivieren der ersten Dynamics 365-Workload als Dynamics 365 Supply Chain Management mit Kunden, die keine Oracle- oder SAP ERP-Kunden (Enterprise Resource Planning) sind | Zielkunden für Dynamics 365 Supply Chain Management | 
| Erstellen einer robusten Lieferkette– Cross-Sell Dynamics 365 Supply Chain Management und/oder Retail oder Commerce an vorhandene Dynamics 365 Customer Engagement-Kunden | Vorhandene Dynamics 365 Customer Engagement-Kunden, die für cross-selling Dynamics 365 Supply Chain Management entwickelt werden. | 
| Erstellen einer robusten Lieferkette: Cross-Sell Dynamics 365 Supply Chain Management und/oder Retail oder Commerce an Dynamics 365 Customer Engagement und Oracle oder SAP | Vorhandene Dynamics 365 Customer Engagement-Kunden mit Oracle oder SAP als Ziel für Dynamics 365 Supply Chain Management | 
| D365BCCluster | Gibt die Kundenneigenz zum Kauf von Dynamics 365 Business Central an. Kunden, die eine Neigung für Business Central zeigen, werden in die Kategorien Mittel und Klein fallen. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie act Now- und Evaluate-Kunden als Ziel haben. | 
| D365BCFit | Interne und externe Datenpunkte, die Firmografien definieren. Bei der Bewertung von Anpassungen wird ein lookalike-Modell für unseren besten SMB verwendet, um Kunden zu vergleichen und zu prüfen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| D365BCIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird bei Anpassen überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| D365FOCluster | Identifiziert die Bereitschaft des Kunden, Dynamics 365 Finance and Operations zu erwerben. Kunden, die eine Neigung für Finance + Operations zeigen, werden in den obersten nicht verwalteten Kategorien angezeigt. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie act Now- und Evaluate-Kunden als Ziel haben. | 
| D365FOFit | Interne und externe Datenpunkte, die Firmografien definieren. Bei der Bewertung von Anpassungen wird ein lookalike-Modell für unseren besten SMB verwendet, um Kunden zu vergleichen und zu prüfen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| D365FOIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| D365CECluster | Gibt die Neigung des Kunden an, Dynamics 365 Customer Engagement zu erwerben. Kunden, die eine Kundenbindung zeigen, werden in die Kategorien Mittel und Klein fallen. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| D365CEFit | Gibt "Fit for Dynamics 365 Customer Engagement" an | 
| D365CEIntent | Gibt die Absicht für Dynamics 365 Customer Engagement an. | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Verlängerung für dynamics on-premises AX oder CRM verfügt. | 
| M365UpsellCustomer | Gibt an, ob der Kunde upsell propensity for Microsoft 365 | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von Google-Produkten zeigt. | 
| Verfügt über AWS | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von AWS-Produkten zeigt. | 
| Verfügt über EA | Gibt an, ob es sich bei einer Verlängerung um ein EA- oder EA-Abonnement handelt. | 
| Hat geöffnet | Gibt an, ob eine Verlängerung eine Open- oder Open Value-Vereinbarung ist. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – Azure-Propensity-Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Kundenbezeichnernummer | 
| DUNS-Nummer | Die Dun-& Brad number des Kunden, der aufgrund der Neigung bewertet wird. | 
| Account Name | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche | 
| Vertical | Die Vertikale des Kunden, der für die Neigung bewertet wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert. | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, dessen Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, dessen Neigung bewertet wird | 
| City | Geografischer Ort | 
| State | Geografischer Zustandsstandort | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Landstandort | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Market" | 
| Zusammenfassung des SMC-Typs | SMC-Typ | 
| Top Nicht verwaltet – Computebasis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Nicht verwaltet – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob es sich bei der Organisation um eine gemeinnützige Organisation handelt (Ja oder Nein). | 
| Migrieren – EOL Windows Server – EOL Windows Server IB mit Cloud Ascent-Neigung – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über 5 oder mehr Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL Windows Server – EOL Windows Server IB mit Cloud Ascent-Propensity – <5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über weniger als 5 Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL Windows Server – EOL Windows Server IB ohne Cloud Ascent Propensity – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat keine Voraussetzungsbewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL Windows Server – EOL Windows Server IB ohne Cloud Ascent Propensity – <5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder früher). Verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Voraussetzungsbewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL SQL – EOL SQL Server IB mit Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL SQL – EOL SQL Server IB mit Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Verfügt über weniger als 5 Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL SQL – EOL SQL Server IB ohne Cloud Ascent-Neigung – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server (d. h. eine EOL-Version oder früher) verfügt. Der Kunde verfügt über 5 oder mehr Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL SQL – EOL SQL Server IB ohne Cloud Ascent-Neigung – <5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server (d. h. eine EOL-Version oder früher) verfügt. Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – Migrieren einer lokalen Windows Server-Umgebung – aktuelle Windows Server IB mit Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Version (d. h. eine neuere Version als EOL) verfügt. Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat eine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – Migrieren einer lokalen Windows Server-Umgebung – aktuelle Windows Server IB mit Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Version (d. h. eine neuere Version als EOL) verfügt. Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung für Azure. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren von lokalem Windows Server – aktuelle Windows Server IB ohne Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über einen aktuellen lokalen Windows Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat keine Voraussetzungsbewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren von lokalem Windows Server – aktuelle Windows Server IB ohne Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über einen aktuellen lokalen Windows Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Voraussetzungsbewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren zu Azure SQL oder virtuellen SQL-Computern (VMs) – aktuelle SQL Server IB mit Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren zu Azure SQL- oder SQL-VMs – aktuelle SQL Server IB mit Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat eine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren: Migrieren zu Azure SQL oder SQL-VMs – current SQL Server IB ohne Cloud Ascent-Neigung – mehr als 5 Lizenzen | Kunde, der über ein aktuelles lokales SQL Server (d. h. eine Version nach EOL) verfügt. Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren: Migrieren zu Azure SQL- oder SQL-VMs – aktuelle SQL Server IB ohne Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über ein aktuelles lokales SQL Server (d. h. eine Version nach EOL) verfügt. Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – OSS – Migrieren zu Open Source-Datenbank (OSS) | Bestehender Kunde mit einem der folgenden Produkte konkurriert: PostgreSQL, MySQL, MariaDB. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – OSS – Linux in Azure | Bestehender Kunde mit Linux. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – SAP – SAP in Azure | Bestehender Kunde mit SAP. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Windows Virtual Desktop – Remotedesktopdienste IB | Identifiziert Kunden mit aktiven Windows-Remotedesktopdienste. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Windows Virtual Desktop – Cross Sell Modern Work zu Azure/WVD | Identifiziert Kunden mit Microsoft 365 und besitzt azure nicht. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – VMware IB | Bestehender Kunde mit dem Produkt: VMware. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Citrix IB | Bestehender Kunde mit dem Produkt: Citrix Systems. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Innovation – Analyse – Power BI IB mit hoher Azure-Beliebtheit | Kunden mit und Active Power BI-Abonnement, einschließlich: Power BI – Eigenständiges Pro, Power BI – Azure-Suiten, Power BI – Office-Suiten, Power BI Sammlungen – Microsoft 365 | 
| Aktivieren – DevOps mit GitHub – Visual Studio/MSDN IB | Identifiziert Kunden mit aktiven Visual Studio Versionen | 
| Windows Server Standard-Version | Zeigt die Version von Windows Server Standard-Käufen durch den Kunden an. | 
| Windows Server Standard-Lizenz | Zeigt den Lizenztyp von Windows Server Standard-Käufen durch den Kunden an. | 
| Windows Server Data Center-Version | Zeigt die Version der Käufe des Windows-Rechenzentrums durch den Kunden an. | 
| Windows Server Data Center-Lizenz | Zeigt den Lizenztyp von Windows Data Center-Käufen durch den Kunden an. | 
| AzureFit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Anpassungsbewertung wird ein lookalike-Modell für unser bestes SMB verwendet, um Kunden zu vergleichen und festzustellen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| AzureIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| AzureCluster | Identifiziert die Kaufneigung des Kunden für Azure, indem die Empfehlungen "Anpassung" und "Absicht" in einem Cluster konsolidiert werden. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| WindowsServerDataCenter_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Verlängerung für Windows Server Datacenter verfügt. | 
| WindowsServerStandard_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Verlängerung für Windows Server Standard verfügt. | 
| AzureUpsellCustomer | Identifiziert, ob der Kunde Upsell-Propensität für Azure anzeigt. | 
| Hat Google | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von Google-Produkten anzeigt. | 
| Verfügt über AWS | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von AWS-Produkten anzeigt. | 
| Verfügt über EA | Gibt an, ob es sich bei einer Verlängerung um ein EA- oder EA-Abonnement handelt. | 
| Hat geöffnet | Gibt an, ob eine Verlängerung eine Open- oder Open Value-Vereinbarung ist. | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent – Bericht zur Vertragsverlängerungsbereitschaft**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Kundenbezeichnernummer | 
| DUNS-Nummer | Die Dun-& Brad number des Kunden, der aufgrund der Neigung bewertet wird. | 
| Account Name | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche | 
| Vertical | Die Vertikale des Kunden, der für die Propensität ermittelt wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert. | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, für den die Bewertung für die Kundenneidigkeit erzielt wird. | 
| Sales Territory | Das Vertriebsgebiet des Kunden, für den die Bewertung für die Propensity erzielt wird. | 
| City | Geografischer Ort | 
| State | Standort des geografischen Bundesstaats | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Landstandort | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Market" | 
| Zusammenfassung des SMC-Typs | SMC-Typ | 
| Top Nicht verwaltet – Computebasis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Nicht verwaltet – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob es sich bei der Organisation um eine gemeinnützige Organisation handelt (Ja oder Nein). | 
| Hat Google | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von AWS-Produkten anzeigt. | 
| Verfügt über AWS | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von AWS-Produkten anzeigt. | 
| Azure-Cluster | Identifiziert die Kaufneigung des Kunden für Azure. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie act Now- und Evaluate-Kunden als Ziel haben. | 
| D365 Finance + Operations-Cluster | Identifiziert die Bereitschaft des Kunden, Dynamics 365 Finance and Operations zu erwerben. Kunden, die eine Neigung für Finance + Operations zeigen, werden in den obersten nicht verwalteten Kategorien angezeigt. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie act Now- und Evaluate-Kunden als Ziel haben. | 
| D365 CE-Cluster | Identifiziert die Bereitschaft des Kunden, Dynamics 365 Customer Engagement zu erwerben. Kunden, die eine Neigung für Customer Engagement zeigen, werden in den Kategorien Mittel und Klein angezeigt. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie act Now- und Evaluate-Kunden als Ziel haben. | 
| D365 BC-Cluster | Identifiziert die Bereitschaft des Kunden, Dynamics 365 Business Central zu erwerben. Kunden, die eine Neigung für Business Central zeigen, werden in den Kategorien Mittel und Klein angezeigt. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| Microsoft 365 Cluster | Identifiziert die Kaufneigenz des Kunden Microsoft 365. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| Lizenzprogramm | Identifiziert den Lizenzprogrammtyp für die Verlängerung. | 
| Vereinbarungs-ID | Bezeichner der Vereinbarung | 
| Enddatum der Vereinbarung | Enddatum der Vereinbarung | 
| Ablauftyp | Ablauftyp | 
| Läuft der Umsatz ab | Umsatz im Zusammenhang mit ablösenden Abonnements | 
| Verfügt über EA | Gibt an, ob eine Verlängerung ein EA- oder ein EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob es sich bei einer Verlängerung um eine Open- oder Open Value-Vereinbarung handelt. | 
| Azure Upsell-Kunde | Gibt an, ob der Kunde upsell-Propensity für Azure zeigt. | 
| Microsoft 365 Upsell-Kunde | Gibt an, ob der Kunde Upsell-Propensität für Microsoft 365 | 
| RevSumDivisionName | Identifiziert das Produkt, das erneuert werden soll. | 

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen finden Sie unter [Herunterladen von Berichten.](pci-download-reports.md)
