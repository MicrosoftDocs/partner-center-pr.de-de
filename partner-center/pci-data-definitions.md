---
title: Insights-Datendefinitionen
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Das Dokument listet verschiedene Berichte und deren Datendefinitionen auf, die Sie von der Berichtsseite Insights-Download herunterladen können.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 721caed2d8b0e24940e7adedeb90cc689a82d2e7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152833"
---
# <a name="export--data-definitions"></a>Export – Datendefinitionen 

**Geeignete Rollen:** Berichts-Viewer| Executive Report Viewer

## <a name="introduction"></a>Einführung 

Mithilfe des Hubs Berichte herunterladen auf dem Insights-Dashboard können Sie die rohen Datasets exportieren. 

Die verschiedenen Berichte, die Sie zusammen mit ihren Datendefinitionen herunterladen können, sind in den folgenden Tabellen aufgeführt: 

### <a name="partner-profile-report"></a>**Partnerprofilbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPNId | Bezeichner Microsoft Partner Network (MPN) | 
| PartnerName | Name des Partners | 
| PGA_MPNId | Bezeichner des MPN des globalen Partnerkontos | 
| PGA_PartnerName | Globaler Partnerkontoname | 
| City | Ort des Partners | 
| Land | Länderstandort des Partners | 
| HierarchyLevel | Gibt an, ob es sich um eine globale MPN-ID oder eine MPN-Standort-ID | 

### <a name="customer-details-report"></a>**Bericht "Kundendetails"**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | Bezeichner des Kunden mandanten | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| CustomerSegment | Kundensegment | 
| CustomerMarket | Geografischer Markt des Kunden | 
| CustomerStatus | Kundenstatus (Aktiv oder Inaktiv) | 
| Produkt | Das Produkt, das per MPN an den Kunden verkauft wurde: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI oder Microsoft Azure | 
| SKU | Produkt-SKU | 
| Month | Monat, für den Nutzung und Umsatz gemeldet werden | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp des Partners | 
| SalesChannel | Vertriebskanal | 
| AvailableSeats | Verfügbare Arbeitsplätze | 
| RevenueUSD | Umsatz in US-Dollar | 

### <a name="reseller-performance-report"></a>**Leistungsbericht des Wiederverkäufers**

> [!Note]
> Umsatz- und ACR-Daten sind nur für Benutzer verfügbar, die Berichts-Viewer von Führungskräften sind.

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| ResellerMPNid | Reseller Microsoft Partner Network-ID | 
| ResellerName | Name des Handelspartners | 
| ResellerMarket | Handelspartnerland des Markts | 
| IndirectProviderMPNId | Bezeichner des indirekten Anbieters Microsoft Partner Network | 
| IndirectProviderName | Name des indirekten Anbieters | 
| Month | Monat, für den Nutzung und Umsatz gemeldet werden | 
| Produkt | Produktname | 
| SubscriptionID | Bezeichner des Abonnements | 
| AvailableSeats | Anzahl verfügbarer Stellen | 
| AssignedSeats | Anzahl zugewiesener Mitarbeiter | 
| BilledRevenueUSD | Abgerechneter Umsatz in US-Dollar | 
| CustomerName | Name des Kunden | 
| CustomerTPid | Bezeichner des obersten übergeordneten Kunden | 
| CustomerSegment | Kundensegment | 
| CustomerMarket | Geografischer Markt des Kunden | 
| ResellerStatus | Reseller-Status | 

### <a name="subscription-details-report"></a>**Bericht zu Abonnementdetails**

>[!Note]
>Umsatz- und ACR-Daten sind nur für Benutzer verfügbar, die Berichts-Viewer der Geschäftsleitung sind.

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Startdatum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionState | Status des Abonnements (Aktiv oder Abwanderung) | 
| Month | Monat, für den Nutzung und Umsatz gemeldet werden | 
| IsAutoRenew | Gibt an, ob das Abonnement neu ist (Ja oder Nein). | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden | 
| CustomerTpid | Oberster übergeordneter Bezeichner des Kunden | 
| CustomerSegment | Segment des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| Produkt | Produkt, das vom Partner an den Kunden verkauft wird | 
| SKU | SKU des Produkts | 
| MPNId | Microsoft Partner Network-ID des Partners | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp für das Abonnement | 
| SalesChannel | Vertriebskanal: Direkt, CSP (Cloud Solution Provider) und so weiter | 
| AvailableSeats | Aktuell verfügbarer Platz | 
| RevenueUSD | Umsatz in US-Dollar | 
| Registrierungs-ID | Registrierungs-ID des Abonnements | 

### <a name="azure-usage-report"></a>**Azure-Nutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Das Datum des Startdatums des Abonnements | 
| SubscriptionEndDate | Das Datum des Endes des Abonnements | 
| SubscriptionState | Aktueller Status des Abonnements (Offen, Geschlossen, Aktiv oder In Karenzzeit) | 
| Month | Nach Monat aggregiertes Datum | 
| Dienstname | Name des Azure-Diensts | 
| MeterCategory | Name der Verbrauchszählerkategorie | 
| UsageUnits | Die Anzahl der Einheiten, die während des Abrechnungszyklus verwendet werden | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Oberste übergeordnete Kunden-ID | 
| CustomerSegment | Segment des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| MPNId | Microsoft Partner Network-ID des Kunden | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttributionType | Zuordnungstyp des Partners | 
| SalesChannel | Vertriebskanal (Direct/CSP, Indirect/CSP, Direct, so weiter) | 
| ACR_USD | Azure Consumed Revenue (ACR) in US-Dollar | 
| Registrierungs-ID | Registrierungs-ID des Azure-Abonnements | 

### <a name="office-365-license-usage-report"></a>**Office 365-Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Übergeordnete ID des Kunden | 
| WorkloadName | Skype for Business, Teams, Exchange Online | 
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

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility-Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Oberste übergeordnete Kunden-ID | 
| WorkloadName | Name der EMS-Workload (Enterprise Mobility + Security) | 
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

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365-Lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Startdatum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionStatus | Status des Abonnements | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| RevSumDivisionName | Name der Rev-Summendivision | 
| RevSumCategoryName | Name der Rev-Summenkategorie | 
| SKU | SKU des Produkts | 
| SKUId | SKU-ID des Produkts | 
| FreeVsPaidSKU | Gibt an, ob es sich um eine kostenlose oder kostenpflichtige SKU | 
| SalesModel | Vertriebskanal, der zum Verkaufen des Abonnements verwendet wird | 
| DetailedSalesModel | Detailliertes Vertriebsmodell für das Abonnement | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kundenmandanten | 
| CustomerTpid | Oberster übergeordneter Bezeichner des Kunden | 
| CustomerSegment | Segment "Market" des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttachType | Zuordnungstyp für das Abonnement | 
| AvailableSeats | Aktuell verfügbarer Platz | 
| AssignedSeats | Aktuell zugewiesener Platz | 
| ActiveSeats | Aktuell aktive Plätzen | 
| DeploymentOpportunity | Aktuelle Bereitstellungschance | 
| ActiveUsagePercent | Prozentsatz der aktuellen aktiven Nutzung | 

### <a name="power-bi-license-usage-report"></a>**Power BI lizenznutzungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Startdatum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionStatus | Status des Abonnements (Aktiv, Inaktiv oder In Toleranzperiode) | 
| Month | Nach Monat aggregiertes Datum | 
| SKU | SKU des Produkts | 
| SKUId | SKU-ID des Produkts | 
| FreeVsPaidSKU | Differenziator für kostenlose oder kostenpflichtige SKU | 
| SalesModel | Vertriebsmodell, das zum Verkaufen des Abonnements verwendet wird | 
| DetailedSalesModel | Detailliertes Vertriebsmodell für das Abonnement | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kundenmandanten | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| CustomerSegment | Segment "Market" des Kunden | 
| CustomerMarket | Geografischer Markt des Kunden | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| PartnerLocation | Geografischer Standort des Partners | 
| PartnerAttachType | Zuordnungstyp für das Abonnement | 
| AvailableSeats | Aktuell verfügbare Stellen | 
| AssignedSeats | Aktuell zugewiesene Plätzen | 
| ActiveSeats | Aktuell aktive Plätzen | 
| DeploymentOpportunity | Aktuelle Bereitstellungschance | 
| ActiveUsagePercent | Prozentsatz der aktuellen aktiven Nutzung | 

### <a name="teams-meetings-and-calls-report"></a>**Bericht zu Teams-Besprechungen und -Aufrufen**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| Unterworkload | Unterauslastung, für die Nutzung gemeldet wird (Besprechungen, Anrufe oder Telefonsysteme) | 
| Anzahl der Besprechungen | Anzahl von Besprechungen | 
| Besprechungsdauer | Gesamtbesprechungsdauer in Stunden | 

### <a name="teams-monthly-usage-report"></a>**Bericht zur monatlichen Nutzung von Teams**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Bezeichner des obersten übergeordneten Kunden | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| Subworkload | Unterarbeitslast, für die die Nutzung gemeldet wird (Besprechungen, Anrufe oder Telefonsysteme) | 
| Desktopbenutzer | Anzahl der Benutzer, die Teams auf dem Desktop verwenden | 
| Mobile Benutzer | Anzahl der Benutzer, die Teams auf mobilgeräten verwenden | 
| Webbenutzer | Anzahl der Benutzer, die Teams im Web verwenden | 
| AllUpParticipants | Anzahl eindeutiger Benutzer von Teams für den Monat | 

### <a name="teams-usage-3p-apps-report"></a>**Bericht zu 3P-Apps für die Teams-Nutzung**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| CustomerTpid | Oberste übergeordnete Kunden-ID | 
| Month | Monat, für den die Nutzung gemeldet wird | 
| 3P-App-Name | Name der Teams-App | 
| Benutzeranzahl | Anzahl der Benutzer für die App | 


### <a name="training-details-report"></a>**Training details report (Trainingdetailsbericht)**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| TrainingActivityId | Bezeichner des Trainings | 
| TrainingTitle | Titel des Trainings | 
| TrainingType | Art der Schulung (Zertifizierung oder Prüfung) | 
| IndividualFirstName | Vorname des Kunden | 
| IndividualLastName | Nachname des Kunden | 
| E-Mail | Persönliche E-Mail-ID des Kunden | 
| CorpEmail | Office-E-Mail-ID des Kunden | 
| TrainingCompletionDate | Abschlussdatum des Trainings | 
| Month | Monat, für den die Daten gemeldet werden | 
| IcMCP | Gibt an, ob der Benutzer ein Microsoft Certified Professional (MCP) ist. | 
| MCPID | MCP-ID des Benutzers | 
| MPNId | Bezeichner der Microsoft Partner Network | 
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
| Produkte | Produkt, für das das Lernmodul gilt | 
| Rollen | Anwendbare Rollen des Trainings | 
| CompletionDate | Datum des Abschlusses des Trainings | 
| MPNId | Bezeichner Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Land | Geografischer Standort des Partners | 

### <a name="competency-summary-and-history-report"></a>**Kompetenzzusammenfassung und Verlaufsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CompetencyName | Name der Kompetenz | 
| CompetencyLevel | Ebene der Kompetenz (Gold oder Silber) | 
| CompetencyStatus | Aktueller Status der Kompetenz (Aktiv, Inaktiv oder In Toleranzperiode) | 
| CompetencyStartDate | Startdatum der Kompetenz | 
| CompetencyEndDate | Enddatum der Kompetenz | 

### <a name="competency-performance-report"></a>**Bericht zur Kompetenzleistung**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CompetencyName | Name der Kompetenz | 
| CompetencyAttainmentOptionName | Name der Kompetenzoption | 
| Month | Monat, für den die Metriken gemeldet werden | 
| MetricName | Name der Metrik, die für die Kompetenz relevant ist | 
| MetricMonthlyContribution | Monatlicher Beitrag der Metrik | 
| TTMAggregate | Aggregierte Metrik für die nachgestellten 12 Monate | 
| AnniversaryYearAggregate | Aggregierte Metrik für das aktuelle Jahrestag | 
| GoldThreshold | Leistungsanforderung zur Erfüllung der Gold-Kompetenz | 
| SilverThreshold | Leistungsanforderung zur Erfüllung der Silver-Kompetenz | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent - Microsoft 365 Propensity report (Bericht zur Cloud-Ascent-Microsoft 365-Neigung)**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Bezeichnernummer des Kunden | 
| DUNS-Nummer | Die Dun & Bradune -Nummer (D&B) des Kunden, der aufgrund der Neigung bewertet wird | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche, zu der die Organisation gehört | 
| Vertical | Die Vertikale des Kunden, der für die Neigungsbewertung ermittelt wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert. | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, für den die Bewertung für die Neigung erzielt wird. | 
| Sales Territory | Das Vertriebsgebiet des Kunden, für den die Bewertung für die Propensity erzielt wird. | 
| City | Geografischer Ort der Organisation | 
| State | Geografischer Standort der Organisation | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Standort des Landes der Organisation | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Market" | 
| Zusammenfassung des SMC-Typs | SMC-Typ | 
| Top Nicht verwaltet – Computebasis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Nicht verwaltet – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob die Organisation nicht gewinnorientiert ist (Ja oder Nein). | 
| Aktivieren von Remotearbeit – Exchange Online als Ziel | Kunden, die über ein aktives Exchange Online-Abonnement verfügen, verkaufen Microsoft 365 | 
| Aktivieren von Remotearbeit – lokaler Erwerb (aktuelle Version) mit Cloud Ascent-Vorteilen – +10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt. Das heißt, die Clientversion liegt später als eine EOL-Version (End of Life). Der Kunde verfügt über 10 oder mehr Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (aktuelle Version) mit Cloud Ascent-Propensität – <10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 10 Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (aktuelle Version) ohne Cloud Ascent-Propensität – +10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über 10 oder mehr Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Aktivieren von Remotearbeit – lokale Übernahme (aktuelle Version) ohne Cloud Ascent-Propensität – <10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine Version höher als EOL). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Aktivieren von Remotearbeit – lokale Übernahme (EOL-Version) mit Cloud Ascent-Neigung – +10 Lizenzen | Kunde, der über einen lokalen Office- oder Windows-Client (d. h. eine EOL-Version oder früher) verfügt. Der Kunde verfügt über 10 oder mehr Lizenzen. Der Kunde hat eine Propensity-Bewertung. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Aktivieren von Remotearbeit – lokale Übernahme (EOL-Version) mit Cloud Ascent-Propensity – <10 Lizenzen | Kunde, der über einen lokalen Office- oder Windows-Client (d. h. eine EOL-Version oder früher) verfügt. Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat eine Propensity-Bewertung. Der Partner sollte auf die Konvertierung in Microsoft 365. | 
| Remotearbeit aktivieren – lokale Übernahme (EOL-Version) ohne Cloud Ascent-Propensität – +10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über 10 oder mehr Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – lokaler Erwerb (EOL-Version) ohne Cloud Ascent-Propensität – <10 Lizenzen | Kunde, der über einen aktuellen lokalen Office- oder Windows-Client verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte für die Konvertierung in Microsoft 365 vorgesehen sein. | 
| Aktivieren von Remotearbeit – Hochreibbarkeitsaussicht für Microsoft 365 (Act NowithEvaluate) | Kunden mit hoher Microsoft 365 | 
| Aktivieren von Remotearbeit – Konkurrieren (Zoom) mit Microsoft 365 | Kunde mit Zoom und Microsoft 365, Ziel für die Konvertierung in Teams | 
| Aktivieren von Remotearbeit – Wettbewerb (Zoom) ohne Microsoft 365 | Kunde mit Zoom, Ziel für die Konvertierung in Teams | 
| Reduzieren von Kosten und Verwaltung– Microsoft 365 E3 für Microsoft 365 E5 | Bestehender Kunde mit Microsoft 365 E3, Ziel für Microsoft 365 E5 | 
| Reduzieren von Kosten und Verwaltung – Microsoft 365 Business Basic- und Business Standard-Kunden, die für Microsoft 365 Business Premium vorgesehen sind | Bestehende Microsoft 365 Business Basic- und Business Standard-Kunden, Ziel für Microsoft 365 Business Premium | 
| Transformieren der Produktivität der Organisation – Oberflächenneigung | Kunde zeigt eine Neigung für Surface an | 
| M365Cluster | Identifiziert die Bereitschaft eines Kunden, Microsoft 365 zu erwerben. Target Act Now und Evaluate clusters because they'll produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Zielkunden nur dann zu pflegen und zu schulen, wenn nach "Jetzt handeln" und "Auswerten" noch Kapazität zur Verfügung steht. | 
| M365Fit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Anpassungsbewertung wird ein lookalike-Modell für unsere besten kleinen oder mittelgroßen Unternehmen (SMBs) verwendet, um Kunden zu vergleichen und festzustellen, ob sie sich für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| M365Intent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| SurfaceCluster | Identifiziert die Kaufneigung eines Kunden an Surface, indem die Empfehlungen "Fit" und "Intent" in einem Cluster konsolidiert werden. Target Act Now and Evaluate clusters because they'll produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Zielkunden nur dann zu schulen, wenn nach "Jetzt handeln" und "Auswerten" noch Kapazität zur Verfügung steht. | 
| SurfaceFit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Anpassungsbewertung wird ein lookalike-Modell für unsere besten SMBs verwendet, um Kunden zu vergleichen und zu prüfen, ob sie sich für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| SurfaceIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird bei Anpassen überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| O365Cluster | Identifiziert die Bereitschaft des Kunden, Office 365 zu erwerben. Target Act Now und Evaluate clusters because they will will produce higher yield. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn nach Act Now und Evaluate-Kunden noch Kapazität vorhanden ist. | 
| O365Fit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Bewertung von Anpassungen wird ein lookalike-Modell für unsere besten SMBs verwendet, um Kunden zu vergleichen und zu sehen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Anpassungsbewertung wird vierteljährlich aktualisiert. | 
| O365Intent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird bei Anpassen überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| M365UpsellCustomer | Gibt an, ob der Kunde Upsell-Propensität für Microsoft 365 | 
| Hat Google | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von Google-Produkten anzeigt. | 
| Verfügt über AWS | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von AWS-Produkten (Amazon Web Services) anzeigt. | 
| Verfügt über EA | Gibt an, ob eine Verlängerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob es sich bei einer Verlängerung um eine Open- oder Open Value-Vereinbarung handelt. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent – Dynamics 365-Propensity-Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Kunden-ID-Nummer | 
| DUNS-Nummer | Die Dun-& Braduma-Nummer des Kunden, für den eine Bewertung für die Neigung erzielt wird. | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche, zu der die Organisation gehört | 
| Vertical | Die Vertikale des Kunden, der für die Neigungsbewertung ermittelt wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert.
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, für den die Bewertung für die Kundenneidigkeit erzielt wird. | 
| Sales Territory | Das Vertriebsgebiet des Kunden, für den die Bewertung für die Propensity erzielt wird. | 
| City | Geografischer Ort | 
| State | Geografischer Zustandsstandort | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Standort des Landes | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Markt" | 
| SMC-Typzusammenfassung | Kategorisierung eines Kunden: Die wichtigsten nicht verwalteten Benutzerbasen sind Kunden mit mehr als 300 Mitarbeitern, die wichtigsten nicht verwalteten Computebasen sind Kunden mit einem Azure-Potenzial von 10.000 USD, mittlere Unternehmen sind Kunden mit 25 oder mehr Mitarbeitern, und kleine Unternehmen sind Kunden mit weniger als 25 Mitarbeitern. | 
| Top Unmanaged – Compute-Basis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Unmanaged – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob die Organisation nicht gewinnorientiert ist (Ja oder Nein). | 
| Aktivieren des digitalen Verkaufs – Microsoft 365 – Größe der Arbeitsplätze >= 25 Arbeitsplätze (SalesPro-Propensitätsmodell) | Kunde ohne Dynamics 365. Größe des Platzes: 25+. Der Partner sollte für den Cross-Selling von Dynamics 365 SalesPro vorgesehen sein. | 
| Aktivieren des digitalen Verkaufs – Dynamics 365 SalesPro-Propensität (Jetzt agieren oder auswerten) | Kunden mit hoher Beliebtheit ohne Dynamics 365. Partner sollte dynamics 365 SalesPro als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base – Navision (Business Central propensity model) (Verwalten von Finanzrisiko- und Betrugsversuchen – Lokale Dynamics-Installationsbasis – Navision (Business Central-Propensity-Modell)) | Bestehender Kunde mit lokalem Navision. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base – Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Bestehender Kunde mit lokalem AX. Partner sollten dynamics 365 Finance + Operations als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base – Great Plains (Business Central propensity model) (Verwalten von Finanzrisiko- und Betrugsversuchen – Lokale Dynamics-Installationsbasis – Great Plains (Business Central-Propensity-Modell)) | Bestehender Kunde mit lokalen Great Plains. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Managing Financial Risk & Fraud – Dynamics on-premises install base ( Managing Financial Risk & Fraud – Dynamics on-premises install base – Soll (Business Central Propensity Model) | Bestehender Kunde mit lokalem System. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Verwalten von & Betrugsversuchen – Lokale Dynamics-Installationsbasis – Andere (Business Central-Propensity-Modell) | Bestehender Kunde mit anderen lokalen Lösungen, die zuvor nicht aufgeführt wurden. Der Partner sollte dynamics 365 Business Central als Ziel haben. | 
| Erstellen von agilen Geschäftsprozessen – Dynamics lokal – Installationsbasis – AX/GP/SL/NAV/Other (Dynamics 365-Propensity-Modell) | Erstellen von agilen Geschäftsprozessen – Dynamics lokal – Installationsbasis – AX/GP/SL/NAV/Other (Dynamics 365-Propensity-Modell) | 
| Erstellen von agilen Geschäftsprozessen – Dynamics-Basis – Mendix/OutSystems/Salesforce (Dynamics 365-Propensity-Modell) | Erstellen agiler Geschäftsprozesse – Dynamics-Konkurrierungsbasis – Mendix/OutSystems/Salesforce (Dynamics 365-Propensity-Modell) | 
| Erstellen agiler Geschäftsprozesse – Dynamics 365 Finance + Operations-Installationsbasis | Bestehende Dynamics 365 Finance + Operations-Kunden. Partner für Power Apps. | 
| Erstellen agiler Geschäftsprozesse – Dynamics 365 Business Central-Installationsbasis | Bestehende Dynamics 365 Business Central-Kunden. Partner für Power Apps. | 
| Erstellen agiler Geschäftsprozesse – Dynamics 365 Customer Engagement-Installationsbasis | Vorhandene Dynamics 365 Customer Engagement-Kunden. Partner für Power Apps. | 
| Erstellen einer resilienten Lieferkette – Windows und Aktivieren der ersten Dynamics 365-Workload als Dynamics 365 Supply Chain Management mit Nicht-Oracle- oder SAP ERP-Kunden (Enterprise Resource Planning) | Zielgruppe für Dynamics 365 Supply Chain Management | 
| Erstellen einer robusten Lieferkette– Cross-Selling von Dynamics 365 Supply Chain Management und/oder Retail oder Commerce an vorhandene Dynamics 365 Customer Engagement-Kunden | Bestehende Dynamics 365 Customer Engagement-Kunden, die sich für cross-selling Dynamics 365 Supply Chain Management als Ziel orientierten. | 
| Erstellen einer robusten Lieferkette: Cross-Selling von Dynamics 365 Supply Chain Management und/oder Retail oder Commerce an Dynamics 365 Customer Engagement und Oracle oder SAP | Vorhandene Dynamics 365 Customer Engagement-Kunden mit Oracle oder SAP für Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identifiziert die Bereitschaft des Kunden, Dynamics 365 Business Central zu erwerben. Kunden, die eine Neigung für Business Central zeigen, werden in den Kategorien Mittel und Klein angezeigt. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie Act Now- und Evaluate-Kunden als Ziel haben. | 
| D365BCFit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Anpassungsbewertung wird ein lookalike-Modell für unser bestes SMB verwendet, um Kunden zu vergleichen und festzustellen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| D365BCIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| D365FOCluster | Gibt die Kundenneigenz an, Dynamics 365 Finance and Operations zu erwerben. Kunden, die eine Neigung für Finance + Operations zeigen, werden in den obersten nicht verwalteten Kategorien enthalten sein. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| D365FOFit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Anpassungsbewertung wird ein lookalike-Modell für unser bestes SMB verwendet, um Kunden zu vergleichen und festzustellen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Bewertung der Anpassung wird vierteljährlich aktualisiert. | 
| D365FOIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird auf "Fit" überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| D365CECluster | Identifiziert die Bereitschaft des Kunden, Dynamics 365 Customer Engagement zu erwerben. Kunden, die eine Neigung für Customer Engagement zeigen, werden in den Kategorien Mittel und Klein angezeigt. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie Act Now- und Evaluate-Kunden als Ziel haben. | 
| D365CEFit | Gibt "Fit for Dynamics 365 Customer Engagement" an | 
| D365CEIntent | Gibt die Absicht für Dynamics 365 Customer Engagement an | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Verlängerung für dynamics on-premises AX oder CRM verfügt. | 
| M365UpsellCustomer | Gibt an, ob der Kunde Upsell-Propensität für Microsoft 365 | 
| Hat Google | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von Google-Produkten anzeigt. | 
| Verfügt über AWS | Identifiziert, ob der Kunde Wettbewerbssignale für den Besitz von AWS-Produkten anzeigt. | 
| Verfügt über EA | Gibt an, ob es sich bei einer Verlängerung um ein EA- oder EA-Abonnement handelt. | 
| Hat geöffnet | Gibt an, ob es sich bei einer Verlängerung um eine Open- oder Open Value-Vereinbarung handelt. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – Azure-Propensity-Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Kunden-ID-Nummer | 
| DUNS-Nummer | Die Dun-& Braduma-Nummer des Kunden, für den eine Bewertung für die Neigung erzielt wird. | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche | 
| Vertical | Die Vertikale des Kunden, der für die Neigungsbewertung ermittelt wird, wie von Microsoft, D&B und anderen Branchenstandards identifiziert. | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Niederlassung des Kunden, für den die Bewertung für die Kundenneidigkeit erzielt wird. | 
| Sales Territory | Das Vertriebsgebiet des Kunden, für den die Bewertung für die Propensity erzielt wird. | 
| City | Geografischer Ort | 
| State | Standort des geografischen Bundesstaats | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Landstandort | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Markt" | 
| Zusammenfassung des SMC-Typs | SMC-Typ | 
| Top Unmanaged – Compute-Basis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Unmanaged – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob die Organisation nicht gewinnorientiert ist (Ja oder Nein). | 
| Migrieren – EOL Windows Server – EOL Windows Server IB mit Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über 5 oder mehr Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL Windows Server – EOL Windows Server IB mit Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über weniger als 5 Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL Windows Server – EOL Windows Server IB ohne Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL Windows Server – EOL Windows Server IB ohne Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine lokale EOL-Version von Windows Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL SQL – EOL SQL Server IB mit Cloud Ascent-Neigung – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server (d. h. eine EOL-Version oder früher) verfügt. Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat eine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – EOL SQL – EOL SQL Server IB mit Cloud Ascent-Propensity – <5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server (d. h. eine EOL-Version oder früher) verfügt. Verfügt über weniger als 5 Lizenzen. Kunde, der über eine Propensity-Bewertung verfügt. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL SQL – EOL SQL Server IB ohne Cloud Ascent Propensity – mehr als 5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über 5 oder mehr Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – EOL SQL – EOL SQL Server IB ohne Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder eine frühere Version). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren von lokalem Windows Server – aktuelle Windows Server IB mit Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über einen aktuellen lokalen Windows Server verfügt (d. h. eine höhere Version als EOL). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren von lokalem Windows Server – aktuelle Windows Server IB mit Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über einen aktuellen lokalen Windows Server verfügt (d. h. eine höhere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde verfügt über eine Propensity-Bewertung für Azure. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – Migrieren einer lokalen Windows Server-Umgebung – aktuelle Windows Server IB ohne Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Version (d. h. eine neuere Version als EOL) verfügt. Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – Migrieren einer lokalen Windows Server-Umgebung – aktuelle Windows Server IB ohne Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Version (d. h. eine neuere Version als EOL) verfügt. Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren: Migrieren zu Azure SQL virtuellen Computern oder virtuellen SQL-Computern (VMs) – aktuelle SQL Server IB mit Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über ein aktuelles lokales SQL Server (d. h. eine Version höher als EOL) verfügt. Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat eine Propensity-Bewertung. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren: Migrieren zu Azure SQL- oder SQL-VMs – current SQL Server IB mit Cloud Ascent-Propensity – <5 Lizenzen | Kunde, der über ein aktuelles lokales SQL Server (d. h. eine Version höher als EOL) verfügt. Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat eine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren zu Azure SQL- oder SQL-VMs – aktuelle SQL Server IB ohne Cloud Ascent-Propensität – mehr als 5 Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Migrieren zu Azure SQL- oder SQL-VMs – aktuelle SQL Server IB ohne Cloud Ascent-Propensität – <5 Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat keine Propensity-Bewertung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – OSS – Migrieren zur Open Source-Datenbank (OSS) | Bestehende Kunden mit einem der folgenden Produkte konkurrieren: PostgreSQL, MySQL, MariaDB. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – OSS – Linux in Azure | Bestehender Kunde mit Linux. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – SAP – SAP in Azure | Bestehender Kunde mit SAP. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren – Windows Virtual Desktop – Remotedesktopdienste IB | Identifiziert Kunden mit aktiven Windows-Remotedesktopdienste. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – Windows Virtual Desktop – Cross Sell Modern Work zu Azure/WVD | Identifiziert Kunden mit Microsoft 365 und nicht über Azure. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – VMware IB | Bestehender Kunde mit dem Produkt: VMware. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Migrieren – Citrix IB | Bestehender Kunde mit dem Produkt: Citrix Systems. Partner sollten diesen Kunden für die Migration zu Azure als Ziel verwenden. | 
| Innovation – Analyse – Power BI IB mit hoher Azure-Neigung | Kunden mit und Active Power BI-Abonnement, einschließlich: Power BI – Standalone Pro, Power BI – Azure-Suiten, Power BI – Office-Suiten, Power BI-Suiten – Microsoft 365 | 
| Aktivieren – DevOps mit GitHub – Visual Studio/MSDN IB | Identifiziert Kunden mit aktiven Visual Studio Versionen | 
| Windows Server Standard-Version | Zeigt die Version von Windows Server Standard-Käufen durch den Kunden an. | 
| Windows Server Standard-Lizenz | Zeigt den Lizenztyp von Windows Server Standard-Käufen durch den Kunden an. | 
| Windows Server Data Center-Version | Zeigt die Version der Käufe des Windows-Rechenzentrums durch den Kunden an. | 
| Windows Server Data Center-Lizenz | Zeigt den Lizenztyp von Windows Data Center-Käufen durch den Kunden an. | 
| AzureFit | Interne und externe Datenpunkte, die Firmographics definieren. Bei der Bewertung von Anpassungen wird ein lookalike-Modell für unseren besten SMB verwendet, um Kunden zu vergleichen und zu prüfen, ob sie für Microsoft-Cloudprodukte geeignet sind. Die Anpassungsbewertung wird vierteljährlich aktualisiert. | 
| AzureIntent | Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht. Die Absichtsbewertung wird bei Anpassen überlagert, um die Cluster zu definieren. Die Absichtsbewertung wird monatlich aktualisiert. | 
| AzureCluster | Identifiziert die Bereitschaft des Kunden, Azure zu erwerben, indem die Empfehlungen für Anpassung und Absicht in einem Cluster konsolidiert werden. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie Act Now- und Evaluate-Kunden als Ziel haben. | 
| WindowsServerDataCenter_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Verlängerung für Windows Server Datacenter verfügt. | 
| WindowsServerStandard_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Verlängerung für Windows Server Standard verfügt. | 
| AzureUpsellCustomer | Identifiziert, ob der Kunde upsell-Propensity für Azure zeigt. | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von Google-Produkten zeigt. | 
| Verfügt über AWS | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von AWS-Produkten zeigt. | 
| Verfügt über EA | Gibt an, ob eine Verlängerung ein EA- oder ein EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob es sich bei einer Verlängerung um eine Open- oder Open Value-Vereinbarung handelt. | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent : Bericht zur Vertragsverlängerung**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnername | Name des Partners | 
| Customer ID | Kunden-ID-Nummer | 
| DUNS-Nummer | Die Dun-& Braduma-Nummer des Kunden, für den eine Bewertung für die Neigung erzielt wird. | 
| Kontoname | Name des Kontos | 
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
| Land | Geografischer Standort des Landes | 
| Segment | Marktsegment | 
| Untersegment | Untersegment "Markt" | 
| SMC-Typzusammenfassung | SMC-Typ | 
| Top Unmanaged – Compute-Basis | Die wichtigsten nicht verwalteten Kunden – Compute | 
| Top Unmanaged – Benutzerbasis | Die wichtigsten nicht verwalteten Kunden – Benutzer | 
| IsNonProfit | Gibt an, ob die Organisation nicht gewinnorientiert ist (Ja oder Nein). | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von AWS-Produkten zeigt. | 
| Verfügt über AWS | Gibt an, ob der Kunde Wettbewerbssignale für den Besitzen von AWS-Produkten zeigt. | 
| Azure-Cluster | Gibt die Kundenneigenz an, Azure zu erwerben. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| D365 Finance + Operations-Cluster | Gibt die Kundenneigenz an, Dynamics 365 Finance and Operations zu erwerben. Kunden, die eine Neigung für Finance + Operations zeigen, werden in den obersten nicht verwalteten Kategorien enthalten sein. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| D365 CE-Cluster | Gibt die Kundenneigenz an, Dynamics 365 Customer Engagement zu erwerben. Kunden, die eine Kundenbindung zeigen, werden in die Kategorien Mittel und Klein fallen. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Kunden nur dann als Ziel haben, wenn noch Kapazität zur Verfügung steht, nachdem Sie auf Act Now and Evaluate customers (Jetzt handeln und Kunden auswerten) gesetzt haben. | 
| D365 BC-Cluster | Gibt die Neigung des Kunden an, Dynamics 365 Business Central zu erwerben. Kunden, die eine Neigung für Business Central zeigen, werden in die Kategorien Mittel und Klein fallen. Target Act Now and Evaluate clusters,because they will produce higher yield. (Jetzt handeln und Cluster auswerten, da sie höhere Ergebnisse erzielen.) Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie Act Now- und Evaluate-Kunden als Ziel haben. | 
| Microsoft 365 Cluster | Identifiziert die Kaufbereitschaft des Kunden Microsoft 365. Target Act Now und Evaluate-Cluster, da sie eine höhere Rendite erzielen. Richten Sie Nurture- und Educate-Kunden nur dann an, wenn noch Kapazität vorhanden ist, nachdem Sie Act Now- und Evaluate-Kunden als Ziel haben. | 
| Lizenzprogramm | Identifiziert den Lizenzprogrammtyp für die Verlängerung. | 
| Vereinbarungs-ID | Bezeichner der Vereinbarung | 
| Enddatum der Vereinbarung | Enddatum der Vereinbarung | 
| Ablauftyp | Ablauftyp | 
| Ablauf des Umsatzes | Umsatz im Zusammenhang mit ablaufenden Abonnements | 
| Verfügt über EA | Gibt an, ob es sich bei einer Verlängerung um ein EA- oder EA-Abonnement handelt. | 
| Hat geöffnet | Gibt an, ob eine Verlängerung eine Open- oder Open Value-Vereinbarung ist. | 
| Azure Upsell-Kunde | Identifiziert, ob der Kunde Upsell-Propensität für Azure anzeigt. | 
| Microsoft 365 Upsell-Kunde | Gibt an, ob der Kunde upsell propensity for Microsoft 365 | 
| RevSumDivisionName | Identifiziert das Produkt, das verlängert werden soll. | 

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen finden Sie unter [Herunterladen von Berichten.](pci-download-reports.md)
