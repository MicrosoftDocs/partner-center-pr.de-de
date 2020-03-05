---
title: Sicherheitsanforderungen für Partner | Partner Center
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Eine Einführung zur Aktivierung der mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA) und des Frameworks „Sicheres Anwendungsmodell“ – beides wird jetzt für Partner vorausgesetzt.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: high
ms.openlocfilehash: b0fe328008ae56272ddd8e22722071e5858881c8
ms.sourcegitcommit: 5379fbbe7fab1a26314c42bca40674c7f2faa432
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/27/2020
ms.locfileid: "77672800"
---
# <a name="partner-security-requirements"></a>Sicherheitsanforderungen für Partner

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direktrechnung
  - Indirekter Anbieter
  - Indirekter Wiederverkäufer
- Alle Control Panel-Anbieter
- Alle Berater

**Geeignete Benutzer**
-   Alle aktivierten Benutzer einschließlich Gastbenutzer

Mehr Sicherheitsmaßnahmen für den Datenschutz und eine höhere Sicherheit gehören zu unseren obersten Prioritäten. Wir wissen, dass die beste Verteidigung die Prävention ist und dass wir nur so stark sind wie unser schwächstes Glied. Deshalb müssen alle in unserem Partnerumfeld handeln und sicherstellen, dass sie über angemessene Sicherheitsvorkehrungen verfügen. Zum Schutz von Partnern und Kunden führen wir eine Reihe von verbindlichen Sicherheitsanforderungen für Berater, Control Panel-Anbieter und Partner ein, die am Cloud Solution Provider-Programm teilnehmen.

## <a name="overview"></a>Übersicht

Partner sind verpflichtet, die mehrstufige Authentifizierung für alle Benutzerkonten in ihrem Partnermandanten durchzusetzen. Die mit den Sicherheitsanforderungen für Partner verbundenen Bestimmungen wurden der Microsoft Partner-Vereinbarung hinzugefügt. In Bezug auf Berater gelten dieselben vertraglichen Anforderungen.

Partner, die die obligatorischen Sicherheitsanforderungen nicht implementieren, werden nicht in der Lage sein, im Cloud Solution Provider-Programm zu agieren oder Kundenmandanten mit delegierten Administratorrechten zu verwalten, sobald diese Anforderungen durchgesetzt sind. Wenn Partner die Sicherheitsanforderungen nicht implementieren, kann zudem ihre Teilnahme an Programmen gefährdet sein.  

Damit Partner und ihre Kunden geschützt sind, setzen wir voraus, dass Partner folgende Maßnahmen sofort umsetzen:  

1. **Aktivieren der Multi-Factor Authentication (MFA) für alle Benutzer in Partnermandanten**. Alle Benutzerkonten in Partnermandanten müssen die Multi-Factor Authentication (MFA) verwenden, wenn sie sich bei kommerziellen Microsoft-Clouddiensten anmelden oder im Cloud Solution Provider-Programm Transaktionen über das Partner Center oder APIs ausführen. 

2. **Übernehmen des Frameworks „Sicheres Anwendungsmodell“** . Übernehmen des Frameworks „Sicheres Anwendungsmodell“ Alle Partner, die eine Integration mit der Partner Center API durchführen, müssen das Framework „Sicheres Anwendungsmodell“ für alle Anwendungs- und Benutzerauthentifizierungsmodelle implementieren.

    > [!IMPORTANT]
    > Es wird dringend empfohlen, dass Partner das sichere Anwendungsmodell für die Integration mit einer Microsoft-API implementieren, z. B. Azure Resource Manager, Microsoft Graph oder Automatisierung wie PowerShell mithilfe von Benutzeranmeldeinformationen. So lassen sich Unterbrechungen während der Durchsetzung von MFA vermeiden.

Durch Aktivieren der Multi-Factor Authentication (MFA) und Übernehmen des Frameworks „Sicheres Anwendungsmodell“ kannst du deine Infrastruktur sowie die Daten deiner Kunden vor potenziellen Sicherheitsrisiken wie Identitätsdiebstahl oder anderen Betrugsversuchen schützen.  

## <a name="actions-that-you-need-to-take"></a>Maßnahmen, die Sie ergreifen müssen

Zur Einhaltung der Sicherheitsanforderungen für Partner musst du die mehrstufige Authentifizierung für jedes Benutzerkonto in deinem Partnermandanten erzwingen. Dies kann auf eine der folgenden Arten erreicht werden:

- Implementieren der [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

- Kauf von Azure Active Directory Premium für jedes Benutzerkonto. Weitere Informationen finden Sie unter [Planen einer cloudbasierten Azure Multi-Factor Authentication-Bereitstellung](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

- Verwendung einer Drittanbieterlösung zur Erzwingung der mehrstufigen Authentifizierung für jedes Benutzerkonto in Ihrem Partnermandanten. Weitere Details, um sicherzustellen, dass die Lösung die erwarteten Informationen bereitstellt, finden Sie unter [Vorgehensweise zum Erzwingen der Sicherheitsanforderungen](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Obwohl die mehrstufige Authentifizierung für eine Sovereign Cloud (21Vianet, US Government und Deutschland) vertraglich nicht verpflichtend ist, wird dringend empfohlen, diese Sicherheitsanforderungen umzusetzen.

## <a name="security-defaults"></a>Sicherheitsstandards

Die Richtlinie für Sicherheitsstandards ist eine der [Optionen](#actions-that-you-need-to-take), die Partner je nach ihren geschäftlichen Bedürfnissen für die Umsetzung von MFA gemäß ihren Sicherheitsanforderungen wählen können. Sie bietet eine grundlegende Sicherheitsstufe, die ohne Zusatzkosten bereitgestellt wird. Informiere dich, wie du MFA im Rahmen von Azure AD für dein Unternehmen aktivieren kannst. Lies darüber hinaus die folgenden wichtigen Informationen, bevor du die Sicherheitsstandards aktivierst.

- Die Baselinerichtlinien bleiben in den nächsten Monaten noch verfügbar, sollen aber Ende Februar 2020 außer Kraft gesetzt werden.

- Partner, die aktuell Baselinerichtlinien verwenden, müssen jetzt handeln und auf Sicherheitsstandards umstellen.

- Die nun allgemein verfügbaren Sicherheitsstandards ersetzen die Baselinerichtlinien aus der Vorschauversion. Nachdem ein Partner die Sicherheitsstandards aktiviert hat, kann er keine Baselinerichtlinien mehr aktivieren.

- Durch die Sicherheitsstandards werden alle Richtlinien in einem Schritt aktiviert. 

- Partner, die den [bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-policy-common) verwenden, [haben keinen Zugang zu Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Die Blockierung der Legacyauthentifizierung wird derzeit für Partner nicht erzwungen. Da die meisten Ereignisse in Zusammenhang mit Identitätsbetrug jedoch bei der Anmeldung über die Legacyauthentifizierung auftreten, sollten Partner besser auf diese älteren Protokolle verzichten.

- Das Azure AD Connect-Synchronisierungskonto ist von den Sicherheitsstandards ausgeschlossen.

- Ausführliche Informationen findest du unter [Aktivieren der mehrstufigen Authentifizierung für dein Unternehmen](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-get-started) und [Azure Active Directory-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Azure AD-Sicherheitsstandards sind die Weiterentwicklung der Baselineschutzrichtlinien in vereinfachter Form. Wenn du die Baselineschutzrichtlinien bereits aktiviert hast, wird dringend empfohlen, die Sicherheitsstandards zu aktivieren.

Informationen zum Umstieg von Baselinerichtlinien auf Sicherheitsstandards findest du unter [Was sind Sicherheitsstandards?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Überlegung

Da diese Anforderungen für alle Benutzerkonten in deinem Partnermandanten gelten, muss du mehrere Punkte berücksichtigen, um eine reibungslose Bereitstellung zu gewährleisten. Dazu zählen die Identifizierung von Benutzerkonten in Azure Active Directory, die die mehrstufige Authentifizierung nicht durchführen können, sowie der Anwendungen und Geräte, die von deinem Unternehmen verwendet werden und keine moderne Authentifizierung unterstützen.

Es wird empfohlen, sich vor der Durchführung von Aktionen folgende Frage zu stellen: 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Verfügen Sie über eine Anwendung oder ein Gerät, von der bzw. dem die Verwendung moderner Authentifizierung nicht unterstützt wird?

Wenn du die mehrstufige Authentifizierung erzwingst, werden Nutzungsprotokolle für die Legacyauthentifizierung wie IMAP, POP3, SMTP usw. blockiert, da mehrstufige Authentifizierung von diesen Protokollen nicht unterstützt wird. Um diese Einschränkung zu berücksichtigen, kann über ein Feature namens [App-Kennwörter](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) sichergestellt werden, dass die Authentifizierung für die Anwendung oder das Gerät weiterhin möglich ist. Sie sollten die Überlegungen zur Verwendung von App-Kennwörtern überprüfen, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um festzustellen, ob sie in Ihrer Umgebung verwendet werden können.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Verfügen Sie über Benutzer, die Office 365 über Lizenzen nutzen, die Ihrem Partnermandanten zugeordnet sind?

Vor der Implementierung einer beliebigen Lösung wird empfohlen, die Microsoft Office-Version zu ermitteln, die von Benutzern in deinem Partnermandanten verwendet wird. Überprüfen Sie den [Plan für die mehrstufige Authentifizierung für Office 365-Bereitstellungen](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa), bevor Sie Maßnahmen ergreifen. Es besteht die Möglichkeit, dass für Ihre Benutzer Verbindungsprobleme bei Anwendungen wie Outlook auftreten. Bevor Sie mehrstufige Authentifizierung erzwingen, sollten Sie sicherstellen, dass Outlook 2013 SP1 oder höher verwendet wird und Ihr Unternehmen über eine moderne Authentifizierung verfügt. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Sie müssen zwei Registrierungsschlüssel erstellen, um eine moderne Authentifizierung für alle Geräte unter Windows zu ermöglichen, auf denen Microsoft Office 2013 installiert ist. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Gibt es eine Richtlinie, die verhindert, dass Benutzer ihre mobilen Geräte während der Arbeit verwenden?

Es ist wichtig, jede Unternehmensrichtlinie zu identifizieren, die Mitarbeiter daran hindert, mobile Geräte während der Arbeit zu verwenden, da sich dies auf die mehrstufige Authentifizierungslösung auswirkt, die Sie implementieren. Es gibt Lösungen, wie die durch die Implementierung von [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) bereitgestellte Lösung, die nur die Verwendung einer Authenticator-App für die Überprüfung zulassen. Für den Fall, dass Ihr Unternehmen über eine Richtlinie verfügt, die die Verwendung von mobilen Geräten verhindert, sollten Sie eine der folgenden Optionen in Betracht ziehen

- Bereitstellen einer Anwendung mit zeitbasiertem Einmalkennwort (TOTP, Time-based One-time Password), die auf einem sicheren System ausgeführt werden kann

- Implementieren einer Lösung eines Drittanbieters, die mehrstufige Authentifizierung für jedes Benutzerkonto im Partnermandanten erzwingt, der die am besten geeignete Überprüfungsoption bietet

- Kauf von [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/)-Lizenzen für die betroffenen Benutzer

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Über welche Automatisierung oder Integration verfügen Sie, die die Benutzeranmeldeinformationen für die Authentifizierung nutzt?

Da es erforderlich ist, MFA für jeden Benutzer, einschließlich Dienstkonten, in Ihrem Partnerverzeichnis durchzusetzen, ist jede Automatisierung oder Integration, die Benutzeranmeldeinformationen für die Authentifizierung nutzt, betroffen. Daher ist es wichtig, dass Sie feststellen, welche Konten in diesen Situationen verwendet werden. Im Folgenden finden Sie eine Liste von Beispielen für Anwendungen oder Dienste, die berücksichtigt werden sollten.

- Systemsteuerung, die für die Bereitstellung von Ressourcen im Namen Ihrer Kunden verwendet wird 

- Integration mit jeder Plattform, die für die Fakturierung (in Bezug auf das CSP-Programm) und Unterstützung Ihrer Kunden verwendet wird

- PowerShell-Skripts, die die Module Az, AzureRM, Azure AD, MS Online, usw. verwenden

Die obige Liste ist nicht vollständig. Daher ist es wichtig, dass Sie eine vollständige Bewertung aller Anwendungen oder Dienste in Ihrer Umgebung durchführen, die Benutzeranmeldeinformationen für die Authentifizierung nutzen. Um die Anforderung für mehrstufige Authentifizierung zu erfüllen, sollten Sie nach Möglichkeit die Anweisungen im [Framework für das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) implementieren.

## <a name="accessing-your-environment"></a>Zugriff auf Ihre Umgebung

Um besser zu verstehen, was oder wer die Authentifizierung vornimmt, ohne zur mehrstufigen Authentifizierung aufgefordert zu werden, wird die Überprüfung der Anmeldeaktivitäten empfohlen. Über Azure Active Directory Premium kannst du den Anmeldebericht nutzen. Weitere Informationen finden Sie unter [Berichte zu Anmeldeaktivitäten im Azure Active Directory-Portal](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins). Wenn du nicht über Azure Active Directory Premium verfügst oder nach einer Möglichkeit suchst, diese Aufgabe über PowerShell zu erledigen, musst du das Cmdlet [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) aus dem Modul [Partner Center PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) verwenden.

## <a name="how-the-requirements-will-be-enforced"></a>Vorgehensweise beim Erzwingen der Anforderungen

Die Sicherheitsanforderungen für Partner werden von Azure Active Directory und im Gegenzug vom Partner Center erzwungen, indem geprüft wird, ob der MFA-Anspruch vorhanden ist, um so zu ermitteln, ob die mehrstufige Authentifizierung durchgeführt wurde. Ab dem 18. November 2019 aktiviert Microsoft zusätzliche Sicherheitsvorkehrungen (früher als „technische Erzwingung“ bezeichnet) für Partnermandanten. 

Nach der Aktivierung werden Benutzer im Partnermandanten aufgefordert, die Überprüfung der Multi-Factor Authentication (MFA) abzuschließen, wenn sie Administratoraufgaben im Auftrag von (AOBO-)Vorgängen ausführen. Wir werden die Sicherheitsmaßnahmen auf weitere Szenarien und Benutzerrollen ausweiten und unsere Partner vorab darüber informieren. Weitere Informationen findest du in diesem Dokument, das wir in kurzen Abständen aktualisieren. Partner, die die Anforderungen nicht erfüllen, sollten diese Maßnahmen schnellstmöglich implementieren, um Geschäftsunterbrechungen zu vermeiden. 

Wenn du Azure Multi-Factor Authentication oder Azure AD-Sicherheitsstandards verwendest, musst du keine weiteren Maßnahmen ergreifen.

Wenn Sie die mehrstufige Authentifizierungslösung eines Drittanbieters verwenden, besteht die Möglichkeit, dass der MFA-Anspruch nicht ausgegeben wird. Wenn dieser Anspruch fehlt, kann Azure Active Directory nicht ermitteln, ob die Authentifizierungsanforderung durch die mehrstufige Authentifizierung angefordert wurde. Informationen dazu, wie du überprüfst, ob deine Lösung den erwarteten Anspruch ausgibt, findest du unter [Testen der Sicherheitsanforderungen für Partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Wenn Ihre Drittanbieterlösung nicht den erwarteten Anspruch ausgibt, müssen Sie mit dem Hersteller zusammenarbeiten, der die Lösung entwickelt hat, um zu bestimmen, welche Maßnahmen ergriffen werden müssen.

## <a name="resources-and-support"></a>Ressourcen und Support

Im Folgenden findest du Ressourcen, über die du Support und Beispielcode erhältst:

- [Partner Center Security Guidance-Gruppe – Community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Dies ist eine Online-Community, in der Sie sich über bevorstehende Veranstaltungen informieren und Fragen stellen können.
- [Partner Center .NET-Beispiele](https://github.com/microsoft/partner-center-dotnet-samples): Dieses GitHub-Repository enthält Beispiele, die mit .NET entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center Java-Beispiele](https://github.com/microsoft/partner-center-java-samples): Dieses GitHub-Repository enthält Beispiele, die mit Java entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center PowerShell – Mehrstufige Authentifizierung](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth): Dies ist ein Artikel, der Details zur Implementierung des Frameworks für das sichere Anwendungsmodell mit PowerShell enthält.
