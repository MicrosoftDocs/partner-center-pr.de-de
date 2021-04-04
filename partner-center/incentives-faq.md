---
title: FAQ zu Incentives
ms.topic: how-to
ms.date: 02/05/2021
description: Häufig gestellte Fragen zu Microsoft-Incentives. Dieser Artikel enthält Fragen zu Benutzer Rollen, zur Registrierung oder zu den Vorgehensweisen für Fehlermeldungen.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 1c3cafa6b5ea280a924a0142da78483d54a18ab9
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179495"
---
# <a name="frequently-asked-questions-on-incentives"></a>Häufig gestellte Fragen zu Incentives

**Geeignete Rollen**

- Incentiveadministrator
- Incentivebenutzer

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>Muss ich der globale Administrator sein, um sich bei den Incentives anzumelden?

Nein. Sowohl der globale Administrator als auch der Konto Administrator können Benutzer als Incentive-Administratoren zuweisen. Incentives-Administratoren verwalten die Incentives-Programme des Unternehmens über Partner Center. Weitere Informationen finden Sie unter [Übersicht über Berechtigungen](permissions-overview.md).

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>Was muss ich tun, wenn mein Unternehmen bereits Mitglied der Microsoft Partner Network (MPN) ist?

Wenn Sie versuchen, MPN beizutreten und Ihr Unternehmen bereits Mitglied ist, erkennt MPN die Domäne und verknüpft Sie mit dem vorhandenen Konto. Das vorhandene Konto kann dasselbe Unternehmen oder ein zugehöriges Unternehmen sein, das dieselbe e-Mail-Domäne oder dasselbe Azure-Aktivitäts Verzeichnis (Azure AD) verwendet, um mehrere Domänen zu verwalten.

Sie können den primären Kontakt auf der Seite rechtliche profile ermitteln. Wenn Ihr Standort der mpnhq-Speicherort ist, müssen Sie nur mit den erforderlichen Berechtigungen zum Verwalten von Anreizen eingerichtet werden. Weitere Informationen zu Rollen und Berechtigungen finden Sie in der [Übersicht über Berechtigungen](permissions-overview.md).

Wenn Sie sich nicht im gleichen Land wie der mpnhq-Speicherort befinden, finden Sie weitere Informationen zu diesem Szenario in den [Anweisungen für mehrere nationale Konten](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) .

## <a name="what-user-roles-are-available"></a>Welche Benutzer Rollen sind verfügbar?

Die Person, die das Unternehmen im Partner Center registriert, wird standardmäßig zum primären Kontakt und globalen Administrator. Der Administrator kann Benutzer im Portal einladen und verwalten.

Die wichtigsten Rollen für die Anreize sind die Administrator-und Incentive-Benutzer von Incentives. Der admin-Administrator kann sich für Incentive-Programme registrieren und Bank-und Steuer Details für den Partner verwalten. Der Benutzer "Incentives" kann Berichte im Tool anzeigen, um zu sehen, was bezahlt wurde, und die Aufschlüsselung der einzelnen Zahlungen, aber keine Bank Details anzeigen oder bearbeiten. Beide Rollen können auf alle Standorte unter dem globalen Partner Konto angewendet werden.

Weitere Informationen finden Sie unter [Übersicht über Berechtigungen](permissions-overview.md).

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>Wie kann ich herausfinden, wer über globale oder Konto Administratorrechte für mein Unternehmen verfügt?

So finden Sie einen globalen Administrator oder Konto Administrator, der Rollen Änderungen vornehmen oder einem neuen Benutzer Rollen zuweisen kann:

1. Wählen Sie im Partner Center über das Symbol "Kontoeinstellungen" in der oberen rechten Ecke " **Benutzerverwaltung**" aus.
2. Filtern Sie entweder nach **globaler Administrator** oder **Konto Administrator**.
3. Sie können auch zu **mein Profil** wechseln, **Rollen und Berechtigungen** auswählen und eine Liste der unterschiedlichen Administratoren anzeigen, die Ihnen helfen können, ihre Berechtigungen zu erhöhen.
 
Weitere Informationen [finden Sie untersuchen ihrer Rolle](find-your-role.md).  

## <a name="i-cant-access-incentives-using-my-credentials"></a>Ich kann nicht über meine Anmelde Informationen auf die Anreize zugreifen.

Der Grund dafür, dass Sie keine Anreize sehen können, liegt darin, dass Sie nicht über die richtigen Berechtigungen verfügen. Verwenden Sie das folgende Verfahren, um dieses Problem zu beheben.

1. Melden Sie sich mit ihren Azure AD Mandanten Anmelde Informationen (Ihre Anmelde Informationen für Ihre Arbeit) beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an. Wenn Sie sich nicht anmelden können, wenden Sie sich an den globalen Administrator Ihres Unternehmens.

2. Wenn Sie bei der Anmeldung aufgefordert werden, aus Ihrem Geschäfts **Konto** oder **persönlichen Konto** auszuwählen, wählen Sie Geschäfts **Konto** aus.

3. Wählen Sie im Partner Center-Menü die Option **Incentives** aus, und klicken Sie dann auf **Übersicht**. Wenn Sie nicht über Administrator-oder Benutzerberechtigungen für Incentives verfügen, werden Ihnen die Kontaktinformationen für alle globalen Administratoren und Konto Administratoren Ihres Unternehmens angezeigt. Wenden Sie sich an einen dieser Administratoren, um die Incentive-Rolle für die erforderlichen MPN-IDs und Incentive-Programme zu erhalten.

4. Wenn Sie bereits über eine Administrator Rolle für Incentives verfügen, sehen Sie die Registrierungen für Ihr Unternehmen für die MPN-IDs und Incentive-Programme, auf die Sie Zugriff haben.

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>Einige Registrierungen fehlen auf der Seite mit den Incentives (Übersicht).

Wenn Sie entweder eine Einladung von erhalten haben oder sich bei angemeldet haben, sollten Sie ein Incentive-Programm, das nicht mehr im Dashboard angezeigt wird, überprüfen, ob Sie über die entsprechenden Zugriffsberechtigungen verfügen. Nur Benutzer mit der Rolle "Incentive-Benutzer" oder "Incentive admin" können das Programm sehen. Siehe [Suchen ihrer Rolle](./find-your-role.md).

Wenn Sie Ihre Rolle oder Berechtigungen ändern müssen, wenden Sie sich an den globalen oder Konto Administrator Ihres Unternehmens. Informationen dazu, wer diese Personen sind, [finden Sie untersuchen des globalen Administrators](./find-your-role.md#find-your-global-admin).

Auf der Übersichtsseite werden nur Registrierungen angezeigt, die dem globalen Partner Konto zugeordnet sind, das dem Azure AD Mandanten zugeordnet ist. Wenn Ihr Unternehmen über mehr als eine PGA verfügt, benötigen Sie jeweils andere Anmelde Informationen.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>An wen sollte ich mich wenden, wenn ich eine Fehlermeldung erhalte oder während des Registrierungsvorgangs Hilfe benötige?

Es gibt einen Online Support Dienst, wenn im Abschnitt "Incentives" des Dashboards Probleme auftreten – Weitere Informationen finden Sie unter Support Option (? Symbol) oben rechts.

## <a name="next-steps"></a>Nächste Schritte

- [Erste Schritte mit Incentives](incentives-get-started-intro.md)