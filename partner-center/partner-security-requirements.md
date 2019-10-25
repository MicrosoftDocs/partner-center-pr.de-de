---
title: Sicherheitsanforderungen für Partner | Partner Center
ms.topic: article
ms.date: 10/11/2019
description: Erfahren Sie mehr über die Sicherheitsanforderungen für Berater und Partner, die am Cloud Solution Provider-Programm teilnehmen.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: high
ms.openlocfilehash: b09588387d3b4f0f3f726a700245999c89755199
ms.sourcegitcommit: 9dd6f1ee0ebc132442126340c9df8cf7e3e1d3ad
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/16/2019
ms.locfileid: "72425203"
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

## <a name="overview"></a>Übersicht

Seit dem 1. August 2019 sind alle Partner verpflichtet, die mehrstufige Authentifizierung für alle Benutzer in ihrem Partnermandanten durchzusetzen. Die mit den Sicherheitsanforderungen für Partner verbundenen Begriffe wurden dem [Programmleitfaden für Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100) hinzugefügt. In Bezug auf Berater gelten dieselben vertraglichen Anforderungen.

> [!NOTE]
> Es wird dringend empfohlen, dass alle Partner, die über eine unabhängige Cloud (21Vianet, US-Regierung und Deutschland) handeln, diese Sicherheitsanforderungen sofort umsetzen. Diese Partner sind jedoch nicht verpflichtet, die Sicherheitsanforderungen zum 1. August 2019 zu erfüllen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

Partner, die die obligatorischen Sicherheitsanforderungen nicht implementieren, werden nicht in der Lage sein, im Cloud Solution Provider-Programm zu agieren oder Kundenmandanten mit delegierten Administratorrechten zu verwalten, sobald diese Anforderungen durchgesetzt sind.

## <a name="actions-that-you-need-to-take"></a>Maßnahmen, die Sie ergreifen müssen

Zur Einhaltung der Sicherheitsanforderungen für Partner müssen Sie die mehrstufige Authentifizierung für jedes Benutzerkonto in Ihrem Partnermandanten erzwingen. Dies kann auf eine der folgenden Arten erreicht werden:

- Implementierung der Basisschutzrichtlinien [MFA für Administratoren erforderlich](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) aus Azure Active Directory ohne zusätzliche Kosten.
- Kauf von Azure Active Directory Premium für jedes Benutzerkonto. Weitere Informationen finden Sie unter [Planen einer cloudbasierten Azure Multi-Factor Authentication-Bereitstellung](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).
- Verwendung einer Drittanbieterlösung zur Erzwingung der mehrstufigen Authentifizierung für jedes Benutzerkonto in Ihrem Partnermandanten. Weitere Details, um sicherzustellen, dass die Lösung die erwarteten Informationen bereitstellt, finden Sie unter [Vorgehensweise zum Erzwingen der Sicherheitsanforderungen](#how-the-requirements-will-be-enforced).

### <a name="consideration"></a>Überlegung

Da diese Anforderungen für alle Benutzer in Ihrem Partnermandanten gelten müssen mehrere Überlegungen angestellt werden, um eine reibungslose Bereitstellung sicherzustellen. Diese Überlegungen umfassen die Identifizierung von Benutzerkonten in Azure Active Directory, die keine mehrstufige Authentifizierung durchführen können, sowie die Identifizierung von Anwendungen und Geräten, die von Ihrem Unternehmen verwendet werden und keine moderne Authentifizierung unterstützen.

Es wird empfohlen, dass Sie vor der Durchführung von Aktionen Folgendes erkennen:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Verfügen Sie über eine Anwendung oder ein Gerät, von der bzw. dem die Verwendung moderner Authentifizierung nicht unterstützt wird?

Wenn Sie die mehrstufige Legacy-Authentifizierung erzwingen, werden Nutzungsprotokolle wie IMAP, POP3, SMTP usw. blockiert, da mehrstufige Authentifizierung von diesen Protokollen nicht unterstützt wird. Um diese Einschränkung zu berücksichtigen, kann ein Feature namens [App-Kennwörter](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) verwendet werden, um sicherzustellen, dass die Authentifizierung für die Anwendung oder das Gerät noch möglich ist. Sie sollten die Überlegungen zur Verwendung von App-Kennwörtern überprüfen, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um festzustellen, ob sie in Ihrer Umgebung verwendet werden können.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Verfügen Sie über Benutzer, die Office 365 über Lizenzen nutzen, die Ihrem Partnermandanten zugeordnet sind?

Vor der Implementierung einer Lösung wird empfohlen, dass Sie feststellen, welche Version von Microsoft Office von Benutzern in Ihrem Partnermandanten verwendet wird. Überprüfen Sie den [Plan für die mehrstufige Authentifizierung für Office 365-Bereitstellungen](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa), bevor Sie Maßnahmen ergreifen. Es besteht die Möglichkeit, dass für Ihre Benutzer Verbindungsprobleme bei Anwendungen wie Outlook auftreten. Bevor Sie mehrstufige Authentifizierung erzwingen, sollten Sie sicherstellen, dass Outlook 2013 SP1 oder höher verwendet wird und Ihr Unternehmen über eine moderne Authentifizierung verfügt. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Sie müssen zwei Registrierungsschlüssel erstellen, um eine moderne Authentifizierung für alle Geräte unter Windows zu ermöglichen, auf denen Microsoft Office 2013 installiert ist. Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Gibt es eine Richtlinie, die verhindert, dass Benutzer ihre mobilen Geräte während der Arbeit verwenden?

Es ist wichtig, jede Unternehmensrichtlinie zu identifizieren, die Mitarbeiter daran hindert, mobile Geräte während der Arbeit zu verwenden, da sich dies auf die mehrstufige Authentifizierungslösung auswirkt, die Sie implementieren. Es gibt Lösungen, wie die durch die Implementierung von [Baselineschutzrichtlinien](/azure/active-directory/conditional-access/concept-baseline-protection) bereitgestellte Lösung, die nur die Verwendung einer Authentifikator-App für die Überprüfung zulassen. Für den Fall, dass Ihr Unternehmen über eine Richtlinie verfügt, die die Verwendung von mobilen Geräten verhindert, sollten Sie eine der folgenden Optionen in Betracht ziehen

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

Um besser zu verstehen, was oder wer die Authentifizierung vornimmt, ohne zur mehrstufigen Authentifizierung aufgefordert zu werden, wird empfohlen, die Überwachungsprotokolle von Azure Active Directory abzufragen. Dies kann mit dem [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview)-Modul und dem folgenden Skript erreicht werden. Es generiert einen Bericht, der Aufschluss darüber gibt, welche Authentifizierungsversuche in den letzten Tagen stattgefunden haben, die nicht zur mehrstufigen Authentifizierung aufgefordert wurden.

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

$report | Where-Object {$_.mfaRequired -eq $false -and $_.loginSucceeded -eq $true} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Nach dem Ausführen des obigen Skripts sind die Details in der Datei „report.csv“ verfügbar. Es enthält eine Liste der Authentifizierungsversuche, die am letzten Tag stattgefunden haben, an dem der Benutzer nicht zur MFA aufgefordert wurde. Sie müssen jeden Eintrag überprüfen, um festzustellen, ob dies das erwartete Verhalten ist, und gegebenenfalls entsprechend handeln.

![Bewertungsbericht](images/security/assessment-report.png)

## <a name="how-the-requirements-will-be-enforced"></a>Vorgehensweise beim Erzwingen der Anforderungen

Die Sicherheitsanforderungen für Partner werden von Azure Active Directory und im Gegenzug vom Partner Center erzwungen, indem geprüft wird, ob der MFA-Anspruch vorhanden ist, um so zu ermitteln, ob die mehrstufige Authentifizierung durchgeführt wurde. Wenn Sie Azure Multi-Factor Authentication oder die Baselineschutzrichtlinien verwenden, müssen Sie keine weiteren Maßnahmen ergreifen.

Wenn Sie die mehrstufige Authentifizierungslösung eines Drittanbieters verwenden, besteht die Möglichkeit, dass der MFA-Anspruch nicht ausgegeben wird. Wenn dieser Anspruch fehlt, kann Azure Active Directory nicht ermitteln, ob die Authentifizierungsanforderung von der mehrstufigen Authentifizierung angefordert wurde. Informationen dazu, wie Sie überprüfen, ob Ihre Lösung den erwarteten Anspruch ausgibt, finden Sie unter [Testen der Sicherheitsanforderungen für Partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements).

> [!IMPORTANT]
> Wenn Ihre Drittanbieterlösung nicht den erwarteten Anspruch ausgibt, müssen Sie mit dem Hersteller zusammenarbeiten, der die Lösung entwickelt hat, um zu bestimmen, welche Maßnahmen ergriffen werden müssen.

## <a name="resources-and-support"></a>Ressourcen und Support

Im Folgenden finden Sie Ressourcen, in denen Sie Support und Beispielcode finden können.

- [Partner Center Security Guidance-Gruppe – Community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Dies ist eine Online-Community, in der Sie sich über bevorstehende Veranstaltungen informieren und Fragen stellen können.
- [Partner Center .NET-Beispiele](https://github.com/microsoft/partner-center-dotnet-samples): Dieses GitHub-Repository enthält Beispiele, die mit .NET entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center Java-Beispiele](https://github.com/microsoft/partner-center-java-samples): Dieses GitHub-Repository enthält Beispiele, die mit Java entwickelt wurden und zeigen, wie Sie das Framework für das sichere Anwendungsmodell implementieren können.
- [Partner Center PowerShell – Mehrstufige Authentifizierung](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth): Dies ist ein Artikel, der Details zur Implementierung des Frameworks für das sichere Anwendungsmodell mit PowerShell enthält.
