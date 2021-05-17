---
title: Ankündigungen für März 2021
description: Ankündigungen für März 2021 zum Microsoft Partner Center, einschließlich neuer Funktionen, Promotions, Angebote, Märkte oder Änderungen an bestehenden Angeboten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 3d91eb26f98005b92a48c6f242ea4439e42cde05
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702874"
---
# <a name="march-2021-announcements"></a>Ankündigungen für März 2021

Auf dieser Seite finden Sie die Ankündigungen vom März 2021 für Microsoft Partner Center.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Bereitschaft: Änderungen an der API zur Überprüfung von Kundenadressen im CSP-Programm (Cloud Solution Provider) gehen im Juni online; Testfunktion jetzt verfügbar

### <a name="categories"></a>Kategorien

- Datum: 30.03.2021
- Bereitschaft

### <a name="summary"></a>Zusammenfassung

Damit Partner und Kunden ihre Geschäfte auf Vertrauensbasis tätigen können, laden wir Partner ein, Änderungen an der Adressüberprüfungs-API für alle Länder weltweit zu testen.

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner mit direkter Abrechnung und indirekte Anbieter, die neue Adressdetails für Kunden erstellen oder bestehende Details aktualisieren

### <a name="details"></a>Details

Microsoft setzt auf Vertrauen. Wir haben uns verpflichtet, eine kompatible und sichere Methode der Überprüfung von Kundenadressen zur Abwicklung von Kundenabonnements im CSP-Programm bereitzustellen. Ab dem 31. März 2021 haben wir Änderungen an der Adressüberprüfungs-API eingeführt, die wir gerne von Partnern testen lassen möchten, bevor die Änderungen im Juni 2021 umgesetzt werden.

Änderungen betreffen nur die Adressüberprüfungs-API. Die APIs zum Erstellen von Kunden und Aktualisieren von Abrechnungsprofilen sind nicht betroffen.

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

Nachdem eine Adresse über die Adressüberprüfungs-API zur Überprüfung übermittelt wurde, wird das folgende Antwortschema zurückgegeben:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Sehen Sie sich die folgende Beispielantwort an. Beachten Sie, dass die Antwort für die USA ein zusätzliches vierstelliges Suffix für die Postleitzahl zurückgibt, wenn Sie nur fünf Ziffern für die Postleitzahl eingeben.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Nächste Schritte

- Teilen Sie dem Fachexperten (Ali Khaki) Ihre Sandbox-Mandanten-ID mit, damit Sie in die Testphase einbezogen werden und mit der Vorbereitung für die Aktualisierung beginnen können.

- Wenden Sie sich an Ihren CPV (Control Panel Vendor), wenn Sie eine CPV-Lösung verwenden.

### <a name="questions"></a>Fragen?

Wenn Sie Unterstützung hinsichtlich des Geschäftsbetriebs mit Microsoft benötigen, wenden Sie sich an Ihre Yammer-Gruppe beim Partner-Support.

### <a name="change-log"></a>Änderungsprotokoll:

- 31. März 2020: Erstveröffentlichung

- 30. April 2021: Aktualisierungen der Details zu Beispielantworten und Postleitzahl

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Neue Benutzeroberfläche des Exchange Admin Center (EAC)

### <a name="categories"></a>Kategorien

- Datum: 29.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Ab dem 27. April 2021 führt das Exchange Admin Center (EAC) eine neue Benutzeroberfläche ein, mit der die tägliche Effizienz für Benutzer verbessert wird.

### <a name="impacted-audience"></a>Zielgruppe

Delegierte Administratoren, die über Partner Center auf Exchange zugreifen

### <a name="details"></a>Details

Ab dem 27. April 2021 werden Partner, die über Partner Center zu Exchange navigieren, zum neuen EAC umgeleitet.

Diese neue Oberfläche ist derzeit als Vorschau verfügbar, und Administratoren können sie aktivieren, indem sie im klassischen EAC die Umschaltfläche in der oberen rechten Ecke auswählen. Administratoren können auch zum neuen EAC navigieren, indem sie auf das Banner „Jetzt ausprobieren“ klicken, das auf allen Seiten angezeigt wird.

Das neue EAC bietet unter anderem folgende Vorteile:

- Zusätzliche Einblicke, Berichte und Warnmechanismen für Probleme im Zusammenhang mit dem Nachrichtenfluss 

- Personalisierte Dashboards zur Steigerung der Produktivität

Als Hilfe beim Navigieren durch die neue Benutzeroberfläche stehen Videos im Abschnitt **Schulung und Leitfaden** auf der neuen EAC-Oberfläche bereit. Diese vermitteln Ihnen einen Überblick darüber, wie Sie das neue Portal optimal verwenden können.

>[!NOTE]
>Durch diese Änderung ist die klassische EAC-Oberfläche nicht veraltet. Sie werden rechtzeitig benachrichtigt, bevor eine Änderung implementiert wird.

### <a name="next-steps"></a>Nächste Schritte

- Sehen Sie sich die [Ressourcen zu diesem Thema](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/) an, die Screenshots der neuen Benutzeroberfläche enthalten.

- Leiten Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrem Unternehmen weiter. 

### <a name="questions"></a>Fragen?

Bei Fragen zu diesen Änderungen können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: Neuer Produkteinführungskalender

### <a name="categories"></a>Kategorien

- Datum: 25.03.2021
- Angebote | Moderner Arbeitsplatz

### <a name="summary"></a>Zusammenfassung

Als Reaktion auf das Feedback von Partnern optimiert Microsoft Operations seine Vorgehensweise für Mitteilungen über Produkteinführungen.

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner (Cloud Solution Provider)

### <a name="details"></a>Details

Microsoft ist bestrebt, die Erfahrungen für seine Partner kontinuierlich zu verbessern. Wir haben Feedback von Ihnen erhalten, dass Ihnen zu viele Mitteilungen von Microsoft zugestellt werden, einschließlich doppelter Ankündigungen von Produkteinführungen.

Als Reaktion auf Ihr Feedback hat Microsoft die Readiness-Oberfläche für Produkteinführungen für neue und vorhandene Angebote optimiert.

Wir stellen Ihnen jetzt eine einzige monatliche Ansicht der Produkteinführungen bereit, die im Operations Readiness-Ressourcenkatalog veröffentlicht wird. Dieser monatliche [Produkteinführungskalender](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) ersetzt einzelne Mitteilungen über Produkteinführungen im Operations Readiness-Ressourcenkatalog und in Partner Center-Ankündigungen.

Sie können auf diesen [Produkteinführungskalender](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) auch über [Communitysammlungen](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [Kalenderansichten](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) und [CSP-Newsletter](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) zugreifen. Wir benachrichtigen Sie, wenn wir den Produkteinführungskalender für einen Monat veröffentlichen, mit einer Ankündigung im Operations Readiness-Ressourcenkatalog.

Informationen zu neuen und vorhandenen Angeboten stehen Ihnen weiterhin in der Preislistenvorschau und den Preislisten-Änderungsprotokollen sowie in Produktblogs, Lizenzierungsleitfäden und auf den Seiten des Produktmarketing zur Verfügung.

Die Änderung betrifft Einführungen für die folgenden Produkte:

- Lokales Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- Tools
- Teams und Telco

Wir senden weiterhin spezifische Ankündigungen für Produkteinführungen, für die Operations Readiness-Details erforderlich sind.

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Änderungen der Anforderungen für das Onboarding von Kunden im CSP-Programm

### <a name="categories"></a>Kategorien

- Datum: 25.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Im Rahmen unserer Verpflichtung, Partner und Kunden bei der Ausführung ihrer Geschäfte auf Vertrauensbasis zu unterstützen, werden wir ab dem 25. März 2021 zusätzliche Kundeninformationen anfordern.

### <a name="impacted-audience"></a>Zielgruppe

CSP-Partner (Cloud Solution Provider) mit direkter Abrechnung und indirekte Anbieter mit neuen Kunden oder Bestandskunden in den im nächsten Abschnitt aufgeführten Ländern

### <a name="details"></a>Details

Microsoft setzt auf Vertrauen. Wir haben uns verpflichtet, eine kompatible und sichere Methode der Kundenüberprüfung zur Abwicklung von Kundenabonnements im CSP-Programm bereitzustellen. Am 25. März 2021 werden wir Verbesserungen der Partner Center-API und -Benutzeroberfläche (UI) einführen, die sich auf Partner auswirken, die die beiden folgenden Kriterien erfüllen:

1. Der Partner hat eine direkte Abrechnungsbeziehung mit Microsoft (das heißt, er ist ein Partner mit direkter Abrechnung oder ein indirekter Anbieter).

2. Der Partner tätigt Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern:

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

Partner, die diese Kriterien erfüllen, müssen beim Onboarding neuer Kunden oder beim Ändern von Bestandskundendetails die **Firmenregistrierungs-ID** des Kunden (auch als **Organisations-INN** des Kunden bezeichnet) und dessen **Telefonnummer** übermitteln. Diese Partner können auch einen optionalen **zweiten Vornamen** für den Kunden eingeben.

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

Partner mit Kunden in anderen Ländern weltweit haben am 25. März 2021 die Möglichkeit, die **Firmenregistrierungs-ID**, die **Telefonnummer** und den **zweiten Vornamen** für Kunden als optionale Details einzugeben.

### <a name="next-steps"></a>Nächste Schritte

- Ausführlichere Anleitungen finden Sie in der technischen Dokumentation und unter den häufig gestellten Fragen in der [jeweiligen Sammlung für Partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).

- Bereiten Sie die Einbindung der Änderungen mithilfe der Partner Center-API und der Webbenutzeroberfläche vor. API/SDKs werden zu Testzwecken bereitgestellt.

- Stellen Sie sicher, dass Sie beim Onboarding neuer Kunden oder beim Ändern von Bestandskundendetails die zusätzlichen Daten übermitteln.

- Wenden Sie sich an Ihren CPV (Control Panel Vendor), wenn Sie eine CPV-Lösung verwenden.

### <a name="questions"></a>Fragen?

Wenn Sie Fragen im Bezug auf die rechtliche Identifizierung (auch INN oder TIN genannt) haben, wenden Sie sich an Ihren Steuerberater oder das örtliche Finanzamt. Microsoft kann in Steuerfragen keine Hilfestellung bieten.

Wenn Sie Unterstützung hinsichtlich des Geschäftsbetriebs mit Microsoft benötigen, [erstellen Sie eine Serviceanfrage](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Korrekturen an der Preisliste für unbefristete Software vom 1. März 2021

### <a name="categories"></a>Kategorien

- Datum: 23.03.2021
- Angebote/Märkte

### <a name="impacted-audience"></a>Zielgruppe

Indirekte Anbieter und Partner mit direkter Abrechnung, die Transaktionen für unbefristete Software im Cloud Solution Provider-Programm durchführen 

### <a name="details"></a>Details

Die Preisliste für unbefristete Software, die am 1. März 2021 veröffentlicht wurde, umfasste Märkte, die nicht hätten enthalten sein dürfen. Die Preisliste für unbefristete Software wurde am 17. März 2021 mit Korrekturen aktualisiert. Diese Korrekturen betrafen ausschließlich Folgendes:

- Produkt-ID: DF77X4D43RKT 
- Produktname: Upgrade von Windows 10 Home auf Pro für Microsoft 365 Business
- Entfernte oder nicht unterstützte Märkte: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Diese Änderungen gelten nur für das oben genannte Produkt. Für andere Produkte wurden keine Korrekturen vorgenommen. 

### <a name="next-steps-and-resources"></a>Nächste Schritte und zusätzliche Ressourcen

- Partner, die Transaktionen für unbefristete Software durchführen, sollten die neueste Preisliste für unbefristete Software herunterladen.
- Eine übersichtliche Zuordnung der Abkürzungen mit zwei Buchstaben zu Ländern finden Sie unter den [Länder- und Regionscodes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries).
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-Release für .NET Standard (v1.17.0)

### <a name="categories"></a>Kategorien

- Datum: 23.03.2021

- Funktionen
 
### <a name="impacted-audience"></a>Zielgruppe

Partner mit direkter Abrechnung und indirekte Anbieter, die am CSP-Programm teilnehmen und das Partner Center .NET SDK verwenden

### <a name="details"></a>Details

Ab dem 23. März 2020 können Partner mit dem Herunterladen der Version von [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) zusammen mit aktualisierten [GitHub-Beispielen](https://github.com/Microsoft/Partner-Center-DotNet-Samples) für das öffentliche Partner Center SDK beginnen. Diese Version enthält Updates für die folgenden Methoden:

#### <a name="audit-updated-new-operation-types"></a>Überwachung aktualisiert: Neue Vorgangstypen

Es wurden neue [Vorgangstypen](https://docs.microsoft.com/partner-center/develop/auditing-resources) hinzugefügt, um zu wissen, wann der Kunde DAP genehmigt und beendet hat.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Überwachung aktualisiert: Neue Ressourcen- und Vorgangstypen

Es wurden neue [Ressourcen- und Vorgangstypen](https://docs.microsoft.com/partner-center/develop/auditing-resources) zur Unterstützung des Szenarios „Kundenverzeichnisrolle“ hinzugefügt.

- Neuer Ressourcentyp „CustomerDirectoryRole“

- Vorgangstypen „AddUserMember“ and „RemoveUserMember“

#### <a name="sdk-updates-to-customer-accounts"></a>SDK-Updates für Kundenkonten

- Unterstützung für GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Weitere Änderungen

Die folgenden Änderungen werden im Rahmen des neuen E-Commerce-Verfahrens eingeführt und stehen derzeit nur per Einladung für Partner zur Verfügung, die an der Technical Preview des neuen E-Commerce-Verfahrens für M365/D365 teilnehmen. Partner, die nicht an der Technical Preview des neuen E-Commerce-Verfahrens teilnehmen, sollten keine Auswirkungen bemerken, und es sollte Abwärtskompatibilität bestehen.

- Katalogänderungen:

  - GET /products/{product-id}/skus/{sku-id}

- Erwerb und Verwaltung:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Nächste Schritte

- Herunterladen der neuesten Version von [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Herunterladen und Überprüfen der [GitHub-Beispiele](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12">Angebot im kommerziellen CSP-Marketplace und CSP-Incentives im Geschäftsjahr 2021 für berechtigte Angebote</a>

### <a name="categories"></a>Kategorien

- Datum: 18.03.2021
- Funktionen

### <a name="impacted-audience"></a>Zielgruppe

Indirekte Anbieter und Partner mit direkter Abrechnung im Cloud Solution Provider-Programm 

### <a name="details"></a>Details

Indirekte Anbieter und Partner mit direkter Abrechnung im Cloud Solution Provider-Programm können Angebote von Drittanbietern verkaufen und ein Rabattincentive für jedes berechtigte Angebot eines Drittanbieters erhalten, für das Transaktionen in Partner Center oder im Azure-Portal durchgeführt werden. Das Incentive erfolgt in Form eines Rabatts auf die in Rechnung gestellten Verkäufe für berechtigte Angebote und ist **bis zum 30. Juni 2021 verfügbar**.  

Weitere Informationen zu diesem Angebot im kommerziellen CSP-Marketplace finden Sie weiter unten. Nehmen Sie noch heute Kontakt zu Ihren Kunden auf, um die richtigen Angebote für deren weiteren Erfolg und die digitale Transformationen zu ermitteln.

Wir arbeiten eng mit unabhängigen Softwareanbietern (Independent Software Vendors, ISVs) zusammen, um für Microsoft-Kunden die neuesten IaaS-und SaaS-Lösungen auf den Markt zu bringen. ISV-Herausgeber können den Vertrieb ihrer Angebote über den Microsoft-Partnerkanal ermöglichen. Unsere für Incentives berechtigten Angebote fallen unter zwei Kategorien:

- Ausgewählte SaaS- und IaaS-Angebote von Drittanbietern mit Incentivestatus für Azure-IP-Co-Selling 

- SaaS-Anwendungen, die in Teams oder mindestens zwei Microsoft 365-Produktivitäts-Apps integriert sind, z. B. PowerPoint, Word, Excel, Outlook oder SharePoint

### <a name="next-steps-and-resources"></a>Nächste Schritte und zusätzliche Ressourcen

- Erfahren Sie, wie Sie [Partnerincentives](https://partner.microsoft.com/membership/partner-incentives) für den Verkauf berechtigter Marketplace-Apps (für Incentive-berechtigte Apps) erhalten. Es werden monatlich neue Angebote hinzugefügt.  
- [Incentiveressourcen für Partner mit direkter Abrechnung im Cloud Solution Provider-Programm](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Incentiveressourcen für indirekte Anbieter im Cloud Solution Provider-Programm](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Sehen Sie sich diese [Präsentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) an, um mehr über das Verkaufen von Apps im kommerziellen Marketplace zu erfahren. Weitere Ressourcen finden Sie [hier](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Erkunden Sie den Katalog des kommerziellen Marketplace in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) oder im [Azure-Portal](https://ms.portal.azure.com/#home).
- Verwenden Sie [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) zum Integrieren von Apps in den Marketplace Ihres Unternehmens.
- Wenden Sie sich an ISVs, mit denen Sie geschäftlich tätig werden möchten.
- Indirekte Anbieter müssen über APIs integriert werden und Wiederverkäufern Anleitungen dazu geben, welche Apps verkauft werden sollen.

### <a name="questions"></a>Haben Sie Fragen?  

In [diesem Artikel](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) finden Sie eine Übersicht über den kommerziellen Marketplace in Partner Center.

Wenn Sie weitere Unterstützung benötigen, können Sie eine Supportanfrage in Partner Center erstellen. Weitere Informationen finden Sie unter [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11">Aktualisierung der Benennung und erforderlichen Komponenten für Power BI Premium-Angebote</a>

### <a name="categories"></a>Kategorien

- Datum: 18.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Die endgültige Preisliste für den 1. April 2021 wird aktualisiert, um für Klarheit bei der Benennung und/oder den erforderlichen Komponenten für Angebote der Power BI Premium-Einzelbenutzerlizenz zu sorgen.

### <a name="impacted-audience"></a>Zielgruppe

Direkte und indirekte CSP-Partner (Cloud Solution Provider)

### <a name="details"></a>Details

Die endgültige Preisliste für den 1. April 2021 wird aktualisiert, um für Klarheit bei der Benennung und/oder den erforderlichen Komponenten für Angebote der Power BI Premium-Einzelbenutzerlizenz zu sorgen.

Verwenden Sie bis zur Aktualisierung der endgültigen Preisliste die Informationen in diesem Abschnitt, um sicherzustellen, dass das richtige Produkt bestellt wird.

Die folgenden Angaben umfassen die betroffene SKU und Informationen zu den erforderlichen Komponenten.

| Angebotsanzeigename in der Preislistenvorschau vom 1. März |  Aktualisierter Angebotsanzeigename in der endgültigen Preisliste für den 1. April| Angebots-ID |
| ------ | ----------- | ----------- |
| Power BI Premium-Einzelbenutzerlizenz-Add-On (Preise für Mitarbeiter gemeinnütziger Organisationen)  |  Power BI Premium-Einzelbenutzerlizenz-Add-On **(Office)** (Preise für Mitarbeiter gemeinnütziger Organisationen)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Für den Erwerb dieses Angebots benötigen Kunden eine der folgenden erforderlichen Komponenten:

| Angebotsanzeigename | Angebots-ID |
| ------ | ----------- |
| Microsoft 365 E5 (Preise für Mitarbeiter gemeinnütziger Organisationen)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 ohne Audiokonferenz (Preise für Mitarbeiter gemeinnütziger Organisationen)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (Preise für Mitarbeiter gemeinnütziger Organisationen)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5-Testversion (Preise für Mitarbeiter gemeinnütziger Organisationen)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 ohne Audiokonferenz (Preise für Mitarbeiter gemeinnütziger Organisationen)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Für den Erwerb des folgenden Power BI Premium-Angebots muss eine erforderliche Komponente vorhanden sein:

| Angebotsanzeigename | Angebots-ID |
| ------ | ----------- |
|   Power BI Premium-Einzelbenutzerlizenz-Add-On (Preise für Mitarbeiter gemeinnütziger Organisationen)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Für den Erwerb dieses Angebots benötigen Kunden die folgende erforderliche Komponente:

| Angebotsanzeigename | Angebots-ID |
| ------ |----------|
| Power BI Pro (Preise für Mitarbeiter gemeinnütziger Organisationen)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.  

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"> Aktualisierungen der Preise im März für Microsoft 365 F3</a>

### <a name="categories"></a>Kategorien

- Datum: 16.03.2021
- Angebote/Märkte

### <a name="summary"></a>Zusammenfassung

Falsche Preise für Microsoft 365 F3 in britischen Pfund (GBP) und Euro (EUR) im März 2021 wurden korrigiert.

### <a name="impacted-audience"></a>Zielgruppe

Partner, die zwischen dem 1. und 17. März 2021 Microsoft 365 F3 in GBP oder EUR über das CSP-Programm (Cloud Solution Provider) erworben haben

### <a name="details"></a>Details

Microsoft hat falsche Preise für Microsoft 365 F3 korrigiert. Die falschen Preise betreffen die Währungen GBP und EUR und nur Angebote, die zwischen dem 1. und 17. März 2021 erworben wurden. Die betroffenen Angebote und die entsprechenden Währungen sind nachfolgend aufgeführt. 

| Angebotsname | Währung | Angebots-ID | Materialkennung |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Wohltätigkeitsorganisationen) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Kommerziell) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Die lizenzbasierten Vorschaupreislisten für März und April wurden am 16. März um 17:00 Uhr (PST) aktualisiert.

### <a name="next-steps"></a>Nächste Schritte

- Partner sollten die aktuellen lizenzbasierten Preislisten (sowohl die Vorschaupreisliste für März als auch April) mit diesen Preiskorrekturen ggf. erneut herunterladen.  
- Microsoft wird in den kommenden Wochen per E-Mail Kontakt mit den betroffenen Partnern aufnehmen, um sie über die weiteren Schritte zur Korrektur betroffener Transaktionen zu informieren.

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Aktualisieren eines rechtlichen Firmennamens über Partner Center

### <a name="categories"></a>Kategorien

- Datum: 16.03.2021
- Fördern von Effizienz und Skalierung

### <a name="summary"></a>Zusammenfassung

Ab März 2021 können MPN-Partner (Microsoft Partner Network) und indirekte Wiederverkäufer im CSP-Programm (CSP Indirect Reseller) ihren rechtlichen Firmennamen über Partner Center aktualisieren.

### <a name="impacted-audience"></a>Zielgruppe

MPN-Partner und indirekte Wiederverkäufer im CSP-Programm (gilt nicht für CSP-Partner mit direkter Abrechnung)

### <a name="details"></a>Details

Ab März 2021 können MPN-Partner und indirekte Wiederverkäufer im CSP-Programm ihren rechtlichen Firmennamen über Partner Center auf konforme, selbstständige Weise aktualisieren. Aufgrund dieser neuen Funktion müssen Partner kein Partner Center-Supportticket mehr einreichen, um ihren Firmennamen zu aktualisieren. So können Partner bei diesen Aktivitäten viel Zeit einsparen. 

Weitere Informationen finden Sie unter [Aktualisieren des rechtlichen Geschäftsprofils](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Vergewissern Sie sich, dass der Firmenname in Ihrem Rechtsgeschäftsprofil keine Rechtschreibfehler und Abkürzungen enthält und den formalen Geschäftsregistrierungsdatensätzen Ihres Unternehmens exakt entspricht. Weitere Informationen zum Aktualisieren Ihres Organisationsprofils finden Sie unter [Überprüfen von Organisationsprofilen](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Nächste Schritte

Leiten Sie diese Informationen an das geeignete Team in Ihrem Unternehmen weiter, damit es seine Prozesse überprüfen und aktualisieren kann.

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Neuerungen bei der Weiterentwicklung des CSP-Programms (Cloud Solution Provider) und Änderungen des Open License-Programms

### <a name="categories"></a>Kategorien

- Datum: 15.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Das CSP-Programm (Cloud Solution Provider) wird um neue Angebote für unbefristete Software für den kommerziellen und öffentlichen Sektor erweitert, und es werden Änderungen am Open Licensing-Programm vorgenommen.

### <a name="impacted-audience"></a>Zielgruppe

Vertriebshändler und verwaltete Vertriebspartner, die Verkäufe über das Open License-Programm tätigen, sowie alle CSP-Partner, die Transaktionen für unbefristete Software durchführen

### <a name="details"></a>Details

Im September 2020 [kündigte Microsoft eine Reihe von Schritten auf einem Weg der digitalen Transformation an](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/), um die Verkaufschancen für Partner im CSP-Programm zu erweitern, einschließlich der Verfügbarkeit lokaler Software für Partner. Diese Änderungen ermöglichen es Partnern, ihre Geschäfte auszubauen und ihre Reichweite auszudehnen, indem sie Softwarelizenzen in CSP nutzen und sich so erfolgreich in der heutigen cloudzentrierten Welt positionieren. Darüber hinaus wird den Kunden der Übergang in die Cloud erleichtert, während Partner die Flexibilität erhalten, die sie für Hybrid Cloud-Umgebungen der Kunden benötigen.

In Fortführung dieser digitalen Transformation kündigen wir die folgenden Änderungen an:

- 1\. Juli 2021: Der Preisliste für das Open License-Programm werden keine neuen SKUs, Produkte oder Promotions hinzugefügt.

- 7\. Juli 2021: Zwei kommerzielle Angebote, Get Genuine Windows und Visual Studio Professional, sowie Angebote für den öffentlichen Sektor (Behörden, Bildungseinrichtungen und gemeinnützige Organisationen – siehe [Ankündigung](./2020-december.md#9)) werden der CSP-Preisliste für unbefristete Software hinzugefügt.  Die Preisliste ist im Abschnitt „Software“ der Seite [Verkaufen > Preise und Angebote](https://partnercenter.microsoft.com/pcv/sales) in Partner Center zu finden und wird an diesem Datum neu veröffentlicht.

Ausführliche Informationen zur Weiterentwicklung des CSP-Programms und den Änderungen des Open License-Programms sind im folgenden Abschnitt **Nächste Schritte** angegeben.

### <a name="next-steps"></a>Nächste Schritte:

- Weiterentwicklung des CSP-Programms: Sehen Sie sich die Readiness-Materialien für [unbefristete Software im Cloud Solution Provider-Programm](https://partner.microsoft.com/resources/collection/software-in-csp#/) an. Verwenden Sie diese [Readiness-Karte](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf), um schnell die richtigen Informationen für Ihre Rolle zu finden.

- Änderungen des Open License-Programms: Sehen Sie sich die Readiness-Materialien zur [Weiterentwicklung des CSP-Programms und Änderungen des Open License-Programms](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) an. Verwenden Sie diese [Readiness-Karte](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf), um schnell die richtigen Informationen für Ihre Rolle zu finden.

### <a name="questions"></a>Fragen

Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Aktualisierung einer früheren Ankündigung: Premiumbewertungen, ein Add-On für Compliance Manager

### <a name="categories"></a>Kategorien

- Datum: 15.03.2021
- Umsatzsteigerung

### <a name="summary"></a>Zusammenfassung

Die Testangebote hätten nicht in der Preisliste aufgeführt werden sollen und werden entfernt.

### <a name="impacted-audience"></a>Zielgruppe

Partner, die Transaktionen im Rahmen des Cloud Solution Provider-Programms ausführen

### <a name="details"></a>Details

Die Testangebote hätten nicht in die Preisliste aufgenommen werden sollen. Sie werden aus der Preisliste für den 1. Mai 2021 entfernt.

Die ursprüngliche Ankündigung finden Sie [hier](./2021-february.md#4).

### <a name="additional-resources"></a>Zusätzliche Ressourcen

- [Microsoft 365 E5 Security & Compliance](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Erstellen und Verwalten von Bewertungen in Microsoft Compliance Manager – Microsoft 365 Compliance](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrieren Ihrer Lösungen von der OCP-Markteinführung (One Commercial Partner GTM) zum kommerziellen Microsoft-Marketplace

### <a name="categories"></a>Kategorien

- Datum: 12.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Ab dem 29. März 2021 können Sie nur eingeschränkte Markteinführungsfunktionen (GTM) in One Commercial Partner (OCP) nutzen. Es wird empfohlen, Ihre Lösungen zum kommerziellen Marketplace in Partner Center zu migrieren.

### <a name="impacted-audience"></a>Zielgruppe

Organisationen, die Co-Selling-Aktivitäten für Lösungen in OCP GTM durchführen

### <a name="details"></a>Details

Im Dezember 2020 haben wir unseren Weg vom Microsoft OCP GTM-Tool zum kommerziellen Microsoft-Marketplace in Partner Center begonnen. Durch diese Umstellung werden die Funktionen des kommerziellen Marketplace erweitert, in dem Sie Ihre Lösungen Millionen von Kunden präsentieren, Verkaufschancen mit anderen Verkäufern von Microsoft und Partnern gemeinsam nutzen sowie innovative Lösungen gemeinsam anbieten können.

Der nächste Meilenstein dieser Umstellung erfolgt am 29. März 2021. Ab diesem Zeitpunkt können Sie nur eingeschränkte GTM-Funktionen in OCP nutzen, wobei dann einige Felder schreibgeschützt sind. Wenn Sie derzeit Co-Selling-Aktivitäten für Lösungen in OCP GTM durchführen, wird empfohlen, Ihre Lösungen zum kommerziellen Marketplace zu migrieren, um von den dessen Funktionen zu profitieren und ihre Veröffentlichungsvorgänge zu vereinfachen. 

Durch den Wechsel zum kommerziellen Marketplace wird Partner Center das primäre Ziel für Co-Selling-Veröffentlichungen. Dort können Sie Ihr Geschäft weiter ausbauen, indem Sie Ihre Lösungen mit unseren gemeinsam Kunden über dieselben Kanäle und produktinternen Funktionen verbinden, die wir für Microsoft-Produkte nutzen. [Weitere Informationen zum kommerziellen Marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Nächste Schritte

- Wenn Sie Ihre Lösungen noch nicht verschoben haben, befolgen Sie die Anweisungen im [Leitfaden für den Übergang](/azure/marketplace/co-sell-solution-migration), oder sehen Sie sich das [Videotutorial mit Schritt-für-Schritt-Anleitungen](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) an, um alle Migrationsaktivitäten durchzuführen und mit der Veröffentlichung Ihrer Lösungen im kommerziellen Marketplace zu beginnen.

- Fragen zur eingeschränkten Funktionsweise von OCP GTM finden Sie unter den [häufig gestellten Fragen zu Co-Selling-Anforderungen für die Veröffentlichung im kommerziellen Microsoft-Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Siehe Abschnitt „Eingeschränkte GTM-Funktionen in OCP ab 29. März 2021“.)

### <a name="questions"></a>Haben Sie Fragen?

Wenn Sie Fragen haben oder weitere Informationen benötigen, wenden Sie sich an den [Support](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Ausweitung des neuen E-Commerce-Verfahrens im CSP-Programm (Cloud Solution Provider) für Azure auf Russland

### <a name="categories"></a>Kategorien

- Datum: 10.03.2021
- Funktionen

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner in Russland, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details

Wir freuen uns, die Verfügbarkeit des **neuen E-Commerce-Verfahrens in CSP für Azure in Russland** ab dem 10. März 2021 ankündigen zu können. Dieses Verfahren optimiert die Art und Weise, wie Kunden Azure-Dienste kaufen und nutzen. Außerdem erhalten Partner im CSP-Programm einen konsistenten Überblick über Azure-Preise in allen Vertriebsprozessen, Preise in USD für globale Konsistenz, Anpassung des Abrechnungsdatums und Zugriff auf Azure Cost Management.

### <a name="next-steps"></a>Nächste Schritte

Es stehen mehrere Ressourcen zur Einführung des neuen E-Commerce-Verfahrens für Azure sowie zusätzliche Informationen zur Verfügung. Im [Ressourcenkatalog für CSP-Programmupdates](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/) finden Sie die neuesten häufig gestellten Fragen, Foliensätze, Videos und mehr.

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Softwarelizenzschlüssel und Softwaredownload in Partner Center

### <a name="categories"></a>Kategorien

- Datum: 04.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Die Partner Center-Funktionen für den Download von Software und Lizenzschlüssel wurden reaktiviert.

### <a name="impacted-audience"></a>Zielgruppe

Alle CSP-Partner (Cloud Solution Provider), die Transaktionen für Bestellungen von unbefristeter Software und Serverabonnementsoftware über Partner Center durchführen

### <a name="details"></a>Details

Als Reaktion auf Partnerfeedback werden die Partner Center-Funktionen zum Abrufen von Software und Lizenzschlüsseln für Bestellungen von unbefristeter Software und Serverabonnementsoftware reaktiviert. Sie werden im vorherigen Zustand vor dem Entfernen am 19. Januar 2021 wiederhergestellt. (Weitere Informationen finden Sie in der [Ankündigung](2020-september.md#17).)

Beachten Sie, dass Lizenzschlüssel und Downloadlinks für Software wertvolle und sehr gefragte Ressourcen geistigen Eigentums sind. Wenn diese kompromittiert werden, können die Aktivierungslimits schnell ausgeschöpft sein und eine negative Erfahrung für Kunden und Partner bewirken.

### <a name="next-steps"></a>Nächste Schritte

In den folgenden Ressourcen finden Sie Hinweise zur Verwendung und wichtige Anleitungen zur Verteilung von Softwareschlüsseln:

- [Verkaufen lokaler Software über das CSP-Programm](../csp-on-premise-software.md)
- [Leitfaden zum neuen E-Commerce-Verfahren in Partner Center](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Abschnitt mit **Anleitungen zur Verteilung von Softwareschlüsseln**)

### <a name="questions"></a>Haben Sie Fragen?

Wenn Sie weitere Fragen zu diesem Hinweis haben, können Sie sich an die entsprechende Yammer-Community wenden.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrieren Ihrer Deals aus Partner Sales Connect (PSC) in Partner Center

### <a name="categories"></a>Kategorien

- Datum: 04.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Partner Sales Connect (PSC) wird ab dem 31. März 2021 auf den schreibgeschützten Zugriff umgestellt. Wir empfehlen daher dringend, mit der Migration Ihrer Deals aus PSC in Partner Center zu beginnen.

### <a name="impacted-audience"></a>Zielgruppe

Partner mit Deals in PSC

### <a name="details"></a>Details

Im Rahmen unserer gemeinsamen Verpflichtung zum Wachstum bietet Ihnen **Co-Selling mit Microsoft** die Möglichkeit, **entdeckt zu werden, ihr Fachwissen bereitzustellen und ihre Kundenbasis zu erweitern**, um somit positive Kundenergebnisse zu erzielen. Bei einem durchschnittlichen Angebot, das **3,5-mal schneller** erfolgt als üblich, ermöglicht Ihnen die Verwaltung Ihrer Co-Selling-Aktivitäten in Partner Center den Verkauf über die Kanäle direkter Kunde, Partner und Microsoft-Verkäufer sowie die Verwaltung der gesamten Empfehlungspipeline an einem Ort.

**PSC** wird ab dem **31. März 2021** auf den **schreibgeschützten Zugriff** umgestellt. Wir empfehlen daher dringend, mit dem Wechsel zu Partner Center zu beginnen und dadurch Zugriff auf folgende Funktionsverbesserungen zu erhalten: 

- **Genauere Weiterleitung** der gemeinsam mit Microsoft genutzten Angebote an den richtigen Verkäufer, basierend auf der Art der benötigten Unterstützung
- **Vorabprüfung von Angeboten** auf für Incentives-berechtigte Lösungen und Erfüllung der Kriterien für das ISV Connect-Programm, um den Genehmigungsprozess und den abschließenden Ausführungsnachweis zu vereinfachen
- **Nahtlose Benutzeroberfläche** zum Verwalten all Ihrer Co-Selling-Verkaufschancen und qualifizierten Vertriebsleads an einem Ort

Darüber hinaus wurden kürzlich neue Features in Partner Center hinzugefügt, die Ihnen bei der Umstellung helfen:

- [Massenvorgänge für Co-Selling-Verkaufschancen](../bulk-operations.md)
- [Funktion für die Dealmigration](../psc-to-pc.md) (Abschnitt zur **Migration von PSC-Deals**)

Durch Verwendung der Co-Selling-Funktionalität in Partner Center haben Ihre Vertriebsteams mehr Zeit, sich auf die Pflege von Leads und Verkaufschancen, den Abschluss von Deals und den Aufbau dauerhafter Kundenbeziehungen zu konzentrieren.

### <a name="next-steps"></a>Nächste Schritte

Im [Leitfaden für den Übergang zu Partner Center](../psc-to-pc.md) werden Sie durch die Schritte zum Migrieren Ihrer Deals von PSC zu Partner Center geführt.

### <a name="questions"></a>Haben Sie Fragen?

Bei weiteren Fragen wenden Sie sich an den [Support](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Neue Microsoft Dynamics 365-Produkte und -Angebote ab 1. April 2021

### <a name="categories"></a>Kategorien

- Datum: 04.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Am 1. April 2021 führt Microsoft mehrere neue Produkte und Angebote für das CSP-Programm (Cloud Solution Provider) ein.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details

Am 1. April 2021 führt Microsoft die folgenden neuen Produkte und Angebote ein:

- Power BI Premium-Einzelbenutzerlizenz
- Geografische und Segmenterweiterung der USL für Customer Voice und Marketing

**Power BI Premium-Einzelbenutzerlizenz**

Microsoft führt die ersten Power BI Premium-Angebote mit Einzelbenutzerlizenz ein. Power BI Premium wird derzeit nur in einem Kapazitätskonstrukt verkauft. Die Power BI Premium-Einzelbenutzerlizenz bietet Zugriff auf Enterprise Business Intelligence (BI) und Analysefunktionen. Diese flexible Einzelplatzlizenzierung eignet sich für kleine bis mittelständische Unternehmen.

Weitere Informationen zu diesem Angebot finden Sie in den [Details zum Power BI-Release](/power-platform-release-plan/2020wave2/power-bi/planned-features).


**Angebotsdetails**

Beachten Sie, dass der Angebotsname leicht von der Preislistenvorschau abweicht.

| Angebotsname | Angebots-ID |
| ------ |----------- |
| Power BI Premium-Einzelbenutzerlizenz | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium-Einzelbenutzerlizenz für Lehrpersonal | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium-Einzelbenutzerlizenz für Schüler/Studenten | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium-Einzelbenutzerlizenz (Preise für Mitarbeiter gemeinnütziger Organisationen) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium-Einzelbenutzerlizenz-Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium-Einzelbenutzerlizenz-Add-On für Lehrpersonal | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium-Einzelbenutzerlizenz-Add-On für Schüler/Studenten | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium-Einzelbenutzerlizenz-Add-On (Preise für Mitarbeiter gemeinnütziger Organisationen) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Geografische und Segmenterweiterung der USL für Customer Voice und Marketing**

Im Anschluss an die Einführung im Dezember 2020 wurden die USL-Angebote für Dynamics 365 Customer Voice und Marketing geändert, um neue Länder und weitere SKUs für gemeinnützige Organisationen und Bildungseinrichtungen hinzuzufügen.

| Angebotsname | Angebots-ID |
| ------ |----------- |
| USL für Dynamics 365 Customer Voice (Preise für Mitarbeiter gemeinnütziger Organisationen) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| USL für Dynamics 365 Customer Voice für Lehrpersonal | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Weitere Informationen zu diesen Angeboten finden Sie auf den folgenden Seiten:

- [Homepage von Dynamics 365 Customer Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Homepage von Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Nächste Schritte

Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.  

### <a name="questions"></a>Haben Sie Fragen?

Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft-Lösung für universelles Drucken jetzt in einigen Suites verfügbar

### <a name="categories"></a>Kategorien

- Datum: 03.03.2021
- Funktionen

### <a name="summary"></a>Zusammenfassung

Die Microsoft-Lösung für universelles Drucken steht ab dem 1. März 2021 für Transaktionen innerhalb ausgewählter Microsoft 365-Suites und als eigenständiges Add-On zur Verfügung.

### <a name="impacted-audience"></a>Zielgruppe

Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen

### <a name="details"></a>Details

[Universelles Drucken](https://aka.ms/universalprint) ist ein Microsoft 365-Druckdienst, durch den keine lokalen Druckerserver mehr benötigt werden und der Windows-Geräten das Drucken an Azure-registrierte Drucker ermöglicht. Er steht ab dem 1. März 2021 für Transaktionen zur Verfügung.

Worker profitieren von treiberlosem Drucken, einer optimierten standortbasierten Druckerermittlung und einem intuitiven Druckvorgang ohne Lernkurve. Geräte, die mit Azure Active Directory (Azure AD) verknüpft sind, nutzen vorhandene Azure AD-Anmeldeinformationen für sicheres Drucken. Administratoren verwalten das Drucken über das Azure-Portal und können Drucker mit nativer Unterstützung für universelles Drucken problemlos verbinden. Universelles Drucken kann bei nicht kompatiblen Druckern mithilfe von Konnektorsoftware für universelles Drucken bereitgestellt werden.

Universelles Drucken wird bei Einführung in Windows E3, A3, E5 und A5 sowie Microsoft 365 BP, F3, E3, A3, E5 und A5 aufgenommen.  

**Angebotsdetails**

Beachten Sie, dass der Angebotsname leicht von der Preislistenvorschau abweicht.

| Angebotsname | Angebots-ID | Materialkennung |
| ------ |----------- |----------- |  
| Universelles Drucken – Volumen-Add-On (500 Aufträge) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Universelles Drucken – Volumen-Add-On (500 Aufträge) für Lehrpersonal – Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Universelles Drucken – Volumen-Add-On (500 Aufträge) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Universelles Drucken – Volumen-Add-On (500 Aufträge) für Lehrpersonal – Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Nächste Schritte

Machen Sie sich mit der Preisliste und der [Übersicht über universelles Drucken](/universal-print/fundamentals/universal-print-whatis) vertraut. Geben Sie diese Informationen an die entsprechenden Kontakte in Ihrer Organisation weiter.

### <a name="questions"></a>Noch Fragen?

Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.
