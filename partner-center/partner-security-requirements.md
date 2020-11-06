---
title: Sicherheitsanforderungen für Partner
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Beschreibt die Sicherheitsanforderungen für Partner, die für die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) und das Framework für das sichere Anwendungsmodell erforderlich sind.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 351d0715645b6e43607279393cdc376d898a7f54
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132976"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Sicherheitsanforderungen für die Verwendung von Partner Center oder Partner Center-APIs

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
- Alle Control Panel-Anbieter
- Alle Berater

**Geeignete Benutzer**

- Alle aktivierten Benutzer einschließlich Gastbenutzer

In diesem Artikel werden die obligatorischen Sicherheitsanforderungen für Berater, Control Panel Vendors und Partner, die am Cloud Solution Provider-Programm teilnehmen, sowie Authentifizierungsoptionen und andere Sicherheitsaspekte erläutert. Datenschutzmaßnahmen und Sicherheit gehören zu unseren obersten Prioritäten. Wir wissen, dass die beste Verteidigung die Prävention ist und dass wir nur so stark sind wie unser schwächstes Glied. Deshalb müssen alle in unserem Partnerumfeld handeln und sicherstellen, dass sie über angemessene Sicherheitsvorkehrungen verfügen.

## <a name="mandatory-security-requirements"></a>Obligatorische Sicherheitsanforderungen

Partner, die die obligatorischen Sicherheitsanforderungen nicht implementieren, werden nicht in der Lage sein, Transaktionen im Cloud Solution Provider-Programm auszuführen oder Kundenmandanten mit delegierten Administratorrechten zu verwalten. Wenn Partner die Sicherheitsanforderungen nicht implementieren, kann zudem ihre Teilnahme an Programmen gefährdet sein. Die mit den Sicherheitsanforderungen für Partner verbundenen Bestimmungen wurden der Microsoft Partner-Vereinbarung hinzugefügt. In Bezug auf Berater gelten dieselben vertraglichen Anforderungen.

Damit Partner und ihre Kunden geschützt sind, setzen wir voraus, dass Partner folgende Maßnahmen sofort umsetzen:  

1. **Aktivieren der Multi-Factor Authentication (MFA) für alle Benutzerkonten im Partnermandanten**. Sie müssen MFA für alle Benutzerkonten in Ihren Partnermandanten erzwingen. Benutzer müssen MFA verwenden, wenn sie sich bei kommerziellen Microsoft-Clouddiensten anmelden oder im Cloud Solution Provider-Programm Transaktionen über das Partner Center oder APIs ausführen.

2. **Übernehmen des Frameworks „Sicheres Anwendungsmodell“** . Alle Partner, die eine Integration mit Partner Center-APIs durchführen, müssen das [Framework „Sicheres Anwendungsmodell“](/partner-center/develop/enable-secure-app-model) für alle Anwendungs- und Benutzerauthentifizierungsmodelle implementieren.

    > [!IMPORTANT]
    > Es wird dringend empfohlen, dass Partner das sichere Anwendungsmodell für die Integration mit einer Microsoft-API, z. B. Azure Resource Manager oder Microsoft Graph, oder bei Nutzung einer Automatisierung wie PowerShell mithilfe von Benutzeranmeldeinformationen implementieren, um Unterbrechungen während der Durchsetzung von MFA zu vermeiden.

Mithilfe dieser Sicherheitsanforderungen können Sie Ihre Infrastruktur schützen und die Daten Ihrer Kunden vor potenziellen Sicherheitsrisiken wie Identitätsdiebstahl oder anderen Betrugsversuchen bewahren.  

## <a name="implementing-multi-factor-authentication"></a>Implementieren von Multi-Factor Authentication

Zur Einhaltung der Sicherheitsanforderungen für Partner müssen Sie MFA für jedes Benutzerkonto in Ihrem Partnermandanten implementieren und erzwingen. Dafür stehen folgende Möglichkeiten zur Verfügung:

- Implementieren Sie [Azure Active Directory (Azure AD)-Sicherheitsstandards](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Weitere Informationen finden Sie im [nächsten Abschnitt](#security-defaults).

- Erwerben Sie Azure Active Directory Premium für jedes Benutzerkonto. Weitere Informationen finden Sie unter [Planen einer Bereitstellung von Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-getstarted).

- Verwenden Sie eine Drittanbieterlösung zur Erzwingung von MFA für jedes Benutzerkonto in Ihrem Partnermandanten. Um sicherzustellen, dass die Lösung die erwarteten Ergebnisse liefert, informieren Sie sich, [wie die Sicherheitsanforderungen durchgesetzt werden](#how-the-requirements-are-enforced).

> [!NOTE]
> Obwohl die mehrstufige Authentifizierung für eine unabhängige Cloud (US Government und Deutschland) vertraglich nicht verpflichtend ist, wird dringend empfohlen, diese Sicherheitsanforderungen umzusetzen.

### <a name="security-defaults"></a>Sicherheitsstandards

Eine der Optionen, die Partner zur Implementierung von MFA-Anforderungen wählen können, ist die Aktivierung der Sicherheitsstandards in Azure AD. Sicherheitsstandards bieten eine grundlegende Sicherheitsstufe ohne Zusatzkosten. Informieren Sie sich, wie Sie MFA im Rahmen von Azure AD für Ihr Unternehmen aktivieren können. Lesen Sie darüber hinaus die folgenden wichtigen Informationen, bevor Sie Sicherheitsstandards aktivieren.

- Partner, die aktuell Baselinerichtlinien verwenden, müssen jetzt handeln und auf Sicherheitsstandards umstellen.

- Die nun allgemein verfügbaren Sicherheitsstandards ersetzen die Baselinerichtlinien aus der Vorschauversion. Nachdem ein Partner die Sicherheitsstandards aktiviert hat, kann er keine Baselinerichtlinien mehr aktivieren.

- Durch die Sicherheitsstandards werden alle Richtlinien in einem Schritt aktiviert.

- Für Partner, die den [bedingten Zugriff](/azure/active-directory/conditional-access/concept-conditional-access-policy-common) verwenden, sind [keine Sicherheitsstandards verfügbar](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Die Legacyauthentifizierung wird derzeit nicht blockiert. Da die meisten Ereignisse in Zusammenhang mit Identitätsbetrug jedoch bei der Anmeldung über die Legacyauthentifizierung auftreten, sollten Partner besser auf diese älteren Protokolle verzichten.

- Das Azure AD Connect-Synchronisierungskonto ist von den Sicherheitsstandards ausgeschlossen.

Ausführliche Informationen finden Sie unter [Übersicht über Azure Multi-Factor Authentication für Ihre Organisation](/azure/active-directory/authentication/concept-mfa-get-started) und [Was sind Sicherheitsstandards?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Azure AD-Sicherheitsstandards sind die Weiterentwicklung der Baselineschutzrichtlinien in vereinfachter Form. Wenn Sie die Baselineschutzrichtlinien bereits aktiviert haben, wird dringend empfohlen, [Sicherheitsstandards](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) zu aktivieren.

## <a name="implementation-considerations"></a>Überlegungen zur Implementierung

Da diese Anforderungen für alle Benutzerkonten in Ihrem Partnermandanten gelten, müssen Sie einige Dinge beachten, um eine reibungslose Bereitstellung zu gewährleisten. Ermitteln Sie beispielsweise Benutzerkonten in Azure AD, die keine MFA durchführen können, sowie Anwendungen und Geräte in Ihrem Unternehmen, die keine moderne Authentifizierung unterstützen.

Es wird empfohlen, vor der Durchführung von Aktionen die folgenden Punkte zu überprüfen. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Verfügen Sie über eine Anwendung oder ein Gerät, von der bzw. dem die Verwendung moderner Authentifizierung nicht unterstützt wird?

Wenn Sie MFA erzwingen, verwendet die Legacyauthentifizierung Protokolle wie IMAP, POP3, SMTP usw., die blockiert werden, da sie MFA nicht unterstützen. Verwenden Sie im Fall dieser Einschränkung das Feature [App-Kennwörter](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords), um sicherzustellen, dass die Authentifizierung für die Anwendung oder das Gerät weiterhin möglich ist. Sehen Sie sich die [Überlegungen zur Verwendung von App-Kennwörtern](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) an, um festzustellen, ob sie in Ihrer Umgebung verwendet werden können.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Verfügen Sie über Office 365-Benutzer mit Lizenzen, die Ihrem Partnermandanten zugeordnet sind?

Vor der Implementierung einer beliebigen Lösung wird empfohlen, die Microsoft Office-Version zu ermitteln, die Benutzer im Partnermandanten verwenden. Es besteht die Möglichkeit, dass für Ihre Benutzer Verbindungsprobleme bei Anwendungen wie Outlook auftreten. Bevor Sie MFA erzwingen, sollten Sie sicherstellen, dass Sie Outlook 2013 SP1 oder höher verwenden und Ihr Unternehmen über eine moderne Authentifizierung verfügt. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung in Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Sie müssen zwei Registrierungsschlüssel erstellen, um eine moderne Authentifizierung für Geräte mit Windows zu ermöglichen, auf denen Microsoft Office 2013 installiert ist. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Gibt es eine Richtlinie, die verhindert, dass Benutzer ihre mobilen Geräte während der Arbeit verwenden?

Es ist wichtig, jede Unternehmensrichtlinie zu identifizieren, die Mitarbeiter daran hindert, mobile Geräte während der Arbeit zu verwenden, da sich dies auf die MFA-Lösung auswirkt, die Sie implementieren. Es gibt Lösungen, wie die durch die Implementierung von [Azure AD-Sicherheitsstandards](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) bereitgestellte Lösung, die nur die Verwendung einer Authenticator-App für die Überprüfung zulassen. Falls Ihr Unternehmen über eine Richtlinie verfügt, die die Verwendung von mobilen Geräten verhindert, sollten Sie eine der folgenden Optionen in Betracht ziehen:

- Stellen Sie eine Anwendung mit zeitbasiertem Einmalkennwort (TOTP, Time-based One-time Password) bereit, die auf einem sicheren System ausgeführt werden kann.

- Implementieren Sie eine Lösung eines Drittanbieters, die MFA für jedes Benutzerkonto im Partnermandanten erzwingt und die am besten geeignete Überprüfungsoption bietet.

- Kaufen Sie [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/)-Lizenzen für die betroffenen Benutzer.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Über welche Automatisierung oder Integration verfügen Sie, die Benutzeranmeldeinformationen für die Authentifizierung nutzt?

Da MFA für jeden Benutzer, einschließlich Dienstkonten, in Ihrem Partnerverzeichnis erzwungen wird, wirkt sich dies auf jede Automatisierung oder Integration aus, die Benutzeranmeldeinformationen für die Authentifizierung nutzt. Daher ist es wichtig, dass Sie feststellen, welche Konten in diesen Situationen verwendet werden. Im Folgenden eine Liste mit Beispielanwendungen oder -diensten, die infrage kommen:

- Systemsteuerung, die für die Bereitstellung von Ressourcen im Namen Ihrer Kunden verwendet wird

- Integration mit jeder Plattform, die für die Fakturierung (in Bezug auf das CSP-Programm) und Unterstützung Ihrer Kunden verwendet wird

- PowerShell-Skripts, die die Module Az, AzureRM, Azure AD, MS Online, usw. verwenden

Die obige Liste ist nicht vollständig. Daher ist es wichtig, dass Sie eine vollständige Bewertung aller Anwendungen oder Dienste in Ihrer Umgebung durchführen, die Benutzeranmeldeinformationen für die Authentifizierung nutzen. Um die Anforderung für MFA zu erfüllen, sollten Sie nach Möglichkeit die Anweisungen im [Framework für das sichere Anwendungsmodell](/partner-center/develop/enable-secure-app-model) implementieren.

## <a name="accessing-your-environment"></a>Zugriff auf Ihre Umgebung

Um besser zu verstehen, was oder wer die Authentifizierung vornimmt, ohne zur MFA aufgefordert zu werden, sollten Sie die Anmeldeaktivitäten überprüfen. Über Azure Active Directory Premium können Sie den Anmeldebericht nutzen. Weitere Informationen zu diesem Thema finden Sie unter [Berichte zu Anmeldeaktivitäten im Azure Active Directory-Portal](/azure/active-directory/reports-monitoring/concept-sign-ins). Wenn Sie nicht über Azure Active Directory Premium verfügen oder nach einer Möglichkeit suchen, diese Anmeldeaktivität über PowerShell abzurufen, müssen Sie das Cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) aus dem [Partner Center PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/)-Modul verwenden.

## <a name="how-the-requirements-are-enforced"></a>Vorgehensweise beim Erzwingen der Anforderungen

Sicherheitsanforderungen für Partner werden von Azure AD und im Gegenzug vom Partner Center erzwungen, indem geprüft wird, ob der MFA-Anspruch vorhanden ist, und so festzustellen, ob die MFA-Überprüfung durchgeführt wurde. Seit dem 18. November 2019 hat Microsoft zusätzliche Sicherheitsvorkehrungen (früher als „technische Erzwingung“ bezeichnet) für Partnermandanten aktiviert.

Nach der Aktivierung werden Benutzer im Partnermandanten aufgefordert, die MFA-Überprüfung abzuschließen, wenn sie AOBO-Vorgänge (Admin-on-Behalf-Of, Administrator im Auftrag von) ausführen, auf das Partner Center-Portal zugreifen oder Partner Center-APIs aufrufen. Weitere Informationen finden Sie unter [Festlegen von Multi-Factor Authentication (MFA) für Ihren Partnermandanten](partner-security-requirements-mandating-mfa.md). 

Partner, die die Anforderungen nicht erfüllen, sollten diese Maßnahmen schnellstmöglich implementieren, um Geschäftsunterbrechungen zu vermeiden. Wenn du Azure Multi-Factor Authentication oder Azure AD-Sicherheitsstandards verwendest, musst du keine weiteren Maßnahmen ergreifen.

Wenn Sie eine MFA-Lösung eines Drittanbieters verwenden, besteht die Möglichkeit, dass der MFA-Anspruch nicht ausgegeben wird. Wenn dieser Anspruch fehlt, kann Azure AD nicht ermitteln, ob die Authentifizierungsanforderung durch MFA angefordert wurde. Informationen dazu, wie du überprüfst, ob deine Lösung den erwarteten Anspruch ausgibt, findest du unter [Testen der Sicherheitsanforderungen für Partner](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Wenn Ihre Drittanbieterlösung nicht den erwarteten Anspruch ausgibt, müssen Sie mit dem Hersteller zusammenarbeiten, der die Lösung entwickelt hat, um zu bestimmen, welche Maßnahmen ergriffen werden müssen.

## <a name="resources-and-samples"></a>Ressourcen und Beispiele

Unterstützung und Beispielcode finden Sie in den folgenden Ressourcen:

- [Partner Center Security Guidance Group-Community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Die Partner Center Security Guidance Group-Community ist eine Onlinecommunity, in der Sie sich über bevorstehende Veranstaltungen informieren und Fragen stellen können.
- [Partner Center – .NET-Beispiele](https://github.com/microsoft/partner-center-dotnet-samples): Dieses GitHub-Repository enthält Beispiele, die mit .NET entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center – Java-Beispiele](https://github.com/microsoft/partner-center-java-samples): Dieses GitHub-Repository enthält Beispiele, die mit Java entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center – Multi-Factor Authentication über PowerShell](/powershell/partnercenter/multi-factor-auth): In diesem Artikel zur Multi-Factor Authentication wird ausführlich erläutert, wie Sie das Framework für das sichere Anwendungsmodell mit PowerShell implementieren.

## <a name="next-steps"></a>Nächste Schritte

- [Festlegen von Multi-Factor Authentication (MFA) für Ihren Partnermandanten](partner-security-requirements-mandating-mfa.md)