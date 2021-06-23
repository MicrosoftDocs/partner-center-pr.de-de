---
title: Migrieren von Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Microsoft-Partner von Partner Sales Connect (PSC) zu Partner Center und von Microsoft-Verkäufern gesendete Angebote erstellen oder verwalten können.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 5be1c09a26cfcc0d038663e5814ccda7e535d4d1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551434"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Leitfaden zum Co-Selling in Partner Center (PC) für Partner, die von Partner Sales Connect (PSC) migrieren

**Geeignete Rollen:** Kontoadministrator-| Empfehlungsadministrator-| Partner Sales Connect (PSC) seller | Partner Sales Connect(PSC) admin | Partner Sales Connect (PSC) Deal Manager

Dieser Artikel enthält Anleitungen für Partner, die von Partner Sales Connect (PSC) zu Partner Center (PC) migrieren, damit sie weiterhin Co-Selling-Deals in Partner Center erstellen und verwalten können.

>[!Note]
> Wenn Sie hier sind, weil Sie in PSC ein Banner zur Migration gesehen haben, sind Sie an der richtigen Stelle. Dieser Leitfaden gilt nicht für Geschäftspartner für die Lösungsbewertung (Solution Assessment, SA) und OEM-Lizenzierung, die ihre Angebote im PSC verwalten.

>[!Important]
> Ab dem 1. April 2021 kann Ihr Unternehmen keine Deals in PSC erstellen oder bearbeiten. **Sie können weiterhin die vorhandenen Dealdaten mithilfe der Massenexportfunktion in PSC herunterladen. Sie können auch offene Angebote von PSC zu Partner Center nach diesem Datum [migrieren.](psc-to-pc.md#psc-deals-migration)** <br><br> Wenn Sie aktiv an Deals arbeiten, die für IP-Co-Selling-Incentive geeignete Lösungen enthalten, haben Sie zwei Möglichkeiten: <br><br> 1. Markieren Sie den Deal als gewonnen, und schließen Sie die Dealregistrierung in PSC vor dem 31. März 2021 ab. <br> 2. [Migrieren Sie die Angebote](psc-to-pc.md#psc-deals-migration) zu Partner Center, damit Sie mehr Zeit für die Arbeit am Deal haben und mit der Dealregistrierung beginnen können.

Wie Sie wissen, **verliert das Unternehmen nach dem 30. April 2021 den Zugriff auf PSC.** Sie finden jedoch weiterhin alles, was Sie in Partner Center tun möchten, z. B. Erstellen von Co-Selling-Abschlüssen, Verwalten Ihrer Deals und Reagieren auf Angebote, die von Microsoft-Verkäufern an Sie gesendet werden.

Es gibt jedoch Unterschiede. Die folgende Anleitung kann Ihnen dabei helfen, den Übergang zu Partner Center reibungsloser und einfacher zu gestalten.

## <a name="before-you-move-things-you-need-to-know"></a>Bevor Sie verschieben, müssen Sie wissen, was Sie wissen müssen.

### <a name="if-you-are-a-psc-admin"></a>Als PSC-Administrator

- Sie benötigen eine Arbeits-E-Mail, um sich bei [Partner Center](https://partner.microsoft.com/)anzumelden.
- Richten Sie Ihr Konto mithilfe des [Partner Center-Kontoadministrators](permissions-overview.md)ein.
- Informationen zum Co-Selling in Partner Center finden Sie in diesem Dokument.
- Richten Sie Benutzerkonten in Partner Center für alle Ihre PSC-Benutzer (Administrator-, Deal-Manager- und Verkäuferrollen) ein, und weisen Sie ihnen [Empfehlungsadministratorrollen](permissions-overview.md)zu.

>[!IMPORTANT]
> Stellen Sie sicher, dass die im PSC-Banner angezeigte Microsoft Partner Network-ID (MPN) in der Liste der MPN-Standorte in Partner Center verfügbar ist.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Abbildung des PSC-Banners, in dem die Partner die MPN-ID finden.":::

 Um zu überprüfen, ob die MPN-ID als Partner Center MPN-Speicherort angezeigt wird, melden Sie sich beim Partner Center [Dashboard](https://partner.microsoft.com/dashboard)an, und wählen Sie dann oben rechts auf dem Bildschirm **Einstellungen** (zahnradsymbol) und dann **Kontoeinstellungen** aus. Wählen Sie im Navigationsmenü auf der zweiten Ebene auf der linken Seite Die Option **Standorte** aus, um die Liste aller MPN-IDs und Speicherorte anzuzeigen, die dem Partner Center-Konto zugeordnet sind.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Als PSC-Deal-Manager oder -Verkäufer

- Sie benötigen eine Arbeits-E-Mail, um sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard)anzumelden.
- Wenn Sie ein nicht geschäftsbezogenes Konto in PSC verwenden oder Ihre Geschäfts-E-Mail-Adresse für ein anderes Unternehmen als das Partnerunternehmen gilt, wenden Sie sich an Ihren PSC-Administrator, um Hilfe bei der Kontoset up-Einrichtung zu erhalten.
- Wenden Sie sich an Ihren PSC-Administrator, ob die Einrichtung Ihres Partner Center-Kontos unabhängig von dem Konto abgeschlossen ist, das Sie für die Anmeldung bei PSC verwenden.
- Überprüfen Sie, ob Sie Zugriff auf Partner Center und den Abschnitt Empfehlungen haben.
- Lesen Sie dieses Dokument, um die Workflows und die Änderungen in Partner Center zu verstehen.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Als Administrator in PSC sind dies Ihre nächsten Schritte.

Wählen Sie im linken **Navigationsmenü** Partner Center die Option Empfehlungen aus. Vergewissern Sie sich, dass Sie auf die Empfehlungsseiten zugreifen können.

  >[!Note]
  > Möglicherweise müssen Sie sich von Partner Center abmelden und sich wieder anmelden, um Ihre Anmeldeinformationen für den Zugriff auf die Empfehlungsseiten zu aktualisieren.

Wenn die Option **Empfehlungen** im Menü Partner Center oder auf Empfehlungen bezogene Seiten nicht angezeigt wird, wenden Sie sich an den [Kontoadministrator](permissions-overview.md) Ihres Unternehmens, und bitten Sie ihn, Ihnen Zugriff auf die Option Empfehlungen und den **zugehörigen** Bereich zu gewähren.

So suchen Sie den Kontoadministrator Ihres Unternehmens:

1. Wählen Sie im Zahnradsymbol oben rechts im dashboard Partner Center **kontoeinstellungen** aus.

1. Wählen Sie im linken Navigationsmenü der zweiten Ebene die Option **Benutzerverwaltung** aus.

1. Wählen Sie oben in der Benutzerliste das Dropdownmenü **Filter** aus. Ändern Sie die Option in **Kontoadministrator**.

   Auf der Seite werden alle Kontoadministratoren mit ihren jeweiligen E-Mail-Adressen angezeigt. Senden Sie eine E-Mail an eine dieser Benutzer, und bitten Sie sie, die Administratorrolle "Empfehlungen" für Ihr Arbeitskonto zuzuweisen.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Abbildung der Kontoadministratoren auf der Seite für die Benutzerverwaltung der Partnereinstellungen":::

>[!Important]
>- Wenn Ihre Rolle nur die Verwaltung von Benutzern in PSC umfasst, bitten Sie den Kontoadministrator Ihres Unternehmens, Ihnen die [Kontoadministratorrolle](permissions-overview.md#manage-mpn-membership-and-your-company) in Partner Center zuzuweisen. 
>- Wenn Ihre Rolle auch die Verwaltung von Co-Selling-Verkaufschancen umfasst, bitten Sie, die [Administratorrolle "Empfehlungen"](permissions-overview.md#manage-referrals) zu erhalten.
> - Es empfiehlt sich, auch einen Change Management-Lead unter den PSC-Administratoren zu benennen. Dadurch wird verhindert, dass alle PSC-Administratoren sich einzeln an Partner Center Kontoadministratoren gewendet müssen. Stattdessen kann der Change Management-Lead die primäre Person sein, die mit dem Partner Center-Kontoadministrator arbeitet.

## <a name="user-migration"></a>Benutzermigration

Nachdem Sie Ihr Konto in Partner Center eingerichtet haben, verwenden Sie den Benutzermigrations-Assistenten auf der Seite Co-Selling-Verkaufschancen, um Mitarbeitern Ihres Unternehmens automatisch Partner Center Rollen zuzuweisen.

>[!Note]
> Die Benutzermigration kann nur von [Kontoadministratoren](permissions-overview.md#manage-mpn-membership-and-your-company) Ihres Unternehmens durchgeführt werden. Wenn Sie nicht über die Kontoadministratorrolle verfügen, suchen Sie einen Kontoadministrator, der Sie beim Einrichten der Benutzerkonten mithilfe des Benutzermigrations-Assistenten unterstützen kann.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Abbildung des Benutzermigrations-Assistenten.":::

Kontoadministratoren wird auf der Seite co-selling opportunities (Co-Selling-Verkaufschancen) neben dem Leitfaden für Empfehlungen ein Link zum PsC-Benutzermigrations-Assistenten angezeigt. Sie können die Benutzermigration initiieren, indem sie auf den Link klicken. Um die Benutzermigration zu initiieren, können Administratoren den Link auswählen. Sie können diesen Benutzermigrationsschritt mehrmals ausführen, bis allen Benutzern in Partner Center die richtigen Rollen zugewiesen werden.

Die Benutzermigrationstabelle enthält die folgenden Details:

- Benutzerkonto: E-Mail-ID des Mitarbeiters
- PSC-Partnerkonto: Das Konto, dem der Mitarbeiter in PSC zugeordnet ist.
- PSC-Benutzerrolle: Eine der drei Rollen, die in PSC zugewiesen sind.
- PC-MPN-Speicherort: Der Speicherort, für den dem Benutzer relevante Partner Center (PC)-Rollen erteilt werden. Das PSC-Partnerkonto-MPN wird verwendet, um den entsprechenden MPN-Speicherort in Partner Center zu suchen, um Berechtigungen zuzuweisen. Die gesamte Organisation gibt die vOrg-MPN-ID an.
- PC-Benutzerrolle: Mitarbeitern werden Rollen basierend auf ihren PSC-Benutzerrollen zugewiesen. Administratoren in PSC werden Administratorrollen für Empfehlungen in Partner Center zugewiesen. Dem Verkäufer wird die Benutzerrolle "Empfehlungen" in Partner Center zugewiesen. Weitere Informationen zu den Partner Center Rollen und zu den Möglichkeiten von Benutzern mit diesen Rollen finden Sie in Partner Center [hier.](permissions-overview.md#manage-referrals)
- PC AAD-Mandant: der Microsoft Azure Active Directory-Mandant (Azure AD), dem die Benutzer in Partner Center
- Status: Es gibt drei mögliche Status für den Status der Migration.
    - **Nicht migriert:** Dem Benutzer ist keine Partner Center Empfehlungsrolle zugewiesen.
    - **Migriert:** Der Benutzer wurde erfolgreich migriert, und die entsprechende Rolle wurde zugewiesen, wie in der Tabelle gezeigt.
    - **Fehler:** Migration kann aufgrund eines Fehlers nicht abgeschlossen werden

Manchmal kann die Migration fehlschlagen und zu Fehlern führen. Im Folgenden finden Sie einige Gründe, warum eine Migration einen Fehler verursachen kann, und einige Möglichkeiten, das Problem zu beheben:

1. Die PSC-Benutzer verwenden möglicherweise ein nicht arbeitsbezogenes Konto.

2. Der PSC-Benutzer verwendet möglicherweise ein Konto aus einer anderen Domäne als dem, das Sie in Partner Center verwenden.

   Um Fehler im Zusammenhang mit Szenarios 1 und 2 zu beheben, bitten Sie den Benutzer, sich mithilfe des an Ihren Azure AD Mandanten angefügten Arbeitskontos bei Partner Center anzumelden. Ihr [globaler Administrator](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kann Ihnen dabei helfen.
   
   So finden Sie Ihren globalen Administrator: 
   - Melden Sie sich beim dashboard Partner Center an, [und](https://partner.microsoft.com/dashboard) wählen Sie oben rechts im Zahnradsymbol **Kontoeinstellungen** aus.
   - Wählen Sie in der linken Navigationsleiste der zweiten Ebene die Option **Benutzerverwaltung** aus.
   - Wählen Sie oben in der Benutzerliste das Dropdownmenü **Filter** aus, und ändern Sie die Option in **Globaler Administrator.** Auf der Seite werden dann alle globalen Administratoren mit ihren jeweiligen E-Mail-Adressen angezeigt. Bitten Sie einen dieser Benutzer, die Rolle "Empfehlungsadministrator" für Ihr Arbeitskonto zuzuweisen.
   
      Der globale Administrator kann entweder ein neues Benutzerkonto in Ihrem Azure AD Mandanten erstellen oder den anderen Domänenkontobenutzern Gastbenutzerzugriff zuweisen. Nachdem die Konten für alle PSC-Deal-Manager und -Benutzer eingerichtet wurden, müssen sie sich bei Partner Center anmelden, im linken **Navigationsmenü Empfehlungen** auswählen und bestätigen, dass die Seite Empfehlungen angezeigt wird.

3. Dem Benutzer ist bereits eine Empfehlungsrolle in Partner Center zugewiesen.
    - Sie können die vorhandene Rolle des Benutzers überprüfen. Wählen Sie in der oberen rechten Ecke von Partner Center **Einstellungen** (zahnradsymbol) und dann **Kontoeinstellungen** aus. Wenn ein zweites Navigationsmenü auf der linken Seite angezeigt wird, wählen Sie **Benutzerverwaltung** aus, und suchen Sie nach dem Benutzer.

## <a name="psc-deals-migration"></a>PSC Deals-Migration

Nachdem Sie die Benutzermigration abgeschlossen haben, verwenden Sie den Assistenten für die Migration von Deals auf der Seite Co-Selling-Verkaufschancen, um alle berechtigten offenen Angebote von PSC auf Partner Center zu bringen. **Der Migrationslink "Deals" ist nur für Empfehlungsadministratoren mit dem gesamten Organisationsumfang in Partner Center sichtbar.** Oben rechts auf der Seite Co-Selling-Verkaufschancen wird der Link **"PSC deal migration" (PSC-Dealmigration)** angezeigt, über den der Assistent für die Dealmigration geöffnet wird.

Lesen Sie diesen Abschnitt, bevor Sie mit der Dealmigration beginnen.

**Geeignet für die Migration**

Nur einige Angebote sind für die Migration von PSC zu Partner Center geeignet. Dieser Migrations-Assistent wurde entwickelt, um Partnern zu helfen, ihre Angebote in Partner Center zu bringen, in denen sie noch aktiv mit ihren Kunden zusammenarbeiten, um den Deal zu schließen. **Nur Angebote, die sich im offenen Zustand befinden, die ab dem 1. Januar 2020 mit gültigen Partnerkontodetails (gültige MPN-ID) erstellt wurden und sich nicht im Rahmen der Dealregistrierung befinden, sind für die Migration berechtigt.**

**Nicht für die Migration geeignet**

- Angebote für die Lösungsbewertung sind nicht für die Dealmigration geeignet.
- Oem licensing business deals are not eligible for deal migration (OEM-Lizenzverträge sind nicht für die Dealmigration geeignet)
- Alle Deals, die in PSC als gewonnen markiert wurden, sind nicht für die Migration geeignet. Die Dealregistrierung, wenn sie für die als gewonnen markierten Deals berechtigt ist, sollte in PSC abgeschlossen werden.

## <a name="pre-requisites-for-deal-migration"></a>Voraussetzungen für die Dealmigration

Bevor Sie mit der Dealmigration von Partner Center, befolgen Sie die folgenden Anweisungen, um die Deals in PSC für eine erfolgreiche Migration zu einrichten.

1. Alle Vertriebsteammitglieder in Ihrem Unternehmen, die an den offenen Geschäften arbeiten, werden über diese Migration informiert.
2. Die Mitglieder des Vertriebsteams werden für die Verwendung von Partner Center deal management trainiert.
3. Die Deals enthalten alle erforderlichen Informationen, wie unten beschrieben.
    - Details des Kundenunternehmens, einschließlich Name und Adresse
    - Kundenkontaktdetails, wenn es sich um einen Co-Sell-Deal handelt
    - Mindestens eine Lösung
    - Mindestens ein Teammitglied mit allen Details : Vorname, Nachname, E-Mail-ID und Telefonnummer
    - Dealwert
    - Geschätztes Abschlussdatum des Abschlusses
    - Partnerhinweise

Sie können die Funktionen zum Massendownload und -upload in PSC verwenden, um alle fehlenden Details im Deal für alle berechtigten Deals hinzuzufügen.

>[!Note]
> Die Dealmigration ist auch dann erfolgreich, wenn die oben genannten Voraussetzungen nicht erfüllt sind. Sie können den Status des Deal jedoch nicht ändern, wenn eines der oben genannten pflichtfelder in Partner Center nicht verfügbar ist. Sie müssen dann alle erforderlichen Informationen eingeben, die in den Deals in Partner Center, um mit der Arbeit an ihnen zu beginnen. **Es wird dringend empfohlen, die berechtigten Deals in PSC zu bereinigten, bevor Sie sie zu Partner Center.**

Die Dealmigration in Partner Center wird als 1-Klick-Erfahrung erstellt. Sie müssen nur die Schaltfläche **"Angebote migrieren"** auswählen, sobald Ihr Unternehmen bereit ist, die berechtigten Angebote zu migrieren. **Sie können nicht die Deals auswählen, die Sie von PSC migrieren möchten. Wenn Sie keine Abschlüsse zu Partner Center, verschieben Sie sie in psc in den geschlossenen Zustand, bevor Sie mit der Migration beginnen.**

>[!Note]
> Nach dem Initiieren der Migration kann es bis **zu 24** Stunden dauern, bis die Abschlüsse migriert werden.

Nach Abschluss der Migration hat sich der Status der Bannermeldung geändert, um den Abschluss mit einem Link zum Migrationsbericht zu erhalten. Laden Sie den Bericht herunter, um die Details der Abschlüsse anzuzeigen, die von PSC zu Partner Center.

Der Bericht enthält die folgenden Details.

1. **Partner Center Engagement-ID:** Der eindeutige Bezeichner in Partner Center für alle Deals in einem Engagement. Es gibt zwei Deals: einen für den Partner und einen für Microsoft in einem Co-Sell-Engagement in Partner Center.
2. **Partner Center Empfehlungs-ID:** Der eindeutige Bezeichner in Partner Center für den Deal, der zum Partner gehört.
3. **Dealname:** Bezeichner, der dem Deal in PSC gegeben wird.
4. **PSC-Deal-ID:** Der eindeutige Bezeichner in PSC für den Deal.
5. **Fehler:** Gibt an, ob bei der Migration eines bestimmten Deal ein Fehler auftritt.

Alle Erfolgreich migrierten Abschlüsse sind in PSC nicht sichtbar. Sie können weiterhin an den migrierten Abschlüssen in Partner Center einschließlich abschluss der Dealregistrierung in Partner Center. Es werden keine Änderungen an den Interaktionen mit den Microsoft-Verkäufern für Co-Sell-Deals vorgenommen.

Vom PSC migrierte Abschlüsse sind basierend auf der Quelle des Deals auf den Registerkarten Eingehend und Ausgehend verfügbar. Alle von Ihrem Unternehmen freigegebenen Deals sind auf der Registerkarte Ausgehend verfügbar, und von Microsoft initiierte Abschlüsse sind auf der Registerkarte Eingehend des Partner Center. Es gibt zwei Arten von Abschlüssen, die nach der Migration erstellt werden.

1. **Co-Sell-Deals:** Deals, die als Co-Sell in PSC gekennzeichnet sind, werden als Co-Sell-Deals in Partner Center.
2. **Partnerorientierte Deals:** Deals, die nicht als Co-Sell gekennzeichnet sind, werden als partnerorientierte Deals in Partner Center. Partnerorientierte Angebote sind für Microsoft-Verkäufer sichtbar und können auf Co-Sell-Deals aktualisiert werden, bevor sie den Endzustand erreichen (gewonnen, verloren). Darüber hinaus sind partnerorientierte Deals für die Registrierung des Deal berechtigt, wenn es eine geeignete Incentivelösung im Deal gibt.

>[!Important]
> Wenn Fehler auftreten, aufgrund derer einige Deals nicht migriert werden konnten, können Sie die Dealmigration erneut initiieren, indem Sie auf die Schaltfläche **"Deals migrieren" klicken.** Sie wird nur aktiviert, wenn noch einige berechtigte Abschlüsse migriert werden müssen. Dies ist auch hilfreich, wenn Sie sich in der Übergangsphase befinden, in der nach dem Initiieren der Dealmigration einige neue Deals in PSC erstellt werden.

Nachdem alle Deals erfolgreich migriert wurden, wird ein Banner mit dem Folgenden **angezeigt: "No deals to migrate"** (Keine Abschlüsse zu migrieren), und die Schaltfläche **"Migrate deals"** (Angebote migrieren) wird **deaktiviert.**

Verwenden Sie nach Abschluss der Benutzermigration und/oder Dealmigration die folgende Anleitung, um die Migrationsstrategie zu bestimmen:

Wenn Ihr Unternehmen über einen Partner Development Manager (PDM) verfügt: Wenn Ihr Partner Center-Konto eingerichtet ist und Ihre Benutzer umgezogen sind und über Rollen und Berechtigungen verfügen, können Sie Ihre Co-Selling-Aktivitäten in Partner Center. Informieren Sie den PDM, den Wechsel zu treffen, anstatt zu warten, bis die Migration abgeschlossen ist. Dadurch können alle ihre neuen Abschlüsse in Partner Center.

>[!Note]
>Nachdem Sie diesen Wechsel vorgenommen haben, können Sie nur noch auf die vorhandenen Active Deals in PSC einschreiten. Sie können weder neue Angebote erstellen noch Angebote von Microsoft-Verkäufern in PSC erhalten.

Wenn Ihr Unternehmen nicht über eine PDM-Datei verfügen: Stellen Sie sicher, dass alle Benutzerkonten von allen Benutzern eingerichtet und überprüft werden. Sie werden über eine E-Mail und ein Banner in PSC über das genaue Datum benachrichtigt, an dem Sie co-selling in Partner Center. Denken Sie daran, dass Sie weiterhin die vorhandenen aktiven Deals in PSC verwalten müssen.

>[!Important]
> Sie haben bis zum 30. April 2021 Zeit, die Als gewonnen markierten Deals zu registrieren.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Nächste Schritte für PSC-Administratoren, PSC-Deal-Manager und PSC-Verkäufer

Erfahren Sie, wie Sie co-sell in Partner Center.
Dies ist ein wichtiger Schritt, der Sie bei der Vorbereitung auf co-selling in Partner Center. Machen Sie sich mit den Workflows und den Änderungen Partner Center, damit Sie sofort effektiv Co-Sell nutzen können. Lesen Sie zunächst dieses Dokument vollständig. Eine gute Gruppe von Ressourcen ist auch im [Katalog co-sell experience verfügbar.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Wichtige Unterschiede zwischen PSC- und Partner Center Workflows

|**Szenario**|**Partner Sales Connect**|**Partner Center**|
|-----|:-----|:-----|
|Benutzerrollen|PSC verfügt über Administrator-, Deal-Manager- und Verkäuferrollen.|Partner Center verfügt nur über die [Rolle "Empfehlungsadministrator",](permissions-overview.md#manage-referrals) die sowohl Lese- als auch Schreibberechtigungen für alle Abschlüsse erteilt.|
|Einladen von Microsoft zu einem Co-Sell-Deal|Vom Microsoft-Verkäufer initiiert, wird der Partner nicht explizit gefragt.|Der Partner muss eine explizite [Anfrage stellen,](manage-co-sell-opportunities.md#add-solutions) wenn ein Microsoft-Verkäufer Hilfe für einen Deal benötigt. Der Microsoft-Verkäufer hat die Möglichkeit, die Anforderung zu ablehnen.|
|Expiry|Es gibt kein Konzept für den Ablauf eines Deal.|Eingehende Partnerangebote laufen in 14 Tagen ab, wenn sie vom Partner nicht akzeptiert werden. Dies gilt auch für ausgehende Partnerangebote, bei denen sie in einen abgelaufenen Zustand wechseln können, wenn der Microsoft-Verkäufer nicht in 14 Tagen auf sie einschließt.|
|Details zum Microsoft-Verkäufer|Wird angezeigt, sobald ein Deal erstellt wird.|Microsoft-Verkäuferdetails werden nur dann an partner weitergegeben, wenn der Verkäufer die Einladung zum Co-Selling vom Partner explizit akzeptiert.|
|[Private Pipeline](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Nicht verfügbar.|Partner können ihre Pipeline freigeben, ohne Microsoft-Verkäufern Transparenz zu bieten.|
|Lösungen|Lösungen, die nur zu einer Preisliste gehören, können einem Deal hinzugefügt werden.|Partner können Lösungen [hinzufügen,](manage-co-sell-opportunities.md#add-solutions) die zu den folgenden Listen gehören. a) Eigene Lösungen b) Lösungen aus dem Microsoft-Erstkatalog (ähnlich der Rolle "Transaktions deal" in PSC) und c) Co-Sell-Lösungen von anderen Drittanbieterpartnern (ähnlich der ISV Deal-Rolle in PSC).|
|Dealzuweisung|Nur zugewiesene Verkäufer können die Angebote anzeigen und entsprechend handeln.|Teammitglieder können zu einem Deal hinzugefügt werden, um die Personen anzugeben, die an einem Deal arbeiten. Andere Empfehlungsadministratoren können diese Deals nicht anzeigen oder für sie agieren.|
|Kundenorganisation|Freiformtexteintrag.|Sie können die [Kundenorganisation mit der](manage-co-sell-opportunities.md#select-your-customer) [Datenbank D&B](https://www.dnb.com/) durchsuchen, indem Sie nur einige Zeichen eingeben. Der rechtliche Name und die Adresse werden basierend auf der Auswahl automatisch aufgefüllt.|
|Kundenkontakt|Nicht obligatorisch.|Für die Freigabe privater Pipelines ist dies nicht zwingend erforderlich. Erforderlich, wenn der Microsoft-Verkäufer zur Teilnahme an einer Co-Selling-Anforderung eingeladen wird.|
|Öffentliche API|Nicht verfügbar.|[Öffentliche API](/partner/develop/referrals) zum programmgesteuerten Verwalten Partner Center Empfehlungen.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Ordnen Sie die Felder in PSC den entsprechenden Feldern in Partner Center

In diesem Abschnitt werden ausgewählte Screenshots für PSC mit der entsprechenden Ansicht im Abschnitt Partner Center Co-Selling-Verkaufschancen verglichen (oder "zuordnungen").

Auf jedem Screenshotpaar werden nummerierte, gelbe oder rote Kreise angezeigt:

- **Was bedeuten gelbe Kreise?** Nummerierte, gelbe Kreise werden zuerst auf jedem PSC-Screenshot angezeigt. Anschließend finden Sie einen Begleit-Partner Center Screenshot darunter mit vielen der gleichen Zahlen.

   Um zu sehen, wie jedes Feld oder Attribut in PSC seinem Pendant in Partner Center zugeordnet wird, passen Sie die nummerierten Kreise in den beiden verwandten Screenshots zusammen. Passen Sie z. B. die nummerierte, gelbe "1" im ersten PSC-Screenshot mit der nummerierten, gelben "1" im zweiten an, Partner Center Screenshot darunter.

- **Was bedeutet ein roter Kreis?** Wenn auf einem Screenshot ein roter Kreis angezeigt wird, der angibt, dass das PSC-Feld in Partner Center nicht verfügbar ist.

Psc-zu-Partner Center Feldzuordnungen werden für die folgenden Bereiche angezeigt:

1. PSC-Startseite, die der Standardansicht Partner Center Co-Selling-Verkaufschancen zugeordnet ist
1. PSC-Rasteransicht, die der Partner Center Deal-Ansicht zugeordnet ist
1. PSC-Detailansicht, die der Detailansicht des Partner Center zugeordnet ist
1. Psc Add Products view mapped to the Partner Center Add solutions view (PSC-Ansicht "Produkte hinzufügen", die der Ansicht "Lösungen hinzufügen" Partner Center zugeordnet ist)
1. PSC-Benutzerverwaltungsansicht, die der Ansicht Partner Center Benutzerverwaltung zugeordnet ist
1. PsC-Benutzerrollenzuweisungsansicht, die der Ansicht Partner Center Rollenzuweisung zugeordnet ist
1. PSC-Benachrichtigungsansicht, die der Partner Center Benachrichtigungsansicht zugeordnet ist

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1– PSC-Startseite, die der Standardansicht Partner Center Co-Selling-Verkaufschancen zugeordnet ist

Vergleichen Sie die übereinstimmenden nummerierten Kreise zwischen dem oberen PSC-Screenshot und dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise weisen darauf hin, dass kein übereinstimmendes Partner Center Feld vorhanden ist.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Abbildung der Feldzuordnungen zwischen der Startseite von Partner Sales Connect und der Standardansicht von Co-Selling-Verkaufschancen in Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2– PSC-Rasteransicht, die der Partner Center Deal-Ansicht zugeordnet ist

Vergleichen Sie die übereinstimmenden nummerierten Kreise zwischen dem oberen PSC-Screenshot und dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise weisen darauf hin, dass kein übereinstimmendes Partner Center Feld vorhanden ist.  

> [!NOTE]
> Weitere Überlegungen werden unterhalb der Screenshots angezeigt.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Abbildung der Feldzuordnungen zwischen der Partner Sales Connect(PSC)-Rasteransicht und der Partner Center Dealansicht." lightbox="images/pscmigration/grid-view-expanded.png":::

**Besondere Überlegungen:**

- Es gibt keine Listenansicht in Partner Center wie psc.  Alle Deals werden basierend auf dem datum des letzten Empfangs oder Erstellungsdatums mit den Kundeninformationen und dem Typ des Deals aufgelistet. Der erste Deal in der Ansicht ist standardmäßig ausgewählt. Die meisten Werte, die im PSC-Tabellenformat angezeigt werden, sind in der Detailansicht des Geschäfts in Partner Center verfügbar.
- Die Rolle "Deal" ist in Partner Center kein Pflichtfeld. Sie wird in keinem der Workflows angezeigt oder erfasst. Es wird automatisch auf der Seite des Microsoft-Verkäufers basierend auf den Lösungen abgeleitet, die dem Deal hinzugefügt wurden.
- Das Datum der letzten Änderung wird auf der Seite mit den Empfehlungsdetails in Partner Center nicht angezeigt. Partner können die Sortierfunktion verwenden, um die Deals basierend auf dem Datum der letzten Aktualisierung zu sortieren.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3– PSC Deal details view mapped to Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen Screenshot (PSC) mit dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise deuten darauf hin, dass in Partner Center kein übereinstimmendes Feld oder kein übereinstimmender Bereich vorhanden ist.

> [!NOTE]
> Weitere Überlegungen werden unterhalb der Screenshots angezeigt.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Abbildung der Feldzuordnungen zwischen der Detailansicht für Partner Sales Connect (PSC) und dem Partner Center Detailansicht." lightbox="images/pscmigration/deal-details-expanded.png":::

**Besondere Überlegungen:**

- Partner können ein Angebot bearbeiten, indem sie in der Detailansicht des Partnerdetails auf die Schaltfläche Bearbeiten klicken (6). Sobald die Schaltfläche "Bearbeiten" ausgewählt ist, können alle Felder bearbeitet werden. Sie haben dann die Möglichkeit, die am Deal vorgenommenen Änderungen zu speichern oder abzubrechen.
- Es gibt keine Option, den Deal in Partner Center als dupliziert zu schließen.
- Das Kundenergebnis ist in Partner Center nicht verfügbar. Alle Details im Zusammenhang mit Kundeninteraktionen können im Abschnitt Hinweise in Partner Center aktualisiert werden.
- Das geschätzte Abschlussdatum der Lösung ist nur für OEM-IOT-Angebote in Partner Center verfügbar. Diese Informationen werden für keine anderen Dealtypen angezeigt.
- Das Lizenzierungsprogramm ist in Partner Center nicht erforderlich. Diese Informationen werden basierend auf den im Deal ausgewählten Lösungen automatisch abgeleitet.

>[!Note]
>Ein als gewonnen oder verloren markierter Deal kann danach nicht mehr bearbeitet werden. Seien Sie vorsichtig, während Sie einen Deal in einen dieser Terminalzustände verschieben.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4– PSC-Ansicht "Produkte hinzufügen", die der Ansicht "Lösungen hinzufügen" Partner Center zugeordnet ist

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen Screenshot (PSC) mit dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise deuten darauf hin, dass in Partner Center kein übereinstimmendes Feld oder kein übereinstimmender Bereich vorhanden ist.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Abbildung der Feldzuordnungen zwischen der Ansicht Partner Sales Connect (PSC) zum Hinzufügen von Produkten und dem Partner Center Ansicht &quot;Lösungen hinzufügen&quot;" lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5: Benutzerverwaltung in PSC im Vergleich zu Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen Screenshot (PSC) mit dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise deuten darauf hin, dass in Partner Center kein übereinstimmendes Feld oder kein übereinstimmender Bereich vorhanden ist.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Abbildung der Feldzuordnungen zwischen der Benutzerverwaltungsseite von Partner Sales Connect (PSC) und der Seitenansicht Partner Center Benutzerverwaltung im Bereich &quot;Kontoeinstellungen&quot;."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6: Zuweisen von Benutzerrollen in PSC im Vergleich zu Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen Screenshot (PSC) mit dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise deuten darauf hin, dass in Partner Center kein übereinstimmendes Feld oder kein übereinstimmender Bereich vorhanden ist.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Abbildung der Feldzuordnungen zwischen der Rollenzuweisungsansicht &quot;Partner Sales Connect&quot; (PSC) und der Ansicht &quot;Partner Center Rollenzuweisung&quot;." lightbox="images/pscmigration/roles-expanded.png":::

**Besondere Überlegungen:**

- Die entsprechende Rolle für den PSC-Administrator ist die Kontoadministratorrolle in Partner Center.
- Es gibt nur eine Rolle in Partner Center für die Co-Selling-Dealverwaltung. Diese Rolle ist die Empfehlungsadministratorrolle.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7: Benachrichtigungen in PSC im Vergleich zu Partner Center

Vergleichen Sie die übereinstimmenden, nummerierten Kreise im oberen Screenshot (PSC) mit dem Partner Center Screenshot darunter. Übereinstimmende Zahlen zeigen an, wo Sie das PSC-bezogene Feature oder Attribut in Partner Center finden. Rote Kreise deuten darauf hin, dass in Partner Center kein übereinstimmendes Feld oder kein übereinstimmender Bereich vorhanden ist.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Abbildung der Zuordnung zwischen den PsC-Benachrichtigungen (Partner Sales Connect) und der Partner Center-Benachrichtigungsansicht"  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Wechsel von PSC zu Partner Center – Häufig gestellte Fragen

In den folgenden Abschnitten werden häufig gestellte Fragen zur Migration beantwortet.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – Was soll ich tun, wenn ich keinen Zugriff auf Partner Center habe?

Sie können sich an Ihre Administratoren wenden, die auf der Seite "Kein Zugriff" aufgeführt sind, um die zugewiesenen Rollen zu erhalten. Sie benötigen die [Rolle "Empfehlungsadministrator"](permissions-overview.md#manage-referrals) für die Lese- und Schreibberechtigung im Abschnitt "Empfehlungen". Wenn Sie nur Geschäftsprofile verwalten, benötigen Sie die Administratorrolle "Geschäftsprofil" im Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Abbildung der Nichtzugriffserfahrung in Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – Wer kann mir Zugriff auf den Abschnitt Empfehlungen in Partner Center gewähren?

Ihr [Kontoadministrator](permissions-overview.md#manage-mpn-membership-and-your-company) kann Ihnen Zugriff auf die Registerkarte Empfehlungen gewähren. Um Ihren Kontoadministrator zu finden, wählen Sie im Zahnradsymbol oben rechts im dashboard Partner Center die Option **Kontoeinstellungen** [aus.](https://partner.microsoft.com/dashboard) Wählen Sie dann in der Navigationsleiste auf der zweiten Ebene die Option **Benutzerverwaltung** aus. Wählen Sie oben in der Benutzerliste das Dropdownmenü **Filter** aus, und ändern Sie die Option in **Kontoadministrator.** Auf der Seite werden alle Kontoadministratoren mit ihren jeweiligen E-Mail-Adressen angezeigt. Bitten Sie einen dieser Benutzer, die Rolle "Empfehlungsadministrator" für Ihr Arbeitskonto zuzuweisen.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3– Die Schaltfläche +neuer Deal ist für unser Konto abgeblendet. Was soll ich tun, um mit der Erstellung von Abschlüssen zu beginnen?

Dies geschieht nur, wenn der MPN-Organisation, die Sie in der MPN-Organisation verwenden, keine Co-Sell Ready-Lösungen Partner Center. Wenden Sie sich an Ihren PDM, um die MPN-ID Ihrer Lösungen zu korrigieren, oder erstellen Sie ein Supportticket, in dem das Problem "Schaltfläche "Neuer Deal" nach der PSC-Migration ausgegraut angezeigt wird.

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4. Kann ich einer bestimmten Person aus unserer Organisation wie PSC Angebote zuweisen?

Sie können Teammitglieder einem bestimmten Deal zuweisen. Sie blockiert nicht, dass andere Empfehlungsadministratoren diese Deals anzeigen oder für diese handeln.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5. Gibt es eine Ansicht aller mir zugewiesenen Deals?

Sie können die Favoritenfunktion verwenden, bei der es sich um eine Registerkarte auf Benutzerebene handelt. Sie können alle Deals, die Ihnen zugewiesen sind, als Favoriten markieren, um einen schnellen Zugriff auf die Deals zu erhalten.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6. Gibt es eine schreibgeschützte Ansicht für die Deals?

Nein, es gibt keine schreibgeschützte Ansicht der Deals im Abschnitt "Empfehlungen". Alle Empfehlungsadministratoren verfügen über vollständigen Lese- und Schreibzugriff auf alle Angebote.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7. Wie kann ich einen Deal registrieren, nachdem ich ihn als gewonnen markiert habe?

Wenn der Deal die unten angegebenen Kriterien erfüllt, wird ein Popupfenster zum Starten der [Dealregistrierung angezeigt.](./register-deals.md)

- Dem Deal ist eine incentivefähige Lösung zugeordnet.
- Microsoft-Verkäufer werden eingeladen, am Deal teilzunehmen, oder sie haben Sie zu dem Deal eingeladen.
- Die Microsoft-Karte befindet sich im Status Akzeptiert oder Gewonnen in Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8– Ich habe eine Fehlermeldung erhalten, wenn ich im Abschnitt Deal Registration (Dealregistrierung) auf die Schaltfläche "+New deal registration" (+Registrierung neuer Deal) klicke. Wie kann ich meine Angebote registrieren?

Die **Schaltfläche +New deal registration** (+Neue Dealregistrierung) soll nur von den Partnern verwendet werden, die im ISV Connect-Programm registriert sind, um einen Deal ohne entsprechende Co-Sell-Verkaufschance in der Partner Center. Für die Registrierung von Geschäften mit einer Co-Sell-Verkaufschance wird ein Popupfenster angezeigt, wenn der Deal als gewonnen markiert ist und die Kriterien für die Dealregistrierung erfüllt sind.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9. Ist das Hinzufügen einer Kundenorganisation obligatorisch?

Ja, das Hinzufügen [einer Kundenorganisation](./manage-co-sell-opportunities.md#select-your-customer) ist in der Partner Center. Suchen Sie zunächst nach dem Standort, an dem sich der Kunde befindet. Basierend auf den Details, die Sie haben; Sie können spezifisch sein, einschließlich des genauen Gebäudenamens, oder geben Sie einfach Ortsdetails an. Die Organisationssuche ruft alle juristischen Personen ab, die mit dem von Ihnen eingeben Namen übereinstimmen, sodass Sie keine Adressdetails eingeben müssen. Alle Details werden basierend auf der ausgewählten Organisation automatisch ausgefüllt.

### <a name="10---are-customer-contact-details-mandatory"></a>10 – Sind Kundenkontaktdetails obligatorisch?

Hängt vom Typ [des Deal ab,](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) den Sie erstellen. Wenn Sie Ihre Pipeline nur freigeben und keine Hilfe von der Microsoft-Vertriebsorganisation benötigen, können Sie auswählen, dass Sie keine Kundenkontaktinformationen geben möchten. Wenn Sie beim Co-Selling aktiv Hilfe beim Microsoft-Verkäufer suchen, müssen Sie die Kontaktdetails des Kunden bereitstellen. Sie sollten eine explizite Zustimmung des Kunden erhalten, bevor Sie eine Co-Sell-Anforderung im Partner Center erstellen.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – Wie viele Lösungen kann ich einem Deal hinzufügen?

Sie können einem Deal bis zu 50 Lösungen (analog zu "Produkten" in PSC) hinzufügen. Im Gegensatz zu PSC können Sie Lösungen aus Ihren eigenen für den Co-Sell berechtigten Lösungen, Microsoft-ERST-SKUs und anderen Drittanbieterlösungen kombinieren, die für den Co-Sell geeignet sind. Es gibt keine Deal-Rolle, die im Partner Center ausgewählt oder verfügbar sein soll. Für Microsoft-SKUs können Sie optional Menge und Preis für jede SKU hinzufügen, die dem Deal hinzugefügt wird.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12. Wann werden die Details des Microsoft-Verkäufers nach dem Erstellen eines Deals bekannt?

Microsoft-Verkäufer werden erst zugewiesen, nachdem sie die genaue Hilfeanforderung erfüllt haben, die beim Erstellen des Deal mit der relevanten Verkäuferpersona auf Microsoft-Seite angegeben wurde. Auch nach der Zuweisung haben Microsoft-Verkäufer die Möglichkeit, die Co-Sell-Einladung entweder anzunehmen oder abzulehnen. Nur wenn eine Co-Sell-Einladung von einem Verkäufer akzeptiert wird, wird der Deal mit den Kontaktdetails des Microsoft-Verkäufers aktualisiert. Die SLA für Microsoft-Verkäufer, die auf den Deal zu handeln haben, beträgt 14 Tage. Es handelt sich um die gleiche SLA, die Partner für den Deal tun müssen, bevor er in den Status "Abgelaufen" übergeht.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – Wo finde ich die Verkaufschance-ID?

Die Opportunity-ID in PSC ist identisch mit der Deal-ID in Partner Center. Sie finden die Deal-ID neben dem Dealnamen, wenn Sie einen Deal öffnen.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14: Wie kann meine PDM Zugriff auf Partner Center?

Partner Center können ihre PDMs im Gegensatz zu PSC nicht direkt auf sie zugreifen. Es gibt mehrere Optionen zum Aktivieren dieser Funktion, die unten erwähnt werden.

- OCP Insights: Wenn PDMs nur die damit verbundenen Deals und Denkfortschritte anzeigen, können sie das Insights-Portal von One Commercial Partner (OCP) verwenden, um Ihre Organisation anzeigen zu lassen. Dies ist ein internes Tool, das nur für PDMs verfügbar ist. OCP-Erkenntnisse sind für die Benutzer Ihres Unternehmens nicht verfügbar.
- Gastbenutzer in Partner Center: Sie können Ihr PDM-Konto als Gastbenutzer im Partner Center hinzufügen und ihm die Rolle "Empfehlungsadministrator" zuweisen, damit er Empfehlungen anzeigen und darauf zugreifen @microsoft.com kann.
- Erstellen eines neuen Benutzers [in](./create-user-accounts-and-set-permissions.md#add-a-new-user) Ihrem Mandanten: Sie können einen neuen Benutzer in Ihrem eigenen Mandanten erstellen und diese Details mit dem PDM teilen, damit er Empfehlungen ähnlich wie andere Empfehlungsbenutzer in Ihrem Konto anzeigen und darauf agieren kann.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Suchen der richtigen MPN-ID, wenn Ihr Konto in PSC nicht einem gültigen MPN zugeordnet ist

Wenn Sie sich hier befinden, weil sie ein Banner in PSC mit der Kennung "PSC invalid MPN ID association problem" (PSC: Problem mit ungültiger MPN-ID-Zuordnung) gesehen haben, befinden Sie sich an der richtigen Stelle. Möglicherweise wurde Ihr Konto aus folgenden Gründen mit einer ungültigen MPN-ID verknüpft:

- Ihr Unternehmen hat kein Partner Center Konto.
- Ihr PDM hat bei der Eingabe der MPN-ID Ihres Kontos in den internen Systemen, die Ihr PSC-Konto mit Ihrem Partner Center(MPN-ID) verknüpfen, einen Fehler gemacht.
- Ihr Unternehmen hat die Migration von Partner Membership Center (PMC) zu Partner Center.

Suchen Sie zunächst die richtige MPN-ID, indem Sie die folgenden Schritte ausführen.

- Melden Sie sich bei Ihrem Partner Center konto an.
- Verwenden Sie die Anleitung in der Dokumentation [zu den Kontoeinstellungen,](./partner-center-account-setup.md#locate-your-mpn-id) um die MPN-ID zu finden.

Unten sehen Sie einen Screenshot, der den genauen Standort zeigt, an dem Sie Ihre mpn Partner Center-ID finden.

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Abbildung der Kontoeinstellungen, in denen der Partner seine MPN-ID finden kann."  lightbox="images/pscmigration/findingMPNID.png":::

Als Nächstes

- Wenn Sie über eine PDM-Datei verfügen, bitten Sie sie, Ihre MPN-ID mit der richtigen MPN-ID aus Ihrem Partner Center-Konto zu korrigieren.
- Wenn Sie nicht über eine PDM verfügen, senden Sie eine E-Mail an die Adresse, die im PSC-Banner angegeben ist, mit den psc-Kontoinformationen, die im PSC-Banner angezeigt werden, und der richtigen MPN-ID aus Ihrem Partner Center-Konto.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Ressourcen zum Erstellen und Verwalten Ihrer Angebote in Partner Center

Wenn Sie die Co-Sell-Hilfethemen noch nicht gelesen haben, helfen Ihnen die folgenden Ressourcen bei der Verwaltung von Geschäften im Partner Center.

|**Aufgabe**   |**Artikel**   |
|-----------------------|:-----------------------|
|Grundlegendes zu den Registerkarten und zur Navigation auf der Seite "Co-Sell Opportunities"|[Navigieren im Abschnitt "Co-Sell"](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Auswählen einer Kundenorganisation aus der D&B-Liste |[Wählen Sie Ihren Kunden aus.](./manage-co-sell-opportunities.md#select-your-customer)|
|Ändern der Felder im Abschnitt "Dealdetails"|[Dealdetails](./manage-co-sell-opportunities.md#deal-details)|
|Hinzufügen ihrer Teammitglieder zu einem Dealteam|[Hinzufügen Ihrer Mitarbeiter](./manage-co-sell-opportunities.md#add-team-members)|
|Reagieren auf einen Co-Sell-Deal|[Verwalten von Co-Sell-Deals](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registrieren Sie Abschlüsse, die Sie in Partner Center |[Registrieren eines neuen Angebots](./register-deals.md)
|Gewinnen sie Erkenntnisse zu Empfehlungen, und erfahren Sie, wie Sich ihre Empfehlungen befinden. |[Einblicke zu Empfehlungen](./referral-insights.md)
|Erstellen und Verwalten von Geschäftsprofilen|[Verwalten von Geschäftsprofilen](./create-a-marketing-profile.md)
|Verwalten von Leads für Ihr Geschäftsprofil |[Verwalten von Leads](./manage-leads.md)|

## <a name="next-steps"></a>Nächste Schritte


- [Partner Sales Connect to Partner Center workbook](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) (Partner sales Connect mit Partner Center Arbeitsmappe) – Arbeitsmappe zum Ausrichten der Vertriebsprozesse und -rollen von Partnern an neuen Vertriebsprozessen über Partner Center im Vergleich zu Partner Sales Connect.
- Partner Center Leitfaden für den Co-Sell-Betrieb: Anleitung zum Identifizieren eines Betriebsmodells über Partner Center, um Leads oder [Co-Sell-Verkaufschancen](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) zu verwalten und Deals zu registrieren.
- [Empfehlungsverwaltungs-Deck:](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) Visualisierte Schritt-für-Schritt-Anleitung zum Verwalten von Leads und Co-Sell-Verkaufschancen über Partner Center.
- [Veröffentlichen und Verwalten im](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) kommerziellen Marketplace: Visualisierte Schritt-für-Schritt-Anleitung zum Erstellen, Verwalten und Veröffentlichen von Angeboten über Partner Center im kommerziellen Marketplace.