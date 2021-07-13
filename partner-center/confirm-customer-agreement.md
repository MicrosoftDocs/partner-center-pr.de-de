---
title: Bestätigen, dass Ihr Kunde die Microsoft-Kundenvereinbarung für das CSP-Programm akzeptiert hat
description: CSP-Partner (Cloud Solution Provider) müssen vor dem Bestellen von Microsoft-Diensten für Kunden die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung bestätigen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277010"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Bestätigen, dass Ihr Kunde die Microsoft-Kundenvereinbarung für das CSP-Programm akzeptiert hat

**Geeignete Rollen:** Administrator-Agent | Vertriebsbeauftragter


Kunden haben zwei Möglichkeiten, die Microsoft-Kundenvereinbarung zu akzeptieren.

**Option 1**: Der Partner bestätigt die Zustimmung des Kunden – Der Partner kann die Zustimmung des Kunden über die Partner Center-API, das Partner Center SDK oder das Partner Center-Dashboard bestätigen.

**Option 2**: Der Kunde stimmt direkt zu: Der Partner kann den Kunden über eine URL einladen, damit dieser die Vereinbarung in Microsoft 365 Admin Center überprüfen und ihr zustimmen kann.

## <a name="access-microsoft-customer-agreement-template"></a>Zugreifen auf die Vorlage für die Microsoft-Kundenvereinbarung

[Hier](https://aka.ms/customeragreement) kannst du die neueste Version der Vorlage für die Microsoft-Kundenvereinbarung manuell herunterladen. Die Microsoft-Kundenvereinbarung ist länderspezifisch. Achte beim Anfordern der Vorlage für die Microsoft-Kundenvereinbarung darauf, basierend auf dem Standort des Kunden das richtige Land/die richtige Region auszuwählen.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Option 1: Bestätigen der Zustimmung des Kunden in Partner Center

Partner mit direkter Abrechnung können die Zustimmung bestehender und neuer Kunden zur Microsoft-Kundenvereinbarung in Partner Center bestätigen. Indirekte Wiederverkäufer können keine Bestätigung im Namen ihrer Kunden abgeben und müssen mit ihrem indirekten Anbieter zusammenarbeiten, um den Vorgang abzuschließen.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Bestätigen der Kundenzustimmung für Neukunden

Wenn Sie in Partner Center einen Mandanten für einen Neukunden erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert hat. Um diese Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus.

2. Machen Sie unter **Kontoinformationen** Angaben zum Unternehmen und seinem primären Kontakt.

3. Aktiviere unter der Option für die **Microsoft-Vereinbarung** das entsprechende Kontrollkästchen, um zu bestätigen, dass der Kunde der Microsoft-Kundenvereinbarung zugestimmt hat.

4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind. Sind sie nicht korrekt, wähle **Aktualisieren** aus, und gib die richtigen Informationen für die Person ein, die die Vereinbarung akzeptiert hat.

6. Wähle **Weiter** aus, um die Erstellung des Kundenmandanten fortzusetzen.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Neukunde.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Bestätigen der Kundenzustimmung für einen Bestandskunden

Um die folgenden Schritte ausführen zu können, musst du Administrator-Agent oder Vertriebsbeauftragter sein:

1. Wählen Sie **Kunden** aus. Suchen und wählen Sie den Kunden aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Wählen Sie unter **Microsoft-Kundenvertrag** die Option **Aktualisieren** aus.

4. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Wählen Sie **Speichern und fortfahren** aus.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestandskunde.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Abrufen der Bestätigung der Kundenzustimmung für einen Bestandskunden

Mithilfe der folgenden Schritte können Sie eine Bestätigung abrufen, dass ein Bestandskunde die Microsoft-Kundenvereinbarung akzeptiert hat. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Unter **Microsoft-Kundenvertrag** wird angezeigt, ob die Bestätigung durch diesen Kunden erfolgt ist.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Bestätigen der Zustimmung des Kunden über die Partner Center-API oder das Partner Center SDK

Du kannst die Partner Center-API oder das Partner Center SDK verwenden, um die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung zu bestätigen. Ausführliche Informationen zur API bzw. zum SDK findest du unter:

- [Abrufen von Vertragsmetadaten für den Microsoft-Kundenvertrag](/partner-center/develop/get-customer-agreement-metadata)

- [Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Abrufen der Bestätigung der Kundenakzeptanz zur Microsoft-Kundenvereinbarung](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Abrufen eines Downloadlinks für die Vorlage des Microsoft-Kundenvertrags](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Option 2: Zustimmung des Kunden im Microsoft 365 Admin Center

Partner können neue und bestehende Kunden über eine URL einladen, die Vereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen. In den nächsten Abschnitten wird Folgendes erläutert:

- Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

- Einladen eines neuen Kunden, die Handelspartnerbeziehung und -vereinbarung zu überprüfen und diesen zuzustimmen

- Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

>[!NOTE]
> Sie können die [Partner Center-API oder das Partner Center SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) verwenden, um den Status der direkten Zustimmung eines Kunden zur Microsoft-Kundenvereinbarung zu ermitteln.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

Mit den folgenden Schritten kannst du einen neuen Kunden im Partner Center erstellen und dann einladen, die Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen.

1. Wähle im Partner Center auf der Registerkarte **Kunden** die Option **Kunden hinzufügen** aus.

2. Gib unter **Kontoinformationen** in allen Pflichtfeldern die Informationen zum neuen Kunden ein, darunter auch der Firmenname und Hauptkontakt des Kunden.

3. Wählen Sie unter **Kundenvereinbarung** die Option **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Der Kunde wird aufgefordert, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen) aus. Fülle alle weiteren Pflichtfelder auf der Seite aus.

4. Wählen Sie **Weiter: Überprüfung** aus und führen Sie dann die Schritte zum Erstellen des Kundenmandanten aus. 

>[!NOTE] 
>Neue Kunden können erst einen Kauf tätigen, nachdem sie der Microsoft-Kundenvereinbarung zugestimmt haben.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Erstellen eines neuen Kunden.":::

5. Sobald im Workflow für neue Kunden der Bildschirm **Bestätigung** angezeigt wird, musst du die Anmeldeinformationen des Kunden speichern. Diese Anmeldeinformationen musst du später dem Kunden mitteilen.

6. Erstelle und sende außerhalb von Partner Center eine E-Mail, um den Kunden einzuladen, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen. Die folgenden Elemente müssen in der E-Mail enthalten sein:

   - Ein Link zu dieser [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Anmeldung erforderlich)

   - Die in Schritt 5 gespeicherten Anmeldeinformationen des Kunden.

7. Der Kunde erhält dann die E-Mail-Einladung vom Partner und wählt die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) aus.

8. Der Kunde meldet sich mit den von Ihnen erhaltenen Kundenanmeldeinformationen beim Microsoft 365 Admin Center an.

9. Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Einladen eines neuen Kunden, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen 

Mit den folgenden Schritten kannst du einen neuen Kunden einladen, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen. 

1. Wähle im Partner Center auf der Registerkarte **Kunden** den Link **Vertriebspartnerschaft beantragen** aus. 

2. Dadurch wird eine automatische E-Mail-Vorlage generiert, die Text und eine parametrisierte URL enthält, durch die der Kunde zum Microsoft 365 Admin Center weitergeleitet wird.

3. Du kannst die automatisch generierte E-Mail-Vorlage anpassen und dann **In Zwischenablage kopieren** oder **In E-Mail öffnen** auswählen.

4. Verwende diese E-Mail-Vorlage, um den Kunden einzuladen, dem Antrag auf eine **Handelspartnerschaft** und der **Microsoft-Kundenvereinbarung** zuzustimmen. (Anmerkung: Achte darauf, dass der Partner in der E-Mail-Einladung auch die automatisch bereitgestellte URL und die kürzlich erstellten Kundenanmeldeinformationen angibt.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Erstellen einer Beziehung.":::

5. Der Kunde empfängt die Einladung per E-Mail und klickt auf die parametrisierte URL. 

6. Der Kunde verwendet die von Ihnen in der E-Mail bereitgestellten Anmeldeinformationen, um sich beim Microsoft 365 Admin Center anzumelden.

7. Der Kunde aktiviert das Kontrollkästchen, um der **Handelspartnerbeziehung** und **Microsoft-Kundenvereinbarung** zuzustimmen. 

8. Der Kunde kann unter derselben URL eine konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet. Er kann einen Partner auswählen, um Details anzuzeigen.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Annehmen einer Vereinbarung.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

Mit den folgenden Schritten kannst du einen bestehenden Kunden einladen, die Microsoft-Kundenvereinbarung zu überprüfen und ihr zuzustimmen. 

1. Erstelle die Kunden-E-Mail mit der eingebetteten URL, um deinen Kunden einzuladen, der Microsoft-Kundenvereinbarung zuzustimmen.

2. Der Kunde erhält die Einladung per E-Mail und klickt auf die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Der Kunde gibt seine Anmeldeinformationen in Microsoft 365 Admin Center ein.

4. Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen. 

5. Der Kunde kann unter derselben URL die konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet. Er kann einen Partner auswählen, um Details anzuzeigen.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Kunde.":::

>[!NOTE]
>In bestimmten Szenarien können Kunden der Microsoft-Kundenvereinbarung u. U. nicht direkt zustimmen. Weitere Informationen zu diesen Situationen finden Sie unter „Zwei Szenarien, in denen Sie die Zustimmung im Namen Ihres Kunden bestätigen müssen“.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Zwei Szenarien, in denen du die Zustimmung im Namen deines Kunden bestätigen musst

Es gibt zwei Szenarien, in denen Kunden der Microsoft-Kundenvereinbarung möglicherweise nicht direkt im Microsoft 365 Admin Center zustimmen können.

**Szenario 1:** Ein Bestandskunde hat über eine bestehende Partnerbeziehung eines der folgenden Produkte erworben: Angebote, Software oder Softwareabonnements, reservierte Instanzen oder einen Azure-Plan. Der Kunde versucht nun, einen neuen Kauf zu tätigen (außer einer automatischen Verlängerung). Wenn dieser Kunde auf die URL klickt, erhält er die Mitteilung, dass er sich an seinen Partner wenden soll, um die Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen.  

**Lösung**: Du musst die Zustimmung im Namen des Kunden bestätigen.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot: Seite im Microsoft 365 Admin Center mit der Bitte, sich an Ihren Partner zu wenden, um Ihre Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen":::

**Szenario 2**: Ein bestehender Kunde hat eines der folgenden Produkte erworben: Angebote, Software und Softwareabonnements, reservierte Instanzen und einen Azure-Plan. Der Kunde versucht nun, einen neuen Kauf bei einem neuen Partner zu tätigen.

Wenn der Kunde auf die URL für das Microsoft 365 Admin Center klickt, um der neuen Partnerbeziehung und Vereinbarung zuzustimmen, erhält er die Mitteilung, dass er sich an seinen Partner wenden soll, um die Zustimmung zur Microsoft-Kundenvereinbarung zu bestätigen.  

**Lösung**: Du musst die Zustimmung im Namen des Kunden bestätigen.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Bestätigen, dass ein Kunde der Vereinbarung zugestimmt hat

Wenn Sie versuchen, einen neuen Auftrag für einen vorhandenen Kunden zu erstellen, den Sie zuvor noch nicht bestätigt haben, erhalten Sie eine Aufforderung, die Bestätigung abzuschließen. Führen Sie dazu die nachfolgend aufgeführten Schritte aus.

1. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) des Benutzers ein, der dem Vertrag zugestimmt hat.

2. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

3. Wählen Sie **Speichern und fortfahren** aus. 

## <a name="next-steps"></a>Nächste Schritte

- [Überprüfen oder Aktualisieren Ihrer Unternehmensprofilinformationen](update-your-partner-profile.md)
- [Microsoft-Kundenvereinbarungen (nach Region, Sprache)](Agreements.md)
