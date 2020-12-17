---
title: Einrichten von Benutzern mit mehrstufiger Authentifizierung
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie Mitarbeiter mit mehrstufiger Authentifizierung (MFA) einrichten.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578287"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Einrichten von Benutzern mit mehrstufiger Authentifizierung

**Geeignete Rollen**

- Globaler Administrator

Mehr Sicherheitsmaßnahmen für den Datenschutz und eine höhere Sicherheit gehören zu unseren obersten Prioritäten. Wir wissen, dass die beste Verteidigung die Prävention ist und dass wir nur so stark sind wie unser schwächstes Glied. Deshalb müssen alle in unserem Partnerumfeld handeln und sicherstellen, dass sie über angemessene Sicherheitsvorkehrungen verfügen. Es wird dringend empfohlen, dass alle Partner die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) für die Benutzer in ihrem Partnermandanten aktivieren. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Hinzufügen der mehrstufigen Authentifizierung für Benutzer

Sie müssen der globale Administrator für Ihr Unternehmen sein, um diese Aufgabe auszuführen.

Die mehrstufige Authentifizierung für Ihre Benutzer kann am einfachsten aktiviert werden, während Sie diese Ihrem Azure AD-Mandanten hinzufügen.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com) an, und wechseln Sie dann zu **Benutzerverwaltung**.
1. Wählen Sie **Multi-Factor Authentication** aus.
1. Wählen Sie den zu aktivierenden Benutzer und dann **Aktivieren** aus.

Dadurch wird Multi-Factor Authentication für diesen Benutzer aktiviert. Aktiviert bedeutet, dass der Benutzer bei der ersten Anmeldung aufgefordert wird, die MFA-Überprüfung einzurichten. Anschließend wird der Benutzer bei der Anmeldung aufgefordert, einen Code anzugeben, der ihm entweder per E-Mail oder SMS (je nach Einrichtung) gesendet wird.  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Festlegen der Überprüfungsmethode":::

>[!NOTE]
>Sie können die Verwendung von Multi-Factor Authentication durch die Benutzer erzwingen, indem Sie die oben beschriebenen Schritte ausführen und dann **Erzwingen** auswählen. Weitere Informationen finden Sie unter [Aktivieren von Azure Multi-Factor Authentication für Einzelbenutzer zum Sichern von Anmeldeereignissen](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates). 

Alle Benutzer sind zunächst  **Deaktiviert**. Wenn Sie Benutzer für Azure Multi-Factor Authentication für Einzelbenutzer registrieren, ändert sich deren Status in  **Aktiviert**. Wenn aktivierte Benutzer sich anmelden und den Registrierungsprozess abschließen, ändert sich der Status in  **Erzwungen**. 

## <a name="next-steps"></a>Nächste Schritte

- [Zuweisen von Rollen und Berechtigungen zu Benutzern](permissions-overview.md)

