---
title: Vorbereiten der Umstellung vom Partner Mitgliedschafts Center auf Partner Center | Partner Center
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dinge, die Sie berücksichtigen sollten, bevor Sie Ihr Geschäft von der PMC zu Partner Center verlagern
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8ad7b761c69cfa1f320eb9427806f5b1803e84e6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652188"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Vorbereiten des Verschiebens von Partner Membership Center (PMC) zu Partner Center

Wir verschieben die Mitgliedschafts Verwaltung aus dem Partner Membership Center (PMC) in das Partner Center-das einzige Ziel, um Ihre geschäftliche Beziehung mit Microsoft zu verwalten. Wir möchten, dass Ihre Umstellung auf Partner Center so effizient und einfach wie möglich ist. Wir haben einige Bereiche identifiziert, in denen sich das Partner Center von der PMC unterscheidet, und wir sind der Ansicht, dass Sie diese vor dem Verschieben verstehen und vorbereiten möchten.

## <a name="account-and-identity-setup"></a>Einrichtung von Konten und Identitäten

**Was ist ein Azure Active Directory (Azure AD)-Geschäftskonto?**

Ein Azure-Geschäftskonto ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud. Das Konto wird für Sie erstellt, wenn Sie einen Microsoft Cloud Service wie Azure, Microsoft Intune oder Office 365 abonnieren.

Ihr Geschäftskonto hostet ihre Azure AD Benutzer und die dazugehörigen Informationen: Ihre e-Mail-Adresse, Kenn Wörter, Profildaten, Berechtigungen usw. Das Geschäftskonto enthält außerdem Gruppen, Anwendungen und andere Informationen zu einem Unternehmen und seiner Sicherheit. Weitere Informationen finden Sie unter...

Im Partner Center verwenden Sie Ihre geschäftliche e-Mail-Adresse, um sich bei Ihrem Konto nicht bei Ihrer persönlichen e-Mail anzumelden.
- Ihr Geschäftskonto: john@contoso.com
- Ihr persönliches Konto: John@outlook.com

Ihre geschäftliche e-Mail-Adresse ist Teil Ihres Azure Active Directory-Mandanten. Wenn Sie über ein Konto im Partner Center verfügen möchten, benötigen Sie einen Aad-Mandanten. Weitere Informationen zu Azure Active Directory finden Sie unter [Erstellen Ihres Verzeichnisses in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Wenn Sie von PMC zu Partner Center wechseln, mit welchem Konto sollten Sie sich bei Partner Center anmelden, wenn Sie über einen Aad-Mandanten mit Microsoft verfügen (z. b. für Office 365) und auch über einen Mandanten für Ihr CSP-Geschäft verfügen?**

Sie können sich mit dem CSP-Konto oder Ihrem MPN Work-e-Mail-Konto bei Partner Center anmelden. Wenn Sie sich für die Anmeldung mit ihrer CSP-Work-e-Mail entscheiden, werden im linken Navigationsbereich auf Ihrem Dashboard sowohl MPN-als auch CSP-Programminformationen angezeigt. Wenn Sie sich mit ihrer MPN-Azure AD-e-Mail-Adresse des Mandanten anmelden, werden nur Ihre MPN-Programminformationen angezeigt. Benutzer Rollen unterscheiden sich zwischen MPN und CSP. Wenn Sie also dasselbe Konto für MPN und CSP Business verwenden, stellen Sie sicher, dass Sie Benutzer Rollen entsprechend zuweisen. Weitere Informationen zu Benutzer Rollen finden Sie unter [Zuweisen von Benutzer Rollen und Berechtigungen](permissions-overview.md).

**Wenn Sie Ihren vorhandenen Office 365 Azure AD-Mandanten nicht für Partner Center verwenden möchten, können Sie vor der Migration von PMC einen neuen Mandanten erstellen.**

Möglicherweise gibt es viele Gründe, warum Sie keinen vorhandenen Azure AD Mandanten verwenden möchten, um Ihr Partner Center-Konto einzurichten. Bevor Sie mit der Migration zu Partner Center beginnen, besuchen Sie den [Azure-Portal](https://ms.portal.azure.com/#home) , um einen neuen Azure AD Mandanten zu erstellen. Befolgen Sie die Anweisungen unter [Erstellen eines neuen Mandanten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Nachdem Sie den neuen Mandanten erstellt haben, verwenden Sie diesen Aad-Mandanten zum Einrichten Ihres Partner Center-Kontos, wenn Sie von der PMC zu Partner Center wechseln. Sie müssen ein globaler Administrator sein, um den Mandanten zu erstellen. Verwenden Sie dieses neue Verzeichnis, um zu Partner Center zu migrieren.


**Worin besteht der Unterschied zwischen der globalen Aad-Administrator Rolle und der globalen PMC-MPN-Administrator Rolle?**

Dabei handelt es sich um zwei ganz andere Rollen mit unterschiedlichen Berechtigungen. Der globale Administrator des Aad-Mandanten in Partner Center verwaltet den Mandanten: Fügt Benutzer hinzu oder entfernt Benutzer, stellt Kenn Wörter, Rollen und Berechtigungen bereit und verwaltet Sie in Partner Center. 

Die globale MPN-Administrator Rolle in der PMC könnte folgende Aktionen ausführen:

- Alle Daten anzeigen und bearbeiten, die dem Unternehmen und allen Standorten des Unternehmens zugeordnet sind

-  Fügen Sie Administratoren auf globaler oder lokaler Ebene hinzu.  Globale Administratoren können auch beliebige Personen an jedem Ort des globalen Administrator Zugriffs zuweisen, der Ihnen unabhängig von dem Standort, dem Sie zugeordnet sind, globalen Zugriff gewährt.
-  Führen Sie eine beliebige Partner Benutzeroberfläche aus, einschließlich: 

-  Benutzer hinzufügen/entfernen

 - Rollen zuweisen/entfernen 

 - Speicherorte hinzufügen/entfernen/aktualisieren 

 - Erwerben von Kompetenzen/Zuordnungen 

-  Vorteile anzeigen

Wenn der globale MPN-Administrator zu Partner Center wechselt, wird die Rolle als MPN-Partner Administrator bezeichnet, der über andere Berechtigungen und Aufgaben als der globale Administrator von Partner Center verfügt. Weitere Informationen zu Rollen und Berechtigungen im Partner Center finden Sie unter [Zuweisen von Benutzern zu Rollen und Berechtigungen](permissions-overview.md).

**Benutzer Rollen einschließlich Gastbenutzer Rollen im Partner Center**

Partner Center verfügt über verschiedene Arten von Rollen, abhängig von den Arbeitsaufgaben, die erforderlich sind. Rollen wie globaler Administrator sind Azure AD Rollen. Einige der Rollen sind spezifisch für Programme, wie z. b. das clouddienstanbieter-Programm oder die-Anreize, und es gibt Rollen, die für MPN spezifisch sind. Informationen dazu, was alle Partner Center-Rollen sind, finden Sie unter [Zuweisen von Benutzern Rollen und Berechtigungen](permissions-overview.md).



**Was geschieht mit den Rollen meiner Benutzer, wenn Sie von der PMC zu Partner Center wechseln?**

Mit Ausnahme des globalen MPN-Administrators oder primären Programm Kontakts, der die Migration durchführt, verlieren alle Benutzer in der PMC Ihre Administrator Rollen. Die Person, die die Migration abschließt, muss im Partner Center Rollen zuweisen. Die Rollen im Partner Center unterscheiden sich von denen in der PMC. Weitere Informationen zu Benutzer Rollen in Partner Center finden Sie unter [Zuweisen von Benutzern Rollen und Berechtigungen] (Berechtigungen-Overview.MD und [Wechseln von der PMC zu Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) .


**Worin besteht der Unterschied zwischen meinem Unternehmensprofil und meinem Geschäftsprofil?**

Ihr Unternehmensprofil ist die Informationen zu Ihrem Unternehmen, das Adresse, Standorte, primäre Kontakt-, Bank-und Steuer Details umfasst.

Ihr Geschäftsprofil ist die Art und Weise, wie Sie Ihren Kunden präsentieren, und ist eine Marketing Seite, auf der Ihr Logo, Details zu ihrem geschäftlichen Fokus, ihr Fachwissen usw. angezeigt wird.

**Was bedeutet Konto Konsolidierung für mein Konto?**

Wenn Sie denselben Azure AD Mandanten verwenden, um mehrere MPN-Konten in Partner Center zu migrieren, erkennt das System diese automatisch, und Sie werden aufgefordert, ihre Konten zu konsolidieren. Dies gilt auch, wenn Sie über mehrere Domänen verfügen, die demselben Azure AD Mandanten zugeordnet sind. 

Sie können weiterhin über separate Aad-Mandanten zu Partner Center migrieren, aber beachten Sie, dass dies zu einer isolierten Auswertung ihrer Kompetenzen und zusätzlicher Kaufkosten führt. 

**Wenn ich mehrere Aad-Mandanten und ein einzelnes MPN-Konto habe, ist es möglich, Sie in Partner Center zu verknüpfen?**

Ja, im Partner Center können Sie mehrere Azure AD Mandanten mit einem Partner Center-Konto verknüpfen.
Weitere Informationen finden Sie hier. 

**Gibt es Einschränkungen beim Hinzufügen mehrerer Azure AD Mandanten zu einem einzelnen Partner Center-Konto?**

Wenn der Azure AD Mandant bereits einem vorhandenen Partner Center-Konto zugeordnet ist, kann er mithilfe des Multi-Mandanten Features nicht mit neuen Partner Center-Konten verknüpft werden. Eine andere Möglichkeit, dies zu übernehmen, besteht darin, dass ein Azure AD Mandant nur einem Partner Center-Konto zugeordnet werden kann, aber einem Partner Center-Konto können mehrere Mandanten zugeordnet sein.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migration der Microsoft Partner Network Mitgliedschaft (MPN) 

**Wer kann den Wechsel von der PMC zu Partner Center durchführen?**

Der globale Administrator des Unternehmens MPN oder der primäre Programm Kontakt (diese beiden Rollen werden oft von derselben Person gehalten) kann die Verschiebung initiieren und durchführen.

**Wird die Person, die die Migration durchführt, zum primären Kontakt zum Unternehmens rechtlichen Profil in Partner Center.**

Der primäre Kontakt muss jedoch nicht unbedingt eine Person sein, die über die Autorisierung zum Signieren von Vereinbarungen verfügt.

**Kann Microsoft meine MPN-Mitgliedschaft für mich migrieren?**

Nein. Microsoft kann Ihnen nicht dabei helfen, Ihr Mitgliedschafts Konto in Partner Center zu verschieben. Sie müssen Ihr Konto verschieben, indem Sie sich mit Ihrem Geschäftskonto (Anmelde Informationen) bei der PMC anmelden, um den Migrations Vorgang zu starten. Nachdem Sie die Schritte zum Verschieben Ihres Kontos abgeschlossen haben, können Sie damit beginnen, Ihre Mitgliedschaft zu verwalten und Ihrem Team Benutzer Rollen und Berechtigungen zuzuweisen, damit Sie auf die Vorteile zugreifen und die Mitgliedschaft verwalten können. Microsoft migriert automatisch die aktuellen Kompetenzen, Vorteile, Standortinformationen, Bank-/Steuerungsinformationen zu Incentives und MCP-Zuordnungen, einschließlich des Zugriffs auf die Partner Universität.

Microsoft migriert automatisch die aktuellen Kompetenzen, Vorteile, Standortinformationen, Bank-/Steuerungsinformationen zu Incentives und MCP-Zuordnungen, einschließlich des Zugriffs auf die Partner Universität.

**Wie wird die Erneuerungs Richtlinie geändert?**

 Im Partner Center wird das Erneuerungs Fenster in den folgenden 30 Tagen von Ihrem Anniversary Date entfernt.

**Bleiben unsere Kompetenzen nach dem Wechsel zu Partner Center unverändert?**

Ja, der Umstieg auf Partner Center hat keine Auswirkungen auf die Kompatibilität. Wenn Sie Abweichungen bemerken, wenden Sie sich an den [Support](https://partner.microsoft.com/support).


 **Ändert sich meine Vorteile (einschließlich Cloud-Vorteilen, technischer Support, Software Vorteile, Visual Studio) nach dem Verschieben?**

 Ihre berechtigten Vorteile werden sich nicht ändern. Wenn Sie Abweichungen bemerken, wenden Sie sich an den [Support](https://partner.microsoft.com/support).

 **Werden unsere Microsoft-Konten, die über Visual Studio-Vorteile verfügen, berücksichtigt?**


 Ja. Visual Studio-Vorteile, die MSAs zugeordnet sind, bleiben erhalten und gelten weiter. Sie werden auch nach der Verlängerung in Partner Center beibehalten. Wenn Sie jedoch eine MSA-Zuordnung entfernen, nachdem Sie im Partner Center migriert wurde, kann Sie nicht wieder in Partner Center hinzugefügt werden.

In Partner Center kann ein Partner Geschäftskonten und Gastbenutzerkonten vom Typ MSA aus demselben Mandanten hinzufügen, in dem der Partner MPN-Administrator im Azure AD-Mandanten ist. Wenn der Partner globaler Administrator in mehreren Azure AD-Mandanten ist und all diese Mandanten demselben Partner Center-Konto zugeordnet sind, kann der Partner Benutzer aus all diesen Mandanten zu Visual Studio-Vorteilen und zu auf der Azure-Nutzung basierenden Zuordnungen hinzufügen.

Ein MPN-Administrator oder globaler Administrator kann zwar Gastbenutzern nutzungsbasierte Visual Studio-Abonnements zuweisen, aber Gastbenutzer können sich nicht mit ihrem MSA bei Partner Center anmelden. Gastbenutzer können sich aber bei Azure und Visual Studio anmelden, um die ihnen zugewiesenen Vorteile zu überprüfen und zu nutzen.


 **Wie sollten wir unsere MCP-Zuordnungen und unseren Partner University-Zugang verwalten?**

 Es gibt keine Änderungen an MCP-Zuordnungen, die von der PMC wechseln. Neue neue Mitarbeiter, die nach dem Wechsel zu Partner Center wechseln, müssen jedoch im Partner Center verknüpft werden. Alle Ihre Partner University-Berechtigungen für vorhandene Benutzer bleiben erhalten, aber alle neuen Mitarbeiter sollten [das Schulungs Center](https://partner.microsoft.com/training) aufrufen, um Informationen dazu zu erhalten, wie Sie auf die Partner Universität zugreifen können.

 **Gewusst wie Anzeigen von MCP-Informationen, sobald ich zu Partner Center verschiebe?**

Wählen Sie im Dashboard im linken Navigationsbereich die Option **Zuständigkeiten** aus. Auf der Seite " **Kompetenzen** " können Sie den Bericht "Skills" herunterladen. Der Bericht "Skills" listet die Benutzer auf, die für die Kompetenzen und Programme in Partner Center relevante Kenntnisse erworben haben. Wenn Ihre Benutzer Fertigkeiten erhalten haben, diese aber nicht für die Fähigkeiten relevant sind, an denen Sie arbeiten, werden Sie nicht im Bericht aufgeführt.


 **Werden Kunden Verweise in Partner Center verwendet?**

 Nein, Sie benötigen keine Kundenreferenzen, um die Kompetenzanforderungen in Partner Center zu erfüllen.

 **Wird Partner von Daten Satz Zuordnungen in Partner Center verschoben?**

 Ja, es gibt keine Änderung am Partner des Datensatzes. Erfahren Sie mehr über [das Verknüpfen ihrer Partner-ID mit ihren Kunden](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Gibt es aufgrund der Umstellung auf Partner Center Auswirkungen auf die Anreize?**

Nein, es gibt keine Auswirkung auf Anreize, wenn Sie Ihr Konto verschoben haben, ohne Standorte zu konsolidieren. Wenn Ihr Unternehmen über mehrere Konten in der PMC verfügt und Sie sich bei der Umstellung auf Partner Center entscheiden, sich für ein globales Konto zu konsolidieren, kommt es nicht zu einem Ausfall, aber es kann zu einer Verzögerung bei der Incentive-Auszahlung kommen. Wenn Sie nicht alle Ihre PMC-Konten verschieben, die in den Programmen "Incentives" involviert sind, werden Sie möglicherweise nicht mehr mit diesen Konten verknüpften Anreizen erwerben.


**Was sind die Incentive-Benutzer Rollen in Partner Center?** 

Die Incentive-Rollen im Partner Center sind Standort basiert und enthalten Administrator-und Incentive-Benutzer von Incentives. Weitere Informationen zu den Möglichkeiten dieser Rollen finden Sie unter [Zuweisen von Benutzern zu Rollen und Berechtigungen](permissions-overview.md).

**Können Benutzer auf globaler Ebene und auf Standortebene zugewiesen werden?**

 Ja. Sie können einen Administrator für Incentives als Incentive-Administrator für alle Standorte zuweisen, oder jeder Standort kann über einen eigenen Administrator für Incentives verfügen.

 **Können Anreize auf globaler oder auf Standortebene gezahlt werden?**

 Anreize werden nur auf Standortebene bezahlt.

**Wie viele geschäftsprofile können wir in Bezug auf Verweise erstellen?**

Ihr Unternehmen kann so viele geschäftsprofile erstellen, wie Sie Ihre Unternehmensinteressen vollständig darstellen müssen. In jedem Geschäftsprofil können Sie bis zu fünf Standorte auflisten, einen Standort pro Land. Jedes Geschäftsprofil kann für jeden seiner Standorte Verweise erhalten.

**Wie werden Verweise zugewiesen, welche Änderungen kann ich erwarten? Wenn ich beispielsweise ein globales Unternehmen auf einem Markt und Standorte in anderen Märkten verwende, wie werden Verweise zugewiesen?**

Verweise werden basierend auf den Suchparametern zugewiesen, die vom Kunden definiert werden. Unabhängig davon, ob Sie einen oder mehrere Orte haben, wenn die Kunden einen gewünschten Standort angeben und ein Unternehmen vorhanden ist, das den anderen Parametern entspricht, wird der Verweis an diesen Speicherort gesendet.








