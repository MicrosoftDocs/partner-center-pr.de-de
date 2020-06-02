---
title: Umstellen vom Partner Membership Center
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Machen Sie sich mit nützlichen Informationen und häufig gestellten Fragen vertraut, bevor Sie Ihr Geschäft vom Partner Membership Center auf das Partner Center umstellen.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 0c1fc9530a978e7202d7a0d58a574546b10c91e9
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795846"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Vorbereiten der Umstellung von Partner Membership Center (PMC) auf Partner Center

**Geeignete Rollen**
- Globaler Administrator
- Benutzeradministrator
- Vertriebsbeauftragter
- Administrator-Agent

Wir stellen die Mitgliedschaftsverwaltung von Partner Membership Center (PMC) auf Partner Center um, den zentralen Ort, um Ihre Geschäftsbeziehung mit Microsoft zu verwalten. Wir möchten, dass Ihre Umstellung auf Partner Center so effizient und einfach wie möglich erfolgt. Wir haben einige Bereiche identifiziert, in denen sich Partner Center von PMC unterscheidet, und wir sind der Ansicht, dass Sie diese vor der Umstellung verstehen und darauf vorbereitet sein sollten.

## <a name="account-and-identity-setup"></a>Einrichtung von Konten und Identitäten

**Was ist ein Azure AD-Geschäftskonto (Azure Active Directory)?**

Ein Azure-Geschäftskonto ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud. Das Konto wird für Sie erstellt, wenn Sie einen Microsoft Cloud Service wie Azure, Microsoft Intune oder Office 365 abonnieren.

Das Geschäftskonto hostet Ihre Azure AD-Benutzer und die zugehörigen Informationen: E-Mail-Nachrichten, Kennwörter, Profildaten, Berechtigungen usw. Zudem enthält das Geschäftskonto Gruppen, Anwendungen und andere Informationen, die ein Unternehmen und seine Sicherheit betreffen. 

Ihre geschäftliche E-Mail-Adresse ist Teil Ihres Azure Active Directory-Mandanten. Wenn Sie ein Konto in Partner Center verwenden möchten, benötigen Sie einen AAD-Mandanten. Weitere Informationen zu Azure Active Directory finden Sie unter [Erstellen Ihres Verzeichnisses in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

In Partner Center verwenden Sie Ihre geschäftliche E-Mail-Adresse (nicht Ihre persönliche E-Mail-Adresse), um sich bei Ihrem Konto anzumelden.
- Ihr Geschäftskonto: john@contoso.com
- Ihr persönliches Konto: John@outlook.com

**Mit welchem Konto sollten Sie sich beim Partner Center anmelden, wenn Sie über einen AAD-Mandanten bei Microsoft (z. B. für Office 365) und zusätzlich über einen Mandanten für Ihr CSP-Geschäft verfügen?**

Sie können sich mit dem CSP-Konto oder Ihrem geschäftlichen MPN-E-Mail-Konto bei Partner Center anmelden. Wenn Sie sich für die Anmeldung mit ihrer geschäftlichen CSP-E-Mail-Adresse entscheiden, werden im linken Navigationsbereich in Ihrem Dashboard sowohl MPN- als auch CSP-Programminformationen angezeigt. Wenn Sie sich mit Ihrer geschäftlichen MPN-E-Mail-Adresse des Azure AD-Mandanten anmelden, werden nur Ihre MPN-Programminformationen angezeigt. 

**Wenn Sie Ihren vorhandenen Office 365 Azure AD-Mandanten nicht für Partner Center verwenden möchten, können Sie vor der Migration von PMC einen neuen Mandanten erstellen.**

Möglicherweise gibt es viele Gründe, warum Sie keinen vorhandenen Azure AD-Mandanten verwenden möchten, um Ihr Partner Center-Konto einzurichten. Bevor Sie mit der Migration zu Partner Center beginnen, navigieren Sie zum [Azure-Portal](https://ms.portal.azure.com/#home), um einen neuen Azure AD-Mandanten zu erstellen. Befolgen Sie die Anweisungen unter [Erstellen eines neuen Mandanten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Verwenden Sie den neuen AAD-Mandanten, um Ihr Partner Center-Konto einzurichten. Sie müssen ein globaler Administrator sein, um den Mandanten erstellen zu können. 


**Benutzerrollen einschließlich Gastbenutzerrollen in Partner Center**

Partner Center verfügt über verschiedene Arten von Rollen, abhängig von den Arbeitsaufgaben, die erforderlich sind. Es gibt Rollen wie den globalen Administrator, die Azure AD-Rollen sind. Einige der Rollen sind spezifisch für Programme wie das Cloud-Dienstanbieter-Programm oder Incentives, und es gibt Rollen, die für MPN spezifisch sind. Informationen zu allen Partner Center-Rollen finden Sie unter [Zuweisen von Rollen und Berechtigungen zu Benutzern](permissions-overview.md).

**Was geschieht mit den Rollen meiner Benutzer, wenn sie von PMC zu Partner Center wechseln?**

Mit Ausnahme des globalen MPN-Administrators oder primären Programmkontakts, der die Migration durchführt, verlieren alle Benutzer in PMC Ihre Administratorrollen. Die Person, die die Migration abschließt, muss Rollen in Partner Center zuweisen. Die Rollen in Partner Center unterscheiden sich von den Rollen in PMC. Weitere Informationen zu Benutzerrollen in Partner Center finden Sie unter [Zuweisen von Rollen und Berechtigungen zu Benutzern] (permissions-overview.md) und [Wechsel von PMC zu Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles).


**Worin besteht der Unterschied zwischen meinem Unternehmensprofil und meinem Geschäftsprofil?**

Ihr Unternehmensprofil besteht aus den Informationen zu Ihrem Unternehmen, die die Adresse, Standorte, de primären Kontakt, Bank- und Steuerdetails umfassen.

Ihr Geschäftsprofil definiert, wie Sie sich Ihren Kunden präsentieren: Es handelt sich um eine Marketingseite, auf der Ihr Logo, Details zu ihrem geschäftlichen Schwerpunkt sowie Ihrem Fachwissen usw. angezeigt werden.

**Was bedeutet Kontokonsolidierung für mein Konto?**

Wenn Sie denselben Azure AD-Mandanten verwenden, um mehrere MPN-Konten zu Partner Center zu migrieren, erkennt das System dies automatisch, und Sie werden aufgefordert, Ihre Konten zu konsolidieren. Dies gilt auch, wenn Sie über mehrere Domänen verfügen, die demselben Azure AD-Mandanten zugeordnet sind. 

Sie können sich dennoch entscheiden, eine Migration zu Partner Center mit separaten AAD-Mandanten durchführen. Beachten Sie jedoch, dass dies eine isolierte Auswertung ihrer Kompetenzen und zusätzliche Einkaufskosten zur Folge hat. Weitere Informationen zur Kontokonsolidierung finden Sie unter [Konsolidieren Ihrer Unternehmenskonten](consolidate-accounts.md).

**Wenn ich mehrere AAD-Mandanten und ein MPN-Konto verwende, ist es dann möglich, diese in Partner Center zu verknüpfen?**

Ja, in Partner Center können Sie mehrere Azure AD-Mandanten mit einem Partner Center-Konto verknüpfen.
Weitere Informationen zur Kontokonsolidierung finden Sie unter [Konsolidieren Ihrer Unternehmenskonten](consolidate-accounts.md).

**Gibt es Einschränkungen beim Hinzufügen mehrerer Azure AD-Mandanten zu einem einzelnen Partner Center-Konto?**

Wenn der Azure AD-Mandant bereits einem vorhandenen Partner Center-Konto zugeordnet ist, kann er nicht mithilfe der Funktion für Mehrinstanzfähigkeit mit neuen Partner Center-Konten verknüpft werden. Anders ausgedrückt: Ein Azure AD-Mandant kann nur einem Partner Center-Konto zugeordnet werden, aber einem Partner Center-Konto können mehrere Mandanten zugeordnet sein.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migration der MPN-Mitgliedschaft (Microsoft Partner Network) 

**Wer kann die Umstellung von PMC auf Partner Center durchführen?**

Der globale MPN-Administrator des Unternehmens oder der primäre Programmkontakt (diese beiden Rollen sind oft derselben Person zugewiese) kann die Umstellung einleiten und durchführen.

**Wird die Person, die die Migration durchführt, zum primären Kontakt im rechtlichen Profil des Unternehmens in Partner Center?**

Nicht notwendigerweise, aber der primäre Kontakt muss eine Person sein, die autorisiert ist, Vereinbarungen zu unterzeichnen.

**Kann Microsoft meine MPN-Mitgliedschaft für mich migrieren?**

Nein Microsoft kann Ihnen nicht dabei helfen, Ihr Mitgliedschaftskonto in Partner Center zu verschieben. Sie müssen Ihr Konto verschieben, indem Sie sich mit Ihrem Geschäftskonto (Anmeldeinformationen) bei PMC anmelden, um den Migrationsvorgang zu starten. Nachdem Sie die Schritte zum Verschieben Ihres Kontos abgeschlossen haben, können Sie damit beginnen, Ihre Mitgliedschaft zu verwalten und Ihrem Team Benutzerrollen und Berechtigungen zuzuweisen, damit die Teammitglieder auf Vorteile zugreifen und die Mitgliedschaft verwalten können. Microsoft migriert automatisch die aktuellen Kompetenzen, Vorteile, Standortinformationen, Bank-/Steuerungsinformationen für Incentives und MCP-Zuordnungen, einschließlich des Zugriffs auf die Partner-Universität.

Microsoft migriert automatisch die aktuellen Kompetenzen, Vorteile, Standortinformationen, Bank-/Steuerungsinformationen für Incentives und MCP-Zuordnungen, einschließlich des Zugriffs auf Partner University.

**Wie ändert sich die Verlängerungsrichtlinie?**

 In Partner Center erstreckt sich das Verlängerungsfenster von Ihrem Jahrestag bis zu den folgenden 30 Tagen.

**Bleiben unsere Kompetenzen nach dem Wechsel zu Partner Center unverändert?**

Ja, der Umstieg auf Partner Center hat keine Auswirkungen auf die Kompetenzen. Wenn Sie Abweichungen bemerken, wenden Sie sich an den [Support](https://partner.microsoft.com/support).


 **Ändern sich meine Vorteile (z. B. Cloudvorteile, technischer Support, Softwarevorteile, Visual Studio) nach dem Umstieg?**

 Die Vorteile, für die Sie berechtigt sind, ändern sich nicht. Wenn Sie Abweichungen bemerken, wenden Sie sich an den [Support](https://partner.microsoft.com/support).

 **Werden unsere Microsoft-Konten, die über Visual Studio-Vorteile verfügen, berücksichtigt?**


 Ja. Visual Studio-Vorteile, die MSAs zugeordnet sind, bleiben erhalten und gelten weiter. Sie werden auch nach der Verlängerung in Partner Center beibehalten. Wenn Sie jedoch nach der Migration zu Partner Center eine MSA-Zuordnung entfernen, kann diese Partner Center nicht erneut hinzugefügt werden.

In Partner Center kann ein Partner Geschäftskonten und Gastbenutzerkonten vom Typ MSA aus demselben Mandanten hinzufügen, in dem der Partner MPN-Administrator im Azure AD-Mandanten ist. Wenn der Partner globaler Administrator in mehreren Azure AD-Mandanten ist und all diese Mandanten demselben Partner Center-Konto zugeordnet sind, kann der Partner Benutzer aus all diesen Mandanten zu Visual Studio-Vorteilen und zu auf der Azure-Nutzung basierenden Zuordnungen hinzufügen.

Ein MPN-Administrator oder globaler Administrator kann zwar Gastbenutzern nutzungsbasierte Visual Studio-Abonnements zuweisen, aber Gastbenutzer können sich nicht mit ihrem MSA bei Partner Center anmelden. Gastbenutzer können sich aber bei Azure und Visual Studio anmelden, um die ihnen zugewiesenen Vorteile zu überprüfen und zu nutzen.


 **Wie sollten wir unsere MCP-Zuordnungen und unseren Partner University-Zugang verwalten?**

 Es gibt keine Änderungen an MCP-Zuordnungen, die aus PMC verschoben werden. Neue Mitarbeiter müssen jedoch nach dem Wechsel zu Partner Center in Partner Center zugeordnet werden. Alle Ihre Partner University-Berechtigungen für vorhandene Benutzer bleiben erhalten, aber alle neuen Mitarbeiter sollten zum [Trainigscenter](https://partner.microsoft.com/training) navigieren, um Informationen dazu zu erhalten, wie Sie auf Partner University zugreifen können.

 **Wie zeige ich nach dem Umstieg auf Partner Center MCP-Informationen an?**

Wählen Sie im linken Navigationsbereich des Dashboards **Kompetenzen** aus. Auf der Seite **Kompetenzen** können Sie den Qualifikationsbericht herunterladen. Der Qualifikationsbericht listet die Benutzer auf, die für die Kompetenzen und Programme in Partner Center relevante Kenntnisse erworben haben. Wenn Ihre Benutzer Qualifikationen erworben haben, diese aber nicht für die Kompetenzen relevant sind, die Sie anbieten möchten, werden sie nicht im Bericht aufgeführt.


 **Werden in Partner Center Kundenreferenzen verwendet?**

 Nein, Sie benötigen keine Kundenreferenzen, um die Kompetenzanforderungen in Partner Center zu erfüllen.

 **Werden registrierte Abonnementberater (Partner of Record) in Partner Center verschoben?**

 Ja, es gibt keine Änderungen bei Partner of Record. Erfahren Sie mehr über das [Verknüpfen Ihrer Partner-ID mit Ihren Kunden](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Gibt es aufgrund der Umstellung auf Partner Center Auswirkungen auf Incentives?**

Nein, es gibt keine Auswirkung auf Incentives, wenn Sie Ihr Konto verschoben haben, ohne Standorte zu konsolidieren. Wenn Ihr Unternehmen über mehrere Konten in PMC verfügt und Sie sich bei der Umstellung auf Partner Center entscheiden, diese in einem globalen Konto zu konsolidieren, kommt es nicht zu einem Verlust von Incentives, aber es kann zu einer Verzögerung bei der Incentiveauszahlung kommen. Wenn Sie nicht alle Ihre PMC-Konten verschieben, die an Incentivepogrammen teilgenommen haben, erwerben Sie möglicherweise keine weiteren mit diesen Konten verknüpften Incentives.


**Was sind die Incentiverollen im Partner Center?** 

Incentiverollen in Partner Center sind standortbasiert und umfassen Incentiveaministrator und Incentivebenutzer. Weitere Informationen zu den Aufgaben, die diese Rollen ausführen können, finden Sie unter [Zuweisen von Rollen und Berechtigungen zu Benutzern](permissions-overview.md).

**Können Incentiveadministratoren auf globaler Ebene und auf Standortebene zugewiesen werden?**

 Ja. Sie können einen Incentiveadministrator als Incentiveadministrator für alle Standorte zuweisen, oder jeder Standort kann über einen eigenen Incentiveadministrator verfügen.

 **Können Incentives auf globaler Ebene oder auf Standortebene bezahlt werden?**

 Incentives werden nur auf Standortebene bezahlt.

**Wie viele Geschäftsprofile können wir in Bezug auf Empfehlungen erstellen?**

Ihr Unternehmen kann so viele Geschäftsprofile wie erforderlich erstellen, um die Interessen Ihres Unternehmens vollständig darzustellen. In jedem Geschäftsprofil können Sie bis zu fünf Standorte auflisten: einen Standort pro Land. Jedes Geschäftsprofil kann für jeden seiner Standorte Empfehlungen erhalten.

**Wie werden Empfehlungen zugewiesen, und welche Änderungen muss ich erwarten? Wenn ich beispielsweise ein globales Unternehmen in einem Markt und Standorte in anderen Märkten habe, wie werden Empfehlungen dann zugewiesen?**

Empfehlungen werden basierend auf den Suchparametern zugewiesen, die der Kunde definiert. Wenn Kunden einen gewünschten Standort angeben und Sie dort ein Unternehmen betreiben, das die anderen Parameter erfüllt, geht die Empfehlung unabhängig davon, ob Sie einen oder mehrere Standorte nutzen, an diesen Standort.








