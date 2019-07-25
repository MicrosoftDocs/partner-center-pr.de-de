---
title: FAQ zu den Sicherheitsanforderungen für Partner | Partner Center
ms.topic: article
ms.date: 07/18/2019
description: Häufig gestellte Fragen zu den Sicherheitsanforderungen des Partners
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider Program, CSP, System Steuerungs Hersteller, CPV, Multi-Factor Authentication, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315549"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Häufig gestellte Fragen zu den Sicherheitsanforderungen des Partners

Dieser Artikel enthält einige häufig gestellte Fragen zu den [Sicherheitsanforderungen des Partners](partner-security-requirements.md). Eine umfassende Liste mit häufig gestellten Fragen finden Sie [hier](http://assetsprod.microsoft.com/security-requirements-faq.pdf).

## <a name="conditional-access"></a>Bedingter Zugriff

### <a name="can-conditional-access-be-used"></a>Kann der bedingte Zugriff verwendet werden?

Ja, Sie können den bedingten Zugriff verwenden, um die MFA für jeden Benutzer, einschließlich der Dienst Konten, in Ihrem Partner Mandanten zu erzwingen. Angesichts der hohen privilegierten Natur eines Partners müssen wir jedoch sicherstellen, dass jeder Benutzer für jede einzelne Authentifizierung über eine MFA-Herausforderung verfügt. Dies bedeutet, dass Sie nicht in der Lage sind, die Funktion des bedingten Zugriffs zu nutzen, die die Anforderung für MFA umgehen.

## <a name="multi-factor-authentication"></a>Mehrstufige Authentifizierung

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Unterliegen meine Kunden den Sicherheitsanforderungen des Partners?

Nein, es ist nicht erforderlich, dass Sie die MFA für jeden Benutzer in den Azure AD Mandanten Ihres Kunden erzwingen. Es wird jedoch empfohlen, dass Sie mit jedem Kunden zusammenarbeiten, um zu bestimmen, wie die Benutzer am besten geschützt werden.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>Können APP-Kenn Wörter mit den baselineschutzrichtlinien verwendet werden?

Ja, [App](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) -Kenn Wörter können verwendet werden. Lesen Sie die Überlegungen zur Verwendung von App-Kenn Wörtern, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um zu ermitteln, ob Sie für Ihre Bedürfnisse unterstützt

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Kann jeder Benutzer von dieser Anforderung ausgeschlossen werden? 

Nein, jeder Benutzer, einschließlich Dienst Konten, muss sich mit MFA authentifizieren.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Gelten die Partner Sicherheitsanforderungen für die Integrations Sandbox?

Ja, die Sicherheitsanforderungen für Partner gelten für die Integrations Sandbox. Dies bedeutet, dass Sie die entsprechende MFA-Lösung für Benutzer im Integration Sandbox-Mandanten implementieren müssen. Es wird empfohlen, dass Sie die Baseline-Schutzrichtlinien implementieren, um MFA bereitzustellen.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Gewusst wie ein Konto für den Notfall Zugriff (Break Glass) konfigurieren?

Es hat sich als bewährte Vorgehensweise bewährt, ein oder zwei Notfall Zugriffs Konten zu erstellen, um zu verhindern, dass Sie versehentlich von Ihrem Azure AD Mandanten gesperrt werden. Hinsichtlich der Partner Sicherheitsanforderungen ist es erforderlich, dass sich jeder Benutzer mit MFA authentifiziert. Dies bedeutet, dass Sie die Definition eines Notfall Zugriffs Kontos ändern müssen. Dabei kann es sich um ein Konto handeln, das eine Drittanbieter Lösung für MFA nutzt.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Wie werden Gastbenutzer von den Sicherheitsanforderungen des Partners betroffen?

Gastbenutzer müssen sich mit MFA authentifizieren, wenn Sie auf Ressourcen in Ihrem Partner Mandanten zugreifen. Die Sicherheitsanforderungen des Partners haben keine Auswirkung darauf, dass der Gastbenutzer auf Ressourcen in seinem eigenen Mandanten zugreift.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Wenn ich eine Drittanbieter Lösung verwende, ist Active Directory Verbunddienst (ADFS) erforderlich? 

Nein, es ist nicht erforderlich, Active Directory Verbunddienst (ADFS) zu haben, wenn Sie eine Drittanbieter Lösung verwenden. Es wird empfohlen, dass Sie mit dem Anbieter der Lösung zusammenarbeiten, um zu bestimmen, welche Anforderungen für die Lösung erfüllt sind.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>Ist es erforderlich, die Baseline-Schutzrichtlinien zu aktivieren?

Nein, es ist nicht erforderlich, die baselineschutzrichtlinien zu aktivieren. Die einzige Voraussetzung besteht darin, dass Sie die MFA für jeden Benutzer, einschließlich der Dienst Konten, in Ihrem Partner Mandanten erzwingen.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Welche Überprüfungs Optionen werden durch die Implementierung der baselineschutzrichtlinien bereitgestellt? 

In Bezug auf die MFA-Version, die über die Implementierung der baselineschutzrichtlinien verfügbar ist, ist die einzige verfügbare Überprüfungs Option eine Authentifikator-app. Die Verwendung einer Telefonanruf-und SMS-Nachricht gilt als weniger sicher. Diese Optionen sind also in dieser MFA-Version nicht verfügbar.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Ist das Dienst Konto, das von verwendet wird, Azure AD Connect von den Sicherheitsanforderungen des Partners betroffen?

Nein, das von Azure AD Connect verwendete Dienst Konto wird von den Sicherheitsanforderungen des Partners nicht beeinträchtigt. Wenn Sie ein Problem mit Azure AD Connect aufgrund der Erzwingung von MFA haben, öffnen Sie eine technische Supportanfrage beim Microsoft-Support.
