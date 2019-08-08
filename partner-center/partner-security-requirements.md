---
title: Sicherheitsanforderungen für Partner | Partner Center
ms.topic: article
ms.date: 08/05/2019
description: Erfahren Sie mehr über die Sicherheitsanforderungen für Berater und Partner, die am Cloud Solution Provider-Programm teilnehmen.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider Program, CSP, System Steuerungs Hersteller, CPV, Multi-Factor Authentication, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: medium
ms.openlocfilehash: 39081f42c326665bdc30bf25df302d9ae00d9723
ms.sourcegitcommit: fe21430f96e203d279714623888224662d2782a2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2019
ms.locfileid: "68787254"
---
# <a name="partner-security-requirements"></a>Sicherheitsanforderungen für Partner

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direkt Rechnung
  - Indirekter Anbieter
  - Indirekter Wiederverkäufer
- Alle System Steuerungs Anbieter
- Alle Berater

Größere Sicherheitsvorkehrungen und Sicherheit sind die wichtigsten Prioritäten. Wir wissen, dass es sich bei der besten Verteidigung um die Verhinderung von Schutzmaßnahmen handelt Aus diesem Grund müssen alle Benutzer in unserem Ökosystem agieren und sicherstellen, dass Sie über die entsprechenden Sicherheitsmaßnahmen verfügen. Um Partner und Kunden zu schützen, stellen wir eine Reihe von obligatorischen Sicherheitsanforderungen für Ratgeber, System Steuerungs Anbieter und Partner ein, die am Cloud Solution Provider-Programm teilnehmen.

Ab dem 1. August 2019 müssen alle Partner die Multi-Factor Authentication für alle Benutzer, einschließlich der Dienst Konten, in Ihrem Partner Mandanten erzwingen.

> [!NOTE]
> Es wird dringend empfohlen, dass alle Partner, die eine Sovereign Cloud (21ViaNet, US Government und Deutschland) durchlaufen, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner müssen jedoch die neuen Sicherheitsanforderungen ab dem 1. August 2019 nicht erfüllen. Microsoft wird in Zukunft weitere Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

Die Bedingungen, die den Sicherheitsanforderungen des Partners zugeordnet sind, wurden dem [Programmhandbuch für den Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100)hinzugefügt. Ab dem 1. August 2019 sollten alle an dem Cloud Solution Provider-Programm beteiligten Partner den Bedingungen entsprechen. Im Zusammenhang mit den Beratern sind dieselben vertraglichen Anforderungen vorhanden.

Partner, die die obligatorischen Sicherheitsanforderungen nicht implementieren, können nicht im Cloud Solution Provider-Programm agieren oder Kunden Mandanten mit Delegierten Administratorrechten verwalten, sobald diese Anforderungen erzwungen werden. Wir stellen gerade eine technische Erzwingung für die Anforderungen her und Benachrichtigen Partner am Datum mit detaillierten Informationen.

## <a name="what-actions-do-i-need-to-take"></a>Welche Aktionen muss ich durchführen?

Angesichts der hohen privilegierten Natur eines Partners müssen wir sicherstellen, dass jeder Benutzer über eine MFA-Herausforderung für jede einzelne Authentifizierung verfügt. Dies kann mit einer der folgenden Methoden erreicht werden:

- Implementieren von Azure AD Premium und sicherstellen, dass die MFA für jeden Benutzer erzwungen wird
- Implementieren der [baselineschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementieren einer Drittanbieter Lösung und sicherstellen, dass die MFA für jeden Benutzer erzwungen wird

> [!IMPORTANT]
> Wenn diese Anforderungen technisch durchgesetzt werden, muss jede einzelne Authentifizierung über eine MFA-Aufforderung verfügen. Sie können keine Funktion des bedingten Zugriffs verwenden, um die Authentifizierung mit MFA zu vermeiden, wenn Sie auf kommerzielle Clouddienste von Microsoft zugreifen.

### <a name="considerations"></a>Überlegungen

Da diese Anforderungen für alle Benutzer, einschließlich der Dienst Konten, in Ihrem Partner Mandanten gelten, müssen Sie mehrere Aspekte beachten, um eine reibungslose Bereitstellung zu gewährleisten. Zu diesen Überlegungen zählen die Identifizierung von Benutzern in Azure AD, die keine MFA durchführen können, sowie Anwendungen und Geräte, die von Ihrer Organisation verwendet werden und die keine moderne Authentifizierung unterstützen.

Vor der Durchführung von Aktionen empfiehlt es sich, Folgendes zu identifizieren:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Verfügen Sie über eine Anwendung oder ein Gerät, die die Verwendung von MFA bei der Authentifizierung nicht unterstützt?

Wenn Sie die MFA-Legacy Authentifizierung erzwingen, werden Protokolle wie IMAP, POP3, SMTP usw. blockiert, da diese Protokolle MFA nicht unterstützen. Um dieser Einschränkung zu genügen, kann ein Feature, das als App-Kenn [Wörter](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) bezeichnet wird, verwendet werden, um sicherzustellen, dass sich die Anwendung oder das Gerät Lesen Sie die Überlegungen zur Verwendung von App-Kenn Wörtern, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um festzustellen, ob Sie in Ihrer Umgebung verwendet werden können

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Verfügen Sie über Benutzer, die Office 365 durch Lizenzen bereitgestellt haben, die Ihrem Partner Mandanten zugeordnet sind?

Vor der Implementierung einer Lösung empfiehlt es sich, zu bestimmen, warum die Version von Microsoft Office von Benutzern in Ihrem Partner Mandanten verwendet wird. Lesen Sie [Planen der Multi-Factor Authentication für Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) -bereit Stellungen, bevor Sie eine Aktion ausführen. Es besteht die Möglichkeit, dass für Ihre Benutzer Konnektivitätsprobleme bei Anwendungen wie Outlook auftreten. Bevor Sie MFA erzwingen, müssen Sie sicherstellen, dass Outlook 2013 SP1 oder höher verwendet wird und dass die moderne Authentifizierung in Ihrer Organisation aktiviert ist. Weitere Informationen finden Sie [unter Aktivieren der modernen Authentifizierung in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) .

Zum Aktivieren der modernen Authentifizierung für Windows-Geräte, auf denen Microsoft Office 2013 installiert ist, müssen Sie zwei Registrierungsschlüssel erstellen. Siehe [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

> [!IMPORTANT]
> Wenn Sie Ihre Benutzer für Azure AD MFA aktiviert haben und über Geräte verfügen, auf denen Office 2013 ausgeführt wird und die nicht für die moderne Authentifizierung aktiviert sind, müssen Sie App-Kenn Wörter auf diesen Geräten verwenden. Weitere Informationen zu app-Kenn Wörtern und wann/wo/wie Sie verwendet werden sollten, finden Sie hier: [App-Kenn Wörter mit Azure Multi-Factor Authentication](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Gibt es eine Richtlinie, die verhindert, dass Benutzer Ihre mobilen Geräte bei der Arbeit verwenden?

Es ist wichtig, alle Unternehmensrichtlinien zu identifizieren, die die Verwendung mobiler Geräte durch Mitarbeiter während der Arbeit verhindern, da Sie sich auf die von Ihnen implementierte MFA-Lösung auswirken. Es gibt MFA-Lösungen, wie z. b. die, die durch die Implementierung der [baselineschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)bereitgestellt werden, die nur die Verwendung einer Authentifikator-App für die Überprüfung zulassen. Wenn Ihre Organisation über eine Richtlinie verfügt, die die Verwendung mobiler Geräte verhindert, sollten Sie eine der folgenden Optionen in Erwägung gezogen haben:

- Bereitstellen eines virtualisierten Android-Geräts, auf dem eine Authentifikator-App installiert werden kann
- Implementieren Sie eine Drittanbieter Lösung, die MFA für jeden Benutzer im Partner Mandanten erzwingt, der die geeignetste Überprüfungs Option bereitstellt.
- Erwerben von [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) Lizenzen für die betroffenen Benutzer

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Welche Automatisierung oder Integration haben Sie, die Benutzer Anmelde Informationen für die Authentifizierung nutzt?

Da es erforderlich ist, die MFA für jeden Benutzer, einschließlich der Dienst Konten, zu erzwingen, wird jede Automatisierung oder Integration, die Benutzer Anmelde Informationen für die Authentifizierung nutzt, beeinträchtigt. Daher ist es wichtig, dass Sie identifizieren, welche Konten in diesen Situationen verwendet werden. Im folgenden finden Sie eine Liste mit Beispielen für Anwendungen oder Dienste, die berücksichtigt werden müssen.

- Systemsteuerung, die für die Bereitstellung von Ressourcen im Namen Ihrer Kunden verwendet wird
- Integration in eine beliebige Plattform, die für die Abrechnung verwendet wird (in Bezug auf das CSP-Programm) und ihre Kunden unterstützt
- PowerShell-Skripts, die die Module AZ, azurerm, Azure AD, MS Online usw. verwenden

Die obige Liste ist nicht vollständig. Daher ist es wichtig, dass Sie eine vollständige Bewertung aller Anwendungen oder Dienste in Ihrer Umgebung durchführen, die Benutzer Anmelde Informationen für die Authentifizierung nutzt. Um die MFA-Anforderung zu erfüllen, sollten Sie die Anleitungen im [sicheren Anwendungsmodell Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) implementieren, sofern möglich. Im folgenden finden Sie weitere Ressourcen, die Ihnen helfen zu verstehen, wie das sichere Anwendungsmodell Framework implementiert werden kann.

- [Partner Center .net-Beispiele](https://github.com/microsoft/partner-center-dotnet-samples) : dieses GitHub-Repository enthält Beispiele, die mit .net entwickelt wurden und veranschaulichen, wie Sie das sichere Anwendungsmodell Framework implementieren können.
- [Partner Center-Java-Beispiele](https://github.com/microsoft/partner-center-java-samples) : dieses GitHub-Repository enthält Beispiele, die mit Java entwickelt wurden, um zu veranschaulichen, wie das sichere Anwendungsmodell Framework implementiert werden kann.
- [Partner Center PowerShell-sicheres Anwendungsmodell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) : in diesem Artikel finden Sie Informationen zum Implementieren des sicheren Anwendungsmodell-Frameworks mithilfe von PowerShell.
- [Partner Center-Sicherheits Leit Faden Gruppe Community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : Dies ist eine Online-Community, in der Sie sich über bevorstehende Veranstaltungen informieren und Fragen stellen können, die Sie möglicherweise haben.

### <a name="enforcing-mfa-for-all-users"></a>Erzwingen der MFA für alle Benutzer

In diesem Abschnitt wird erläutert, wie Sie die [Baseline-Schutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) verwenden können, um die MFA für jeden Benutzer (einschließlich Dienst Konten) in Ihrem Partner Mandanten zu erzwingen. Wenn Sie beabsichtigen, Azure AD Premium zu verwenden, führen Sie die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)beschriebenen Schritte aus.

> [!NOTE]
> Eine Drittanbieter Lösung, die mit Azure AD kompatibel ist, kann verwendet werden, um die MFA für alle Benutzer, einschließlich Dienst Konten, zu erzwingen. Weitere Informationen zur Implementierung der Lösung finden Sie in der Dokumentation des Herstellers.

Grundlegende Schutzrichtlinien sind eine Reihe vordefinierter Richtlinien, mit denen Organisationen vor vielen häufigen Angriffen geschützt werden. Diese häufigen Angriffe können Kenn Wort Spray, Wiedergabe und Phishing einschließen. Baselineschutzrichtlinien sind in allen Editionen von Azure Active Directory verfügbar. Microsoft stellt diese grundlegenden Schutzrichtlinien allen Benutzern zur Verfügung, um Kunden und Partnern die Implementierung von bewährten Sicherheitsmethoden zu ermöglichen.

Die beiden grundlegenden Schutzrichtlinien, die aktiviert werden sollten, sind in der folgenden Tabelle beschrieben.

|**Richtlinie**| |
|-----|-----|
|**MFA für Administratoren erforderlich**|Wenn Sie die Richtlinie MFA für Administratoren anfordern aktivieren, müssen sich Benutzer in den Administrator Rollen mithilfe der Authenticator-App für MFA registrieren. Nachdem die MFA-Registrierung fertiggestellt wurde, müssen Administratoren bei jeder Anmeldung MFA durchführen.|
|**Endbenutzer Schutz**|Der Endbenutzer Schutz ist eine risikobasierte MFA-baselineschutzrichtlinie, mit der alle Benutzer in einem Verzeichnis geschützt werden. Wenn Sie diese Richtlinie aktivieren, müssen sich alle Benutzer mithilfe der Authenticator-App für MFA registrieren. Benutzer können die Eingabeaufforderung für die MFA-Registrierung 14 Tage lang ignorieren. Danach wird die Anmeldung blockiert, bis Sie sich für MFA registrieren. Nach der Registrierung für MFA werden Benutzer nur bei riskanten Anmelde versuchen zur Eingabe der MFA aufgefordert. Kompromittierte Benutzerkonten werden blockiert, bis Ihr Kennwort zurückgesetzt und Risiko Ereignisse verworfen wurden.|

Wenn diese Richtlinien aktiviert sind, kann jeder Benutzer Azure MFA mithilfe der Authenticator-App für die Überprüfung ohne zusätzliche Kosten Nutzen.

#### <a name="configure-self-service-password-reset"></a>Self Service-Kenn Wort Zurücksetzung konfigurieren

Die Self-Service-Kenn Wort Zurücksetzung (Self-Service Password Reset, sspr) ist ein Azure Active Directory Feature, mit dem Benutzer ihre Kenn Wörter zurücksetzen können, ohne dass Sie sich Benutzer müssen sich für die Self-Service-Kenn Wort Zurücksetzung registrieren oder Sie registrieren, bevor Sie den Dienst verwenden. Während der Registrierung wählt der Benutzer eine oder mehrere Authentifizierungsmethoden aus, die von seiner Organisation aktiviert wurden.

Wenn die Schutzrichtlinie für den [Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) aktiviert ist, werden alle kompromittierten Benutzerkonten blockiert, bis Ihr Kennwort zurückgesetzt wird und die Risiko Ereignisse verworfen wurden. Es wird empfohlen, dass jeder Benutzer, der ein globaler Administrator ist, die folgenden Aktionen ausführt, um sich für sspr zu registrieren, damit diese nicht gesperrt werden.

1. Navigieren Sie zur [Seite sspr-Setup](https://aka.ms/ssprsetup) .
2. Benutzernamen und Kennwort eingeben
3. Konfigurieren Sie mindestens eine der Überprüfungs Optionen, die verwendet werden, um zu überprüfen, ob Sie das Kennwort zurücksetzen.  

Wenn ein Konto kompromittiert wurde, muss der Administrator Maßnahmen ergreifen, um den Zugriff für den betroffenen Benutzer wiederherzustellen. Weitere Informationen zum Vorgang zum Entsperren des Benutzers finden [Sie in den Schritten zum Entsperren eines Benutzers](#recovering-compromised-accounts) .

#### <a name="require-mfa-for-admins"></a>MFA für Administratoren erforderlich

Die Baseline-Richtlinie *MFA für Admin erforderlich* erfordert MFA für die folgenden Verzeichnis Rollen, die als privilegierteste Azure Active Directory Rollen gelten:

- Globaler Administrator
- SharePoint-Administrator
- Exchange-Administrator
- Administrator für bedingten Zugriff
- Sicherheitsadministrator
- Helpdesk-Administrator/Kenn Wort Administrator
- Rechnungsadministrator
- Benutzer Administrator

Wenn Sie die Richtlinie MFA für Administratoren anfordern aktivieren, sind die oben genannten neun Administrator Rollen erforderlich, um sich mit der Authenticator-App für MFA zu registrieren. Nachdem die MFA-Registrierung durchgeführt wurde, müssen Administratoren die MFA jedes Mal ausführen, wenn Sie sich anmelden.

Wenn in Ihrer Organisation diese Konten in Skripts oder Codes verwendet werden, sollten Sie Sie in Erwägung gezogen, Sie durch [verwaltete Identitäten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)zu ersetzen.

So aktivieren Sie diese Richtlinie und schützen Ihre Administratoren:

1. Melden Sie sich beim **Azure-Portal** als globaler Administrator, Sicherheits Administrator oder Administrator für den bedingten Zugriff an.
2. Navigieren Sie zu **Azure Active Directory** > **bedingter Zugriff**.
3. Wählen Sie **in der Liste der Richtlinien die Option Baseline-Richtlinie: Erfordert MFA für Administratoren**.
4. Legen Sie Richt **Linie aktivieren** auf **Richtlinie sofort verwenden**fest.
5. Klicken Sie auf **Speichern**.

> [!WARNING]
> Bevor Sie diese Richtlinie aktivieren, stellen Sie sicher, dass Ihre Benutzer keine Legacy Authentifizierungsprotokolle verwenden. Durch die Implementierung dieser Richtlinie wird die Legacy Authentifizierung blockiert.

> [!IMPORTANT]
> Es gibt ein bekanntes Problem, das sich auf ihre Fähigkeit zum Herstellen einer Verbindung mit Exchange Online PowerShell mithilfe Delegierter Administratorrechte auswirkt. Wenn Sie dieses PowerShell-Modul verwenden, sehen Sie sich das bekannte Problem von [Exchange Online PowerShell](#exchange-online-powershell) an, bevor Sie diese Richtlinie aktivieren.

#### <a name="end-user-protection"></a>Endbenutzer Schutz

Die Baseline-Richtlinie für den Endbenutzer Schutz schützt alle Benutzer in einem Verzeichnis. Wenn Sie diese Richtlinie aktivieren, müssen sich alle Benutzer innerhalb von 14 Tagen für Azure MFA registrieren. Nach der Registrierung werden Benutzer nur bei riskanten Anmelde versuchen zur Eingabe von MFA aufgefordert. Kompromittierte Benutzerkonten werden blockiert, bis das Zurücksetzen des Kennworts und das Risiko von

Richtlinien **Basis Richtlinie: Der Endbenutzer** Schutz ist vorkonfiguriert und wird am oberen Rand angezeigt, wenn Sie in Azure-Portal zum Blatt "bedingter Zugriff" navigieren.

So aktivieren Sie diese Richtlinie und schützen Ihre Benutzer:

1. Melden Sie sich beim **Azure-Portal** als globaler Administrator, Sicherheits Administrator oder Administrator für den bedingten Zugriff an.
2. Navigieren Sie zu **Azure Active Directory** > **bedingter Zugriff**.
3. Wählen Sie **in der Liste der Richtlinien die Option Baseline-Richtlinie: Endbenutzer Schutz (Vorschau)** .
4. Legen Sie Richt **Linie aktivieren** auf **Richtlinie sofort verwenden**fest.
5. Klicken Sie auf **Speichern**.

> [!WARNING]
> Bevor Sie diese Richtlinie aktivieren, stellen Sie sicher, dass Ihre Benutzer keine Legacy Authentifizierungsprotokolle verwenden. Durch die Implementierung dieser Richtlinie wird die Legacy Authentifizierung blockiert.

> [!IMPORTANT]
> Es gibt bekannte Probleme, die sich auf ihre Fähigkeit zum Herstellen einer Verbindung mit Exchange Online PowerShell mithilfe Delegierter Administratorrechte auswirken. Wenn Sie dieses PowerShell-Modul verwenden, sehen Sie sich das bekannte Problem von [Exchange Online PowerShell](#exchange-online-powershell) an, bevor Sie diese Richtlinie aktivieren.

## <a name="common-issues"></a>Allgemeine Probleme

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Nach dem Aktivieren der Baseline-Richtlinien können Sie feststellen, dass bei der Automatisierung oder Integration eine Ausnahme wie die folgende auftritt.

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Der Grund für diese Ausnahme ist, dass Sie eine Authentifizierung mit Benutzer Anmelde Informationen durchzuführen und MFA nun erforderlich ist. Um diese Ausnahme zu beheben, müssen Sie ein Zugriffs Token für die Authentifizierung verwenden. Weitere Informationen finden Sie im [Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) .

>[!IMPORTANT]
>Die meisten modernen APIs und PowerShell-Module unterstützen die Verwendung eines Zugriffs Tokens für die Authentifizierung. Es gibt jedoch einige, die diese Funktion derzeit nicht unterstützen. Wenn Sie Hilfe benötigen, um zu ermitteln, ob die zu verwendende API oder das PowerShell-Modul die Verwendung eines Zugriffs Tokens für die Authentifizierung unterstützt, senden Sie eine Nachricht in der [Partner Center-Sicherheits Leit Faden-Gruppen](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) Community.

#### <a name="aadsts700082"></a>AADSTS700082

Nachdem Sie das sichere Anwendungsmodell Framework implementiert haben, besteht die Möglichkeit, dass Sie nach dem Erstellen des ersten Aktualisierungs Tokens 90 Tage die folgende Ausnahme erhalten.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

In Bezug auf Azure Active Directory die maximale Lebensdauer für ein Aktualisierungs Token 90 Tage. Um diesen Fehler zu beheben, müssen Sie ein neues Aktualisierungs Token generieren und sicher speichern. Beachten Sie, dass es möglich ist, das Aktualisierungs Token Programm gesteuert zu aktualisieren, da bei jeder Anforderung zum Azure Active Directory für ein Zugriffs Token ein neues Aktualisierungs Token zurückgegeben wird. Sie können die entsprechende Logik implementieren, um das sicher gespeicherte Aktualisierungs Token zu aktualisieren, bevor es abläuft.

Weitere Informationen finden Sie [unter konfigurierbare tokengültzeiten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) .

### <a name="recovering-compromised-accounts"></a>Wiederherstellen kompromittierter Konten

Der kompromittierte Anmelde Informationsdienst von Microsoft findet öffentlich verfügbare Benutzername/Kennwort-Paare, um unsere Kunden zu schützen. Wenn Sie einem unserer Benutzer entsprechen, können wir dieses Konto sofort sichern. Benutzer, deren Anmelde Informationen mit einem kompromittierten Anmelde Informations Nachweis gekennzeichnet sind, sind gefährdet. Diese Benutzer werden daran gehindert, sich anzumelden, bis Ihr Kennwort zurückgesetzt wird.

Benutzer, denen eine Azure AD Premium Lizenz zugewiesen ist, können den Zugriff über die Self-Service-Kenn Wort Zurücksetzung (sspr) wiederherstellen, wenn die Funktion in Ihrem Verzeichnis aktiviert ist Benutzer ohne Premium-Lizenz, die blockiert werden, müssen sich an einen Administrator wenden, um ein manuelles Zurücksetzen des Kennworts auszuführen und das gekennzeichnete Benutzer Risiko Ereignis abzulegen.

#### <a name="steps-to-unblock-a-user"></a>Schritte zum Entsperren eines Benutzers

Vergewissern Sie sich, dass der Benutzer durch die Richtlinie blockiert wurde, indem Sie die Anmelde Protokolle des Benutzers überprüfen.

1. Ein Administrator muss sich beim **Azure-Portal** anmelden und zu **Azure Active Directory** > **Benutzer** Navigieren > auf den Namen des Benutzers klicken und zu Anmeldungen navigieren.
2. Um die Kenn Wort Zurücksetzung für einen gesperrten Benutzer zu initiieren, muss ein Administrator zu **Azure Active Directory** > **Benutzer mit Risiko Markierung** navigieren.
3. Klicken Sie auf den Benutzer, dessen Konto blockiert ist, um Informationen zur aktuellen Anmelde Aktivität des Benutzers anzuzeigen.
4. Klicken Sie auf Kennwort zurücksetzen, um ein temporäres Kennwort zuzuweisen, das bei der nächsten Anmeldung geändert werden muss
5. Klicken Sie auf alle Ereignisse verwerfen, um die Risikobewertung des Benutzers zurückzusetzen.

Der Benutzer kann sich jetzt anmelden, sein Kennwort zurücksetzen und auf die Anwendung zugreifen.

## <a name="known-issues"></a>Bekannte Probleme

### <a name="exchange-online-powershell"></a>Exchange Online-PowerShell

Wenn MFA erzwungen wird, können Partner ihre delegierten Administratorrechte mit Exchange Online PowerShell nicht nutzen, um Aktionen für Ihre Kunden auszuführen. Weitere Informationen zu dieser Einschränkung finden [Sie unter Herstellen einer Verbindung mit Exchange Online PowerShell mithilfe von Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) .

Sie können diese Einschränkung umgehen, indem Sie ein neues Konto erstellen und es niemals zum Ausführen einer interaktiven Authentifizierung verwenden. Es wird empfohlen, [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) zu nutzen, um das neue Konto zu erstellen und die Erstkonfiguration auszuführen. Mit dem folgenden PowerShell-Befehl können Sie das Konto erstellen und konfigurieren.

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

Wenn Sie das nächste Mal mithilfe von PowerShell eine Verbindung mit Exchange Online herstellen, wird dieses Konto wie erwartet funktionieren.

> [!IMPORTANT]
> Die Fähigkeit für Partner, ihre delegierten Administratorrechte mit Exchange Online PowerShell zu nutzen, um Aktionen für Ihre Kunden durchzuführen, wenn MFA erzwungen wird, wird in Zukunft verfügbar sein. Bis zu diesem Zeitpunkt sollten Sie dieses Problem umgehen.

## <a name="resources-and-support"></a>Ressourcen und Support

Mithilfe der [Partner Center-Sicherheits Leit Faden-Gruppen Community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) können Sie weitere Ressourcen finden und sich über bevorstehende Veranstaltungen wie z. b. technische Bürostunden informieren. Weitere Informationen zu den Anforderungen finden Sie im Dokument [häufig gestellte Fragen](partner-security-requirements-faq.md) .
