---
title: Verwalten der Lizenzierung in Marketplace-Angeboten
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die Lizenzierung für Ihre IsV-Angebote im kommerziellen Marketplace einrichten und verwalten.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147954"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Verwalten der Lizenzierung in Marketplace-Angeboten

**Geeignete Rollen:** globale | Kontoadministrator

In diesem Artikel erfahren Sie, wie Sie ein Angebot in Partner Center einrichten, es in Microsoft AppSource zur Verfügung stellen und dann Lizenzen für dieses Angebot verwalten.  

>[!IMPORTANT]
>Die Funktionen in diesem Artikel befinden sich derzeit in Public Preview.

## <a name="before-you-begin"></a>Voraussetzungen

### <a name="commercial-marketplace-basics"></a>Grundlagen des kommerziellen Marketplace

Bevor Sie mit diesem Prozess beginnen, sollten Sie sich mit den Grundlagen des kommerziellen Marketplace vertraut machen. Die Artikel in der folgenden Tabelle helfen Ihnen beim Einstieg. 

| Thema  | Artikel  |
|-------|--------|
|Pläne für den kommerziellen Marketplace | [Pläne und Preise für Angebote im kommerziellen Marketplace](/azure/marketplace/plans-pricing)    |
|Angebote im kommerziellen Marketplace  | [Auflisten von Typen](/azure/marketplace/determine-your-listing-type)    |
|Konten im kommerziellen Marketplace |  [Erstellen eines Kontos im kommerziellen Marketplace in Partner Center](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Ermitteln Ihrer Angebots-ID

In den folgenden Verfahren werden Sie aufgefordert, eine Angebots-ID einzugeben. Nehmen Sie sich einige Zeit, um eine geeignete Angebots-ID zu haben, und beachten Sie dabei die folgenden Punkte:

- Diese ID wird für Kunden unter der Webadresse für das Marketplace-Angebot und ggf. in Azure Resource Manager-Vorlagen angezeigt.
- Die Angebots-ID darf zusammen mit der Herausgeber-ID nicht länger als 40 Zeichen lang sein.
- Verwenden Sie nur Kleinbuchstaben und Zahlen. Die Angebots-ID kann Bindestriche und Unterstriche, aber keine Leerzeichen enthalten. Wenn Ihre Herausgeber-ID beispielsweise lautet `testpublisherid` und Sie `test-offer-1` eingeben, lautet die Webadresse des Angebots `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Diese ID kann nach dem Auswählen von **Erstellen** nicht mehr geändert werden.

### <a name="determine-your-offer-alias"></a>Ermitteln Ihres Angebotsalias

Der Angebotsalias ist der Name, der für das Angebot in Partner Center verwendet wird. Außerdem benötigen Sie einen geeigneten Angebotsalias, der den folgenden Richtlinien entspricht:

- Dieser Name wird im Marketplace nicht verwendet und unterscheidet sich vom Angebotsnamen und anderen Werten, die den Kunden angezeigt werden.
- Dieser Name kann nach der Auswahl von Erstellen nicht mehr geändert werden.

## <a name="create-your-offer"></a>Erstellen Ihres Angebots

Der erste Schritt im Lizenzierungsprozess besteht darin, Ihr Angebot für den kommerziellen Marketplace zu erstellen. 

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.
2. Wählen Sie im linken Navigationsmenü **kommerzieller Marketplace/Übersicht aus.**
3. Wählen Sie oben auf der Seite Übersicht **die** Option Neues Angebot und dann **Dynamics 365 for Customer Engagement & PowerApps aus.**
4. Geben Sie die **Angebots-ID und** **den Angebotsalias ein,** die Sie zuvor erstellt haben.
5. Wählen Sie **Erstellen** aus, um das Angebot zu generieren und fortzufahren.
6. Wählen Sie Ihre Lizenzierungsoptionen aus.

    - Um die Lizenzverwaltung für Ihr Angebot zu aktivieren, wählen **Sie App-Lizenzverwaltung über Microsoft aktivieren aus.** Dies ist eine einmalige Einstellung, die Sie nach der Veröffentlichung Ihres Angebots nicht mehr ändern können.

    - Sie können kunden auch ermöglichen, die Basisfunktionen Ihrer App ohne Lizenz und Premium-Features nach dem Kauf einer Lizenz ausführen zu können. Wählen Sie hierzu Allow customers to install my app even if licenses are not assigned (Kunden erlauben, meine App zu **installieren, auch wenn lizenzen nicht zugewiesen sind) aus.**

    - Wenn Sie nicht möchten, dass die Lizenzverwaltung für Ihr Angebot aktiviert ist, wählen Sie Jetzt erwerben **(Kostenlos)** **,** Kostenlose Testversion oder Kontakt mit **mir auf.**

## <a name="create-your-plan"></a>Erstellen Ihres Plans

In diesen Schritten definieren Sie den Plan oder die Pläne, die Sie für Ihr Angebot aktivieren möchten.

1. Wählen Sie im linken Navigationsmenü **plan overview (Planübersicht)** und dann **Create new plan (Neuen Plan erstellen) aus.**
2. Geben Sie eine **Plan-ID und** **einen Plannamen ein,** und wählen Sie dann **Erstellen aus.**
3. Geben Sie auf **der Seite Planlistung** Ihre **Planbeschreibung ein.**
4. Wählen Sie Entwurf speichern aus, um die Beschreibung zu speichern **und später fertig zu stellen.**

5. Wenn Sie fertig sind, wählen Sie **Überprüfen und veröffentlichen aus.** Die Planinformationen werden nun auf der Seite appsource.microsoft.com Angebotsliste (Abschnitt "Pläne") angezeigt.

6. Nachdem Sie alle Pläne für dieses Angebot erstellt haben, müssen Sie die Dienst-ID jedes Plans kopieren. Wählen **Sie oben auf** der Seite Planlistung die Option Planübersicht aus. Kopieren Sie die Dienst-ID für jeden Plan an einen sicheren Ort.

## <a name="add-service-ids-to-your-solution"></a>Hinzufügen von Dienst-IDs zu Ihrer Lösung

Im nächsten Schritt aktualisieren Sie Ihre Lösung, indem Sie die Dienst-IDs für jeden soeben kopierten Plan hinzufügen. Eine Anleitung hierzu finden Sie unter [Erstellen eines AppSource-Pakets für Ihre Projektmappe.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Hochladen Ihres Pakets und Veröffentlichen Ihres Angebots

1. Wählen Sie im linken Navigationsbereich **kommerzieller Marketplace** und dann **Technische Konfiguration** aus.
2. Wählen Sie unter **Basislizenzmodell** die Option **Benutzer** aus.
3. Geben Sie unter **CRM-Paket** die URL Ihres Paketspeicherorts ein.
4. Verwenden Sie die anderen Registerkarten im linken Navigationsbereich, um weitere erforderliche Informationen einzugeben. Wenn Sie fertig sind, wählen Sie **Überprüfen und veröffentlichen** aus.

Nachdem Sie das Angebot veröffentlicht haben, überprüfen wir Ihre Informationen. Wenn bei diesem Prozess Probleme auftreten, benachrichtigen wir Sie. Wenn alle Probleme behoben wurden, erhalten Sie eine Benachrichtigung, dass Ihr Angebot in AppSource verfügbar ist. An diesem Punkt können Sie es live machen.

## <a name="make-your-offer-live-in-partner-center"></a>Ihr Angebot in Partner Center live zu machen

Das folgende Verfahren führt Sie durch den Prozess, ihr Angebot in AppSource live zu machen. Weitere Informationen zu diesem Prozess finden Sie unter [Einführung in das Auflisten von Optionen.](/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Nachdem Sie Ihr Angebot veröffentlicht haben, dauert es 4 bis 6 Stunden, bis es live zugehen kann.

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.
2. Wählen Sie im linken Navigationsmenü **kommerzieller Marketplace/Übersicht** aus.
3. Suchen Sie auf der Seite **Übersicht** nach dem gewünschten Angebot. Angebote, die veröffentlicht werden können, haben den Status **Vorschau**. Wählen Sie das Angebot.
4. Wählen Sie auf der Seite **Angebotsübersicht** die Option **Liveschalten** aus.
Das Angebot wird in 4 bis 6 Stunden live lebbar sein.
5. Wählen Sie unten auf der Seite Angebotsübersicht den Link AppSource aus, um Ihre Angebotsliste in **AppSource** **anzuzeigen.**

    - **Für lizenzfähige Angebote:** Wenn Ihr Angebot eine Lizenzprüfung erfordert, können Benutzer nur durch Klicken auf Kontakt mit **mir** aufnehmen einen Lead eingeben, damit Sie mit ihnen kommunizieren können.

    - **Für lizenzaktivierte Angebote mit kostenloser Installationsoption:** Wenn für Ihr Angebot keine Lizenzprüfung erforderlich ist, wird Administratorbenutzern zusätzlich zu **Kontakt mit mir** die Schaltfläche **Jetzt** anfordern angezeigt. Benutzer, die Ihre kostenlose Installationsoption ausprobieren möchten, sollten auf **Jetzt abrufen** klicken, um das Angebot in Power Platform Admin Center zu installieren. Benutzer können weiterhin **Kontakt mit mir aufnehmen,** wenn sie Fragen haben oder ein Upgrade auf einen kostenpflichtigen Plan durchführen möchten.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registrieren des ISV Connect-Abschlusses bei der Dealregistrierung

Bevor Sie einem Kunden Lizenzen zuweisen können, muss jeder Verkauf in Partner Center registriert werden. Informationen hierzu finden Sie unter [Registrieren Ihrer Angebote.](register-deals.md)

## <a name="invite-the-customer"></a>Einladen des Kunden

Gehen Sie wie folgt vor, um den Kunden zur Teilnahme an diesem Deal einzuladen.  

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.
2. Wählen Sie im linken Navigationsmenü **kommerzieller Marketplace/Übersicht** aus.
3. Wählen Sie im linken **Navigationsmenü Empfehlungen** und dann **Deal Registration (Dealregistrierung)** aus.
4. Filtern Sie nach **Übermittelte** Angebote, wählen Sie die Registerkarte **In Bearbeitung** aus, und wählen Sie dann das gewünschte Angebot aus.
5. Wählen Sie auf der Übersichtsseite für diesen Deal die Option **Lizenzen verwalten** aus.
6. Wählen **Sie** im Fenster Lizenzen verwalten in der Dropdownliste **Kundendetails** den Kunden aus. Wenn die Kundenbeziehung noch nicht vorhanden ist, wählen Sie **+ Neuen Kunden einladen aus, um zuzustimmen.**
7. Kopieren Sie den angezeigten Link.
8. Senden Sie diesen Link per E-Mail an den Abrechnungsadministrator oder globalen Administrator Ihres Kunden, und lassen Sie diesen Link verwenden, um auf admin.microsoft.com zuzugreifen und die von Ihnen einzurichtende Beziehung zu akzeptieren und zu autorisieren.

    >[!NOTE]
    >Die Beziehung wird erst hergestellt, wenn der Kunde diesen Schritt ausführt.

## <a name="activate-manage-and-remove-your-licenses"></a>Aktivieren, Verwalten und Entfernen Ihrer Lizenzen

Nachdem Ihr Kunde die Beziehung mit Ihnen autorisiert hat, können Sie mit dem Hinzufügen von Plänen aus Ihrem Angebot und dem Zuweisen von Lizenzen zu jedem Plan beginnen.

1. Wählen Sie im Fenster Lizenzen für diesen Deal verwalten **die Option + Plan hinzufügen aus.**
2. Füllen Sie **die Felder Pläne für diese Lösung und** Anzahl von Lizenzen **aus,** und wählen Sie dann **Lizenzen aktualisieren aus.** Die Lizenzen sind auf der admin.microsoft.com verfügbar, die Kunden verwalten und Mitarbeitern zuweisen können.

    - Um die Anzahl der Lizenzen für einen vorhandenen Plan zu ändern, geben Sie die neue Nummer in das Feld **Anzahl der** Lizenzen ein, und wählen Sie dann Lizenzen **aktualisieren aus.**

    - Um Lizenzen für einen Deal zu deaktivieren oder zu entfernen, wählen Sie im Feld **Aktionen** das Papierkorbsymbol und dann **Lizenzen aktualisieren aus.**

## <a name="next-steps"></a>Nächste Schritte

[Ressourcen zu „Lizenzierung“](support-resources-licensing.md)