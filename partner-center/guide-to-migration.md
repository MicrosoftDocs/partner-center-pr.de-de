---
title: Leitfaden für die Migration von PMC zu Partner Center | Partner Center
ms.topic: article
ms.date: 04/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Was Sie wissen sollten, wenn Sie Ihr Unternehmen von der PMC zu Partner Center migrieren?
author: LauraBrenner
ms.author: labrenne
keywords: PMC, Migration, Wechsel zu Partner Center
ms.localizationpriority: medium
ms.openlocfilehash: a39c4114758004ff4291bc577182fd8ba469149b
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653098"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Leitfaden für die Migration von PMC zu Partner Center

Die Microsoft-Partner Website unter Partner.Microsoft.com ist ein einheitliches digitales Verfahren für Partner. Auf der Partner-Website können Sie Ihre Verkaufschancen untersuchen und sich mit geführten Erfahrungen befassen, die Ihrem Unternehmen bei der Erstellung und dem Vertrieb Ihrer Apps und Dienste mit Microsoft helfen. Mithilfe des dashboardlinks, der auf der Partner Website verfügbar ist, können Mitglieder des Microsoft Partner Network sich beim Partner Center anmelden, in dem Sie Ihre Beziehung mit Microsoft verwalten, Programme registrieren und sich für Angebote registrieren. 

Das Partner Membership Center (PMC) wird außer Betrieb gesetzt. Ihr Unternehmen wurde eingeladen, Ihre Microsoft Partner Network Mitgliedschafts Verwaltung auf Partner Center umstellen. In dieser Anleitung werden Sie darauf vorbereitet, was zu erwarten ist, wenn Sie den Wechsel von der PMC zu Partner Center durchführen.

>[!Note]
>Auch wenn Ihr Unternehmen über mehr als ein Konto oder einen Standort verfügt, beginnt der Umstieg auf Partner Center mit dem Verschieben eines (Ihrem ersten) Konto in Partner Center.

## <a name="get-started"></a>„Erste Schritte“

Der Verschiebe Vorgang beginnt in der PMC. Ihr globaler Administrator erhält eine Einladung, um mit dem Verschieben zu beginnen. 

**Vorbereiten in der PMC**
- Überprüfen der Unternehmens Details 
- Kontakt zum primären Programm überprüfen 
- Überprüfen von Geschäftsstandorten
- Aktualisieren genehmigter Benutzer

**Wenn Sie bereit sind**

Wählen Sie in Ihrer Einladung **den Einstieg in** Ihre Einladung aus. Sie gelangen zur Partner Center-Anmeldeseite.

![„Erste Schritte“](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>Mit Ihrer Geschäfts-e-Mail starten

Wenn Ihr Unternehmen nicht über eine geschäftliche e-Mail-Adresse und einen Aad-Mandanten verfügt, können wir Sie beim Einrichten eines Partner Center-Anmelde Prozesses unterstützen. Wenn Sie versuchen, sich mit einem e-Mail-Konto anzumelden, bei dem es sich nicht um eine geschäftliche e-Mail-Adresse (z. b. Ihr persönliches Konto) handelt, werden Sie angewiesen, Informationen zu Ihrem Unternehmen bereitzustellen, damit wir einen Aad-Mandanten und eine
Diese Unternehmens Details werden verwendet, um Ihr Konto im Partner Center abzuschließen. Achten Sie daher darauf, dass Sie korrekt sind.

>[!Note]
>Wenn Sie ein Partner in China sind und sowohl im Microsoft Partner Network als auch im Cloud Solution Provider-Programm (CSP) registriert sind, verfügen Sie über einen separaten Mandanten für jedes Konto. Ihr Konto mit dem Cloud Solution Provider-Programm wird in der nationalen Cloud verwaltet, und Ihr Microsoft Partner Network Konto wird in der globalen Cloud verwaltet. Die beiden Konten können nicht verknüpft werden.

![Erzählen Sie uns von Ihrem Unternehmen.](images/migration/newtellusabout.png)

Nachdem Sie die Informationen überprüft oder aktualisiert haben, wählen Sie **annehmen und Fortfahren**aus.
Die Bestimmungen auf dieser Seite sind **exakt identisch** mit der Vereinbarung, die Ihr Unternehmen bereits in der PMC angemeldet hat.  
Dadurch wird die Erstellung Ihres Azure AD Mandanten initiiert, und ihr wird mit dem Geschäftskonto bereitstellen.

Wenn Sie **akzeptieren und Fortfahren** auswählen, werden auch folgende Schritte ausgeführt:

• Migriert Ihr Konto zusammen mit allen zugehörigen Standorten zu Partner Center.

• Migriert alle Kompetenzen oder Zuordnungen, die Sie möglicherweise in der PMC erworben haben.

• Migriert alle Vorteile (Maps, Silver, Gold), die in der PMC vorhanden waren.

## <a name="invite-employees-to-join-you"></a>Einladen von Mitarbeitern, ihnen beizutreten

Wenn Sie Ihren neuen Azure AD Mandanten erstellt haben, können Sie Ihre Mitarbeiter bitten, sich bei Partner Center anzumelden.

![Mitarbeiter einladen](images/migration/invite.png)


Wenn Sie sich mit einem vorhandenen Aad-Mandanten angemeldet haben, sind Ihre Mitarbeiter mit Ihnen in der Hand. Weisen Sie in diesem Fall Ihre Mitarbeiter Rollen zu, die bestimmen, welche Möglichkeiten Sie in Partner Center haben. Hinweis: Rollen im Partner Center unterscheiden sich von den Rollen in der PMC. Weitere Informationen finden [Sie unter Wechsel von der PMC zu Partner Center](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Überprüfen der Domäne und als globaler Administrator  

Wenn Ihr Aad-Mandant neu ist, wird keinem der Rolle globaler Administrator zugewiesen. Um zum globalen Administrator zu werden, müssen Sie den Domänen Besitz überprüfen. Möglicherweise benötigen Sie den Domänen Administrator, um dies zu unterstützen. Beachten Sie, dass Sie, während Sie die bereits erworbenen Angebote verwenden können, erst dann neue Angebote erwerben können, wenn Sie einen globalen Administrator erhalten. 

![Kontrolle übernehmen](images/migration/takecontrol.png)

Wenn Sie auf "starten" klicken, wird der folgende Bildschirm angezeigt:

![Domänen Besitz überprüfen](images/migration/verifytxt.png)

Ihre Domänen Registrierungsstelle wird bereits für Sie ausgefüllt. Nur der Domänen Besitzer kann die DNS-Datei aktualisieren. Wenn Sie also die Textdatei kopieren und in Ihren DNS-Datensatz einfügen, können wir überprüfen, ob Sie der Besitzer sind. Es dauert einige Minuten, bis das Update ausgeführt wird. Sie müssen sich von Partner Center abmelden und dann wieder anmelden. Ihre Rolle wird in globaler Administrator geändert. 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Machen Sie sich mit Ihrem Dashboard und Partner Center vertraut.

Sehen Sie sich das Dashboard an. Hier können Sie Ihre Mitgliedschaft verwalten, ein Geschäftsprofil für Verweise hinzufügen, sich für das Cloud Solution Provider-Programm registrieren und die für Ihr Unternehmen relevanten Benachrichtigungen und Angebote jederzeit durch Auswahl von **Dashboard**anzeigen. Sie können auch die Anreize verwalten, auf dem Marketplace erwerben, sich für Markt Einführungs Dienste registrieren und vieles mehr.  

![Tour durchführen](images/migration/fre.png)

## <a name="next-steps"></a>Nächste Schritte

- [Erstellen von Benutzerkonten ](create-user-accounts-and-set-permissions.md)
- [Zuweisen von Benutzerrollen und Berechtigungen](permissions-overview.md)
- [Verwalten der Microsoft Partner Network-Mitgliedschaftsprogramme](renew-mpn-offers.md)
- [Erstellen Ihres Unternehmensprofils](create-a-marketing-profile.md)
- [Kontaktaufnahme mit Kunden durch Empfehlungen](responding-to-referrals.md)

## <a name="see-also"></a>Weitere Informationen:

- [Leitfaden zum Migrieren mehrerer Unternehmen von der PMC zu Partner Center](move-multiple-companies.md)
