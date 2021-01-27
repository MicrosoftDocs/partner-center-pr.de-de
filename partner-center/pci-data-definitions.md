---
title: Insights-Datendefinitionen
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Im Dokument werden verschiedene Berichte und deren Daten Definitionen aufgelistet, die Sie auf der Seite zum Herunterladen von Erkenntnissen herunterladen können.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861392"
---
# <a name="export--data-definitions"></a>Exportieren von –-Daten Definitionen 

 **Geeignete Rollen** 

- Berichtleser 
- Executive Report-Leser 

## <a name="introduction"></a>Einführung 

Wenn Sie den Hub "Berichte herunterladen" auf dem Insights-Dashboard verwenden, können Sie die unformatierten Datasets exportieren. 

Die verschiedenen Berichte, die Sie zusammen mit den zugehörigen Daten Definitionen herunterladen können, sind in den folgenden Tabellen aufgeführt: 

### <a name="partner-profile-report"></a>**Partner Profil Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPNId | Bezeichner der Microsoft Partner Network (MPN) | 
| PartnerName | Name des Partners | 
| PGA_MPNId | Bezeichner des globalen Partnerkontos MPN | 
| PGA_PartnerName | Globaler Partner Konto Name | 
| City | Orts Standort des Partners | 
| Land | Länder Standort des Partners | 
| Hierarchylevel | Gibt an, ob es sich um eine globale MPN-ID oder eine globale MPN-ID | 

### <a name="customer-details-report"></a>**Bericht "Kunden Details"**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | Bezeichner des Kunden Mandanten | 
| Customertpid | Bezeichner des übergeordneten Elements des Kunden | 
| Customersegment | Kundensegment | 
| Customermarket | Geografischer Markt des Kunden | 
| Customerstatus | Kundenstatus (aktiv oder inaktiv) | 
| Produkt | Das Produkt, das von MPN an den Kunden verkauft wurde: O365, Dynamics 365, Enterprise Mobility + Security, Power BI oder Microsoft Azure | 
| SKU | Produkt-SKU | 
| Month (Monat) | Monat, für den Nutzung und Umsatz berichtet werden | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Standort des Partners | 
| Partnerattributiontype | Der Zuweisungs Typ des Partners. | 
| SalesChannel | Vertriebskanal | 
| Availableseats | Verfügbare Arbeitsplätze | 
| Revenueusd | Umsatz in US-Dollar | 

### <a name="reseller-performance-report"></a>**Reseller Performance Report**

> [!Note]
> Umsatz-und ACR-Daten sind nur für Benutzer verfügbar, die als Viewer für ausführbare Berichte dienen.

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| Resellermpnid | Reseller-Microsoft Partner Network Bezeichner | 
| ResellerName | Name des Handelspartners | 
| Resellermarket | Reseller Country of Market | 
| Derekprovidermpnid | Der Bezeichner des indirekten Anbieters Microsoft Partner Network | 
| Derekprovidername | Name des indirekten Anbieters | 
| Month (Monat) | Monat, für den Nutzung und Umsatz berichtet werden | 
| Produkt | Produktname | 
| SubscriptionID | Der Bezeichner des Abonnements. | 
| Availableseats | Anzahl verfügbarer Arbeitsplätze | 
| Assignedseats | Anzahl zugewiesener Arbeitsplätze | 
| Billedrevenueusd | Umsatz in US-Dollar in Rechnung gestellt | 
| CustomerName | Name des Kunden | 
| Customertpid | Bezeichner des übergeordneten Elements des Kunden | 
| Customersegment | Kundensegment | 
| Customermarket | Geografischer Markt des Kunden | 
| Resellerstatus | Reseller-Status | 

### <a name="subscription-details-report"></a>**Bericht zu Abonnement Details**

>[!Note]
>Umsatz-und ACR-Daten sind nur für Benutzer verfügbar, die als Viewer für ausführbare Berichte dienen.

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Start Datum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionState | Status des Abonnements ("aktiv" oder "abgelehnt") | 
| Month (Monat) | Monat, für den Nutzung und Umsatz berichtet werden | 
| Isautorumew | Gibt an, ob das Abonnement eine automatische Anmeldung hat (yes oder No). | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden | 
| Customertpid | Oberster übergeordneter Bezeichner des Kunden | 
| Customersegment | Marktsegment des Kunden | 
| Customermarket | Geografischer Markt des Kunden | 
| Produkt | Das Produkt wurde vom Partner an den Kunden verkauft. | 
| SKU | SKU des Produkts | 
| MPNId | Microsoft Partner Network-ID des Partners | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Standort des Partners | 
| Partnerattributiontype | Der Zuweisungs Typ für das Abonnement. | 
| SalesChannel | Channel von Sales-Direct, CSP (Cloud Solution Provider) usw. | 
| Availableseats | Aktueller verfügbarer Arbeitsplatz | 
| Revenueusd | Umsatz in US-Dollar | 
| Registrierungs-ID | Registrierungs-ID des Abonnements | 

### <a name="azure-usage-report"></a>**Azure-Verwendungs Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Das Datum des Starts des Abonnements. | 
| SubscriptionEndDate | Das Datum, an dem das Abonnement endet. | 
| SubscriptionState | Aktueller Status des Abonnements ("offen", "geschlossen", "aktiv" oder "in der Toleranz Periode") | 
| Month (Monat) | Nach Monat aggregierte Datumsangaben | 
| Dienstname | Name des Azure-Dienstanbieter | 
| MeterCategory | Name der Kategorie der Verbrauchseinheit | 
| Usageunits | Die Anzahl der Einheiten, die während des Abrechnungszeitraums verwendet werden. | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| Customertpid | Top Parent-ID des Kunden | 
| Customersegment | Segment des Kunden | 
| Customermarket | Geografischer Markt des Kunden | 
| MPNId | Microsoft Partner Network-ID des Kunden | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Länder Standort des Partners | 
| Partnerattributiontype | Der Zuweisungs Typ des Partners. | 
| SalesChannel | Kanal der Verkäufe (Direct/CSP, indirekt/CSP, Direct usw.) | 
| ACR_USD | Von Azure verbrauchter Umsatz (ACR) in US-Dollar | 
| Registrierungs-ID | Registrierungs-ID des Azure-Abonnements | 

### <a name="office-365-license-usage-report"></a>**Office 365-Lizenz Verwendungs Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| Customertpid | Top Parent-ID des Kunden | 
| WorkloadName | Skype for Business, Teams, Exchange Online | 
| Month (Monat) | Monat, für den die Nutzung gemeldet wird | 
| Paidavailableunits | Anzahl der bezahlten verfügbaren Einheiten | 
| Monthlyactiveusers | Anzahl der monatlich aktiven Benutzer | 
| CustomerName | Name des Kunden | 
| Customermarket | Geografischer Länder Standort des Kunden Markts | 
| Customersegment | Kundensegment | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Standort des Partners | 
| Partnerattributiontype | Der Zuweisungs Typ des Partners. | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility-Lizenz Verwendungs Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| Customertpid | Top Parent-ID des Kunden | 
| WorkloadName | Name der Arbeitsauslastung des Enterprise Mobility + Security (EMS) | 
| Month (Monat) | Monat, für den die Nutzung gemeldet wird | 
| Paidavailableunits | Anzahl der bezahlten verfügbaren Einheiten | 
| Monthlyactiveusers | Anzahl der monatlich aktiven Benutzer | 
| CustomerName | Name des Kunden | 
| Customermarket | Geografischer Länder Standort des Kunden Markts | 
| Customersegment | Kundensegment | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Standort des Partners | 
| Partnerattributiontype | Der Zuweisungs Typ des Partners. | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365-Lizenz Verwendungs Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Start Datum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionStatus | Status des Abonnements | 
| Month (Monat) | Monat, für den die Nutzung gemeldet wird | 
| Revsumdivisionname | Name der Rev Sum-Division | 
| Revsumcategoryname | Name der Kategorie der Rev-Summe | 
| SKU | SKU des Produkts | 
| SKUId | SKU-ID des Produkts | 
| Freevspaidsku | Gibt an, ob es sich um eine kostenlose oder kostenpflichtige SKU | 
| SalesModel | Der Vertriebskanal, der zum Verkauf des Abonnements verwendet wird. | 
| Detailedsalesmodel | Detailliertes Vertriebsmodell für das Abonnement | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden Mandanten | 
| Customertpid | Oberster übergeordneter Bezeichner des Kunden | 
| Customersegment | Marktsegment des Kunden | 
| Customermarket | Geografischer Markt des Kunden | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Länder Standort des Partners | 
| Partnerattachtype | Der Zuweisungs Typ für das Abonnement. | 
| Availableseats | Aktueller verfügbarer Arbeitsplatz | 
| Assignedseats | Aktuell zugewiesener Arbeitsplatz | 
| Activeseats | Aktuell aktive Arbeitsplätze | 
| Deploymentopportunity | Aktuelle Bereitstellungs Chance | 
| Activeusageprozent | Aktuell aktiver Verwendungs Prozentsatz | 

### <a name="power-bi-license-usage-report"></a>**Bericht zur Power BI Lizenz Verwendung**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| SubscriptionId | GUID des Abonnements | 
| SubscriptionStartDate | Start Datum des Abonnements | 
| SubscriptionEndDate | Enddatum des Abonnements | 
| SubscriptionStatus | Status des Abonnements (aktiv, inaktiv oder in Toleranz Periode) | 
| Month (Monat) | Nach Monat aggregierte Datumsangaben | 
| SKU | SKU des Produkts | 
| SKUId | SKU-ID des Produkts | 
| Freevspaidsku | Kostenloser oder kostenpflichtiger SKU-Unterscheidungs Unterschied | 
| SalesModel | Das Vertriebsmodell, das zum Verkauf des Abonnements verwendet wird. | 
| Detailedsalesmodel | Detailliertes Vertriebsmodell für das Abonnement | 
| CustomerName | Name des Kunden | 
| CustomerTenantId | GUID des Kunden Mandanten | 
| Customertpid | Bezeichner des übergeordneten Elements des Kunden | 
| Customersegment | Marktsegment des Kunden | 
| Customermarket | Geografischer Markt des Kunden | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Partnerort | Geografischer Länder Standort des Partners | 
| Partnerattachtype | Der Zuweisungs Typ für das Abonnement. | 
| Availableseats | Aktuell verfügbare Arbeitsplätze | 
| Assignedseats | Aktuell zugewiesene Arbeitsplätze | 
| Activeseats | Aktuell aktive Arbeitsplätze | 
| Deploymentopportunity | Aktuelle Bereitstellungs Chance | 
| Activeusageprozent | Aktuell aktiver Verwendungs Prozentsatz | 

### <a name="teams-meetings-and-calls-report"></a>**Teambesprechungen und Aufrufe von Berichten**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| Customertpid | Bezeichner des übergeordneten Elements des Kunden | 
| Month (Monat) | Monat, für den die Nutzung gemeldet wird | 
| Unterauslastung | Unterauslastung, für die die Nutzung gemeldet wird (Besprechungen, Anrufe oder Telefonsysteme) | 
| Besprechungs Anzahl | Anzahl von Besprechungen | 
| Besprechungs Dauer | Gesamte Besprechungs Dauer (in Stunden) | 

### <a name="teams-monthly-usage-report"></a>**Bericht zur monatlichen Verwendung von Teams**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| Customertpid | Bezeichner des übergeordneten Elements des Kunden | 
| Month (Monat) | Monat, für den die Nutzung gemeldet wird | 
| Unterauslastung | Unterauslastung, für die die Nutzung gemeldet wird (Besprechungen, Anrufe oder Telefonsysteme) | 
| Desktop Benutzer | Anzahl von Benutzern, die Teams auf dem Desktop verwenden | 
| Mobile Benutzer | Anzahl von Benutzern, die Teams auf Mobilgeräten verwenden | 
| Webbenutzer | Anzahl der Benutzer, die Teams im Web verwenden | 
| Allupparticipants | Anzahl der eindeutigen Benutzer von Teams für den Monat | 

### <a name="teams-usage-3p-apps-report"></a>**Bericht zur Verwendung von 3p-Apps für Teams**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| CustomerTenantId | Mandanten-ID des Kunden | 
| Customertpid | Top Parent-ID des Kunden | 
| Month (Monat) | Monat, für den die Nutzung gemeldet wird | 
| 3p-App-Name | Name der Teams-App | 
| Benutzeranzahl | Anzahl der Benutzer für die APP | 


### <a name="training-details-report"></a>**Bericht "Schulungs Details"**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| Trainingactivityid | Bezeichner des Trainings | 
| Trainingtitle | Titel der Schulung | 
| Trainingtype | Trainingart (Zertifizierung oder Prüfung) | 
| Individual FirstName | Vorname des Kunden | 
| Individual Name | Nachname des Kunden | 
| Email | Persönliche e-Mail-ID des Kunden | 
| Corpeer-Mail | Büro-e-Mail-ID des Kunden | 
| Trainingcompletiondate | Abschlussdatum der Schulung | 
| Month (Monat) | Monat, für den die Daten gemeldet werden | 
| Icmcp | Gibt an, ob der Benutzer ein Microsoft Certified Professional (MCP) ist. | 
| Mcpid | MCP-ID des Benutzers | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Partner City Location | Geografischer Ort des Partners | 
| Partnercountrylocation | Geografischer Länder Standort des Partners | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| UserName | Name des Benutzers | 
| UserId | GUID des Benutzers | 
| Trainingname | Name der Schulung | 
| Trainingtype | Trainingsart (Modul oder Lernpfad) | 
| Produkte | Das Produkt, für das das Lernmodul anwendbar ist. | 
| Rollen | Anwendbare Rollen des Trainings | 
| Completiondate | Datum der Fertigstellung der Schulung | 
| MPNId | Bezeichner der Microsoft Partner Network | 
| PartnerName | Name des Partners | 
| Land | Geografischer Länder Standort des Partners | 

### <a name="competency-summary-and-history-report"></a>**Kompetenz Zusammenfassung und Verlaufs Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| Competencyname | Der Name der Kompetenz. | 
| Competencylevel | Ebene der Kompetenz (Gold oder Silber) | 
| Competencystatus | Aktueller Status der Kompetenz (aktiv, inaktiv oder in Toleranz Periode) | 
| Competencystartdate | Start Datum der Kompetenz | 
| Competencyenddate | Enddatum der Kompetenz | 

### <a name="competency-performance-report"></a>**Kompetenz Leistungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| Competencyname | Der Name der Kompetenz. | 
| Competencyattainmentoptionname | Name der Option zum Erreichen von Kompetenzen | 
| Month (Monat) | Monat, für den die Metriken gemeldet werden | 
| MetricName | Der Name der Metrik, die für die Kompetenz relevant ist. | 
| Metricmonthlycontribution | Monatlicher Beitrag der Metrik | 
| Ttmaggregate | Aggregierte Metrik für die nachfolgenden 12 Monate | 
| Anniversaryyear-Aggregat | Aggregierte Metrik für das aktuelle Jahres Jahr | 
| Goldthreshold | Leistungsanforderung zum erfüllen der Gold-Kompetenz | 
| Silverthreshold | Leistungsanforderung zum erfüllen der Silver-Kompetenz | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud-Aufstieg-Microsoft 365-neiglichkeits Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner Name | Name des Partners | 
| Customer ID | Bezeichnernummer des Kunden | 
| DUNS-Nummer | Die & bradstraße (D&B)-Nummer des Kunden, der aus Gründen der Neigung bewertet wird | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche, zu der die Organisation gehört | 
| Vertical | Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft, D&B und anderen Industriestandards identifiziert | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Tochtergesellschaft des Kunden, der aus Gründen der Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, der aus Gründen der Neigung bewertet wird | 
| City | Geografischer Ort der Organisation | 
| State | Standort des geografischen Zustands der Organisation | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Länder Standort der Organisation | 
| Segment | Marktsegment | 
| Unter Segment | Markt Subsegment | 
| Übersicht über den SMC | SMC-Typ | 
| Oberste nicht verwaltete computebasis | Top nicht verwaltete Kunden – Compute | 
| Oberste nicht verwaltete Benutzerbasis | Top nicht verwaltete Kunden – Benutzer | 
| Isnonprofit | Gibt an, ob die Organisation nicht Profit (ja oder Nein) ist. | 
| Aktivieren von Remote Arbeit-Ziel Exchange Online | Kunden, die über ein aktives Exchange Online-Abonnement verfügen, Upselling to Microsoft 365 | 
| Aktivieren Sie den Erwerb von Remote arbeitsspeicherort (aktuelle Version) mit cloudaufstiegs-Neigung-+ 10 Lizenzen | Kunde, der über einen aktuellen lokalen Office-oder Windows-Client verfügt. Das heißt, die Client Version ist später als eine Version der Lebensdauer (EOL). Der Kunde hat 10 oder mehr Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der lokalen Bereitstellung von lokalen Arbeitsumgebungen (aktuelle Version) mit clouderfassungs Neigung-<10 Lizenzen | Kunde, der über einen aktuellen lokalen Office-oder Windows-Client verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 10 Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren Sie den Erwerb von Remote arbeitsspeicherort (aktuelle Version) ohne cloudaufstiegs Neigung-+ 10 Lizenzen. | Kunde, der über einen aktuellen lokalen Office-oder Windows-Client verfügt (d. h. eine neuere Version als EOL). Der Kunde hat 10 oder mehr Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der lokalen Bereitstellung von lokalen Arbeitsumgebungen (aktuelle Version) ohne Cloud-Aufstiegs Neigung-<10 Lizenzen | Kunde, der über einen aktuellen lokalen Office-oder Windows-Client verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der Aktivierung von lokalem Arbeits Speicherort (EOL-Version) mit Cloud-Aufstiegs Neigung-+ 10 Lizenzen | Kunde, der über eine lokale EOL-Niederlassung oder einen Windows-Client verfügt (d. h. eine EOL-Version oder früher). Der Kunde hat 10 oder mehr Lizenzen. Der Kunde hat eine Neigung. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der lokalen Bereitstellung von lokalen Arbeitsumgebungen (EOL-Version) mit Cloud-Aufstiegs Neigung-<10 Lizenzen | Kunde, der über eine lokale EOL-Niederlassung oder einen Windows-Client verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat eine Neigung. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der Aktivierung von lokalem Arbeits Speicherort (EOL-Version) ohne Cloud-Aufstiegs Neigung-+ 10 Lizenzen | Kunde, der über einen aktuellen lokalen Office-oder Windows-Client verfügt (d. h. eine EOL-Version oder früher). Der Kunde hat 10 oder mehr Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der lokalen Bereitstellung von lokalen Arbeitsumgebungen (EOL-Version) ohne Cloud-Aufstiegs Neigung-<10 Lizenzen | Kunde, der über einen aktuellen lokalen Office-oder Windows-Client verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte für die Konvertierung in Microsoft 365 als Ziel haben. | 
| Aktivieren der Option "Remote Arbeit-hohe Neigung für Microsoft 365 (Act nowitevaluate)" | Interessenten für Kunden mit hoher Neigung für Microsoft 365 | 
| Aktivieren des Remote-Arbeits Wettbewerbs (Zoom) mit Microsoft 365 | Kunde mit Zoom und Microsoft 365, Ziel für die Konvertierung in Teams | 
| Aktivieren des Remote-Arbeits Wettbewerbs (Zoom) ohne Microsoft 365 | Kunde mit Zoom, Ziel für die Konvertierung in Teams | 
| Kosten senken und verwalten-Microsoft 365 E3 für Microsoft 365 E5 | Vorhandener Kunde mit Microsoft 365 E3, Ziel für Microsoft 365 E5 | 
| Senken Sie Kosten und Verwaltung-Microsoft 365 Business Basic-und Business Standard-Kunden, die auf Microsoft 365 Business Premium abzielen | Vorhandene Microsoft 365 Business Basic-und Business Standard-Kunden, Ziel für Microsoft 365 Business Premium | 
| Transformieren der Produktivität der Organisation: oberflächenneigung | Kunde zeigt eine Neigung für die Oberfläche an | 
| M365Cluster | Identifiziert die Neigung eines Kunden, Microsoft 365 zu erwerben. Das Ziel ist jetzt Act und wertet Cluster aus, da Sie eine höhere Rendite erzielen. Richten Sie Kunden nur dann ein, wenn Sie nach dem Act-Vorgang noch Kapazität haben, und bewerten Sie Kunden als Ziel. | 
| M365Fit | Interne und externe Datenpunkte, die firmugraphics definieren. Die Anpassungs Bewertung verwendet ein Lookalike-Modell für unsere am besten kleinen oder mittelständischen Unternehmen (smsb), um Kunden zu vergleichen und zu sehen, ob Sie für Microsoft-cloudprodukte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert. | 
| M365Intent | Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist für die Definition der Cluster angepasst. Die beabsichtigte Bewertung wird monatlich aktualisiert. | 
| Surfakecluester | Identifiziert die Neigung eines Kunden zur Kauf Oberfläche durch Konsolidieren der Eignung und der beabsichtigten Empfehlungen in einem Cluster. Das Ziel ist jetzt Act und wertet Cluster aus, da Sie eine höhere Rendite erzielen. Richten Sie Kunden nur dann ein, wenn Sie nach dem Act-Vorgang noch Kapazität haben, und bewerten Sie Kunden als Ziel. | 
| "Surfacefit" | Interne und externe Datenpunkte, die firmugraphics definieren. Die Anpassungs Bewertung verwendet ein Lookalike-Modell zu unseren besten smsb zum Vergleichen von Kunden und zum Überprüfen, ob Sie für Microsoft-cloudprodukte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert. | 
| Surfakeintent | Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist für die Definition der Cluster angepasst. Die beabsichtigte Bewertung wird monatlich aktualisiert. | 
| O365Cluster | Gibt die Neigung des Kunden an, Office 365 zu erwerben. Das Ziel ist jetzt Act und wertet Cluster aus, da Sie eine höhere Rendite erzielen. Richten Sie Kunden nur dann ein, wenn Sie nach dem Act-Vorgang noch Kapazität haben, und bewerten Sie Kunden als Ziel. | 
| O365Fit | Interne und externe Datenpunkte, die firmugraphics definieren. Die Anpassungs Bewertung verwendet ein Lookalike-Modell zu unseren besten smsb zum Vergleichen von Kunden und zum Überprüfen, ob Sie für Microsoft-cloudprodukte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert. | 
| O365Intent | Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist für die Definition der Cluster angepasst. Die beabsichtigte Bewertung wird monatlich aktualisiert. | 
| M365UpsellCustomer | Gibt an, ob der Kunde Upselling-Neigung für Microsoft 365 anzeigt. | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbs Signale für die besitzenden Google-Produkte anzeigt | 
| Hat AWS | Gibt an, ob der Kunde Wettbewerbs Signale zum Besitz von AWS-Produkten (Amazon Web Services) anzeigt. | 
| Hat EA | Gibt an, ob eine Erneuerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob eine Erneuerung eine Open-oder Open Value-Vereinbarung ist. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloudaufstieg-Dynamics 365-neiglichkeits Bericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner Name | Name des Partners | 
| Customer ID | Kunden-ID-Nummer | 
| DUNS-Nummer | Die Dun & Bradstreet-Nummer des Kunden, der aus Gründen der Neigung bewertet wird | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche, zu der die Organisation gehört | 
| Vertical | Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft, D&B und anderen Industriestandards identifiziert
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Tochtergesellschaft des Kunden, der aus Gründen der Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, der aus Gründen der Neigung bewertet wird | 
| City | Standort der geografischen Stadt | 
| State | Standort des geografischen Zustands | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Länder Standort | 
| Segment | Marktsegment | 
| Unter Segment | Markt Subsegment | 
| Übersicht über den SMC | Die Kategorisierung eines Kunden: die wichtigsten nicht verwalteten Benutzer Basen sind Kunden mit mehr als 300 Mitarbeitern, die wichtigsten nicht verwalteten computebasen sind Kunden mit USD10, 000 in Azure-drei Jahren, mittelständische Unternehmen sind Kunden mit 25 Mitarbeitern oder höher, und kleine Unternehmen sind Kunden mit weniger als 25 Mitarbeitern. | 
| Oberste nicht verwaltete computebasis | Top nicht verwaltete Kunden – Compute | 
| Oberste nicht verwaltete Benutzerbasis | Top nicht verwaltete Kunden – Benutzer | 
| Isnonprofit | Gibt an, ob die Organisation nicht Profit (ja oder Nein) ist. | 
| Aktivieren Sie den Digital Selling-Microsoft 365-Seat-Größe >= 25 Arbeitsplätze (SalesPro-neiglichkeits Modell). | Kunde ohne Dynamics 365. Arbeitsplatz Größe: 25 +. Der Partner sollte auf einen Kreuz Verkauf von Dynamics 365 SalesPro abzielen. | 
| Aktivieren von Digital Selling-Dynamics 365 SalesPro-Neigung (jetzt agieren oder evaluieren) | Kunden mit hoher Neigung ohne Dynamics 365. Der Partner sollte für Dynamics 365 SalesPro als Ziel haben. | 
| Verwalten von Finanzrisiken & betrug-Dynamics lokale Installation Basis-Navision (Geschäfts zentrales Konzeptmodell) | Vorhandener Kunde mit lokalem Navision. Der Partner sollte für Dynamics 365 Business Central als Ziel haben. | 
| Verwalten von Finanzrisiken & Betrugs basierte Dynamics-Installation Base-Dynamics AX (Dynamics 365 Finance + Operations-Modell) | Vorhandener Kunde mit lokalem AX. Der Partner sollte auf Dynamics 365 Finance +-Vorgänge abzielen. | 
| Verwalten von Finanzrisiken & betrug-Dynamics lokale Installation Basis-tolle Ebenen (Geschäfts zentrales Modell) | Vorhandener Kunde mit der lokalen Umgebung. Der Partner sollte für Dynamics 365 Business Central als Ziel haben. | 
| Verwalten von Finanzrisiken & betrug-Dynamics lokale Installation Basis-Solomon (Geschäfts zentrales Modell) | Vorhandener Kunde mit lokalem Solomon. Der Partner sollte für Dynamics 365 Business Central als Ziel haben. | 
| Verwalten von Finanzrisiken & betrug-Dynamics lokale Installationsbasis-andere (Geschäfts zentrales Modell) | Vorhandener Kunde mit anderen lokalen Lösungen, die zuvor nicht aufgeführt waren. Der Partner sollte für Dynamics 365 Business Central als Ziel haben. | 
| Entwickeln von Agile-Geschäftsprozessen: Dynamics lokale Installation Basis-AX/GP/SL/NAV/other (Dynamics 365-neiglichkeits Modell) | Entwickeln von Agile-Geschäftsprozessen: Dynamics lokale Installation Basis-AX/GP/SL/NAV/other (Dynamics 365-neiglichkeits Modell) | 
| Entwickeln von Agile-Geschäftsprozessen-Dynamics konkurrierende Basis-mendix/Outsystems/Salesforce (Dynamics 365-neiglichkeits Modell) | Entwickeln von Agile-Geschäftsprozessen-Dynamics konkurrierende Basis-mendix/Outsystems/Salesforce (Dynamics 365-neiglichkeits Modell) | 
| Erstellen von Agile-Geschäftsprozessen: Dynamics 365 Finance + Operations-Installationsbasis | Vorhandene Dynamics 365 Finance + Operations-Kunden. Partner für Power apps. | 
| Entwickeln von Agile-Geschäftsprozessen: Dynamics 365 Business Central-Installationsbasis | Vorhandene Dynamics 365 Business Central-Kunden. Partner für Power apps. | 
| Erstellen von Agile-Geschäftsprozessen: Dynamics 365 Customer Engagement-Installationsbasis | Vorhandene Dynamics 365 Customer Engagement-Kunden. Partner für Power apps. | 
| Erstellen Sie eine robuste Lieferkette, und aktivieren Sie die erste Dynamics 365-Arbeitsauslastung als Dynamics 365 Supply Chain Management mit nicht-Oracle-oder SAP ERP-Kunden (Enterprise Resource Planning). | Zielkunden für die Dynamics 365-Lieferketten Verwaltung | 
| Erstellen Sie eine robuste Lieferkette, und verkaufen Sie Dynamics 365 Supply Chain Management und/oder Retail oder Commerce an bestehende Dynamics 365 Customer Engagement-Kunden | Vorhandene Dynamics 365 Customer Engagement-Kunden, die für eine Kreuz Selling Dynamics 365 Supply Chain Management abzielen. | 
| Erstellen Sie eine robuste Lieferkette, und verkaufen Sie Dynamics 365 Supply Chain Management und/oder Retail oder Commerce für Dynamics 365 Customer Engagement und Oracle oder SAP. | Vorhandene Dynamics 365 Customer Engagement-Kunden mit Oracle oder SAP für die Dynamics 365-Lieferketten Verwaltung | 
| D365BCCluster | Identifiziert die Neigung des Kunden, Dynamics 365 Business Central zu erwerben. Kunden, die eine Neigung für Business Central anzeigen, werden in den Kategorien Mittel und klein aufgeführt. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| D365BCFit | Interne und externe Datenpunkte, die firmugraphics definieren. Die Anpassungs Bewertung verwendet ein Lookalike-Modell, um Kunden zu vergleichen und zu sehen, ob Sie für Microsoft-cloudprodukte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert. | 
| D365BCIntent | Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist für die Definition der Cluster angepasst. Die beabsichtigte Bewertung wird monatlich aktualisiert. | 
| D365FOCluster | Identifiziert die Neigung des Kunden, Dynamics 365 Finance und Operations zu erwerben. Kunden, die eine Neigung für Finanzen und Vorgänge anzeigen, werden in den obersten nicht verwalteten Kategorien aufgeführt. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| D365FOFit | Interne und externe Datenpunkte, die firmugraphics definieren. Die Anpassungs Bewertung verwendet ein Lookalike-Modell, um Kunden zu vergleichen und zu sehen, ob Sie für Microsoft-cloudprodukte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert. | 
| D365FOIntent | Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist für die Definition der Cluster angepasst. Die beabsichtigte Bewertung wird monatlich aktualisiert. | 
| D365CECluster | Gibt die Neigung des Kunden an, Dynamics 365 Customer Engagement zu erwerben. Kunden, die eine Neigung für Customer Engagement anzeigen, werden in den Kategorien Mittel und klein aufgeführt. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| D365CEFit | Gibt an, dass für Dynamics 365 Customer Engagement geeignet ist. | 
| D365CEIntent | Gibt die Absicht für Dynamics 365 Customer Engagement an | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Erneuerung für Dynamics lokal AX oder CRM verfügt. | 
| M365UpsellCustomer | Gibt an, ob der Kunde Upselling-Neigung für Microsoft 365 anzeigt. | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbs Signale für die besitzenden Google-Produkte anzeigt | 
| Hat AWS | Gibt an, ob der Kunde Wettbewerbs Signale für besitzende AWS-Produkte anzeigt. | 
| Hat EA | Gibt an, ob eine Erneuerung ein EA-oder EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob eine Erneuerung eine Open-oder Open Value-Vereinbarung ist. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud-Aufstieg: Azure-Bereitstellungsbericht**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner Name | Name des Partners | 
| Customer ID | Kunden-ID-Nummer | 
| DUNS-Nummer | Die Dun & Bradstreet-Nummer des Kunden, der aus Gründen der Neigung bewertet wird | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche | 
| Vertical | Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft, D&B und anderen Industriestandards identifiziert | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Tochtergesellschaft des Kunden, der aus Gründen der Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, der aus Gründen der Neigung bewertet wird | 
| City | Standort der geografischen Stadt | 
| State | Standort des geografischen Zustands | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Länder Standort | 
| Segment | Marktsegment | 
| Unter Segment | Markt Subsegment | 
| Übersicht über den SMC | SMC-Typ | 
| Oberste nicht verwaltete computebasis | Top nicht verwaltete Kunden – Compute | 
| Oberste nicht verwaltete Benutzerbasis | Top nicht verwaltete Kunden – Benutzer | 
| Isnonprofit | Gibt an, ob die Organisation nicht Profit (ja oder Nein) ist. | 
| Migration-EOL Windows Server-EOL Windows Server IB mit Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über einen lokalen EOL-Windows-Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über fünf oder mehr Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL Windows Server-EOL Windows Server IB mit Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über einen lokalen EOL-Windows-Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über weniger als 5 Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL Windows Server-EOL Windows Server IB ohne Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über einen lokalen EOL-Windows-Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL Windows Server-EOL Windows Server IB ohne Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über einen lokalen EOL-Windows-Server verfügt (d. h. eine EOL-Version oder früher). Verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL SQL-EOL SQL Server IB mit Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde hat fünf Lizenzen. Der Kunde hat eine Neigung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL SQL-EOL SQL Server IB mit Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder früher). Verfügt über weniger als 5 Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL SQL-EOL SQL Server IB ohne Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über fünf oder mehr Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-EOL SQL-EOL SQL Server IB ohne Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über eine lokale EOL-SQL Server verfügt (d. h. eine EOL-Version oder früher). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren von lokalem Windows Server-current Windows Server IB mit Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Instanz verfügt (d. h. eine neuere Version als EOL). Der Kunde hat fünf Lizenzen. Der Kunde hat eine Neigung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren von lokalem Windows Server-current Windows Server IB mit Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Instanz verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Customer hat eine Neigung für Azure. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren von lokalem Windows Server-Aktuelles Windows Server-IB ohne Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Instanz verfügt (d. h. eine neuere Version als EOL). Der Kunde hat fünf Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren von lokalem Windows Server-current Windows Server IB ohne Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über eine aktuelle lokale Windows Server-Instanz verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren zu Azure SQL-oder SQL-VMS (Virtual Machines, VMS)-Aktuelles SQL Server IB mit Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde hat fünf Lizenzen. Der Kunde hat eine Neigung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration: Migrieren zu Azure SQL-oder SQL-VMS-Aktuelles SQL Server IB mit Cloud-Aufstiegs Neigung <5 Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat eine Neigung. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren zu Azure SQL-oder SQL-VMS-Current SQL Server IB ohne Cloud-Aufstiegs Neigung-5 + Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde hat fünf Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren: Migrieren zu Azure SQL-oder SQL-VMS-Current SQL Server IB ohne Cloud-Aufstiegs Neigung-<5 Lizenzen | Kunde, der über eine aktuelle lokale SQL Server verfügt (d. h. eine neuere Version als EOL). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-OSS-Migrieren zu Open Source-Datenbanken (OSS) | Vorhandener Kunde mit einem der folgenden konkurrierenden Produkte: PostgreSQL, MySQL und MariaDB. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-OSS-Linux in Azure | Vorhandener Kunde mit Linux. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migrieren von SAP-SAP in Azure | Vorhandener Kunde mit SAP. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-virtueller Windows-Desktop-Remotedesktopdienste IB | Identifiziert Kunden mit aktiven Windows-Remotedesktopdienste. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-virtueller Windows-Desktop-Cross Selling modern work zu Azure/WVD | Identifiziert Kunden mit Microsoft 365 und verfügt nicht über Azure. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-VMware IB | Vorhandener Kunde mit dem Produkt: VMware. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Migration-Citrix IB | Vorhandener Kunde mit dem Produkt: Citrix Systems. Der Partner sollte diesen Kunden für die Migration zu Azure als Ziel haben. | 
| Innovation-Analytics-Power BI IB mit hoher Azure-Neigung | Kunden mit und Active Power BI-Abonnement, einschließlich: Power BI eigenständiger pro, Power BI-Azure Suites, Power BI-Office-Suites Power BI Suites-Microsoft 365 | 
| Enable-devops mit GitHub: Visual Studio/MSDN IB | Identifiziert Kunden mit aktiven Visual Studio-Versionen | 
| Windows Server-Standard Version | Zeigt die Version von Windows Server Standard-Käufen vom Kunden an | 
| Windows Server-Standard Lizenz | Hiermit wird der Lizenztyp von Windows Server Standard-Käufen vom Kunden angezeigt. | 
| Version des Windows Server-Rechenzentrums | Zeigt die Version der Windows-Rechenzentrums Käufe des Kunden an. | 
| Lizenz für das Windows Server-Rechenzentrum | Hiermit wird der Lizenztyp des Windows-Rechenzentrums von Kunden angezeigt. | 
| Azurefit | Interne und externe Datenpunkte, die firmugraphics definieren. Die Anpassungs Bewertung verwendet ein Lookalike-Modell, um Kunden zu vergleichen und zu sehen, ob Sie für Microsoft-cloudprodukte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert. | 
| Azureintent | Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist für die Definition der Cluster angepasst. Die beabsichtigte Bewertung wird monatlich aktualisiert. | 
| Azurecluester | Gibt Aufschluss über den Kundenwunsch, Azure zu erwerben, indem er die Eignung und beabsichtigten Empfehlungen in einem Cluster konsolidiert. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| WindowsServerDataCenter_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Erneuerung für Windows Server Datacenter verfügt. | 
| WindowsServerStandard_HasOpenRenewal | Gibt an, ob der Kunde über eine offene Erneuerung für Windows Server Standard verfügt. | 
| Azureupsellcustomer | Gibt an, ob der Kunde die Upselling-Neigung für Azure anzeigt. | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbs Signale für die besitzenden Google-Produkte anzeigt | 
| Hat AWS | Gibt an, ob der Kunde Wettbewerbs Signale für besitzende AWS-Produkte anzeigt. | 
| Hat EA | Gibt an, ob eine Erneuerung ein EA-oder EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob eine Erneuerung eine Open-oder Open Value-Vereinbarung ist. | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud-Aufstieg-Bericht zum Erneuern von Vereinbarungs Bedingungen**

| Spaltenname | Datenbeschreibung | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner Name | Name des Partners | 
| Customer ID | Kunden-ID-Nummer | 
| DUNS-Nummer | Die Dun & Bradstreet-Nummer des Kunden, der aus Gründen der Neigung bewertet wird | 
| Kontoname | Name des Kontos | 
| Domain | Domäne des Kontos | 
| Organisationsgröße | Größe der Organisation | 
| Branche | Branche | 
| Vertical | Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft, D&B und anderen Industriestandards identifiziert | 
| Bereich | Geografischer Bereich des Standorts | 
| Niederlassung | Die Tochtergesellschaft des Kunden, der aus Gründen der Neigung bewertet wird | 
| Sales Territory | Das Vertriebsgebiet des Kunden, der aus Gründen der Neigung bewertet wird | 
| City | Standort der geografischen Stadt | 
| State | Standort des geografischen Zustands | 
| Postleitzahl | Postleitzahl der Organisation | 
| Land | Geografischer Länder Standort | 
| Segment | Marktsegment | 
| Unter Segment | Markt Subsegment | 
| Übersicht über den SMC | SMC-Typ | 
| Oberste nicht verwaltete computebasis | Top nicht verwaltete Kunden – Compute | 
| Oberste nicht verwaltete Benutzerbasis | Top nicht verwaltete Kunden – Benutzer | 
| Isnonprofit | Gibt an, ob die Organisation nicht Profit (ja oder Nein) ist. | 
| Hat Google | Gibt an, ob der Kunde Wettbewerbs Signale für besitzende AWS-Produkte anzeigt. | 
| Hat AWS | Gibt an, ob der Kunde Wettbewerbs Signale für besitzende AWS-Produkte anzeigt. | 
| Azure-Cluster | Gibt die Neigung des Kunden an, Azure zu erwerben. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| D365 Finance + Operations-Cluster | Identifiziert die Neigung des Kunden, Dynamics 365 Finance und Operations zu erwerben. Kunden, die eine Neigung für Finanzen und Vorgänge anzeigen, werden in den obersten nicht verwalteten Kategorien aufgeführt. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| D365 CE-Cluster | Gibt die Neigung des Kunden an, Dynamics 365 Customer Engagement zu erwerben. Kunden, die eine Neigung für Customer Engagement anzeigen, werden in den Kategorien Mittel und klein aufgeführt. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| D365 BC-Cluster | Identifiziert die Neigung des Kunden, Dynamics 365 Business Central zu erwerben. Kunden, die eine Neigung für Business Central anzeigen, werden in den Kategorien Mittel und klein aufgeführt. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| Microsoft 365 Cluster | Identifiziert die Neigung des Kunden, Microsoft 365 zu erwerben. Das Ziel agiert jetzt und wertet Cluster aus, da Sie eine höhere Rendite erzielen werden. Richten Sie Kunden nur dann ein, wenn Sie nach dem abzielen von "jetzt agieren" und evaluieren von Kunden noch Überkapazität verfügen. | 
| Lizenzprogramm | Identifiziert den Typ des Lizenzprogramms für die Verlängerung. | 
| Vereinbarungs-ID | Der Bezeichner der Vereinbarung. | 
| Enddatum der Vereinbarung | Enddatum der Vereinbarung | 
| Ablauftyp | Typ des Ablaufs | 
| Ablauf der Einnahmen | Umsatz im Zusammenhang mit ablaufenden Abonnements | 
| Hat EA | Gibt an, ob eine Erneuerung ein EA-oder EA-Abonnement ist. | 
| Hat geöffnet | Gibt an, ob eine Erneuerung eine Open-oder Open Value-Vereinbarung ist. | 
| Azure-Upsell-Kunde | Gibt an, ob der Kunde die Upselling-Neigung für Azure anzeigt. | 
| Microsoft 365 Upsell-Kunde | Gibt an, ob der Kunde Upselling-Neigung für Microsoft 365 anzeigt. | 
| Revsumdivisionname | Identifiziert das Produkt, das für die Verlängerung eingerichtet ist. | 

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen finden Sie unter [Herunterladen von Berichten](pci-download-reports.md).
