---
title: Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahre, wie du bestätigst, dass ein Kunde der Microsoft-Kundenvereinbarung zugestimmt hat. Dies ist für CSPs erforderlich, um Microsoft-Produkte und -Dienste für Kunden zu bestellen.
author: LauraBrenner
ms.author: labrenne
keywords: Kunden, Kunden, Zustimmung, MCA, Microsoft Cloud-Vertrag, Microsoft-Kundenvertrag, Vorlagen für Kundenverträge
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c6d67c7e970d042704e1cc1c731d6ae1e85d6687
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453267"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Bestätigen der Zustimmung des Kunden zur Microsoft-Kundenvereinbarung im CSP-Partnerprogramm

**Zielgruppe**

- Partner Center
- Microsoft 365 Admin Center

**Geeignete Rollen**

- Administrator-Agent
- Vertriebsbeauftragter

**Geeignete Partnertypen**

- Indirekte Handelspartner, Partner mit direkter Abrechnung, indirekte Anbieter

Am 1. Oktober 2019 hat Microsoft die **Microsoft-Kundenvereinbarung** für das CSP-Programm eingeführt, die den Microsoft Cloud-Vertrag ersetzt. Zusätzliche Informationen findest du in den [Anleitungen](indirect-reseller-tasks-in-partner-center.md) für indirekte Handelspartner. Um die Migration von Partnern zur neuen Vereinbarung zu erleichtern, werden beide Vereinbarungen bis zum 31. Januar 2020 unter dem CSP-Programm fortgeführt. Ab dem 1. Februar 2020 wird der Microsoft Cloud-Vertrag durch die Microsoft-Kundenvereinbarung ersetzt.

Kunden haben zwei Möglichkeiten, die Microsoft-Kundenvereinbarung zu akzeptieren. 

**Option 1**: Der Partner bestätigt die Zustimmung des Kunden – Der Partner kann die Zustimmung des Kunden über die Partner Center-API, das Partner Center SDK oder das Partner Center-Dashboard bestätigen.

**Option 2**: Der Kunde stimmt direkt zu: Der Partner kann den Kunden über eine URL einladen, damit dieser die Vereinbarung in Microsoft 365 Admin Center überprüfen und ihr zustimmen kann.

## <a name="access-microsoft-customer-agreement-template"></a>Zugreifen auf die Vorlage für die Microsoft-Kundenvereinbarung

[Hier](https://aka.ms/customeragreement) kannst du die neueste Version der Vorlage für die Microsoft-Kundenvereinbarung manuell herunterladen. Die Microsoft-Kundenvereinbarung ist länderspezifisch. Achte beim Anfordern der Vorlage für die Microsoft-Kundenvereinbarung darauf, basierend auf dem Standort des Kunden das richtige Land/die richtige Region auszuwählen.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Option 1: Bestätigen der Zustimmung des Kunden in Partner Center

Partner können die Zustimmung bestehender und neuer Kunden zur Microsoft-Kundenvereinbarung in Partner Center bestätigen. Handelspartner können keine Bestätigung im Namen ihrer Kunden abgeben und müssen mit ihrem indirekten Anbieter zusammenarbeiten, um den Vorgang abzuschließen.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Bestätigen der Kundenzustimmung für Neukunden

Wenn Sie in Partner Center einen Mandanten für einen Neukunden erstellen, führen Sie die folgenden Schritte aus, um zu bestätigen, dass der Kunde den Microsoft-Kundenvertrag akzeptiert hat. Um diese Schritte ausführen zu können, müssen Sie Administrator-Agent oder Vertriebsbeauftragter sein.

1. Wählen Sie **Kunden** und dann **Neuer Kunde** aus.

2. Machen Sie unter **Kontoinformationen** Angaben zum Unternehmen und seinem primären Kontakt.

3. Aktiviere unter der Option für die **Microsoft-Vereinbarung** das entsprechende Kontrollkästchen, um zu bestätigen, dass der Kunde der Microsoft-Kundenvereinbarung zugestimmt hat.

4. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Stellen Sie sicher, dass die angezeigten Kontaktinformationen für den primären Benutzer korrekt sind. Sind sie nicht korrekt, wähle **Aktualisieren** aus, und gib die richtigen Informationen für die Person ein, die die Vereinbarung akzeptiert hat.

6. Wähle **Weiter** aus, um die Erstellung des Kundenmandanten fortzusetzen.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Neukunde":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Bestätigen der Kundenzustimmung für einen Bestandskunden

Um die folgenden Schritte ausführen zu können, musst du Administrator-Agent oder Vertriebsbeauftragter sein:

1. Wählen Sie **Kunden** aus. Suchen und wählen Sie den Kunden aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Wählen Sie unter **Microsoft-Kundenvertrag** die Option **Aktualisieren** aus.

4. Geben Sie **Vorname**, **Nachname**, **E-Mail-Adresse** und **Telefonnummer** (optional) der Person ein, die dem Vertrag zugestimmt hat. Geben Sie unter **Datum der Vertragsannahme** das entsprechende Datum ein. Dieses kann nicht auf ein Datum in der Zukunft festgelegt werden.

5. Wählen Sie **Speichern und fortfahren** aus.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestandskunde":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Abrufen der Bestätigung der Kundenzustimmung für einen Bestandskunden

Mithilfe der folgenden Schritte können Sie eine Bestätigung abrufen, dass ein Bestandskunde den Microsoft-Kundenvertrag akzeptiert hat. Beachten Sie, dass Sie dafür ein Administrator-Agent oder Vertriebsbeauftragter sein müssen.

1. Wählen Sie **Kunden** aus, und suchen Sie dann nach dem Kunden, den Sie anzeigen möchten. Wählen Sie diesen aus.

2. Wählen Sie **Kontoinformationen** aus.

3. Unter **Microsoft-Kundenvertrag** wird angezeigt, ob die Bestätigung durch diesen Kunden erfolgt ist.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Bestätigen der Zustimmung des Kunden über die Partner Center-API oder das Partner Center SDK

Du kannst die Partner Center-API oder das Partner Center SDK verwenden, um die Zustimmung des Kunden zur Microsoft-Kundenvereinbarung zu bestätigen. Ausführliche Informationen zur API bzw. zum SDK findest du unter:

- [Abrufen von Vertragsmetadaten für den Microsoft-Kundenvertrag](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Abrufen der Bestätigung der Kundenakzeptanz zur Microsoft-Kundenvereinbarung](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Abrufen eines Downloadlinks für die Vorlage des Microsoft-Kundenvertrags](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Option 2: Zustimmung des Kunden im Microsoft 365 Admin Center

Partner können neue und bestehende Kunden über eine URL einladen, die Vereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen. In den nächsten Abschnitten wird Folgendes erläutert:

- Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

- Einladen eines neuen Kunden, die Handelspartnerbeziehung und -vereinbarung zu überprüfen und diesen zuzustimmen

- Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

>[!NOTE]
> Sie können die [Partner Center-API oder das Partner Center SDK](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) verwenden, um den Status der direkten Zustimmung eines Kunden zur Microsoft-Kundenvereinbarung zu ermitteln.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Erstellen eines neuen Kunden und Einladen des Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

Mit den folgenden Schritten kannst du einen neuen Kunden im Partner Center erstellen und dann einladen, die Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zu überprüfen und ihr zuzustimmen.

1. Wähle im Partner Center auf der Registerkarte **Kunden** die Option **Kunden hinzufügen** aus.

2. Gib unter **Kontoinformationen** in allen Pflichtfeldern die Informationen zum neuen Kunden ein, darunter auch der Firmenname und Hauptkontakt des Kunden.

3. Wähle unter **Kundenvereinbarung** die erste Option aus: **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Der Kunde wird aufgefordert, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen). Fülle alle weiteren Pflichtfelder auf der Seite aus.

4. Wählen Sie **Weiter: Überprüfung** aus und führen Sie dann die Schritte zum Erstellen des Kundenmandanten aus. (Anmerkung: Neue Kunden können erst einen neuen Kauf tätigen, nachdem sie der Microsoft-Kundenvereinbarung zugestimmt haben.)  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Erstellen eines neuen Kunden":::

5. Sobald im Workflow für neue Kunden der Bildschirm **Bestätigung** angezeigt wird, musst du die Anmeldeinformationen des Kunden speichern. Diese Anmeldeinformationen musst du später dem Kunden mitteilen.

6. Erstelle und sende außerhalb von Partner Center eine E-Mail, um den Kunden einzuladen, der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zuzustimmen. Die folgenden Elemente müssen in der E-Mail enthalten sein:

   - Ein Link zu dieser [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Anmeldung erforderlich)

   - Die in Schritt 5 gespeicherten Anmeldeinformationen des Kunden

7. Der Kunde erhält dann die E-Mail-Einladung vom Partner und wählt die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) aus.

8. Der Kunde meldet sich mit den zuvor vom Partner erhaltenen Kundenanmeldeinformationen beim Microsoft 365 Admin Center an.

9. Anschließend aktiviert der Kunde das entsprechende Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Einladen eines neuen Kunden, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen 

Mit den folgenden Schritten kannst du einen neuen Kunden einladen, die Handelspartnerbeziehung und Microsoft-Kundenvereinbarung zu überprüfen und diesen zuzustimmen. 

1. Wähle im Partner Center auf der Registerkarte **Kunden** den Link **Vertriebspartnerschaft beantragen** aus. 

2. Dadurch wird eine automatische E-Mail-Vorlage generiert, die Text und eine parametrisierte URL enthält, durch die der Kunde zum Microsoft 365 Admin Center weitergeleitet wird.

3. Du kannst die automatisch generierte E-Mail-Vorlage anpassen und dann **In Zwischenablage kopieren** oder **In E-Mail öffnen** auswählen.

4. Verwende diese E-Mail-Vorlage, um den Kunden einzuladen, dem Antrag auf eine **Handelspartnerschaft** und der **Microsoft-Kundenvereinbarung** zuzustimmen. (Anmerkung: Achte darauf, dass der Partner in der E-Mail-Einladung auch die automatisch bereitgestellte URL und die kürzlich erstellten Kundenanmeldeinformationen angibt.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Erstellen einer Beziehung":::

5. Der Kunde empfängt die Einladung per E-Mail und klickt auf die parametrisierte URL. 

6. Der Kunde verwendet die vom Partner in der E-Mail bereitgestellten Anmeldeinformationen, um sich beim Microsoft 365 Admin Center anzumelden.

7. Der Kunde aktiviert das Kontrollkästchen, um der **Handelspartnerbeziehung** und **Microsoft-Kundenvereinbarung** zuzustimmen. 

8. Der Kunde kann unter derselben URL eine konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet. Er kann einen Partner auswählen, um Details anzuzeigen.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zustimmen zur Vereinbarung":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Einladen eines bestehenden Kunden, die Vereinbarung zu überprüfen und ihr zuzustimmen

Mit den folgenden Schritten kannst du einen bestehenden Kunden einladen, die Microsoft-Kundenvereinbarung zu überprüfen und ihr zuzustimmen. 

1. Erstelle die Kunden-E-Mail mit der eingebetteten URL, um deinen Kunden einzuladen, der Microsoft-Kundenvereinbarung zuzustimmen.

2. Der Kunde erhält die Einladung per E-Mail und klickt auf die [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Der Kunde gibt seine Anmeldeinformationen in Microsoft 365 Admin Center ein.

4. Der Kunde aktiviert das Kontrollkästchen, um der Microsoft-Kundenvereinbarung zuzustimmen. 

5. Der Kunde kann unter derselben URL die konsolidierte Liste verschiedener Partner anzeigen, mit denen er zusammenarbeitet. Er kann einen Partner auswählen, um Details anzuzeigen.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Kunde":::

>[!NOTE]
>In bestimmten Szenarien können Kunden der Microsoft-Kundenvereinbarung u. U. nicht direkt zustimmen. Weitere Informationen zu diesen Situationen findest du unter [Zwei Szenarien, in denen du die Zustimmung im Namen deines Kunden bestätigen musst](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Verlaufsbezogene Zeitachsendetails

| Datum | Meilenstein | Details |
|------------|------------|--------------------------------|
|1\. August 2019|In Sandbox verfügbare UX-Vorschau|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center-Dashboard in der CSP-Sandboxumgebung bestätigen. Partner, die Zugriff auf die CSP-Sandboxumgebung haben, erhalten eine Vorschau auf die Änderungen bei der Benutzeroberfläche. Partner ohne Sandboxzugriff können sich in diesem Thema über die Änderungen informieren.|
|03. September 2019|In Sandbox verfügbare API-Vorschau|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über die Partner Center-API in der CSP-Sandboxumgebung bestätigen. API-Partner können diese Gelegenheit nutzen, um sich eine Vorschau der API-Änderungen anzusehen und mit der API-Integration zur Unterstützung des neuen Vertrags zu beginnen.|
|20. September 2019|Vorschau des .NET SDK ist in Sandbox verfügbar.|Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center .NET SDK in der CSP-Sandboxumgebung bestätigen. API-Partner können diese Gelegenheit nutzen, um sich eine Vorschau der Änderungen des .NET SDK anzusehen und mit der API-Integration zur Unterstützung des neuen Vertrags zu beginnen.|
|1\. Oktober 2019|Microsoft-Kundenvertrag in der Produktionsumgebung verfügbar|Microsoft stellt den Microsoft-Kundenvertrag für das CSP-Programm vor, der den Microsoft Cloud-Vertrag ersetzt. Partner können die Zustimmung des Kunden zum Microsoft-Kundenvertrag über das Partner Center-Dashboard und die entsprechende API in der Produktionsumgebung bestätigen. Der Microsoft Cloud-Vertrag wird innerhalb des CSP-Partnerprogramms weiterhin unterstützt. Partnern wird jedoch empfohlen, mit der Migration zum Microsoft-Kundenvertrag zu beginnen. Neue Käufe und Änderungen an der Anzahl der Arbeitsplätze für vorhandene Abonnements erfordern eine Bestätigung des Microsoft-Kundenvertrags oder des Microsoft Cloud-Vertrags durch den Partner. Bestimmte neue Angebote (z. B. der neue Azure-Plan) erfordern eine Bestätigung des Microsoft-Kundenvertrags.|
|31. Januar 2020|Microsoft Cloud-Vertrag aus der Produktionsumgebung entfernt|Der Microsoft Cloud-Vertrag wird innerhalb des CSP-Partnerprogramms nicht mehr akzeptiert. Neue Käufe und Änderungen an der Anzahl der Arbeitsplätze für vorhandene Abonnements erfordern eine Bestätigung des Microsoft-Kundenvertrags durch den Partner. Diese Anforderung gilt für neue Kunden und Bestandskunden, die möglicherweise zuvor den Microsoft Cloud-Vertrag angenommen haben.|
|3\. Februar 2020|Der Partner hat jetzt die Möglichkeit, den Kunden über eine URL einzuladen, damit dieser die Vereinbarung im authentifizierten Microsoft 365 Admin Center überprüfen und ihr zustimmen kann. | Der Kunde kann der Microsoft-Kundenvereinbarung im Microsoft 365 Admin Center zustimmen. Wenn der Kunde der Vereinbarung direkt im Microsoft 365 Admin Center zustimmt, erkennt er die Nutzungsbedingungen an. 
