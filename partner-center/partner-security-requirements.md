---
title: Sicherheitsanforderungen für Partner | Partner Center
ms.topic: article
ms.date: 08/05/2019
description: Erfahren Sie mehr über die Sicherheitsanforderungen für Berater und Partner, die am Cloud Solution Provider-Programm teilnehmen.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: medium
ms.openlocfilehash: 40f5ac3e1481c0b630fc7e22e680409b1ca80926
ms.sourcegitcommit: a5d5bd83e20649e9f02d2d82d682f87bb28a0265
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/09/2019
ms.locfileid: "68912625"
---
# <a name="partner-security-requirements"></a>Sicherheitsanforderungen für Partner

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direktrechnung
  - Indirekter Anbieter
  - Indirekter Wiederverkäufer
- Alle Control Panel-Anbieter
- Alle Berater

Mehr Sicherheitsmaßnahmen für den Datenschutz und eine höhere Sicherheit gehören zu unseren obersten Prioritäten. Wir wissen, dass die beste Verteidigung die Prävention ist und dass wir nur so stark sind wie unser schwächstes Glied. Deshalb müssen alle in unserem Ökosystem handeln und sicherstellen, dass sie über angemessene Sicherheitsvorkehrungen verfügen. Zum Schutz von Partnern und Kunden führen wir eine Reihe von verbindlichen Sicherheitsanforderungen für Berater, Control Panel-Anbieter und Partner ein, die am Cloud Solution Provider-Programm teilnehmen.

Seit dem 1. August 2019 sind alle Partner verpflichtet, die mehrstufige Authentifizierung für alle Benutzer, einschließlich Dienstkonten, in ihrem Partnermandanten durchzusetzen.

> [!NOTE]
> Es wird dringend empfohlen, dass alle Partner, die über eine unabhängige Cloud (21Vianet, US-Regierung und Deutschland) handeln, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner sind jedoch nicht verpflichtet, die neuen Sicherheitsanforderungen zum 1. August 2019 zu erfüllen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

Die mit den Sicherheitsanforderungen für Partner verbundenen Begriffe wurden dem [Programmleitfaden für Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100) hinzugefügt. Ab dem 1. August 2019 sollten alle am Cloud Solution Provider-Programm teilnehmenden Partner die Bedingungen erfüllen. In Bezug auf Berater gelten dieselben vertraglichen Anforderungen.

Partner, die die obligatorischen Sicherheitsanforderungen nicht implementieren, werden nicht in der Lage sein, im Cloud Solution Provider-Programm zu agieren oder Kundenmandanten mit delegierten Administratorrechten zu verwalten, sobald diese Anforderungen durchgesetzt sind. Wir sind dabei, einen Termin für die technische Durchsetzung der Anforderungen festzulegen und werden die Partner mit detaillierten Informationen zu diesem Termin benachrichtigen.

## <a name="what-actions-do-i-need-to-take"></a>Welche Maßnahmen muss ich ergreifen?

Angesichts der privilegierten Natur der Partner müssen wir sicherstellen, dass jeder Benutzer für jede einzelne Authentifizierung über eine MFA-Herausforderung verfügt. Dies kann auf eine der folgenden Arten erreicht werden:

- Implementieren von Azure AD Premium und Sicherstellen, dass MFA für jeden Benutzer erzwungen wird
- Implementieren der [grundlegenden Schutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementieren der Lösung eines Drittanbieters und Sicherstellen, dass MFA für jeden Benutzer erzwungen wird

> [!IMPORTANT]
> Sobald diese Anforderungen technisch durchgesetzt sind, muss jede einzelne Authentifizierung über eine MFA-Abfrage verfügen. Sie können keine Features für den bedingten Zugriff verwenden, um die Authentifizierung mit MFA beim Zugriff auf kommerzielle Clouddienste von Microsoft zu vermeiden.

### <a name="considerations"></a>Überlegungen

Da diese Anforderungen für alle Benutzer in Ihrem Partnermandanten gelten, einschließlich Dienstkonten, müssen mehrere Überlegungen angestellt werden, um eine reibungslose Bereitstellung sicherzustellen. Diese Überlegungen umfassen die Identifizierung von Benutzern in Azure AD, die keine MFA durchführen können, sowie die Identifizierung von Anwendungen und Geräten, die von Ihrem Unternehmen verwendet werden und keine moderne Authentifizierung unterstützen.

Es wird empfohlen, dass Sie vor der Durchführung von Aktionen Folgendes erkennen:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Verfügen Sie über eine Anwendung oder ein Gerät, von der bzw. dem die Verwendung von MFA bei der Authentifizierung nicht unterstützt wird?

Wenn Sie die MFA-Legacy-Authentifizierung erzwingen, werden Nutzungsprotokolle wie IMAP, POP3, SMTP usw. blockiert, da MFA von diesen Protokollen nicht unterstützt wird. Um diese Einschränkung zu berücksichtigen, kann ein Feature namens [App-Kennwörter](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) verwendet werden, um sicherzustellen, dass die Authentifizierung für die Anwendung oder das Gerät noch möglich ist. Sie sollten die Überlegungen zur Verwendung von App-Kennwörtern überprüfen, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um festzustellen, ob sie in Ihrer Umgebung verwendet werden können.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Verfügen Sie über Benutzer, die Office 365 über Lizenzen nutzen, die Ihrem Partnermandanten zugeordnet sind?

Vor der Implementierung einer Lösung wird empfohlen, dass Sie feststellen, warum die Version von Microsoft Office von Benutzern in Ihrem Partnermandanten verwendet wird. Überprüfen Sie den [Plan für die mehrstufige Authentifizierung für Office 365-Bereitstellungen](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa), bevor Sie Maßnahmen ergreifen. Es besteht die Möglichkeit, dass für Ihre Benutzer Verbindungsprobleme bei Anwendungen wie Outlook auftreten. Bevor Sie MFA erzwingen, sollten Sie sicherstellen, dass Outlook 2013 SP1 oder höher verwendet wird und Ihr Unternehmen über eine moderne Authentifizierung verfügt. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Sie müssen zwei Registrierungsschlüssel erstellen, um eine moderne Authentifizierung für alle Geräte unter Windows zu ermöglichen, auf denen Microsoft Office 2013 installiert ist. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

> [!IMPORTANT]
> Wenn Sie Ihre Benutzer für Azure AD MFA aktiviert haben und sie über Geräte mit Office 2013 verfügen, die für eine moderne Authentifizierung nicht aktiviert sind, müssen sie App-Kennwörter auf diesen Geräten verwenden. Weitere Informationen zu App-Kennwörtern und wann, wo und wie sie verwendet werden sollen, finden Sie hier: [App-Kennwörter mit Azure Multi-Factor Authentication](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Gibt es eine Richtlinie, die verhindert, dass Benutzer ihre mobilen Geräte während der Arbeit verwenden?

Es ist wichtig, jede Unternehmensrichtlinie zu identifizieren, die Mitarbeiter daran hindert, mobile Geräte während der Arbeit zu verwenden, da sich dies auf die MFA-Lösung auswirkt, die Sie implementieren. Es gibt MFA-Lösungen, wie die durch die Implementierung der [Baselineschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) bereitgestellte Lösung, die nur die Verwendung einer Authentifikator-App für die Überprüfung zulassen. Für den Fall, dass Ihr Unternehmen über eine Richtlinie verfügt, die die Verwendung von mobilen Geräten verhindert, sollten Sie eine der folgenden Optionen in Betracht ziehen

- Bereitstellen einer Anwendung mit zeitbasiertem Einmalkennwort (TOTP, Time-based One-time Password), die auf einem sicheren System ausgeführt werden kann
- Implementieren einer Lösung eines Drittanbieters, die MFA für jeden Benutzer im Partnermandanten erzwingt, der die am besten geeignete Überprüfungsoption bietet
- Erwerben von [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/)-Lizenzen für die betroffenen Benutzer

Die Unterstützung für die Verwendung von FIDO-Sicherheitsschlüsseln ist auf der Roadmap für die Baselineschutzrichtlinien enthalten. Nachdem die Unterstützung hinzugefügt wurde, können Sie die FIDO-Sicherheitsschlüssel für den zweiten Faktor der Authentifizierung nutzen. Bis dahin sind Sie auf die Verwendung der Authentifikator-App beschränkt.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Über welche Automatisierung oder Integration verfügen Sie, die die Benutzeranmeldeinformationen für die Authentifizierung nutzt?

Da es erforderlich ist, MFA für jeden Benutzer, einschließlich Dienstkonten, in Ihrem Partnerverzeichnis durchzusetzen, ist jede Automatisierung oder Integration, die Benutzeranmeldeinformationen für die Authentifizierung nutzt, betroffen. Daher ist es wichtig, dass Sie feststellen, welche Konten in diesen Situationen verwendet werden. Im Folgenden finden Sie eine Liste von Beispielen für Anwendungen oder Dienste, die berücksichtigt werden sollten.

- Systemsteuerung, die für die Bereitstellung von Ressourcen im Namen Ihrer Kunden verwendet wird
- Integration mit jeder Plattform, die für die Fakturierung (in Bezug auf das CSP-Programm) und Unterstützung Ihrer Kunden verwendet wird
- PowerShell-Skripts, die die Module Az, AzureRM, Azure AD, MS Online, usw. verwenden

Die obige Liste ist nicht vollständig. Daher ist es wichtig, dass Sie eine vollständige Bewertung aller Anwendungen oder Dienste in Ihrer Umgebung durchführen, die Benutzeranmeldeinformationen für die Authentifizierung nutzen. Um die Anforderung für MFA zu erfüllen, sollten Sie nach Möglichkeit die Anweisungen im [Framework für das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) implementieren. Im Folgenden finden Sie weitere Ressourcen, die Ihnen helfen zu verstehen, wie das Framework für das sichere Anwendungsmodell implementiert werden kann.

- [Partner Center .NET-Beispiele](https://github.com/microsoft/partner-center-dotnet-samples): Dieses GitHub-Repository enthält Beispiele, die mit .NET entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center Java-Beispiele](https://github.com/microsoft/partner-center-java-samples): Dieses GitHub-Repository enthält Beispiele, die mit Java entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center PowerShell – Sicheres Anwendungsmodell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model): Dies ist ein Artikel, der Details zur Implementierung des Frameworks für das sichere Anwendungsmodell mit PowerShell enthält.
- [Partner Center Security Guidance-Gruppe – Community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Dies ist eine Online-Community, in der Sie sich über bevorstehende Veranstaltungen informieren und Fragen stellen können.

### <a name="enforcing-mfa-for-all-users"></a>Erzwingen von MFA für alle Benutzer

In diesem Abschnitt wird erläutert, wie Sie die [Baselineschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) verwenden können, um MFA für jeden Benutzer, einschließlich Dienstkonten, in Ihrem Partnermandanten zu erzwingen. Wenn Sie die Verwendung von Azure AD Premium planen, folgen Sie den [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted) dokumentierten Schritten.

> [!NOTE]
> Es kann eine Lösung eines Drittanbieters, die mit Azure AD kompatibel ist, verwendet werden, um MFA für alle Benutzer, einschließlich der Dienstkonten, zu erzwingen. Weitere Informationen zur Implementierung der Lösung finden Sie in der Dokumentation des Anbieters.

Baselineschutzrichtlinien sind eine Reihe von vordefinierten Richtlinien, die dabei helfen, Unternehmen vor vielen allgemeinen Angriffen zu schützen. Diese allgemeinen Angriffe können Password Spray, Replay und Phishing einbeziehen. Die Baselineschutzrichtlinien sind in allen Editionen von Azure Active Directory verfügbar. Microsoft stellt diese Baselineschutzrichtlinien allen zur Verfügung, um Kunden und Partnern die Implementierung von erstklassigen Sicherheitsverfahren zu ermöglichen.

Die beiden Baselineschutzrichtlinien, die aktiviert werden sollten, sind in der folgenden Tabelle beschrieben.

|**Richtlinie**| |
|-----|-----|
|**MFA für Administratoren erfordern**|Wenn Sie die Richtlinie „MFA für Administratoren erfordern“ aktivieren, müssen sich Benutzer in den Administratorrollen über die Authentifikator-App für MFA registrieren. Nachdem die MFA-Registrierung abgeschlossen ist, müssen Administratoren MFA bei jeder Anmeldung durchführen.|
|**Endbenutzerschutz**|Der Endbenutzerschutz ist eine risikobasierte MFA-Baselineschutzrichtlinie, die alle Benutzer in einem Verzeichnis schützt. Wenn Sie diese Richtlinie aktivieren, müssen sich alle Benutzer über die Authentifikator-App für MFA registrieren. Benutzer können die MFA-Registrierungsaufforderung 14 Tage lang ignorieren. Danach wird ihnen die Anmeldung verwehrt, bis sie sich für MFA registriert haben. Nach der Registrierung für MFA werden die Benutzer nur noch während risikobehafteter Anmeldeversuche zur MFA aufgefordert. Kompromittierte Benutzerkonten werden gesperrt, bis ihr Kennwort zurückgesetzt und Risikoereignisse abgewiesen wurden.|

Wenn diese Richtlinien aktiviert sind, kann jeder Benutzer Azure MFA mit der Authentifikator-App ohne zusätzliche Kosten zur Überprüfung nutzen.

#### <a name="configure-self-service-password-reset"></a>Konfigurieren der Self-Service-Kennwortzurücksetzung

Die Self-Service-Kennwortzurücksetzung (Self-Service Password Reset, SSPR) ist ein Azure Active Directory-Feature, mit dem Benutzer ihre Kennwörter zurücksetzen können, ohne sich an das Supportteam wenden zu müssen. Benutzer müssen sich für die Self-Service-Kennwortzurücksetzung registrieren oder registriert sein, bevor sie den Dienst nutzen können. Während der Registrierung wählt der Benutzer eine oder mehrere Authentifizierungsmethoden aus, die von seinem Unternehmen aktiviert wurden.

Wenn die Baselineschutzrichtlinie für den [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) aktiviert ist, werden alle kompromittierten Benutzerkonten gesperrt, bis ihr Kennwort zurückgesetzt und die Risikoereignisse zurückgewiesen wurden. Daher wird empfohlen, dass jeder Benutzer, der ein globaler Administrator ist, die folgenden Schritte durchführt, um sich für SSPR zu registrieren, damit er nicht gesperrt wird.

1. Navigieren Sie zur Seite für das [SSPR-Setup](https://aka.ms/ssprsetup).
2. Geben Sie Ihren Benutzernamen und Ihr Kennwort ein.
3. Konfigurieren Sie mindestens eine der Überprüfungsoptionen, mit denen überprüft wird, wer Sie sind, wenn Sie Ihr Kennwort zurücksetzen.  

Wenn ein Konto kompromittiert wurde, muss ein Administrator Maßnahmen ergreifen, um den Zugriff für den betroffenen Benutzer wiederherzustellen. Weitere Informationen zum Entsperren des Benutzers finden Sie unter den Schritten zum [Entsperren eines Benutzers](#recovering-compromised-accounts).

#### <a name="require-mfa-for-admins"></a>MFA für Administratoren erfordern

Die Baselineschutzrichtlinie *MFA für Administratoren erfordern* erfordert MFA für die folgenden Verzeichnisrollen, die als die Azure Active Directory-Rollen mit den höchsten Berechtigungen betrachtet werden:

- Globaler Administrator
- SharePoint-Administrator
- Exchange-Administrator
- Administrator für bedingten Zugriff
- Sicherheitsadministrator
- Helpdeskadministrator/Kennwortadministrator
- Rechnungsadministrator
- Benutzeradministrator

Beim Aktivieren der Richtlinie „MFA für Administratoren erfordern“ sind die obigen neun Administratorrollen für die Registrierung über die Authentifikator-App für MFA erforderlich. Nachdem die MFA-Registrierung abgeschlossen ist, müssen Administratoren bei jeder Anmeldung eine MFA durchführen.

Wenn diese Konten in Ihrem Unternehmen in Skripts oder Code verwendet werden, sollten Sie sie durch [verwaltete Identitäten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) ersetzen.

So aktivieren Sie diese Richtlinie und schützen Ihre Administratoren

1. Melden Sie sich beim  **Azure-Portal** als globaler Administrator, Sicherheitsadministrator oder Administrator für bedingten Zugriff an.
2. Navigieren Sie zu **Azure Active Directory** > **Bedingter Zugriff**.
3. Wählen Sie in der Liste der Richtlinien die Option **Baselinerichtlinie: MFA für Administratoren erfordern** aus.
4. Legen Sie **Richtlinie aktivieren** auf **Richtline sofort verwenden** fest.
5. Klicken Sie auf  **Speichern**.

> [!WARNING]
> Bevor Sie diese Richtlinie aktivieren, stellen Sie sicher, dass Ihre Benutzer keine Legacy-Authentifizierungsprotokolle verwenden. Durch die Implementierung dieser Richtlinie wird die Legacy-Authentifizierung blockiert.

> [!IMPORTANT]
> Es gibt ein bekanntes Problem, das sich auf Ihre Fähigkeit auswirkt, eine Verbindung mit Exchange Online PowerShell über delegierte Administratorrechte herzustellen. Wenn Sie dieses PowerShell-Modul verwenden, finden Sie weitere Informationen unter dem bekannten [Exchange Online PowerShell](#exchange-online-powershell)-Problem, bevor Sie diese Richtlinie aktivieren.

#### <a name="end-user-protection"></a>Endbenutzerschutz

Die Baselinerichtlinie für den Endbenutzerschutz schützt alle Benutzer in einem Verzeichnis. Wenn Sie diese Richtlinie aktivieren, müssen sich alle Benutzer innerhalb von 14 Tagen für Azure MFA registrieren. Nach der Registrierung werden die Benutzer nur noch während risikobehafteter Anmeldeversuche zur MFA aufgefordert. Kompromittierte Benutzerkonten werden bis zum Zurücksetzen des Kennworts gesperrt und riskieren eine Ablehnung.

Die Richtlinie **Baselinerichtlinie: Endbenutzerschutz** ist vorkonfiguriert und wird am Anfang angezeigt, wenn Sie zum Blatt „Bedingter Zugriff“ im Azure-Portal navigieren.

So aktivieren Sie diese Richtlinie und schützen Ihre Benutzer

1. Melden Sie sich beim  **Azure-Portal** als globaler Administrator, Sicherheitsadministrator oder Administrator für bedingten Zugriff an.
2. Navigieren Sie zu **Azure Active Directory** > **Bedingter Zugriff**.
3. Wählen Sie in der Liste der Richtlinien die Option **Baselinerichtlinie: Endbenutzerschutz (Vorschau)** aus.
4. Legen Sie **Richtlinie aktivieren** auf **Richtline sofort verwenden** fest.
5. Klicken Sie auf  **Speichern**.

> [!WARNING]
> Bevor Sie diese Richtlinie aktivieren, stellen Sie sicher, dass Ihre Benutzer keine Legacy-Authentifizierungsprotokolle verwenden. Durch die Implementierung dieser Richtlinie wird die Legacy-Authentifizierung blockiert.

> [!IMPORTANT]
> Es gibt ein bekanntes Problem, das sich auf Ihre Fähigkeit auswirkt, eine Verbindung mit Exchange Online PowerShell über delegierte Administratorrechte herzustellen. Wenn Sie dieses PowerShell-Modul verwenden, finden Sie weitere Informationen unter dem bekannten [Exchange Online PowerShell](#exchange-online-powershell)-Problem, bevor Sie diese Richtlinie aktivieren.

## <a name="assessing-your-environment"></a>Bewerten der Umgebung

Durch eine der aktuellen Sicherheitsanforderungen des Partners müssen Sie MFA für jeden Benutzer in Ihrem Partnermandanten erzwingen lassen. Da diese Anforderung durch eine Reihe von verschiedenen Methoden erfüllt werden kann, ist es möglicherweise schwierig zu beurteilen, ob zusätzliche Maßnahmen erforderlich sind. Sie können Tools wie die Azure Active Directory-Überwachungsprotokolle und [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score) nutzen, um zu bewerten, ob zusätzliche Maßnahmen erforderlich sind, um Ihren Mandanten durch MFA zu schützen. Microsoft arbeitet an einer Umgebung im Partner Center, um eine schnelle Konformitätsprüfung der MFA und der Anforderungen des sicheren Anwendungsmodells zu ermöglichen.

Microsoft Secure Score bietet Ihnen zuverlässige Visualisierungen, Integration mit anderen Microsoft-Produkten, Vergleich Ihrer Ergebnisse mit anderen Unternehmen, Filterung nach Kategorien und vieles mehr. Mit diesem Tool können Sie Maßnahmen zur Verbesserung der Sicherheit in Ihrem Unternehmen durchführen und den Verlauf Ihrer Bewertung verfolgen. Die Bewertung kann auch widerspiegeln, wenn Lösungen von Drittanbietern empfohlene Verbesserungsaktionen behandelt haben.

![Microsoft Secure Score](images/security/secure-score.png)

> [!NOTE]
> Maßnahmen, die Sie ergreifen können, um Ihr Microsoft Secure Score zu verbessern, können bis zu 24 Stunden dauern, bis sie berücksichtigt werden.

Microsoft Secure Score liefert nur eine numerische Darstellung Ihrer Sicherheitslage. Um besser zu verstehen, was oder wer die Authentifizierung vornimmt, ohne zur MFA aufgefordert zu werden, wird empfohlen, die Überwachungsprotokolle von Azure Active Directory abzufragen. Dies kann mit dem [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview)-Modul und dem folgenden Skript erreicht werden. Es generiert einen Bericht, der Aufschluss darüber gibt, welche Authentifizierungsversuche in den letzten Tagen stattgefunden haben, die nicht zur MFA aufgefordert wurden.

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Nach dem Ausführen des obigen Skripts sind die Details in der Datei „report.csv“ verfügbar. Es enthält eine Liste der Authentifizierungsversuche, die am letzten Tag stattgefunden haben, an dem der Benutzer nicht zur MFA aufgefordert wurde. Sie müssen jeden Eintrag überprüfen, um festzustellen, ob dies das erwartete Verhalten ist, und gegebenenfalls entsprechend handeln.

![Bewertungsbericht](images/security/assessment-report.png)

## <a name="common-issues"></a>Allgemeine Probleme

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Nachdem Sie die Baselinerichtlinien aktiviert haben, werden Sie möglicherweise feststellen, dass bei Ihrer Automatisierung oder Integration eine Ausnahme wie die folgende auftritt.

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Der Grund für diese Ausnahme ist, dass Sie sich mit Benutzeranmeldeinformationen authentifizieren und jetzt MFA erforderlich ist. Sie müssen ein Zugriffstoken für die Authentifizierung verwenden, um diese Ausnahme zu behandeln. Weitere Informationen finden Sie im [Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

>[!IMPORTANT]
>Die meisten modernen APIs und PowerShell-Module unterstützen die Möglichkeit, ein Zugriffstoken zur Authentifizierung zu verwenden. Allerdings wird diese Funktionalität derzeit von einigen nicht unterstützt. Wenn Sie Hilfe bei der Ermittlung benötigen, ob die API oder das PowerShell-Modul, die bzw. das Sie zu nutzen versuchen, die Verwendung eines Zugriffstokens für die Authentifizierung unterstützt, posten Sie eine Nachricht in der Community der [Partner Center Security Guidance-Gruppe](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

#### <a name="aadsts700082"></a>AADSTS700082

Nachdem Sie das Framework für das sichere Anwendungsmodell implementiert haben, besteht die Möglichkeit, dass Sie 90 Tage nach dem Generieren des ersten Aktualisierungstokens die folgende Ausnahme erhalten.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

In Bezug auf Azure Active Directory beträgt die maximale Lebensdauer für einen Aktualisierungstoken 90 Tage. Sie müssen ein neues Aktualisierungstoken generieren und sicher speichern, um diesen Fehler zu beheben. Beachten Sie, dass es möglich ist, das Aktualisierungstoken programmgesteuert zu aktualisieren, da bei jeder Anforderung an Azure Active Directory für ein Zugriffstoken ein neues Aktualisierungstoken zurückgegeben wird. Sie können die entsprechende Logik implementieren, um das sicher gespeicherte Aktualisierungstoken zu aktualisieren, bevor es abläuft.

Weitere Informationen finden Sie unter [Konfigurierbare Lebensdauer von Token in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

### <a name="recovering-compromised-accounts"></a>Wiederherstellen von kompromittierten Konten

Um unsere Kunden zu schützen, findet der Microsoft-Dienst für durchgesickerte Anmeldeinformationen öffentlich zugängliche Benutzername-Kennwort-Paare. Wenn sie mit einem unserer Benutzer übereinstimmen, helfen wir Ihnen, dieses Konto sofort zu schützen. Benutzer, für die bestätigt wurde, dass ihre Anmeldeinformationen durchgesichert sind, gelten als kompromittiert. Diese Benutzer werden für die Anmeldung gesperrt, bis ihr Kennwort zurückgesetzt wurde.

Benutzer, denen eine Azure AD Premium-Lizenz zugewiesen wurde, können den Zugriff durch Self-Service-Kennwortzurücksetzung (SSPR) wiederherstellen, wenn die Funktion in ihrem Verzeichnis aktiviert ist. Benutzer ohne Premium-Lizenz, die blockiert werden, müssen sich an einen Administrator wenden, um eine manuelle Kennwortzurücksetzung durchzuführen und das gekennzeichnete Benutzerrisikoereignis zu verwerfen.

#### <a name="steps-to-unblock-a-user"></a>Schritte zum Entsperren eines Benutzers

Bestätigen Sie, dass der Benutzer durch die Richtlinie blockiert wurde, indem Sie die Anmeldeprotokolle des Benutzers überprüfen.

1. Ein Administrator muss sich beim **Azure-Portal** anmelden und zu **Azure Active Directory** > **Benutzer** navigieren. Anschließend muss er auf den Namen des Benutzers klicken und zu den Anmeldungen navigieren.
2. Um das Zurücksetzen des Kennworts für einen blockierten Benutzer einzuleiten, muss ein Administrator zu **Azure Active Directory** > **Als Risiko gekennzeichnete Benutzer** navigieren.
3. Klicken Sie auf den Benutzer, dessen Konto blockiert ist, um Informationen zur letzten Anmeldeaktivität des Benutzers anzuzeigen.
4. Klicken Sie auf „Kennwort zurücksetzen“, um ein temporäres Kennwort zuzuweisen, das bei der nächsten Anmeldung geändert werden muss.
5. Klicken Sie auf „Alle Ereignisse verwerfen“, um die Risikobewertung des Benutzers zurückzusetzen.

Der Benutzer kann sich jetzt anmelden, sein Kennwort zurücksetzen und auf die Anwendung zugreifen.

## <a name="known-issues"></a>Bekannte Probleme

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Wenn MFA erzwungen wird, können Partner ihre delegierten Administratorrechte mit Exchange Online PowerShell nicht nutzen, um Aktionen für ihre Kunden durchzuführen. Weitere Informationen zu dieser Einschränkung finden Sie unter [Herstellen einer Verbindung mit Exchange Online PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).

Sie können diese Einschränkung umgehen, indem Sie ein neues Konto erstellen und es niemals zur Durchführung einer interaktiven Authentifizierung verwenden. Es wird empfohlen, [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) zu verwenden, um das neue Konto zu erstellen und die erste Konfiguration durchzuführen. Mithilfe der folgenden PowerShell-Befehle können Sie das Konto erstellen und konfigurieren:

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

Wenn Sie sich das nächste Mal über PowerShell eine Verbindung mit Exchange Online über dieses Konto herstellen, funktioniert es wie erwartet.

> [!IMPORTANT]
> Die Möglichkeit für Partner, ihre delegierten Administratorrechte mit Exchange Online PowerShell zu nutzen, um Aktionen für ihre Kunden bei erzwungener MFA durchzuführen, wird in Zukunft verfügbar sein. Bis dahin sollten Sie diese Problemumgehung nutzen.

## <a name="resources-and-support"></a>Ressourcen und Support

Über die Community für die [Partner Center Security Guidance-Gruppe](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) können Sie zusätzliche Ressourcen finden und sich über anstehende Veranstaltungen wie technische Geschäftszeiten informieren. Weitere Informationen zu den Anforderungen finden Sie im Dokument [Häufig gestellte Fragen](partner-security-requirements-faq.md).
