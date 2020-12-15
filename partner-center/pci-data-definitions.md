---
title: Insights-Daten Definitionen
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Das Dokument enthält die Liste der verschiedenen Berichte und die Daten Definitionen der einzelnen Berichte, die Sie auf der Seite zum Herunterladen des Berichts herunterladen können.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501748"
---
# <a name="export--data-definitions"></a>Exportieren von –-Daten Definitionen 

 **Geeignete Rollen** 

- Berichtleser 
- Executive Report-Leser 

## <a name="introduction"></a>Einführung 

Der Hub für das Herunterladen von Berichten im Insights-Dashboard ermöglicht Ihnen das Exportieren der Rohdaten Datasets.  

Die verschiedenen Berichte, die zusammen mit der Datendefinition heruntergeladen werden können, lauten wie folgt: 

**Partner Profil**: die Daten Definitionen der verschiedenen Felder des Profil Berichts lauten: 


| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|MPNId|Microsoft Partner Network-ID|
|PartnerName|Name des Partners |
|PGA_MPNId|MPN-ID für globales Partner Konto|
|PGA_PartnerName|Globaler Partner Konto Name|
|City|Orts Standort des Partners |
|Land|Länder Standort des Partners |
|Hierarchylevel|Gibt an, ob es sich um eine globale MPN-ID oder Speicherort-MPN|

**Kunden Details**: die Daten Definitionen der verschiedenen Felder im Bericht "Kunden Details" lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|CustomerName|Name des Kunden |
|CustomerTenantId|Mandanten-ID des Kunden |
|Customertpid|Oberster übergeordneter Bezeichner des Kunden |
|Customersegment|Kunden Segment |
|Customermarket|Geografischer Markt des Kunden  |
|Customerstatus|Kunden Status (aktiv/inactive) |
|Produkt|Das Produkt, das vom MPN an den Kunden verkauft wurde. Dabei handelt es sich um einen der O365-, D365-, Enterprise Mobility-, Power BI Microsoft Azure.|
|SKU|   Produkt-SKU|
|Month (Monat)| Monat, für den Nutzung und Umsatz berichtet werden|
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   Name des Partners|
|Partnerort|   Geografischer Standort des Partners|
|Partnerattributiontype|    Zuweisungs Typ von Partner|
|SalesChannel|  Sales Channel|
|Availableseats|    Verfügbare Arbeitsplätze| 
|Revenueusd|    Umsatz in USD|

Wieder **Verkäufer Leistung**: die Daten Definitionen der verschiedenen Felder der Leistungsberichte des Wiederverkäufers lauten:

> [!Note]
> Umsatz-und ACR-Daten stehen nur Benutzern zur Verfügung, die als Viewer für ausführbare Berichte dienen.

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|Resellermpnid|Reseller-Microsoft Partner Network Bezeichner| 
|Name des Wiederverkäufers|Name des Handelspartners|
|Resellermarket|Reseller Country of Market| 
|Derekprovidermpnid|Indirekter Anbieter Microsoft Partner Network Bezeichner|
|Derekprovidername|Name des indirekten Anbieters|
|Month (Monat)|Monat, für den Nutzung und Umsatz berichtet werden|
|Produkt|Produktname|
|SubscriptionID|Abonnement Bezeichner|
|Availableseats|Anzahl verfügbarer Arbeitsplätze|
|Assignedseats|Anzahl zugewiesener Arbeitsplätze|
|Billedrevenueusd|Umsatz in Rechnung gestellt (in $)|
|CustomerName|Name des Kunden| 
|Customertpid|Oberster übergeordneter Bezeichner des Kunden| 
|Customersegment|Kunden Segment |
|Customermarket|Geografischer Markt des Kunden |
|Resellerstatus|Reseller-Status| 

**Abonnement Details**: die Daten Definitionen der verschiedenen Felder des Abonnement Detail Berichts lauten:

>[!Note]
>Umsatz-und ACR-Daten stehen nur Benutzern zur Verfügung, die als Executive-Bericht-Viewer dienen.

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|SubscriptionId|    GUID des Abonnements|
|SubscriptionStartDate| Start Datum des Abonnements|
|SubscriptionEndDate|   Enddatum des Abonnements|
|SubscriptionState| Status des Abonnements ("aktiv" oder "abgelehnt")|
|Month (Monat)| Monat, für den Nutzung und Umsatz berichtet werden|
|Isautorumew|   Gibt an, ob das Abonnement automatisch erneuert wird. (j/N)|
|CustomerName|  Customer Name| 
|CustomerTenantId|  Kunden-GUID|
|Customertpid|  Oberster übergeordneter Bezeichner des Kunden| 
|Customersegment|   Markt Segment des Kunden| 
|Customermarket|    Geografischer Markt des Kunden|
|Produkt|   Das Produkt wurde vom Partner an den Kunden verkauft.| 
|SKU|   SKU des Produkts |
|MPNId| Microsoft Partner Network-ID des Partners |
|PartnerName|   Name des Partners |
|Partnerort|   Geografischer Standort des Partners |
|Partnerattributiontype|    Der Zuweisungs Typ für das Abonnement.|
|SalesChannel|  Kanal des Umsatzes (Direct/CSP usw.) |
|Availableseats|    Aktueller verfügbarer Arbeitsplatz|
|Revenueusd|    Umsatz in USD|
|Registrierungs-ID| Registrierungs-ID des Abonnements|

**Azure-Nutzung**: die Daten Definitionen der verschiedenen Felder des Azure-Verwendungs Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|SubscriptionId|    GUID des Abonnements|
|SubscriptionStartDate| Das Datum des Starts des Abonnements.|
|SubscriptionEndDate|   Das Datum, an dem das Abonnement endet.|
|SubscriptionState| Aktueller Status des Abonnements (offen/geschlossen/aktiv/Intoleranz-Zeitraum)|
|Month (Monat)| Nach Monat aggregierte Datumsangaben |
|Dienstname|   Name des Azure-Dienstanbieter|
|MeterCategory| Name der Kategorie der Verbrauchseinheit|
|Usageunits|    Die Anzahl der während des Abrechnungszeitraums verwendeten Einheiten. |
|CustomerName|  Name des Kunden |
|CustomerTenantId|  Mandanten-ID des Kunden |
|Customertpid|  Top Parent-ID des Kunden |
|Customersegment|   Segment des Kunden |
|Customermarket|    Geografischer Markt des Kunden |
|MPNId  |Microsoft Partner Network-ID des Kunden |
|PartnerName|   Name des Partners |
|Partnerort    |Geografischer Länder Standort des Partners |
|Partnerattributiontype |Zuweisungs Typ von Partner|
|SalesChannel|  Kanal der Verkäufe (Direct/CSP indirekt/CSP Direct usw.) |
|ACR_USD|   Azure-Umsatz in USD|
|Registrierungs-ID| Registrierungs-ID des Azure-Abonnements|

**Office 365-Lizenz Verwendung**: die Daten Definitionen der verschiedenen Felder des Office 365-Lizenz Verwendungs Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|CustomerTenantId|  Mandanten-ID des Kunden| 
|Customertpid|  Top Parent-ID des Kunden |
|WorkloadName|  SFB, Teams, Exo |
|Month (Monat)| Monat, für den die Nutzung gemeldet wird|
|Paidavailableunits|    Anzahl der bezahlten verfügbaren Einheiten|
|Monthlyactiveusers|    Anzahl der monatlich aktiven Benutzer|
|CustomerName|  Name des Kunden|
|Customermarket|    Geografischer Länder Standort des Kunden Markts |
|Customersegment|   Kunden Segment |
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   Name des Partners|
|Partnerort|   Geografischer Standort des Partners|
|Partnerattributiontype|    Zuweisungs Typ von Partner|

**Enterprise Mobility – Lizenz Verwendung**: die Datendefinition der verschiedenen Felder des EMS –-Lizenz Verwendungs Berichts lautet:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|CustomerTenantId|  Mandanten-ID des Kunden| 
|Customertpid|  Top Parent-ID des Kunden |
|WorkloadName|  Name der EMS-Arbeitsauslastung |
|Month (Monat)| Monat, für den die Nutzung gemeldet wird|
|Paidavailableunits|    Anzahl der bezahlten verfügbaren Einheiten|
|Monthlyactiveusers|    Anzahl der monatlich aktiven Benutzer|
|CustomerName|  Name des Kunden|
|Customermarket|Geografischer Länder Standort des Kunden Markts |
|Customersegment|   Kunden Segment |
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   Name des Partners|
|Partnerort|   Geografischer Standort des Partners|
|Partnerattributiontype|    Zuweisungs Typ von Partner|

**Dynamics 365 – License Usage**: die Datendefinition der verschiedenen Felder des Dynamics 365 – License Usage-Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|SubscriptionId|GUID des Abonnements|
|SubscriptionStartDate| Start Datum des Abonnements|
|SubscriptionEndDate|   Enddatum des Abonnements|
|SubscriptionStatus|    Status des Abonnements |
|Month (Monat)| Monat, für den die Nutzung gemeldet wird|
|Revsumdivisionname|    Name der Rev Sum-Division|
|Revsumcategoryname|    Name der Kategorie der Rev-Summe|
|SKU|   SKU des Produkts |
|SKUId| SKU-ID des Produkts |
|Freevspaidsku| Gibt an, ob es sich um eine kostenlose oder kostenpflichtige SKU |
|SalesModel|    Der Vertriebskanal, der zum Verkauf des Abonnements verwendet wird.|
|Detailedsalesmodel|    Detailliertes Vertriebsmodell für das Abonnement|
|CustomerName|  Customer Name |
|CustomerTenantId|  GUID des Kunden Mandanten |
|Customertpid|  Oberster übergeordneter Bezeichner des Kunden |
|Customersegment|   Marktsegment des Kunden |
|Customermarket|    Geografischer Markt des Kunden |
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   Name des Partners |
|Partnerort|   Geografischer Länder Standort des Partners |
|Partnerattachtype| Der Zuweisungs Typ für das Abonnement.|
|Availableseats|    Aktueller verfügbarer Arbeitsplatz|
|Assignedseats| Aktuell zugewiesener Arbeitsplatz |
|Activeseats|   Aktuell aktive Arbeitsplätze |
|Deploymentopportunity| Aktuelle Bereitstellungs Chance|
|Activeusageprozent|    Aktueller aktiver Verwendungs Prozentsatz|
 
**Power BI Lizenz Verwendung**: die Datendefinition der verschiedenen Felder des Power BI – License Usage-Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|SubscriptionId|    GUID des Abonnements|
|SubscriptionStartDate| Start Datum des Abonnements|
|SubscriptionEndDate|   Enddatum des Abonnements|
|SubscriptionStatus|    Status des Abonnements (aktiv oder In-Active oder in der Toleranz Periode)|
|Month (Monat)| Nach Monat aggregierte Datumsangaben |
|SKU|   SKU des Produkts |
|SKUId| SKU-ID des Produkts |
|Freevspaidsku| Kostenloser oder kostenpflichtiger SKU-Unterscheidungs Unterschied |
|SalesModel|    Das Vertriebsmodell, das zum Verkauf des Abonnements verwendet wird.|
|Detailedsalesmodel|    Detailliertes Vertriebsmodell für das Abonnement|
|CustomerName|  Customer Name |
|CustomerTenantId|  GUID des Kunden Mandanten |
|Customertpid|  Oberster übergeordneter Bezeichner des Kunden| 
|Customersegment|   Markt Segment des Kunden |
|Customermarket|    Geografischer Markt des Kunden |
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   Name des Partners |
|Partnerort|   Geografischer Länder Standort des Partners |
|Partnerattachtype| Der Zuweisungs Typ für das Abonnement.|
|Availableseats|    Aktuell verfügbare Arbeitsplätze|
|Assignedseats| Aktuell zugewiesene Arbeitsplätze|
|Activeseats|   Aktuell aktive Arbeitsplätze|
|Deploymentopportunity| Aktuelle Bereitstellungs Chance|
|Activeusageprozent|    Aktueller aktiver Verwendungs Prozentsatz|

**Verwendung von Teams – Besprechungen und Anrufe**: die Daten Definitionen der verschiedenen Felder lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|CustomerTenantId|  Mandanten-ID des Kunden |
|Customertpid|  Top Parent-ID des Kunden |
|Month (Monat)| Monat, für den die Nutzung gemeldet wird|
|Unterauslastung|   Untergeordnete Arbeitsauslastung, für die die Nutzung gemeldet wird (Besprechungen, Anrufe, Telefonsysteme)|
|Besprechungs Anzahl| Anzahl von Besprechungen|
|Besprechungs Dauer|  Gesamte Besprechungs Dauer (in Stunden)|

**Teams-monatliche Nutzungs Details**: die Daten Definitionen der verschiedenen Felder lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|CustomerTenantId|  Mandanten-ID des Kunden |
|Customertpid|  Top Parent-ID des Kunden |
|Month (Monat)| Monat, für den die Nutzung gemeldet wird|
|Unterauslastung|   Untergeordnete Arbeitsauslastung, für die die Nutzung gemeldet wird (Besprechungen, Anrufe, Telefonsysteme)|
|Desktop Benutzer| Anzahl von Benutzern, die Teams auf dem Desktop verwenden|
|Mobile Benutzer|  Anzahl von Benutzern, die Teams auf Mobilgeräten verwenden|
|Webbenutzer| Anzahl von Benutzern, die Teams im Web verwenden|
|Allupparticipants| Anzahl der unterschiedlichen Benutzer von Teams für den Monat|

**Verwendung von Teams – 3P-apps**: die Daten Definitionen der verschiedenen Felder lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|CustomerTenantId|  Mandanten-ID des Kunden| 
|Customertpid|  Top Parent-ID des Kunden |
|Month (Monat)| Monat, für den die Nutzung gemeldet wird|
|3p-App-Name|   Name der Teams-App|
|Benutzeranzahl|    Anzahl der Benutzer für die APP|


**Schulungs Details**: die Daten Definitionen der verschiedenen Felder des Trainings Detail Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|Trainingactivityid|    Bezeichner des Trainings |
|Trainingtitle| Titel der Schulung |
|Trainingtype|  Trainingsart (Zertifizierung/Prüfung)|
|Individual FirstName|   Vorname des Kunden| 
|Individual Name|    Nachname des Kunden| 
|E-Mail| Persönliche e-Mail-ID des Kunden|
|Corpeer-Mail| E-Mail-ID des Kunden|
|Trainingcompletiondate|    Abschlussdatum der Schulung |
|Month (Monat)| Monat, für den die Daten gemeldet werden|
|Icmcp| Gibt an, ob der Benutzer ein Microsoft Certified Professional ist.|
|Mcpid| MCP-ID des Benutzers|
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   Name des Partners |
|Partner City Location|   Geografischer Ort des Partners |
|Partnercountrylocation|    Geografischer Länder Standort des Partners |

**Microsoft Learn**: die Daten Definitionen der verschiedenen Felder des Microsoft Learn Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|UserName|Name des Benutzers| 
|UserId|Benutzer-GUID |
|Trainingname|Name der Schulung |
|Trainingtype|Trainingsart (Modul/Learning Pfad)|
|Produkte|Das Produkt, für das das Lernmodul anwendbar ist.|
|Rollen|Anwendbare Rollen des Trainings |
|Completiondate|Datum der Beendigung des Trainings |
|MPNId|Microsoft Partner Network-ID |
|PartnerName|Name des Partners |
|Land|Geografischer Länder Standort des Partners |

**Kompetenz Zusammenfassung und Verlauf**: die Datendefinition der verschiedenen Felder der Zusammenfassung der Kompetenz und des Verlaufs Berichts lautet:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|Competencyname|Der Name der Kompetenz. |
|Competencylevel|Grad der Kompetenz (Gold/Silver)|
|Competencystatus|Aktueller Status der Kompetenz (aktiv/inaktiv/in der Toleranz Periode)|
|Competencystartdate|Start Datum der angegebenen Kompetenz| 
|Competencyenddate|Enddatum der angegebenen Kompetenz |

**Kompetenz Leistung**: die Daten Definitionen der verschiedenen Felder des Kompetenz Leistungs Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|Competencyname|    Der Name der Kompetenz. |
|Competencyattainmentoptionname|    Name der Option zum Erreichen von Kompetenzen|
|Month (Monat)| Monat, für den die Metriken gemeldet werden|
|MetricName|    Name der Metrik, die für die Kompetenz relevant ist|
|Metricmonthlycontribution| Monatlicher Beitrag der Metrik|
|Ttmaggregate|  Aggregierte Metrik für die nachfolgenden 12 Monate|
|Anniversaryyear-Aggregat|  Aggregierte Metrik für das aktuelle Jahres Jahr|
|Goldthreshold| Leistungsanforderung zum erfüllen der Gold-Kompetenz|
|Silverthreshold|   Leistungsanforderung zum erfüllen der Silver-Kompetenz|

**Cloud-Aufstieg M365 Neigung**: die Daten Definitionen der verschiedenen Felder des cloudaufstiegs M365-neiglichkeits Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner Name|  Name des Partners|
|Customer ID|   Kunden-ID-Nummer |
|DUNS-Nummer|   Die Dun & Bradstreet-Nummer des Kunden, der für die Neigung bewertet wird.|
|Kontoname|  Name des Kontos |
|Domain|    Domäne des Kontos|
|Organisationsgröße|  Organisationsgröße|
|Branche|  Branche  |
|Vertical|  Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft und anderen Industriestandards (D&B) identifiziert|
|Bereich|  Geografischer Bereich des Standorts|
|Niederlassung|    Die Tochtergesellschaft des Kunden, der für die Neigung bewertet wird|
|Sales Territory|   Das Vertriebsgebiet des Kunden, der für die Neigung bewertet wird|
|City|  Standort der geografischen Stadt |
|Staat| Standort des geografischen Zustands|
|Postleitzahl|   Postleitzahl|
|Land|   Geografischer Länder Standort |
|Segment|   Marktsegment |
|Unter Segment|   Markt Subsegment |
|Übersicht über den SMC|  SMC-Typ |
|Oberste nicht verwaltete computebasis|  Top nicht verwaltete Kunden – Compute|
|Oberste nicht verwaltete Benutzerbasis| Top nicht verwaltete Kunden – Benutzer|
|Isnonprofit|   Ob Non-Profit oder Profit (Yes/No)|
|Aktivieren von Remote Arbeit-Ziel Exchange Online|   Kunden, die über ein aktives Exchange Online-Abonnement verfügen, Upselling an M365|
|Aktivieren Sie die Remote Ausführung bei der lokalen Ausführung (aktuelle Version) mit der Clas-Neigung-+ 10-Lizenzen|Kunde, der über aktuelle Office-oder Win-Clients verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde hat 10 oder mehr Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren Sie den lokalen lokalen Arbeits Abruf (aktuelle Version) mit der Clas-<10 Lizenzen.|Kunde, der über aktuelle Office-oder Win-Clients verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde verfügt über weniger als 10 Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren Sie die Remote Ausführung bei der lokalen Ausführung (aktuelle Version) ohne die Verwendung von Clas| Kunde, der über aktuelle Office-oder Win-Clients verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde hat 10 oder mehr Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren Sie die Remote Ausführung bei der lokalen Ausführung (aktuelle Version) ohne die <10 Lizenzen.| Kunde, der über aktuelle Office-oder Win-Clients verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren Sie die Remote Arbeit-on-Prem-Übernahme (EOS) mit der Größe der Clas-und 10-Lizenzen.|Kunde, der EOS in Office oder Win Client hat (also Versionen vor und einschließlich EOS-Produkten). Der Kunde hat 10 oder mehr Lizenzen. Der Kunde hat eine Neigung. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren Sie die Remote Arbeit-on-Prem-Übernahme (EOS) mit der <10-Lizenzen.|Kunde, der EOS in Office oder Win Client hat (also Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat eine Neigung. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren Sie die Aktivierung von lokalem Arbeits-on-Prem-Erwerb (EOS) ohne die Verwendung von Clas und 10 Lizenzen.| Kunde, der über aktuelle Office-oder Win-Clients verfügt (d. h. Versionen vor und einschließlich EOS-Produkten). Der Kunde hat 10 oder mehr Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren von Remote Arbeit-on-Prem-Erwerb (EOS) ohne unter <10 Lizenzen| Kunde, der über aktuelle Office-oder Win-Clients verfügt (d. h. Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über weniger als 10 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten eine Konvertierung in M365 durchsuchen.|
|Aktivieren der Option "Remote Arbeit-hohe Neigung für M365" (jetzt agieren/auswerten)| Interessenten für Kunden mit hoher Neigung für M365.|
|Aktivieren des Remote-Arbeits Wettbewerbs (Zoom) mit M365| Kunden mit Zoom und M365, Ziel für die Konvertierung in Teams|
|Aktivieren von Remote Arbeit-Wettbewerb (Zoom) ohne M365|  Kunden mit Zoom, Ziel für die Konvertierung in Teams|
|Kosten senken und verwalten M365 E3 für M365 E5| Vorhandener Kunde mit M365 E3, Ziel für M365 E5|
|Kosten und Verwaltung senken M365 BB-und BS-Kunden, die auf M365 BP abzielen|    Vorhandene M365 BB-und BS-Kunden, die diese für M365 BP als Ziel haben.|
|Transformieren der Produktivität der Organisation: oberflächenneigung|    Customer zeigt die Neigung der Oberfläche an.|
|M365Cluster|Identifiziert die Neigung des Kunden, M365 zu erwerben.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|M365Fit|   Interne und externe Datenpunkte, die firmugraphics definieren. Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert.|
|M365Intent|    Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren. Die beabsichtigte Bewertung wird monatlich aktualisiert.|
|Surfakecluester|    Dadurch wird die Eignung der Kunden an der Kauf Oberfläche identifiziert, indem die Eignung und die beabsichtigten Empfehlungen in einem Cluster konsolidiert werden.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|"Surfacefit"|    Interne und externe Datenpunkte, die firmugraphics definieren. Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert.|
|Surfakeintent| Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren. Die beabsichtigte Bewertung wird monatlich aktualisiert.|
|O365Cluster|   Dadurch wird die Neigung des Kunden für den Erwerb von O365 identifiziert.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|O365Fit|   Interne und externe Datenpunkte, die firmugraphics definieren. Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert.|
|O365Intent|    Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren. Die beabsichtigte Bewertung wird monatlich aktualisiert.|
|M365UpsellCustomer|    Dies identifiziert, ob der Kunde Upselling-Neigung für M365 anzeigt.|
|Hat Google|    Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden Google-Produkte anzeigt.|
|Hat AWS|   Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden AWS-Produkte anzeigt.|
|Hat EA|    Hiermit wird ermittelt, ob eine Erneuerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist.|
|Hat geöffnet|  Hiermit wird angegeben, ob eine Erneuerung eine offene oder eine Open Value-Vereinbarung ist.|

**Cloud-Aufstieg D365 Neigung**: die Daten Definitionen der verschiedenen Felder des cloudaufstiegs D365-neiglichkeits Berichts lauten:

| **Spaltenname** | **Daten Beschreibung** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner Name|  Name des Partners|
|Customer ID|   Kunden-ID-Nummer |
|DUNS-Nummer|   Die Dun & Bradstreet-Nummer des Kunden, der für die Neigung bewertet wird.|
|Kontoname|  Name des Kontos |
|Domain|    Domäne des Kontos|
|Organisationsgröße|  Organisationsgröße|
|Branche|  Branche  |
|Vertical|  Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft und anderen Industriestandards (D&B) identifiziert
|Bereich|  Geografischer Bereich des Standorts|
|Niederlassung|    Die Tochtergesellschaft des Kunden, der für die Neigung bewertet wird|
|Sales Territory|   Sales Territory|
|City|  Standort der geografischen Stadt |
|Staat| Standort des geografischen Zustands|
|Postleitzahl|   Postleitzahl|
|Land|   Geografischer Länder Standort |
|Segment|   Marktsegment |
|Unter Segment|   Markt Subsegment |
|Übersicht über den SMC|  Die Kategorisierung eines Kunden: die obersten, nicht verwalteten Benutzer Basen sind Kunden mit mehr als 300 Mitarbeitern, die wichtigste nicht verwaltete computebasis sind Kunden mit einer Kapazität von 10.000 US-Dollar in Azure 3 Jahren, mittelständische Unternehmen sind Kunden mit 25 Mitarbeitern oder mehr, kleine Unternehmen sind Kunden mit weniger als 25 Mitarbeitern.|
|Oberste nicht verwaltete computebasis   |Top nicht verwaltete Kunden – Compute|
|Oberste nicht verwaltete Benutzerbasis| Top nicht verwaltete Kunden – Benutzer|
|Isnonprofit|   Ob Non-Profit oder Profit (Yes/No)|
|Aktivieren des Digital Selling-M365-Seat-Größen >= 25 Arbeitsplätze (SalesPro-neiglichkeits Modell)|   Customer ohne D365. Arbeitsplatz Größe: 25 +. Partner sollten auf den Cross-Selling von D365 SalesPro abzielen|
|Aktivieren von Digital Selling-D365 SalesPro-Neigung (jetzt agieren/auswerten) |Kunden mit hoher Neigung ohne D365.  Partner sollten auf D365 SalesPro abzielen.|
|Verwalten von Finanzrisiken & Betrugs basierte Dynamics-Installation Base-Navision (BC-neiglichkeits Modell)|Vorhandener Kunde mit lokalem Navision.  Partner sollte auf D365 BC abzielen|
|Verwalten von Finanzrisiken & "Betrugs basierte Dynamics-Installation" Base-AX (F&O-neiglichkeits Modell)    |Vorhandener Kunde mit lokalem AX.  Partner sollte auf D365 F&O abzielen|
|Verwalten von Finanzrisiken & "Betrug-Dynamics on-Prem Installation Base-Great Plains" (BC-neiglichkeits Modell)|  Vorhandener Kunde mit einer hervorragend großen Ebene.  Partner sollte auf D365 BC abzielen|
|Verwalten von Finanzrisiken & Betrugs basierte Dynamics-Installation Base-Solomon (BC-neiglichkeits Modell)|Vorhandener Kunde mit lokalem Solomon.  Partner sollte auf D365 BC abzielen|
|Verwalten von Finanzrisiken & "Betrug-Dynamics on-Prem Installation Base-andere" (BC-neiglichkeits Modell) |Vorhandener Kunde mit anderen lokalen Lösungen, die oben nicht aufgeführt sind.  Partner sollte auf D365 BC abzielen|
|Erstellen von Agile-Geschäftsprozessen: Dynamics-lokale Installation Basis-AX/GP/SL/NAV/other (D365-Modell Modell)|   Erstellen von Agile-Geschäftsprozessen: Dynamics-lokale Installation Basis-AX/GP/SL/NAV/other (D365-Modell Modell)|
|Entwickeln von Agile-Geschäftsprozessen-Dynamics konkurrierende Basis-mendix/Outsystems/Salesforce (D365-Modell Modell)| Entwickeln von Agile-Geschäftsprozessen-Dynamics konkurrierende Basis-mendix/Outsystems/Salesforce (D365-Modell Modell)|
|Erstellen von Agile-Geschäftsprozessen D365 F&O-Installationsbasis |Vorhandene D365 F&O-Kunden.  Partner für Power apps.|
|Erstellen von Agile-Geschäftsprozessen D365 BC-Installationsbasis| Vorhandene D365 BC-Kunden. Partner für Power apps.|
|Erstellen von Agile-Geschäftsprozessen D365 CE-Installationsbasis| Vorhandene D365 CE-Kunden. Partner für Power apps.|
|Erstellen einer robusten Lieferkette: gewinnen und aktivieren Sie zuerst D365 Workloads als D365 Lieferkette mit nicht-Oracle/SAP ERP-Kunden|  Zielkunden für die D365-Lieferkette.|
|Erstellen Sie eine robuste Lieferkette, Cross-Selling D365 Lieferkette und/oder Einzelhandel/Handel für vorhandene D365 CE-Kunden |Vorhandene D365 CE-Kunden, die für Cross Selling D365 Supply Chain als Ziel haben|
|Erstellen Sie eine robuste Lieferkette, Cross-Selling D365 sup. Kette und/oder Retail/Commerce zu D365 CE und (Oracle oder SAP)| Vorhandene D365 CE-Kunden mit Oracle oder SAP als Ziel für die D365-Lieferkette|
|D365BCCluster| Dies identifiziert die Neigung des Kunden, D365 Business Central zu erwerben.  Kunden, die eine Neigung für BC darstellen, werden in den Kategorien Mittel und klein angezeigt.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|D365BCFit| Interne und externe Datenpunkte, die firmugraphics definieren. Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert.|
|D365BCIntent|  Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren. Die beabsichtigte Bewertung wird monatlich aktualisiert.|
|D365FOCluster| Dies identifiziert die Neigung des Kunden, D365 Finanzen und Vorgänge zu erwerben.  Kunden, die eine Neigung für F&O darstellen, werden in den obersten nicht verwalteten Kategorien angezeigt. Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|D365FOFit| Interne und externe Datenpunkte, die firmugraphics definieren. Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert.|
|D365FOIntent|  Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren. Die beabsichtigte Bewertung wird monatlich aktualisiert.|
|D365CECluster| Dies identifiziert die Kunden Neigung D365 Kunden Engagement.  Kunden, die die Neigung für CE sehen, werden in den Kategorien Mittel und klein angezeigt.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|D365CEFit| An D365 CE anpassen|
|D365CEIntent|  Absicht für D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Hiermit wird festgelegt, ob ein Kunde über eine offene Erneuerung für Dynamics on-Prem AX oder CRM verfügt.|
|M365UpsellCustomer|    Dies identifiziert, ob der Kunde Upselling-Neigung für M365 anzeigt.|
|Hat Google|    Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden Google-Produkte anzeigt.|
|Hat AWS|   Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden AWS-Produkte anzeigt.|
|Hat EA |Hiermit wird ermittelt, ob eine Erneuerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist.|
|Hat geöffnet|  Hiermit wird angegeben, ob eine Erneuerung eine offene oder eine Open Value-Vereinbarung ist.|

**Cloud-Ascent-Azure Neigung**: die Daten Definitionen der verschiedenen Felder des Cloud Ascent-Azure-Diensts lauten:

|**Spaltenname** |**Daten Beschreibung** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner Name|  Name des Partners|
|Customer ID|   Kunden-ID-Nummer |
|DUNS-Nummer|   Die Dun & Bradstreet-Nummer des Kunden, der für die Neigung bewertet wird.|
|Kontoname|  Name des Kontos |
|Domain|    Domäne des Kontos|
|Organisationsgröße|  Organisationsgröße|
|Branche|  Branche  |
|Vertical|  Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft und anderen Industriestandards (D&B) identifiziert|
|Bereich|  Geografischer Bereich des Standorts|
|Niederlassung|    Die Tochtergesellschaft des Kunden, der für die Neigung bewertet wird|
|Sales Territory|   Sales Territory|
|City|  Standort der geografischen Stadt |
|Staat| Standort des geografischen Zustands|
|Postleitzahl|   Postleitzahl|
|Land|   Geografischer Länder Standort |
|Segment|   Marktsegment |
|Unter Segment|   Markt Subsegment |
|Übersicht über den SMC|  SMC-Typ |
|Oberste nicht verwaltete computebasis|  Top nicht verwaltete Kunden – Compute|
|Oberste nicht verwaltete Benutzerbasis| Top nicht verwaltete Kunden – Benutzer|
|Isnonprofit|   Ob Non-Profit oder Profit (Yes/No)|
|Migration-EOS Win Server-EOS Windows Server IB mit der Größe von Clas-5 und höher|   Kunde, der über EOS on-Prem Win Server verfügt (d. h. Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über fünf oder mehr Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt.  Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-EOS Win Server-EOS Windows Server IB mit Clas-<5 Lizenzen|   Kunde, der über EOS (End of Service) auf dem lokalen Win-Server verfügt (d. h. Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über weniger als 5 Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt.  Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-EOS Win Server-EOS Windows Server IB ohne die Clas-Neigung-5 + Lizenzen |Kunde, der über EOS on-Prem Win Server verfügt (d. h. Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über mehr als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-EOS Win Server-EOS Windows Server IB ohne Clas-<5 Lizenzen|    Kunde, der über EOS on-Prem Win Server verfügt (d. h. Versionen vor und einschließlich EOS-Produkten). Verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-EOS SQL-EOS SQL Server IB mit der Größe von Clas-5 und höher|  Kunde, der EOS lokal SQL Server (also Versionen vor und einschließlich EOS-Produkten). Der Kunde hat fünf Lizenzen. Der Kunde hat eine Neigung.  Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-EOS SQL-EOS SQL Server IB mit Clas-<5 Lizenzen|  Kunde, der EOS lokal SQL Server (also Versionen vor und einschließlich EOS-Produkten). Verfügt über weniger als 5 Lizenzen. Kunde, der über ein neiglichkeits Ergebnis verfügt. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren-EOS SQL-EOS SQL Server IB ohne die von|   Kunde, der EOS lokal SQL Server (also Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über fünf oder mehr Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-EOS SQL-EOS SQL Server IB ohne Clas-<5 Lizenzen|   Kunde, der EOS lokal SQL Server (also Versionen vor und einschließlich EOS-Produkten). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren von lokalem Win-Server-current Windows Server IB mit der Clas-Neigung-5 + Lizenzen|   Kunde, der über den aktuellen lokalen Win-Server verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde hat fünf Lizenzen. Der Kunde hat eine Neigung. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren von lokalem Win Server-current Windows Server IB mit Clas-<5 Lizenzen|   Kunde, der über den aktuellen lokalen Win-Server verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde verfügt über weniger als 5 Lizenzen. Customer hat eine Neigung für Azure. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren von lokalem Win-Server-Aktuelles Windows Server-IB ohne die Größe der Clas|    Kunde, der über den aktuellen lokalen Win-Server verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde hat fünf Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren von lokalem Win Server-current Windows Server IB ohne Clas-<5 Lizenzen |Kunde, der über den aktuellen lokalen Win-Server verfügt (d. h. Versionen, die nach EOS-Produkten liegen). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren zu Azure SQL-oder SQL-VMS-Current SQL Server IB mit der Größe von Clas-5 und höher|  Kunde, der über aktuelle lokale SQL Server verfügt (d. h. Versionen, die auf EOS-Produkte basieren). Der Kunde hat fünf Lizenzen. Der Kunde hat eine Neigung. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren zu Azure SQL-oder SQL-VMS-Aktuelles SQL Server IB mit "Clas"-<5 Lizenzen|  Kunde, der über aktuelle lokale SQL Server verfügt (d. h. Versionen, die auf EOS-Produkte basieren). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat eine Neigung. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren zu Azure SQL-oder SQL-VMS-Current SQL Server IB ohne die Verb Neigung von Clas-5 und höher|   Kunde, der über aktuelle lokale SQL Server verfügt (d. h. Versionen, die auf EOS-Produkte basieren). Der Kunde hat fünf Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren: Migrieren zu Azure SQL-oder SQL-VMS-Current SQL Server IB ohne die <5 Lizenzen|   Kunde, der über aktuelle lokale SQL Server verfügt (d. h. Versionen, die auf EOS-Produkte basieren). Der Kunde verfügt über weniger als 5 Lizenzen. Der Kunde hat kein neiglichkeits Ergebnis. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-OSS-Migrieren zu OSS DB| Vorhandener Kunde mit einem der folgenden konkurrierenden Produkte: PostgreSQL, MySQL und MariaDB. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-OSS-Linux in Azure |Vorhandener Kunde mit dem Produkt: Linux. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migrieren von SAP-SAP in Azure|  Vorhandener Kunde mit dem Produkt: SAP. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-WVD-RDS-IB |Identifiziert Kunden mit aktiven Windows-Remotedesktopdienste. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-WVD-Cross Selling modern work zu Azure/WVD|   Identifiziert Kunden mit M365 und hat nicht Azure. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-VMware IB|   Vorhandener Kunde mit dem Produkt: VMware. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Migration-Citrix IB|   Vorhandener Kunde mit dem Produkt: Citrix Systems. Partner sollten diese Kunden für die Migration zu Azure als Ziel haben.|
|Innovation-Analytics-Power BI IB w/hohe Azure-Neigung|   Kunden mit und Active Power BI-Abonnement, einschließlich: Power BI eigenständiger pro, Power BI-Azure Suites, Power BI-Office-Suites, Power BI Suites-M365|
|Enable-devops mit GitHub-VisualStudio/MSDN IB|    Identifizierte Kunden mit aktiven Visual Studio-|
|Win Server Standard-Version|   Hiermit wird die Version von Windows Server Standard-Käufen vom Kunden angezeigt.|
|Win Server Standard-Lizenz|   Hiermit wird der Lizenztyp von Windows Server Standard-Käufen durch den Kunden angezeigt.|
|Windows Server-Rechenzentrums Version|    Hiermit wird die Version der Windows-Rechenzentrums Käufe angezeigt, die vom Kunden erworben wurden.|
|Win Server-Daten Center Lizenz| Dies zeigt den Lizenztyp von Windows-Rechenzentrums Käufen, die vom Kunden erworben wurden.|
|Azurefit|  Interne und externe Datenpunkte, die firmugraphics definieren. Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind. Die passingbewertung wird vierteljährlich aktualisiert.|
|Azureintent|   Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt. Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren. Die beabsichtigte Bewertung wird monatlich aktualisiert.|
|Azurecluester|  Dadurch wird die Eignung des Kunden für den Erwerb von Azure identifiziert, indem die Eignung und die beabsichtigten Empfehlungen in einem Cluster konsolidiert werden.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|WindowsServerDataCenter_HasOpenRenewal|    Hiermit wird festgelegt, ob ein Kunde über eine offene Erneuerung für ein Windows Server-Rechenzentrum verfügt.|
|WindowsServerStandard_HasOpenRenewal|  Hiermit wird ermittelt, ob ein Kunde eine offene Erneuerung für einen Windows Server-Standard hat.|
|Azureupsellcustomer|   Hiermit wird festgelegt, ob der Kunde Upselling-Neigung für Azure anzeigt.|
|Hat Google|    Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden Google-Produkte anzeigt.|
|Hat AWS|   Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden AWS-Produkte anzeigt.|
|Hat EA |Hiermit wird ermittelt, ob eine Erneuerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist.|
|Hat geöffnet|  Hiermit wird angegeben, ob eine Erneuerung eine offene oder eine Open Value-Vereinbarung ist.|

**Cloud-Ascent-Agreement Erneuerungen von Erneuerungen**: die Daten Definitionen der verschiedenen Felder des Berichts für die Verlängerung der Cloud-Aufstiegs Vereinbarung lauten:

|**Spaltenname** |**Daten Beschreibung** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner Name|  Name des Partners|
|Customer ID|   Kunden-ID-Nummer |
|DUNS-Nummer|   Die Dun & Bradstreet-Nummer des Kunden, der für die Neigung bewertet wird.|
|Kontoname|  Name des Kontos |
|Domain|    Domäne des Kontos|
|Organisationsgröße|  Organisationsgröße|
|Branche|  Branche  |
|Vertical|  Die vertikale der Kunden, die für die Neigung bewertet werden, wie von Microsoft und anderen Industriestandards (D&B) identifiziert|
|Bereich|  Geografischer Bereich des Standorts|
|Niederlassung|    Die Tochtergesellschaft des Kunden, der für die Neigung bewertet wird|
|Sales Territory|   Sales Territory|
|City|  Standort der geografischen Stadt |
|Staat| Standort des geografischen Zustands|
|Postleitzahl|   Postleitzahl|
|Land|   Geografischer Länder Standort |
|Segment|   Marktsegment |
|Unter Segment|   Markt Subsegment |
|Übersicht über den SMC|  SMC-Typ |
|Oberste nicht verwaltete computebasis|  Top nicht verwaltete Kunden – Compute|
|Oberste nicht verwaltete Benutzerbasis| Top nicht verwaltete Kunden – Benutzer|
|Isnonprofit|Ob Non-Profit oder Profit (Yes/No)|
|Hat Google|Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden AWS-Produkte anzeigt.|
|Hat AWS|Dieses Flag gibt an, ob ein Kunde Wettbewerbs Signale für die besitzenden AWS-Produkte anzeigt.|
|Azure-Cluster|Dadurch wird die Kunden Neigung zum Kauf von Azure identifiziert.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|D365 F&O-Cluster|  Dies identifiziert die Neigung des Kunden, D365 Finanzen und Vorgänge zu erwerben.  Kunden, die eine Neigung für F&O darstellen, werden in den obersten nicht verwalteten Kategorien angezeigt.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|D365 CE-Cluster|   Dies identifiziert die Kunden Neigung D365 Kunden Engagement.  Kunden, die die Neigung für CE sehen, werden in den Kategorien Mittel und klein angezeigt.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|D365 BC-Cluster|   Dies identifiziert die Neigung des Kunden, D365 Business Central zu erwerben.  Kunden, die eine Neigung für BC darstellen, werden in den Kategorien Mittel und klein angezeigt.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|M365-Cluster|  Dadurch wird die Neigung des Kunden für den Erwerb von M365 identifiziert.  Cluster werden nun ausgeführt, und die Auswertung sollte als Ziel verwendet werden, um einen höheren Ertrag zu erzielen.  Kunden von Pflege und Ausbildung sollten nur als Ziel verwendet werden, wenn nach der Zielgruppe noch Kapazität besteht und Kunden evaluiert werden.|
|Lizenzprogramm|   Hiermit wird der Lizenz Programmtyp für die Verlängerung identifiziert.|
|Vereinbarungs-ID|  Vertrags Bezeichner|
|Enddatum der Vereinbarung|    Enddatum der Vereinbarung |
|Ablauftyp|   Typ des Ablaufs|
|Ablauf der Einnahmen|  Umsatz im Zusammenhang mit ablaufenden Abonnements|
|Hat EA|    Hiermit wird ermittelt, ob eine Erneuerung ein Enterprise Agreement (EA) oder ein EA-Abonnement ist.|
|Hat geöffnet|  Hiermit wird angegeben, ob eine Erneuerung eine offene oder eine Open Value-Vereinbarung ist.|
|Azure-Upsell-Kunde| Hiermit wird festgelegt, ob der Kunde Upselling-Neigung für Azure anzeigt.|
|M365 Upsell Customer|  Dies identifiziert, ob der Kunde Upselling-Neigung für M365 anzeigt.|
|Revsumdivisionname|    Hiermit wird das Produkt identifiziert, das für die Verlängerung eingerichtet ist.|

## <a name="next-steps"></a>Nächste Schritte

Berichte finden Sie unter [Herunterladen von Berichten](pci-download-reports.md).
