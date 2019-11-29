---
title: Leitfaden zum Migrieren von PMC zu Partner Center | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Ihr Unternehmen vom Partner Membership Center (PMC) zu Partner Center migrieren.
author: LauraBrenner
ms.author: labrenne
keywords: PMC, Migration, Wechsel zu Partner Center
ms.localizationpriority: high
ms.openlocfilehash: f9ce53adddd2faecf22ef795e8ffe97189c57353
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252210"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Leitfaden zum Migrieren von PMC zu Partner Center

Die Microsoft-Partner-Website unter „partner.microsoft.com“ ist ein einheitliches digitales Verfahren für Partner. Über die Partner-Website können Sie Ihre Verkaufschancen untersuchen und sich mit Anleitungen befassen, die Ihrem Unternehmen bei der Erstellung und dem Vertrieb Ihrer Apps und Dienste mit Microsoft helfen. Über den Dashboard-Link, der auf der Partner-Website zur Verfügung steht, können sich Mitglieder des Microsoft Partner Networks bei dem Partner Center anmelden, in dem Sie Ihre Beziehung mit Microsoft verwalten sowie sich für Programme und Angebote registrieren. 

Das Partner Membership Center (PMC) wird außer Betrieb gesetzt. Ihr Unternehmen wurde eingeladen, Ihre Microsoft Partner Network-Mitgliedschaftsverwaltung auf Partner Center umzustellen. In dieser Anleitung werden Sie darauf vorbereitet, was zu erwarten ist, wenn Sie den Wechsel von PMC zu Partner Center durchführen.

>[!Note]
>Auch wenn Ihr Unternehmen mehrere Konten oder Standorte hat, beginnt der Wechsel zu Partner Center mit dem Verschieben eines (Ihres ersten) Kontos in Partner Center.

## <a name="get-started"></a>Beginnen

Der Verschiebevorgang beginnt in PMC. Ihr globaler Administrator erhält eine Einladung, mit dem Verschieben zu beginnen. 

**Vorbereiten in PMC**
- Überprüfen Ihrer Unternehmensdetails 
- Überprüfen Ihres primären Programmkontakts 
- Überprüfen Ihrer Unternehmensstandorte
- Aktualisieren Ihrer genehmigten Benutzer

**Wenn Sie bereit sind**

Wählen Sie in Ihrer Einladung **Erste Schritte** aus. Daraufhin wird die Anmeldeseite von Partner Center angezeigt.

![Beginnen](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>Beginnen mit Ihrer geschäftlichen E-Mail-Adresse

Wenn Ihr Unternehmen keine geschäftliche E-Mail-Adresse und keinen AAD-Mandanten hat, können wir Ihnen während des Partner Center-Anmeldevorgangs helfen, eine/einen einzurichten. Wenn Sie versuchen, sich mit einem E-Mail-Konto anzumelden, das keine geschäftliche E-Mail-Adresse ist (z.B. Ihr persönliches Konto), werden Sie aufgefordert, Informationen zu Ihrem Unternehmen anzugeben, damit wir einen AAD-Mandanten und eine geschäftliche E-Mail-Adresse einrichten können.
Weil diese Unternehmensdetails zum Fertigstellen Ihres Kontos in Partner Center verwendet werden, sorgen Sie dafür, dass sie korrekt sind.

>[!Note]
>Wenn Sie ein Partner in China sind und sowohl im Microsoft Partner Network als auch im Cloud Solution Provider-Programm (CSP) registriert sind, haben Sie einen separaten Mandanten für jedes Konto. Ihr Konto mit dem Cloud Solution Provider-Programm wird in der nationalen Cloud verwaltet und Ihr Microsoft Partner Network-Konto in der globalen Cloud. Die beiden Konten können nicht verknüpft werden.

![Informieren Sie uns über Ihr Unternehmen](images/migration/newtellusabout.png)

Nachdem Sie die Informationen überprüft oder aktualisiert haben, wählen Sie **Zustimmen und fortfahren** aus.
Die „Bestimmungen“ auf dieser Seite sind **identisch mit denjenigen** in der Vereinbarung, die Ihr Unternehmen bereits in PMC unterzeichnet hat.  
Dadurch wird die Erstellung Ihres Azure AD-Mandanten eingeleitet und Ihnen Ihr Geschäftskonto bereitgestellt.

Wenn Sie **Zustimmen und fortfahren** auswählen, werden auch folgende Schritte ausgeführt:

•   Ihr Konto wird zusammen mit ALLEN zugehörigen Standorten zu Partner Center migriert.

•   Kompetenzen oder MAPs, die Sie möglicherweise in PMC erworben haben, werden migriert.

•   Vorteile (MAPs, Silver, Gold), die Sie in PMC hatten, werden migriert.

## <a name="invite-employees-to-join-you"></a>Einladen von Mitarbeitern, Ihnen beizutreten

Nachdem Ihr neuer Azure AD-Mandant erstellt wurde, können Sie Ihre Mitarbeiter einladen, sich bei Partner Center anzumelden.

![Einladen von Mitarbeitern](images/migration/invite.png)


Falls Sie sich bei einem vorhandenen AAD-Mandanten angemeldet haben, wurden Ihre Mitarbeiter zusammen mit Ihnen verschoben. Weisen Sie in diesem Fall Ihren Mitarbeitern Rollen zu, die festlegen, welche Berechtigungen sie in Partner Center haben. Hinweis: Rollen in Partner Center unterscheiden sich von Rollen in PMC. Weitere Informationen finden Sie unter [Wechsel von PMC zu Partner Center](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Überprüfen Ihrer Domäne und ein globaler Administrator werden  

Sollte Ihr AAD-Mandant neu sein, wurde niemandem die Rolle „globaler Administrator“ zugewiesen. Wenn Sie der globale Administrator werden möchten, müssen Sie Ihren Domänenbesitz überprüfen. Möglicherweise müssen Sie dazu den Domänenadministrator um Hilfe bitten. Beachten Sie: Während Sie bereits erworbene Angebote sofort nutzen können, können Sie neue Angebote erst dann erwerben, nachdem Sie den Schritt „ein globaler Administrator werden“ abgeschlossen haben. 

![Übernehmen der Kontrolle](images/migration/takecontrol.png)

Wenn Sie „Erste Schritte“ auswählen, wird folgender Bildschirm angezeigt:

![Domänenbesitz überprüfen](images/migration/verifytxt.png)

Ihre Domänenregistrierungsstelle wurde bereits automatisch ausgefüllt. Nur der Domänenbesitzer kann die DNS-Datei aktualisieren. Wenn Sie also die Textdatei kopieren und Ihrem DNS-Datensatz hinzufügen, können wir überprüfen, ob Sie der Besitzer sind. Es dauert ein paar Minuten, bis das Update erfolgt. Sie müssen sich bei Partner Center abmelden und dann wieder anmelden. Jetzt lautet Ihre Rolle „globaler Administrator“. 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Vertrautmachen mit Ihrem Dashboard und Partner Center

Sehen Sie sich die Einführung zum Dashboard an. Hier können Sie Ihre Mitgliedschaft verwalten, ein Geschäftsprofil für Empfehlungen hinzufügen, sich beim Cloud Solution Provider-Programm registrieren sowie für Ihr Unternehmen relevante Benachrichtigungen und Angebote jederzeit anzeigen, indem Sie **Dashboard**auswählen. Sie können auch Incentives verwalten, auf dem Marketplace kaufen, sich für Markteinführungsdienste registrieren und vieles mehr ausführen.  

![Tour](images/migration/fre.png)

## <a name="next-steps"></a>Nächste Schritte

- [Erstellen von Benutzerkonten ](create-user-accounts-and-set-permissions.md)
- [Zuweisen von Benutzerrollen und Berechtigungen](permissions-overview.md)
- [Verwalten der Microsoft Partner Network-Mitgliedschaftsprogramme](renew-mpn-offers.md)
- [Erstellen Ihres Unternehmensprofils](create-a-marketing-profile.md)
- [Kontaktaufnahme mit Kunden durch Empfehlungen](responding-to-referrals.md)

## <a name="see-also"></a>Weitere Informationen

- [Leitfaden zum Migrieren mehrerer Unternehmen von PMC zu Partner Center](move-multiple-companies.md)
