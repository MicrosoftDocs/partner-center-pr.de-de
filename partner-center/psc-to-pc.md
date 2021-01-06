---
title: Migration von Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Microsoft-Partner von Partner Sales Connect (PSC) zu Partner Center migrieren und von Microsoft-Verkäufern gesendete Angebote erstellen oder verwalten können.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 8ab1e2f2abae8af4c3949615653f83553e65fe25
ms.sourcegitcommit: e4f30d29073cc0bcc28c4fe48791a19aa28ba734
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/06/2021
ms.locfileid: "97950585"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Leitfaden zum Co-Selling im Partner Center (PC) für Partner, die von Partner Sales Connect (PSC) migrieren

**Geeignete Rollen**

- Kontoadministrator
- Empfehlungsadministrator
- Partner Sales Connect-Verkäufer (PSC)
- Partner Sales Connect-Administrator (PSC)
- Partner Sales Connect (PSC)-Deal-Manager

Dieser Artikel führt Sie durch die Migration von Partner Verkäufen zum Partner Center, sodass Sie weiterhin Co-Selling-Angebote im Partner Center erstellen und verwalten können.

Wie Sie wissen, verliert Ihr Unternehmen den Zugriff auf das PSC nach dem 31. März 2021. Allerdings finden Sie weiterhin alle Elemente, die Sie in Partner Center verwenden möchten, wie z. b. das Erstellen von Co-Selling-Geschäften, das Verwalten Ihrer Geschäfte und das Handeln von angeboten, die von Microsoft-Verkäufern an Sie gesendet werden.

Es gibt jedoch Unterschiede. Anhand der folgenden Anleitungen können Sie den Übergang zu Partner Center vereinfachen und einfacher gestalten.

>[!Important]
> Wenn Sie sich hier befinden, weil Sie ein Banner zu der Migration gesehen haben, sind Sie an der richtigen Stelle. Dieses Handbuch gilt nicht für Lösungs Bewertungs (SA) und OEM-IOT-Partner, die ihre Geschäfte in PSC verwalten.

## <a name="before-you-move-things-you-need-to-know"></a>Bevor Sie fortfahren, müssen Sie wissen, was Sie wissen müssen.

### <a name="if-you-are-a-psc-admin"></a>Wenn Sie PSC-Administrator sind

- Sie benötigen eine geschäftliche e-Mail-Adresse für die Anmeldung bei [Partner Center](https://partner.microsoft.com/).
- Richten Sie Ihr Konto mit der Hilfe des Partner Center- [Konto Administrators](permissions-overview.md)ein.
- Lesen Sie dieses Dokument, um zu erfahren, wie Sie im Partner Center mitverkaufen.
- Richten Sie Benutzerkonten im Partner Center für alle Ihre PSC-Benutzer (admin-, Manager-und Verkäufer Rollen) ein, und weisen Sie Ihnen [Verweis Administrator Rollen](permissions-overview.md)zu.

>[!IMPORTANT]
> Stellen Sie sicher, dass die im PSC-Banner angezeigte MPN-ID in der Liste der MPN-Standorte im Partner Center verfügbar ist.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Bild, das das PSC-Banner anzeigt, in dem die Partner die MPN-ID finden können.":::

 Um sicherzustellen, dass die MPN-ID als Partner Center-MPN-Speicherort angezeigt wird, melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann oben rechts auf dem Bildschirm **Einstellungen** (das Zahnrad Symbol) und anschließend **Kontoeinstellungen** aus. Wählen Sie im linken Navigationsmenü der zweiten Ebene die Option Speicher **Orte** aus, um die Liste aller MPN-IDs und-Standorte anzuzeigen, die dem Partner Center-Konto zugeordnet sind.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Wenn Sie ein PSC-Deal-Manager oder-Verkäufer sind

- Sie benötigen eine geschäftliche e-Mail-Adresse, um sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)anzumelden.
- Wenn Sie ein nicht Geschäftskonto in PSC verwenden oder Ihre geschäftliche e-Mail-Adresse für ein anderes Unternehmen als das Partnerunternehmen verwendet wird, wenden Sie sich für die Einrichtung des Kontos an Ihren PSC-Administrator.
- Wenden Sie sich an Ihren PSC-Administrator, wenn das Einrichten Ihres Partner Center-Kontos unabhängig von dem Konto, mit dem Sie sich beim PSC anmelden, fertiggestellt ist.
- Überprüfen Sie, ob Sie Zugriff auf Partner Center und den Abschnitt "Verweise" haben.
- Lesen Sie dieses Dokument, um sich mit den Workflows und den Änderungen in Partner Center vertraut zu machen.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Als Administrator in PSC sind dies die nächsten Schritte.

Wählen Sie aus dem linken Navigationsmenü von Partner Center die Option **Verweise** aus. Vergewissern Sie sich, dass Sie auf die Seite "Verweise" zugreifen können.

  >[!Note]
  > Möglicherweise müssen Sie sich bei Partner Center abmelden und wieder anmelden, um Ihre Anmelde Informationen für den Zugriff auf die Seite "Verweise" zu aktualisieren.

Wenn die Option " **Verweise** " im Partner Center-Menü oder auf seitenbezogenen Seiten nicht angezeigt wird, wenden Sie sich an den [Konto Administrator](permissions-overview.md) Ihres Unternehmens, und bitten Sie ihn, Ihnen Zugriff auf die Option " **Verweise** " und den zugehörigen Bereich zu verschaffen.

So finden Sie den Konto Administrator Ihres Unternehmens:

1. Wählen Sie über das Zahnrad Symbol rechts oben auf dem Partner Center-Dashboard **Kontoeinstellungen** aus.

1. Wählen Sie **Benutzerverwaltung** im linken Navigationsmenü der zweiten Ebene aus.

1. Wählen Sie oben in der Benutzerliste das Dropdown Menü **Filter** aus. Ändern Sie die Option in **Konto Administrator**.

   Auf der Seite werden alle Konto Administratoren mit ihren jeweiligen e-Mail-Adressen angezeigt. Senden Sie eine e-Mail an Sie, und bitten Sie Sie, die Administrator Rolle "referenrals" für Ihr Geschäftskonto zuzuweisen.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Bild, das die Konto Administratoren auf der Seite &quot;Partner Einstellungen Benutzerverwaltung&quot; anzeigt.":::

>[!Important]
>- Wenn Ihre Rolle nur die Verwaltung von Benutzern im PSC umfasst, bitten Sie den Konto Administrator Ihres Unternehmens, Ihnen die [Konto Administrator](permissions-overview.md#manage-mpn-membership-and-your-company) Rolle im Partner Center zuzuweisen. 
>- Wenn Ihre Rolle auch die Verwaltung von Co-Selling-Verkaufschancen umfasst, bitten Sie, der Administrator Rolle " [referenrals](permissions-overview.md#manage-referrals) " zuzuweisen.
> - Es empfiehlt sich, auch einen Change Management Lead zwischen den PSC-Administratoren zu benennen. Dadurch wird verhindert, dass alle PSC-Administratoren sich einzeln an Partner Center-Konto Administratoren wenden müssen. Stattdessen kann der Change Management Lead die primäre Person sein, die mit dem Partner Center-Konto Administrator arbeitet.

## <a name="user-migration"></a>Benutzermigration

Nachdem Sie Ihr Konto in Partner Center eingerichtet haben, verwenden Sie den Benutzermigrations-Assistenten auf der Seite Co-Selling-Chancen, um den Mitarbeitern Ihres Unternehmens automatisch Partner Center-Rollen zuzuweisen.

>[!Note]
> Die Benutzer Migration kann nur von [Konto Administratoren](permissions-overview.md#manage-mpn-membership-and-your-company) Ihres Unternehmens ausgeführt werden. Wenn Sie nicht über die Konto Administrator Rolle verfügen, finden Sie einen Konto Administrator, der beim Einrichten der Benutzerkonten mithilfe des Benutzermigrations-Assistenten behilflich sein kann. Die Funktionen für die Benutzer Migration werden ab dem 18. November 2020 verfügbar sein.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Das Bild zeigt den Benutzermigrations-Assistenten.":::

Konto Administratoren sehen einen Link für den PSC-Benutzermigrations-Assistenten auf der Seite Co-Selling-Verkaufschancen neben dem Leitfaden für Verweise. Sie können die Benutzer Migration initiieren, indem Sie den Link auswählen. Administratoren können den Link auswählen, um die Benutzer Migration zu initiieren. Sie können diesen Schritt für die Benutzer Migration mehrmals durchführen, bis allen Benutzern im Partner Center die richtigen Rollen zugewiesen sind.

Die Benutzer Migrations Tabelle enthält die folgenden Details:

- Benutzerkonto-e-Mail-ID des Mitarbeiters
- PSC-Partnerkonto: das Konto, mit dem der Mitarbeiter in PSC verknüpft ist.
- PSC-Benutzerrolle: eine der drei Rollen, die in PSC zugewiesen sind.
- PC-MPN-Speicherort: der Speicherort, für den dem Benutzer relevante PC-Rollen zugewiesen werden. Der MPN des PSC-Partnerkontos wird verwendet, um den entsprechenden MPN-Speicherort im Partner Center zu finden und Berechtigungen zuzuweisen. Die gesamte Organisation bezeichnet die Vorg-MPN-ID.
- PC-Benutzer Rollen: Mitarbeiter werden basierend auf Ihren PSC-Benutzer Rollen Rollen zugewiesen. Admin in PSC erhält Verweise auf Administrator Rollen auf dem PC. Dem Verkäufer wird die Benutzerrolle "referenrals" auf dem PC zugewiesen. Weitere Informationen zu den PC-Rollen und den Benutzern, die diese Rollen in Partner Center verwenden können, finden Sie [hier](permissions-overview.md#manage-referrals) .
- PC Aad-Mandant: der Mandant, dem die Benutzer im Partner Center zugewiesen sind
- Status: Es gibt drei mögliche Zustände für den Status der Migration.
    - **Nicht migriert** -dem Benutzer ist keine Rolle "PC-Verweise" zugewiesen.
    - **Migriert** : der Benutzer wurde erfolgreich mit der entsprechenden zugewiesenen Rolle migriert, wie in der Tabelle gezeigt.
    - **Fehler** : die Migration kann aufgrund eines Fehlers nicht durchgeführt werden.

Manchmal kann eine Migration fehlschlagen und zu Fehlern führen. Im folgenden finden Sie einige Gründe, warum eine Migration zu einem Fehler führen kann, und einige Möglichkeiten, das Problem zu beheben:

1. Die PSC-Benutzer verwenden möglicherweise ein nicht-Geschäftskonto.

2. Der PSC-Benutzer verwendet möglicherweise ein Konto aus einer anderen Domäne als dem, das Sie im Partner Center verwenden.

   Um Fehler im Zusammenhang mit den Szenarien 1 und 2 zu beheben, bitten Sie den Benutzer, sich mit seinem Geschäftskonto bei Partner Center anzumelden, das an Ihren Azure AD Mandanten angeschlossen ist. Ihr [globaler Administrator](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kann Ihnen helfen.
   
   So finden Sie Ihren globalen Administrator: 
   - Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard) an, und wählen Sie im Zahnrad Symbol rechts oben die Option **Kontoeinstellungen** aus.
   - Wählen Sie in der linken Navigationsleiste der zweiten Ebene die Option **Benutzerverwaltung** aus.
   - Wählen Sie oben in der Benutzerliste das Dropdown Menü **Filter** aus, und ändern Sie die Option in **globaler Administrator**. Auf der Seite werden dann alle globalen Administratoren mit ihren jeweiligen e-Mail-Adressen angezeigt. Bitten Sie einen von Ihnen, die Verweis Administrator Rolle für Ihr Geschäftskonto zuzuweisen.
   
      Der globale Administrator kann entweder ein neues Benutzerkonto in Ihrem Azure AD-Mandanten erstellen oder den Benutzern Zugriff auf Gastbenutzer zuweisen. Nachdem die Konten für alle PSC-Deal-Manager und-Benutzer eingerichtet wurden, müssen Sie sich bei Partner Center anmelden, im linken Navigationsmenü **Verweise** auswählen und bestätigen, dass die Seite "Verweise" angezeigt wird.

3. Dem Benutzer ist bereits eine Verweis Rolle im Partner Center zugewiesen.
    - Sie können die vorhandene Rolle des Benutzers überprüfen. Wählen Sie in der oberen rechten Ecke von Partner Center die Option **Einstellungen** (das Zahnrad Symbol) und dann **Kontoeinstellungen** aus. Wenn ein zweites Navigationsmenü angezeigt wird, wählen Sie **Benutzerverwaltung** aus, und suchen Sie nach dem Benutzer.

Nachdem Sie die Benutzer Migration abgeschlossen haben, verwenden Sie die folgenden Anleitungen, um die Migrationsstrategie zu bestimmen:

Wenn Ihr Unternehmen über einen Partner Development Manager (PDM) verfügt: Wenn Ihr Partner Center-Konto eingerichtet ist und Ihre Benutzer überrollen und Berechtigungen verfügen, können Sie Ihre Co-Selling-Aktivitäten in Partner Center verschieben. Informieren Sie das PDM, dass Sie den Switch anstatt warten müssen, bis der Stichtag für die Migration vollständig ist. Dadurch können alle neuen Angebote in Partner Center übertragen werden.

>[!Note]
>Nachdem Sie diesen Switch vorgenommen haben, können Sie nur auf die vorhandenen aktiven Vorgänge in PSC reagieren. Sie können weder neue Angebote erstellen noch Angebote von Microsoft-Verkäufern im PSC erhalten.

Wenn Ihr Unternehmen nicht über ein PDM verfügt, stellen Sie sicher, dass alle Benutzerkonten von allen Benutzern eingerichtet und überprüft werden. Sie werden über eine e-Mail und ein Banner im PSC benachrichtigt, wenn Sie mit dem Co-Selling im Partner Center beginnen können. Denken Sie daran, dass Sie weiterhin die vorhandenen aktiven Geschäfte in PSC verwalten müssen.

>[!Important]
>Aktive Geschäfte werden nicht auf den PC migriert. Bis zum 31. März 2021 müssen die Geschäfte geschlossen und registriert werden.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Nächste Schritte für PSC-Administratoren, PSC-Deal-Manager und PSC-Verkäufer

Erfahren Sie, wie Sie im Partner Center mitverkaufen.
Dies ist ein wichtiger Schritt, der Ihnen bei der Vorbereitung auf Co-Selling im Partner Center behilflich ist. Machen Sie sich mit den Workflows und den Änderungen im Partner Center vertraut, sodass Sie sich sofort direkt verkaufen können. Beginnen Sie, indem Sie dieses Dokument vollständig lesen. Ein guter Satz an Ressourcen ist auch im [Co-Selling Gallery](https://aka.ms/cosellexperience)-Katalog verfügbar.

## <a name="major-differences-between-psc-and-pc-workflows"></a>Wichtige Unterschiede zwischen PSC-und PC-Workflows

|**Szenario**|**Partner Sales Connect**|**Partner Center**|
|-----|:-----|:-----|
|Benutzerrollen|PSC verfügt über die Rollen admin, Deal Manager und Verkäufer.|Der PC verfügt nur über die Rolle " [Verweis Administrator](permissions-overview.md#manage-referrals) ", die Lese-und Schreibberechtigungen für alle Geschäfte erteilt.|
|Einladen von Microsoft für einen Co-Selling-Deal|Vom Microsoft-Verkäufer initiiert, gibt es keine explizite Frage nach Partner.|Der Partner muss eine [explizite Anfrage](manage-co-sell-opportunities.md#add-solutions) stellen, wenn eine Microsoft-Verkäufer Hilfe benötigt wird. Der Microsoft-Verkäufer hat die Möglichkeit, die Anforderung abzulehnen.|
|Expiry|Es gibt kein Konzept für eine Ablaufzeit.|Eingehende Partner Verträge laufen in 14 Tagen ab, wenn Sie vom Partner nicht akzeptiert werden. Dasselbe gilt für ausgehende Partnerangebote, bei denen Sie in den abgelaufenen Status wechseln können, wenn der Microsoft-Verkäufer nicht innerhalb von 14 Tagen darauf reagiert.|
|Details des Microsoft-Verkäufers|Sichtbar, sobald ein Problem erstellt wird.|Details des Microsoft-Verkäufers werden nur dann für Partner freigegeben, wenn der Verkäufer die Einladung zum Co-Selling von Partner explizit akzeptiert.|
|[Private Pipeline](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Nicht verfügbar.|Partner können ihre Pipeline freigeben, ohne den Microsoft-Verkäufern Einblick zu geben.|
|Lösungen|Es können nur Lösungen hinzugefügt werden, die zu einer Preisliste gehören.|Partner können [Lösungen](manage-co-sell-opportunities.md#add-solutions) hinzufügen, die den folgenden Listen angehören. a) ihre eigenen Lösungen b) Lösungen aus dem Microsoft First Party Catalog (ähnlich der Rolle "Transaktions Rolle in PSC") und "c" Co-Selling-Lösungen von anderen Drittanbieter Partnern (ähnlich wie die Rolle "ISV-Rolle" in PSC).|
|Zuweisungs Zuweisung|Nur der zugewiesene Verkäufer kann die Geschäfte anzeigen und darauf reagieren.|Team Mitglieder können einem Teil hinzugefügt werden, um die Mitarbeiter anzugeben, die an einem Teil arbeiten. es gibt keine Blockierung anderer verweisadministratoren, die diese Aktionen nicht anzeigen oder darauf reagieren.|
|Kundenorganisation|Freier Formular Text Eintrag.|Sie können die [Kundenorganisation](manage-co-sell-opportunities.md#select-your-customer) anhand der [D-&B-Datenbank](https://www.dnb.com/) durchsuchen, indem Sie nur einige Zeichen eingeben. Der rechtliche Name und die Adresse werden automatisch basierend auf der Wahl aufgefüllt.|
|Kundenkontakt|Nicht obligatorisch.|Für die private Pipeline Freigabe nicht obligatorisch. Erforderlich, wenn der Microsoft-Verkäufer eingeladen wird, an einer Co-Selling-Anforderung teilzunehmen.|
|Öffentliche API|Nicht verfügbar.|[Öffentliche API](/partner/develop/referrals) zum programmgesteuerten Verwalten von Partner Center-verweisen.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Zuordnen der Felder in PSC zu den entsprechenden Feldern im Partner Center

In diesem Abschnitt werden ausgewählte Screenshots, die für PSC angezeigt werden, mit der entsprechenden Ansicht im Bereich Partner Center-Co-Selling-Verkaufschancen verglichen.

Für jedes Paar von Screenshots werden nummerierte, gelbe oder rote Kreise angezeigt:

- **Was bedeuten gelbe Kreise?** Nummerierte, gelbe Kreise werden zuerst in jedem PSC-Bildschirmfoto angezeigt. Sie finden dann einen begleitenden Partner Center-Screenshot, der viele der gleichen Zahlen enthält.

   Um zu sehen, wie die einzelnen Felder oder Attribute in PSC ihrer Entsprechung in Partner Center zugeordnet werden, stimmen Sie den nummerierten Kreisen in den beiden, verwandten Screenshots zu. Vergleichen Sie z. b. die nummerierte, gelbe "1" im ersten, PSC-Screenshot mit der nummerierten, gelben "1" im zweiten, Partner Center-Bildschirm Abbildung darunter.

- **Was bedeutet ein roter Kreis?** Wenn in einem Screenshot ein roter Kreis angezeigt wird, bedeutet dies, dass das Feld "PSC" im Partner Center nicht verfügbar ist.

Die Feld Zuordnungen von PSC zu Partner Center werden für die folgenden Bereiche angezeigt:

1. PSC-Startseite, die der Partner Center-Standardansicht für Co-Selling-Verkaufschancen zugeordnet ist
1. Der Partner Center-Ansicht "Ansicht" zugeordnete PSC-Rasteransicht
1. PSC-Detailansicht, die der Partner Center-Detailansicht zugeordnet ist
1. PSC-Ansicht "Produkte hinzufügen", die der Ansicht Partner Center Add Solutions zugeordnet ist
1. PSC-Benutzer Verwaltungs Ansicht, die der Partner Center-Benutzer Verwaltungs Ansicht zugeordnet ist
1. PSC-Benutzer Rollen Zuweisungs Ansicht, die der Partner Center-Rollen Zuweisungs Ansicht zugeordnet ist
1. PSC-Benachrichtigungs Ansicht der Partner Center-Benachrichtigungs Ansicht zugeordnet

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1: PSC-Homepage wird der Partner Center-Standardansicht für Co-Selling-Verkaufschancen zugeordnet

Vergleichen Sie die übereinstimmenden, nummerierten Kreise zwischen dem Top-PSC-Bildschirmfoto und dem Partner Center-Bildschirmfoto darunter. Übereinstimmende Zahlen zeigen, wo Sie das PSC-Verwandte Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Partner Center-Feld vorhanden ist.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Das Bild zeigt die Feld Zuordnungen zwischen der Startseite von Partner Sales Connect und der Standardansicht der Co-Selling-Verkaufschancen in Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2: PSC-Rasteransicht, die der Partner Center-Ansicht "Deal" zugeordnet ist

Vergleichen Sie die übereinstimmenden, nummerierten Kreise zwischen dem Top-PSC-Bildschirmfoto und dem Partner Center-Bildschirmfoto darunter. Übereinstimmende Zahlen zeigen, wo Sie das PSC-bezogene Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Partner Center-Feld vorhanden ist.  

> [!NOTE]
> Weitere Überlegungen werden unter den Screenshots angezeigt.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Das Bild zeigt die Feld Zuordnungen zwischen der Ansicht &quot;Partner Sales Connect&quot; (PSC) und der Partner Center-Ansicht." lightbox="images/pscmigration/grid-view-expanded.png":::

**Besondere Überlegungen:**

- Im Partner Center gibt es keine Listenansicht wie die des PSC.  Alle Geschäfte werden basierend auf dem Datum der letzten empfangenen oder erstellten Informationen mit den Kundeninformationen und dem Typ des Deals aufgelistet. Der erste Teil der Ansicht ist standardmäßig ausgewählt. Die meisten der Werte, die im PSC-Tabellenformat angezeigt werden, sind in der Detailansicht des PCs (PC) verfügbar.
- Die Rolle "Geschäft" ist kein Pflichtfeld im PC. Es wird nicht in einem der Workflows angezeigt oder aufgezeichnet. Es wird automatisch auf der Seite des Microsoft-Verkäufers basierend auf den Lösungen abgeleitet, die dem Geschäft hinzugefügt werden.
- Das Datum der letzten Änderung wird nicht auf der Seite mit den Verweis Details auf dem PC angezeigt. Partner können die Sortierungs Funktionen verwenden, um die Geschäfte basierend auf dem Datum der letzten Aktualisierung zu sortieren.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-PSC-Detailansicht, die Partner Center zugeordnet ist

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen (PSC-) Screenshot mit dem untergeordneten Partner Center-Bildschirmfoto. Übereinstimmende Zahlen zeigen, wo Sie das PSC-bezogene Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Feld oder Bereich im Partner Center vorhanden ist.

> [!NOTE]
> Weitere Überlegungen werden unter den Screenshots angezeigt.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Das Bild zeigt die Feld Zuordnungen zwischen der Partner Sales Connect (PSC)-Detailansicht und der Partner Center-Detailansicht." lightbox="images/pscmigration/deal-details-expanded.png":::

**Besondere Überlegungen:**

- Partner können einen Teil bearbeiten, indem Sie die Schaltfläche Bearbeiten in der Detailansicht für Partner Details (6) auswählen. Nachdem die Schaltfläche Bearbeiten ausgewählt wurde, werden alle Felder bearbeitbar. Sie haben dann die Möglichkeit, die bearbeitbaren Änderungen zu speichern oder abzubrechen.
- Es gibt keine Option zum Schließen des Deals als Duplizierung in Partner Center.
- Das Kunden Ergebnis ist nicht im Partner Center verfügbar. Alle Details im Zusammenhang mit Kundeninteraktionen können im Abschnitt "Hinweise" des PCs aktualisiert werden.
- Das geschätzte Lösungs Schluss Datum ist nur für OEM-IOT-Angebote im Partner Center verfügbar. Diese Informationen werden für andere Typen von Typen nicht angezeigt.
- Das Lizenzierungsprogramm ist auf dem PC nicht erforderlich. Diese Informationen werden basierend auf den in der Vereinbarung ausgewählten Lösungen automatisch abgeleitet.

>[!Note]
>Alle als "gewinnt" oder "verloren" markierten Geschäfte können im Anschluss nicht bearbeitet werden. Seien Sie vorsichtig, wenn Sie eine Aufgabe in einen dieser Terminal Zustände verschieben.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-PSC-Ansicht "Produkte hinzufügen" wird der Partner Center-Ansicht "Lösungen hinzufügen" zugeordnet

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen (PSC-) Screenshot mit dem untergeordneten Partner Center-Bildschirmfoto. Übereinstimmende Zahlen zeigen, wo Sie das PSC-bezogene Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Feld oder Bereich im Partner Center vorhanden ist.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Das Bild zeigt die Feld Zuordnungen zwischen der Ansicht Partner Sales Connect (PSC) Add Products (Partner Sales Connect) und der Partner Center-Ansicht Lösungen hinzufügen." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5: Benutzerverwaltung im PSC im Vergleich zu Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen (PSC-) Screenshot mit dem untergeordneten Partner Center-Bildschirmfoto. Übereinstimmende Zahlen zeigen, wo Sie das PSC-bezogene Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Feld oder Bereich im Partner Center vorhanden ist.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Das Bild zeigt die Feld Zuordnungen zwischen der Partner Sales Connect (PSC)-Startseite und der Partner Center-Benutzer Verwaltungsseite im Bereich Kontoeinstellungen an."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6: Benutzer Rollenzuweisung im PSC und Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen (PSC-) Screenshot mit dem untergeordneten Partner Center-Bildschirmfoto. Übereinstimmende Zahlen zeigen, wo Sie das PSC-bezogene Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Feld oder Bereich im Partner Center vorhanden ist.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Das Bild zeigt die Feld Zuordnungen zwischen der Rollen Zuweisungs Ansicht Partner Sales Connect (PSC) und der Partner Center-Rollen Zuweisungs Ansicht." lightbox="images/pscmigration/roles-expanded.png":::

**Besondere Überlegungen:**

- Die entsprechende Rolle für den PSC-Administrator ist die Konto Administrator Rolle in Partner Center.
- Im Partner Center gibt es nur eine Rolle für die Co-Selling-Verwaltung. Diese Rolle ist die Rolle "Verweis Administrator".

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-Benachrichtigungen im PSC im Vergleich zum Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen (PSC-) Screenshot mit dem untergeordneten Partner Center-Bildschirmfoto. Übereinstimmende Zahlen zeigen, wo Sie das PSC-bezogene Feature oder Attribut im Partner Center finden. Rote Kreise geben an, dass kein entsprechendes Feld oder Bereich im Partner Center vorhanden ist.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Das Image zeigt die Zuordnung zwischen den PSC-Benachrichtigungen (Partner Sales Connect) und der Partner Center-Benachrichtigungs Ansicht."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Wechseln vom PSC zu Partner Center: häufig gestellte Fragen

In den folgenden Abschnitten werden häufige Fragen zur Migration beantwortet.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1. Was soll ich tun, wenn ich keinen Zugriff auf Partner Center habe?

Sie können sich an Ihre Administratoren wenden, die auf der Seite "kein Zugriff" aufgeführt sind, um die zugewiesenen Rollen zu erhalten. Sie benötigen die Rolle " [Verweis Administrator](permissions-overview.md#manage-referrals) " für Lese-und Schreibberechtigungen im Abschnitt "Verweise". Wenn Sie nur geschäftsprofile verwalten, benötigen Sie die Rolle "Geschäftsprofil Administrator" im Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Bild, das den Zugriff ohne Zugriff in Partner Center anzeigt.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2: Wer kann mir Zugriff auf den Abschnitt "Verweise" in Partner Center gewähren?

Ihr [Konto Administrator](permissions-overview.md#manage-mpn-membership-and-your-company) kann Ihnen Zugriff auf die Registerkarte "Verweise" gewähren. Um Ihren Konto Administrator zu suchen, wählen Sie im Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)in der oberen rechten Ecke des Zahnrad Symbols **Kontoeinstellungen** aus. Wählen Sie dann in der linken Navigationsleiste der zweiten Ebene die Option **Benutzerverwaltung** aus. Wählen Sie oben in der Benutzerliste das Dropdown Menü **Filter** aus, und ändern Sie die Option in **Konto Administrator**. Auf der Seite werden alle Konto Administratoren mit ihren jeweiligen e-Mail-Adressen angezeigt. Bitten Sie einen von Ihnen, die Verweis Administrator Rolle für Ihr Geschäftskonto zuzuweisen.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3: die Schaltfläche "+ neu" ist für unser Konto abgeblendet. Was soll ich tun, um mit dem Erstellen von Deals zu beginnen?

Dies geschieht nur, wenn keine Co-Selling-Lösungen an die MPN-Organisation angefügt sind, die Sie im Partner Center verwenden. Wenden Sie sich an Ihr PDM, um die MPN-ID Ihrer Lösungen korrigiert zu erhalten, oder erstellen Sie ein Support Ticket, in dem das Problem "neue Schaltfläche nach der PSC-Migration abgeblendet" angezeigt wird.

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4. kann ich einem bestimmten Benutzer, wie z. b. PSC, eine bestimmte Person zuweisen?

Sie können Teammitglieder einer bestimmten Sache zuweisen. Es verhindert nicht, dass andere Verweises-Administratoren diese Angebote anzeigen oder darauf reagieren.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5: gibt es eine Ansicht aller mir zugewiesenen Angebote?

Sie können das Feature "Favoriten" verwenden, das eine Registerkarte auf Benutzerebene ist. Sie können alle als Favoriten zugewiesenen Angebote markieren, um einen schnellen Zugriff auf die Geschäfte zu erhalten.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6: gibt es eine schreibgeschützte Ansicht für die Geschäfte?

Nein, es gibt keine schreibgeschützte Ansicht der Deals im Abschnitt "Verweise". Alle verweisadministratoren verfügen über vollständigen Lese-und Schreibzugriff auf alle Geschäfte.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7: Wie kann ich ein Problem registrieren, nachdem es als "gewonnen" gekennzeichnet wurde?

Wenn der Vorgang die unten aufgeführten Kriterien erfüllt, wird ein Popup Fenster angezeigt, um die [Registrierung](./register-deals.md)zu beginnen.

- Es gibt eine berechtigte berechtigte Lösung, die an den Vertrag angeschlossen ist.
- Der Microsoft-Verkäufer ist eingeladen, am Umgang teilzunehmen, oder Sie haben Sie zur Sache eingeladen.
- Die Microsoft-Karte hat den Status "akzeptiert" oder "Won" im Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-Ich erhalte eine Fehlermeldung, wenn ich die Schaltfläche "+ New-Deal-Registrierung" im Abschnitt "Registrierungs Registrierung" auswähle. Wie kann ich meine Geschäfte registrieren?

Die Schaltfläche **+ neue Registrierung** wird nur von den Partnern verwendet, die im ISV Connect-Programm registriert sind, um ein Geschäft ohne entsprechende Co-Selling-Verkaufschancen in Partner Center zu registrieren. Für die Registrierung mit einer Co-Selling-Verkaufschance wird ein Popup Fenster angezeigt, wenn das Geschäft als gewonnen gekennzeichnet ist, und wenn es die Kriterien für die Registrierungs Registrierung erfüllt.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9: Hinzufügen einer Kundenorganisation obligatorisch?

Ja, das Hinzufügen einer [Kundenorganisation](./manage-co-sell-opportunities.md#select-your-customer) ist im Partner Center obligatorisch. Zuerst suchen Sie nach dem Speicherort, an dem sich der Kunde befindet. Basierend auf den Details, die Sie besitzen. Sie können genau den genauen Gebäude Namen einschließen oder nur die Details der Stadt angeben. Bei der Organisations Suche werden alle juristischen Entitäten abgerufen, die mit dem eingegebenen Namen übereinstimmen, sodass Sie keine Adressen Details eingeben müssen. Alle Details werden automatisch basierend auf der ausgewählten Organisation ausgefüllt.

### <a name="10---are-customer-contact-details-mandatory"></a>10: sind Kundenkontakt Details obligatorisch?

Hängt vom [Typ des](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) zu erstellenden Typs ab. Wenn Sie nur ihre Pipeline freigeben und keine Hilfe von der Microsoft-Vertriebsorganisation benötigen, können Sie auswählen, dass Sie keine Kundenkontaktinformationen erhalten. Wenn Sie gemeinsam mit der Unterstützung von Microsoft-Verkäufern Hilfe benötigen, müssen Sie die Details des Kundenkontakts angeben. Sie sollten vor dem Erstellen einer Co-Selling-Anforderung im Partner Center eine explizite Zustimmung des Kunden erhalten.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11. wie viele Lösungen kann ich zu einem Teil hinzufügen?

Sie können bis zu 50 Lösungen (analog zu "Products" in PSC) zu einem Geschäft hinzufügen. Anders als bei PSC können Sie Lösungen aus ihren eigenen Co-Selling-Lösungen, von Microsoft-SKUs für erste Parteien und von anderen Co-Selling-Lösungen von Drittanbietern kombinieren. Es gibt keine Rolle "Rolle", die ausgewählt oder im Partner Center verfügbar sein soll. Bei Microsoft-SKUs können Sie optional die Menge und den Preis für jede SKU hinzufügen, die dem jeweiligen Geschäft hinzugefügt wird.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12: Wann erhalte ich die Details des Microsoft-Verkäufers nach dem Erstellen eines Deals?

Microsoft-Verkäufer werden erst zugewiesen, nachdem die genaue Hilfe Anforderung abgeglichen wurde, die beim Erstellen des Deals mit der relevanten Verkäufer-Persona auf der Microsoft-Seite angegeben wurde. Auch nach der Zuweisung haben Microsoft-Verkäufer die Möglichkeit, die Co-Selling-Einladung anzunehmen oder abzulehnen. Nur wenn eine Co-Selling-Einladung von einem Verkäufer akzeptiert wird, wird der Vorgang mit den Kontaktinformationen des Microsoft-Verkäufers aktualisiert. Die SLA für Microsoft-Verkäufer, die für das Geschäft tätig sein soll, ist 14 Tage. Es handelt sich um die gleiche SLA, die Partner für das Geschäft tun müssen, bevor Sie in den abgelaufenen Zustand übergeht.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13. wo kann ich die Verkaufschancen-ID finden?

Die Verkaufschancen-ID im PSC ist mit der ID des Deals im PC identisch. Sie können die ID des Deals neben dem Namen des Deals finden, wenn Sie eine beliebige Menge öffnen.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14: Wie kann meine PDM auf den PC zugreifen?

Ihr PDMS kann nicht direkt im Gegensatz zu PSC auf Partner Center zugreifen. Es gibt mehrere Optionen, um diese Funktion zu aktivieren, die unten erwähnt werden.

- OCP Insights: Wenn PDMS nur die zugehörigen Geschäfte und Fortschritte anzeigen, können Sie das OCP Insights-Portal verwenden, um Ihre Organisations Ansicht zu erhalten. Hierbei handelt es sich um ein internes Tool, das nur für PDMS verfügbar ist. Beachten Sie, dass OCP Insights für die Benutzer Ihres Unternehmens nicht verfügbar ist.
- Gastbenutzer in Partner Center: Sie können Ihr PDM- @microsoft.com Konto als Gastbenutzer in Partner Center hinzufügen und ihm eine verweisadministrator-Rolle zuweisen, damit Sie Verweise anzeigen und darauf reagieren können.
- Erstellen eines [neuen Benutzers](./create-user-accounts-and-set-permissions.md#add-a-new-user) in Ihrem Mandanten: Sie können einen neuen Benutzer in Ihrem eigenen Mandanten erstellen und diese Details mit dem PDM teilen, sodass Sie Verweise anzeigen und auf ähnliche Verweise wie andere verweisbenutzer in Ihrem Konto reagieren können.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Ermitteln der richtigen MPN-ID, wenn Ihr Konto in PSC keinem gültigen MPN zugeordnet ist

Wenn Sie sich hier befinden, weil Sie ein Banner mit der Bezeichnung "PSC-ungültige MPN-ID-Zuordnungs Problem" erkannt haben, sind Sie an der richtigen Stelle.

Suchen Sie zuerst nach der richtigen MPN-ID, indem Sie die folgenden Schritte ausführen.

- Melden Sie sich bei Ihrem Partner Center-Konto an
- Verwenden Sie die Anweisungen in der [Dokumentation zu den Kontoeinstellungen](./partner-center-account-setup.md#locate-your-mpn-id) , um die MPN-ID zu ermitteln.

Als Nächstes

- Wenn Sie über ein PDM verfügen, bitten Sie Sie, ihre MPN-ID mit der richtigen MPN-ID aus Ihrem Partner Center-Konto zu korrigieren.
- Wenn Sie über kein PDM verfügen, senden Sie eine e-Mail an die im PSC-Banner angegebene Adresse, wobei Sie sowohl die im PSC-Banner angezeigten PSC-Kontoinformationen als auch die richtige MPN-ID aus Ihrem Partner Center-Konto angeben.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Ressourcen, die Sie beim Erstellen und Verwalten Ihrer Geschäfte in Partner Center unterstützen

Wenn Sie die Hilfe Themen für die Co-Selling-Hilfe noch nicht gelesen haben, helfen Ihnen die folgenden Ressourcen bei der Verwaltung von Geschäften im Partner Center.

|**Aufgabe**   |**Artikel**   |
|-----------------------|:-----------------------|
|Grundlegendes zu den Registerkarten und Navigation auf der Seite mit den Möglichkeiten|[Navigieren im Co-Selling-Abschnitt](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Auswählen einer Kundenorganisation aus der Liste der D-&B |[Wählen Sie Ihren Kunden aus](./manage-co-sell-opportunities.md#select-your-customer)|
|Ändern der Felder im Abschnitt "Details zum Abschnitt"|[Details zum Umgang](./manage-co-sell-opportunities.md#deal-details)|
|Hinzufügen von Teammitgliedern zu einem Deal-Team|[Mitarbeiter hinzufügen](./manage-co-sell-opportunities.md#add-team-members)|
|Antworten auf einen Co-Selling-Deal|[Verwalten von Co-Selling-Geschäften](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Von Ihnen im Partner Center ersicherte Angebote registrieren |[Registrieren eines neuen Angebots](./register-deals.md)
|Verschaffen Sie sich Einblicke, und informieren Sie sich über die Funktionsweise ihrer Verweise. |[Einblicke zu Empfehlungen](./referral-insights.md)
|Erstellen und Verwalten von Geschäftsprofilen|[Verwalten von Geschäftsprofilen](./create-a-marketing-profile.md)
|Verwalten von Leads für Ihr Geschäftsprofil |[Verwalten von Leads](./manage-leads.md)|

## <a name="next-steps"></a>Nächste Schritte

Befolgen Sie diese zusätzlichen Ressourcen:

- [Partner Verkäufe stellen eine Verbindung mit der Partner Center-Arbeitsmappe](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) her, um die Vertriebsprozesse und-Rollen der Partner mithilfe von Partner Center im Vergleich zu Partner Sales Connect mit neuen Vertriebsprozessen auszurichten.
- [Partner Center Co-Selling Operating Guide](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) : Leitfaden zum Identifizieren eines Betriebsmodells über Partner Center, um Leads oder Co-Selling-Verkaufschancen zu verwalten und Angebote zu registrieren.
- [Referenz Verwaltung](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : eine Schritt-für-Schritt-Anleitung zum Verwalten von Leads und Co-Selling-Verkaufschancen über Partner Center.
- [Veröffentlichen und Verwalten von in der kommerziellen Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -visualisierten Schritt-für-Schritt-Anleitung zum Erstellen, verwalten und Veröffentlichen von Angeboten über Partner Center im kommerziellen Marketplace.