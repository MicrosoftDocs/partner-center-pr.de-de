---
title: Erstellen von Benutzerkonten und Festlegen von Berechtigungen | Partner Center
ms.topic: article
ms.date: 02/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie im Partner Center Benutzerkonten erstellen und Rollen für jeden Mitarbeiter zuweisen, der Zugriff benötigt. Benutzer mit unterschiedlichen Administratorrechten können dies erledigen.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: jasonwhowell
ms.author: jasonh
Keywords: Rollen, Berechtigungen, Benutzer hinzufügen, Rolle zuweisen, Administrator, Agent
ms.localizationpriority: high
ms.openlocfilehash: 98dce89c0eab132ec0f247d25632617d8dd503cc
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2020
ms.locfileid: "80389649"
---
# <a name="create-user-accounts-and-assign-permissions"></a>Erstellen von Benutzerkonten und Zuweisen von Berechtigungen

**Geeignete Rollen**

- Kontoadministrator
- Globaler Administrator
- Benutzerverwaltungsadministrator

Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf das Partner Center benötigen. Diese Aufgaben müssen von einem Administrator für die Benutzerverwaltung, Kontoadministrator oder vom globalen Administrator durchgeführt werden. Dem Benutzer, der diese Aufgaben ausführt, müssen auch die AAD-Rollen (Azure Active Directory) „Benutzeradministrator“ und „Globaler Administrator“ zugewiesen werden. Weitere Informationen zu AAD-Rollen findest du unter [Berechtigungen für Administratorrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).


## <a name="add-a-new-user"></a>Neuen Benutzer hinzufügen

1. Klicken Sie im Partner Center rechts oben auf das Symbol **Einstellungen** und dann auf **Benutzerverwaltung**.

2. Wählen Sie **Benutzer hinzufügen** aus.

3. Gib den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.

4. Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten. Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt.  Wenn Benutzer eine Rollenzuweisung wünschen, finden sie die zu kontaktierenden globalen Administratoren unter **Benutzerverwaltung** durch Filtern nach „globaler Administrator“.

5. Wählen Sie **Hinzufügen** aus, um das Benutzerkonto zu erstellen. Bestätigen Sie die Details des Benutzers auf der nächsten Seite.

> [!IMPORTANT]  
> Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden. Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können. 


Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden. Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern. 


### <a name="find-your-global-admin"></a>Finden des globalen Administrators

Es kann vorkommen, dass ein Benutzer seine Rolle ändern lassen muss oder ein neuer Benutzer eine Zuweisung zu einer bestimmten Rolle wünscht.  
Um einen globalen Administrator zu finden, der Rollenänderungen vornehmen oder einem neuen Benutzer Rollen zuweisen kann, klicken Sie rechts oben im Partner Center auf das Symbol **Einstellungen**, wählen Sie **Benutzerverwaltung** aus, und filtern Sie nach „Globaler Administrator“. 


### <a name="new-global-admin"></a>Neuer globaler Administrator

Wenn Ihr globaler Administrator aus dem Unternehmen ausscheidet und diese Aufgabe von jemand anderem übernommen wird, können Sie ein Ticket an das Azure-Team oder an das Office 365-Team senden. Wählen Sie eine der folgenden Optionen aus, um zu erfahren, wie Sie dazu vorgehen.

[Neuer globaler Administrator für Azure](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Neuer globaler Administrator für Office 365](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>Zuweisen von Benutzerrollen

Um im Partner Center arbeiten zu können, muss Ihnen eine Rolle zugewiesen sein.  Derzeit gibt es Rollen für Azure Active Directory-Mandanten, Cloud Solution Provider (CSP) und nicht auf AAD bezogene Rollen im Unternehmen. Ein einzelnes Unternehmen kann eine alle diese Rollen benötigen.

>[!Important]
>Benutzer müssen in Ihrem Mandanten aufgeführt sein, um auf das Partner Center zugreifen zu können. Rollenzuweisungen gewähren zusätzliche Zugriffsrechte.


**AAD-Mandantenrollen**:
- Globaler Administrator
- Benutzeradministrator

**CSP-Rollen**:
- Administrator-Agent
- Abrechnungsadministrator
- Vertriebsbeauftragter
- Helpdesk-Agent

**Rollen für die Verwaltung der MPN-Mitgliedschaft und des Unternehmens (außerhalb von AAD)**
- MPN-Partneradministrator
- Kontoadministrator
- Administrator für Empfehlungen
- Unternehmensprofiladministrator
- Incentives-Administrator und -Benutzer

**Control Panel Vendor ist eine CSP- und keine AAD-Rolle**.
- Globaler Administrator

**Gastbenutzer** muss Teil des AAD-Mandanten sein und eine beliebige AAD-externe Rolle haben.

Spezifische Informationen zu den Rollen und ihren Möglichkeiten finden Sie unter [Zuweisen von Benutzerberechtigungen](permissions-overview.md).

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>Zuordnen des Microsoft Learn Kontos eines Benutzers im Partner Center

Damit Sie die Schulungs- und Lernpfade anzeigen können, die Ihre Benutzer für Kompetenzen verwenden, müssen sie Ihre MCP-ID ihrem Partner Center-Konto zuordnen. Wenn Sie als globaler Administrator neue Benutzer hinzufügen, müssen Sie sie daran erinnern, ihre MCP-ID ihrem Konto zuzuordnen. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>Zuordnen Ihrer MCP-ID zu Ihrem Partner Center-Konto

1. Wähle im Partner Center-Dashboard das Symbol für **Dein Konto** in der rechten Ecke des Dashboards aus, und wähle dann **Mein Profil** aus.

2. Unter **Dein Learning** kannst du dein Microsoft Learning-Konto zuordnen und auch dein Microsoft-Konto mit Partner University verbinden.







