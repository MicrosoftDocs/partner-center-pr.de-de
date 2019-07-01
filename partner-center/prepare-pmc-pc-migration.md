---
title: Vorbereiten für die Migration Partner Membership Center zu Partner Center | Partner Center
ms.topic: article
ms.date: 06/13/2019
description: Problemstellungen zu bedenken, bevor Sie Ihr Unternehmen zu Partner Center von PMC verschieben
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0f1df50c5fa94707ac733a91b0d981b6821de8c0
ms.sourcegitcommit: 7b3847a788365a05628a4cf2938dfd61782d6e4e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2019
ms.locfileid: "67468024"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Vorbereiten Sie für die Migration von Partner Membership Center (PMC) zum Partner Center

Verwalten der Gruppenmitgliedschaft Verschieben von Partner Membership Center (PMC) an das Partnercenter – der einzige Ort zum Verwalten Ihrer Business-Beziehung mit Microsoft wir. Die Migration zu Partner Center so effizient und einfach wie möglich sein soll. Wir haben einige Bereiche gekennzeichnet, wobei das Partner Center unterscheidet sich von PMC und wir glauben, dass Sie verstehen und dafür vorbereiten, bevor Sie die Verschiebung vornehmen möchten.

## <a name="account-and-identity-setup"></a>Konten- und Identitätsdaten-setup

**Was ist ein Geschäftskonto für Azure Active Directory (Azure AD)?**

Ein Azure-Geschäftskonto ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud. Das Konto wird für Sie erstellt, wenn Sie einen der Microsoft Cloud Services wie Azure, Microsoft Intune oder Office 365 abonnieren.

Ihr Geschäftskonto hostet Ihre Azure AD-Benutzer und die Informationen zu diesen - ihre e-Mail-Adresse, Kennwörter, Profildaten, Berechtigungen und So weiter. Das Geschäftskonto enthält außerdem Gruppen, Anwendungen und andere Informationen für ein Unternehmen und seine Sicherheit. Weitere Informationen finden Sie unter...

Verwenden Sie Ihre geschäftliche e-Mail-Adresse im Partner Center in Ihrem Konto nicht Ihre persönliche e-Mail-Adresse anmelden.
- Ihrem Geschäftskonto an: john@contoso.com
- Ihr persönliches Konto: John@outlook.com

Ihre geschäftliche e-Mail-Adresse ist Teil Ihres Azure active Directory-Mandanten. Um ein Konto im Partner Center zu verfügen, müssen Sie einen AAD-Mandanten verfügen. Weitere Informationen zu Azure Active Directory, finden Sie in [erstellen Sie Ihr Verzeichnis in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Beim Wechsel zum Partner Center von PMC, welches Konto Sie sich bei Partner Center mit, wenn Sie anmelden sollten haben ein AAD-Mandanten mit Microsoft (für Office 365, z. B.), und Sie auch ein Mandant für Ihr Unternehmen CSP?**

Sie können mit dem CSP-Konto oder Ihrem MPN-e-Mail-Geschäftskonto in Partner Center anmelden. Wenn Sie entscheiden, melden Sie sich mit Ihrem CSP geschäftliche e-Mail-Adresse, werden im linke Navigationsbereich auf Ihrem Dashboard sowohl MPN und CSP-Programm angezeigt. Wenn Sie sich mit Ihrer MPN-Azure AD-Mandanten geschäftliche e-Mail-Adresse anmelden, sehen Sie nur Ihre MPN-Programm-Informationen. MPN und CSP von Benutzerrollen zu unterscheiden, wenn Sie das gleiche Konto für sowohl MPN und CSP-Unternehmen verwenden, seien Sie sicher, dass Sie entsprechend Benutzerrollen zuweisen. Lesen Sie Informationen zu Benutzerrollen, [weisen Sie Benutzerrollen und Berechtigungen](permissions-overview.md).

**Was ist der Unterschied zwischen der globalen Administratorrolle AAD und die globale Administratorrolle für die PMC MPN?**

Hierbei handelt es sich um zwei völlig verschiedene Rollen mit verschiedenen Berechtigungen. Globale Administrator die AAD-Mandanten im Partner Center des Mandanten verwaltet – hinzugefügt oder entfernt Benutzer, bietet und verwaltet die Kennwörter, Rollen und Berechtigungen und hat Zugriff auf ihre Unternehmens-Programme im Partner Center. 

Die globale Administratorrolle MPN in PMC könnte Folgendes ausführen:

- Zeigen Sie an und bearbeiten Sie die Daten, die für das Unternehmen und alle Standorte des Unternehmens zugeordnet

-  Fügen Sie auf der globalen oder lokalen Administratoren hinzu.  Darüber hinaus können globale Administratoren von einer Person an einem beliebigen Speicherort globalen Administratorzugriff zuweisen, die sie globalen Zugriff gewährt, unabhängig davon, welcher, dem Stelle sie zugeordnet sind.
-  Führen Sie alle Partner mit Internetzugriff, einschließlich der UI-Funktion: 

-  Hinzufügen/Entfernen von Benutzern

 - Weisen Sie/Entfernen von Rollen 

 - Hinzufügen/Entfernen/Aktualisieren von Standorten 

 - Erwerb der Kompetenz/Zuordnungen 

-  Anzeigen von Vorteilen

Wechselt der globale Administrator von MPN zum Partner Center heißt die Rolle den MPN-Partner-Administrator mit anderen Berechtigungen und Aufgaben als dem globalen Partner Center-Administrator. Finden Sie weitere Informationen zu Rollen und Berechtigungen in Partner Center, [weisen Benutzerrollen und Berechtigungen](permissions-overview.md)

**Einschließlich der Gast-Benutzerrollen im Partner Center-Benutzerrollen**

Partner Center verfügt über verschiedene Arten von Rollen je nach Art der Arbeit durchgeführt werden musste. Es gibt Rollen wie z. B. globaler Administrator, die Azure AD-Rollen sind. Einige der Rollen beziehen sich auf Programme, z. B. Cloud Service Provider-Programm oder Anreize, und sind Rollen, die spezifisch für MPN sind. Um herauszufinden, was alle Partner Center-Rollen sind, lesen Sie [weisen Benutzerrollen und Berechtigungen](permissions-overview.md).



**Was geschieht mit meiner Benutzer Rollen, wenn sie PMC zum Partner Center wechseln?**

Mit Ausnahme des MPN globaler Administrator oder die primäre Anwendung wenden Sie sich an, die die Migration führt, verlieren alle Benutzer in der PMC die Administratorrollen aus. Die Person, die Abschluss der Migration müssen zum Zuweisen von Rollen im Partner Center. Die Rollen im Partner Center unterscheiden sich von denen in der PMC. Lesen [weisen Benutzerrollen und Berechtigungen](permissions-overview) und [verschieben aus der PMC in Partner Center](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) für weitere zu Benutzerrollen in Partner Center.


**Was ist der Unterschied zwischen meinem Unternehmensprofil und Meine Business-Profil?**

Ihr Unternehmensprofil ist die Informationen über Ihr Unternehmen, die enthält die Adresse, Standorte, primäre Ansprechpartner, Bank- und Steuerdaten Details.

Ihre Business-Profil wie Sie sich an Kunden vorhanden ist, und es ist eine marketing-Seite, die das Logo, Informationen zu den Fokus des Business, Ihr Fachwissen usw. angezeigt.

**Was die Konsolidierung der Mittelwert für mein Konto berücksichtigt werden?**

Wenn Sie den gleichen Azure AD-Mandanten verwenden, um mehrere MPN-Konten in Partner Center zu migrieren, das System automatisch erkennen, und Sie werden aufgefordert, Ihre Konten zu konsolidieren. Dies gilt auch, wenn Sie mehrere Domänen, die demselben Azure AD-Mandanten zugeordnet haben. 

Sie können weiterhin migrieren möchten, zum Partner Center mit separaten AAD-Mandanten, aber beachten Sie, dass diese Ergebnisse in isolierten Evaluierung Ihre Kompetenzen und zusätzliche Kosten zu erwerben. 

**Wenn ich mehrere AAD-Mandanten und ein einzelnes MPN-Konto verfügen, ist es möglich, um sie im Partner Center verknüpfen?**

Ja, können Sie im Partner Center mehrere Azure AD-Mandanten und einzelnen Partner Center-Konto verknüpfen.
Hier erfahren Sie mehr. 

**Gibt es Einschränkungen beim Hinzufügen von mehreren Azure AD-Mandanten zu einem einzelnen Partner Center-Konto?**

Wenn Azure AD-Mandanten bereits ein vorhandenes Partner Center-Konto zugeordnet ist, darf nicht die neue Partner Center-Konten, die mithilfe der Funktion für mehrere Mandanten zugeordnet sein. Ist eine weitere Möglichkeit vorstellen, Azure AD-Mandant kann nur mit einem Partner Center-Konto zugeordnet werden, aber ein Partner Center-Konto kann mehrere Mandanten zugeordnet haben.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) Membership-migration 

**Das Verschieben von PMC zum Partner Center ausführen kann?**

Ihr Unternehmen MPN globaler Administrator oder der primären Anwendung wenden Sie sich an (diese beiden Rollen werden häufig von derselben Person aufrechterhalten) kann initiieren, und führen Sie die Verschiebung.

**Wird die Person, die Abschließen der Migration der primäre Ansprechpartner im Unternehmen rechtliche Profil im Partner Center?**

Der primäre Ansprechpartner muss, einen Benutzer handeln, die Autorisierung zum Signieren von Vereinbarungen verfügt jedoch nicht notwendigerweise.

**Kann Microsoft Meine MPN-Mitgliedschaft für mich migrieren?**

Nein. Mit Hilfe von Microsoft kann nicht Sie Ihr Konto für die Mitgliedschaft in Partnercenter zu verschieben. Sie benötigen, um Ihr Konto zu verschieben, melden Sie sich die PMC mit Ihrem Geschäftskonto (Anmeldung Anmeldeinformationen), um die Migration zu starten. Nach Abschluss der Schritte aus, um Ihr Konto verschieben können Sie beginnen der Verwaltung von Ihrer Mitgliedschaft und von Benutzerrollen und Berechtigungen für Ihr Team zuweisen, damit sie Zugriff auf Vorteile und die Mitgliedschaft verwalten können. Microsoft migriert automatisch die aktuellen Kompetenzen, Vorteile, Informationen zum Speicherort, Bank/Steuerinformationen für Incentives und MCP-Zuordnungen, einschließlich des Zugriffs der Partner University-Plattform.

Microsoft migriert automatisch die aktuellen Kompetenzen, Vorteile, Informationen zum Speicherort, Bank/Steuerinformationen für Incentives und MCP-Zuordnungen, einschließlich des Zugriffs der Partner University-Plattform.

**Wie wird die Richtlinie für die Verlängerung ändern?**

 Ist im Partner Center im erneuerungsfenster aus Ihrer Jahrestag über die folgenden 30 Tage.

**Bleibt unsere Kompetenzen unverändert nach der Umstellung auf Partner Center?**

Ja, sind Compentencies durch den Wechsel zu Partner Center nicht betroffen. Wenn Sie Unterschiede feststellen, wenden Sie sich an [Unterstützung](https://partner.microsoft.com/support).


 **Ändern (einschließlich Cloud-Vorteile "," technischer Support "," Vorteile durch Software, Visual Studio) sich meine Leistungen nach dem wir verschieben?**

 Ihre berechtigten Vorteile werden nicht geändert werden. Wenn Sie Unterschiede feststellen, wenden Sie sich an [Unterstützung](https://partner.microsoft.com/support).

 **Werden unsere Microsoft-Konten, die Zuordnungen für Visual Studio-Vorteile werden berücksichtigt?**


 Ja. Visual Studio-Vorteile, die für MSAs zugeordnet werden berücksichtigt und beibehalten werden. Sie werden auch nach der Erneuerung im Partner Center beibehalten. Wenn Sie entfernen eine MSA-Verteilung einmal migriert wird, im Partner Center, es kann nicht hinzugefügt werden, wieder in Partner Center.

Im Partner Center kann ein Partner Geschäftskonten und Benutzerkonten für Gäste die MSA aus dem gleichen Mandanten sind, ist der Partner MPN-Administrator in Azure AD-Mandanten hinzufügen. Wenn der Partner ein globaler Administrator in mehreren Azure AD-Mandanten ist, und alle diese Mandanten das gleiche Partner Center-Konto zugewiesen sind, ist der Partner zum Hinzufügen von Benutzern für alle diese Mandanten in die Vorteile für Visual Studio und Azure nutzungsbasierten Zuordnungen zulässig.

Obwohl Gastbenutzer nutzungsbasierte Abonnements von Visual Studio von der MPN-Administrator oder den globalen Administrator zugewiesen werden, können, können keine Gastbenutzer zum Partner Center melden Sie sich mit ihrer MSA. Gastbenutzer können jedoch, melden Sie sich für Azure und Visual Studio, um zu überprüfen, und nutzen Sie ihre zugewiesenen Vorteile.


 **Wie sollten wir unsere MCP-Zuordnungen und unsere Partner University-Zugriff verwalten?**

 Es gibt keine Änderungen an der MCP-Zuordnungen, die von PMC zu verschieben. Allerdings müssen alle neuen neue Mitarbeiter nach dem Wechsel zu Partner Center im Partner Center verknüpft werden soll. Alle Partner University-Berechtigungen für vorhandene Benutzer bleibt jedoch alle neuen Mitarbeiter sollte zum [der Schulungscenter](https://partner.microsoft.com/training) Informationen für den Zugriff auf Partner University-Plattform.

 **Werden Kundenreferenzen werden im Partner Center verwendet?**

 Nein, nicht Kundenreferenzen Kompetenz im Partner Center Anforderungen erforderlich.

 **Werden Partner of Record-Zuordnungen werden zum Partner Center verschoben?**

 Ja, es ist keine Änderung an den Partner of Record. Erfahren Sie mehr über [Verknüpfen Ihrer Partner-ID für Ihre Kunden](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Gibt es Auswirkungen auf Incentives sammeln, wenn aufgrund der Umstieg auf Partner Center?**

Nein, besteht keine Auswirkungen auf Anreize, wenn Sie Ihr Konto ohne Konsolidierung Speicherorte verschoben haben. Wenn Ihr Unternehmen verfügt über mehrere Konten in PMC und beim Wechsel zu Partner Center, die Sie in ein globales Konto konsolidieren möchten, ohne Datenverlust zu Incentives ordnungsgemäß abgerechnet werden, aber möglicherweise eine Verzögerung in anreizprogramm Auszahlung. Wenn Sie alle Ihre Konten über die PMC verschieben nicht, die in Programmen für Incentives beteiligt gewesen sein, können Sie beenden, gibt an, dass Incentives ordnungsgemäß abgerechnet, die für diese Konten verknüpft sind.


**Was sind die anreizprogramm Benutzerrollen im Partner Center?** 

Incentive Rollen im Partner Center sind: die standortbasierte und umfassen Incentives Admin und Anreize für Benutzer. Weitere Informationen zu diesen Rollen Möglichkeiten, finden Sie unter [weisen Benutzerrollen und Berechtigungen](permissions-overview.md).

**Können Incentives sammeln, wenn Benutzer auf der globalen und Standort werden zugewiesen?**

 Ja. Können Sie einen Administrator Incentives sammeln, wenn die Incentives für Administratorrechte für alle Speicherorte zuweisen kann jedem Standort auch eigene Incentives-Administrator.

 **Können Incentives sammeln, wenn auf der globalen oder Speicherort werden bezahlt?**

 Incentives werden nur auf Standortebene bezahlt.

**Können wir in Bezug auf Verweise wie viele Geschäftsprofile erstellen?**

Ihr Unternehmen kann beliebig viele Geschäftsprofile als Ihren Bedarf vollständig Ihres Unternehmens Interessen darstellen. In jedes Geschäftsprofils festlegen können Sie bis zu fünf Orte, einem Ort pro Land auflisten. Erhalten der Business-Profilen der einzelnen Verweise für jede Position ein.

**Wie Verweise zugeordnet werden, welche Änderungen kann ich erwarten? Beispielsweise ein globales Unternehmen in einem Markt und Speicherorte im anderen Märkten vorliegt, werden wie Verweise werden zugewiesen?**

Verweise werden basierend auf den Suchparametern, die vom Kunden definierten zugewiesen. Also unabhängig davon, ob Sie haben einen Speicherort oder viele, wenn Kunden gibt an, den gewünschten Speicherort und haben ein Unternehmen gibt es, die die anderen Parameter entspricht, und klicken Sie dann den Verweis auf diesen Speicherort gesendet würde.








