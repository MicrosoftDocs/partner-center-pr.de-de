---
title: Erstellen von Benutzerkonten und Zuweisen von Rollen
description: Jedem Mitarbeiter muss eine Rolle zugewiesen werden, bevor er auf das Partner Center zugreifen kann. Erfahren Sie, wie Sie Benutzerkonten erstellen, Rollen zuweisen und Berechtigungen festlegen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006769"
---
# <a name="create-user-accounts"></a>Erstellen Sie Benutzerkonten  

**Geeignete Rollen**

- Kontoadministrator
- Globaler Administrator
- Benutzerverwaltungsadministrator

Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf das Partner Center benötigen. Diese Aufgaben müssen von einem Administrator für die Benutzerverwaltung, Kontoadministrator oder vom globalen Administrator durchgeführt werden. Dem Benutzer, der diese Aufgaben ausführt, müssen auch die AAD-Rollen (Azure Active Directory) „Benutzeradministrator“ und „Globaler Administrator“ zugewiesen werden. Weitere Informationen zu AAD-Rollen findest du unter [Berechtigungen für Administratorrollen in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Neuen Benutzer hinzufügen

1. Klicken Sie im Partner Center rechts oben auf das Symbol **Einstellungen**. Wählen Sie dann **Kontoeinstellungen** und anschließend **Benutzerverwaltung** aus.

2. Wählen Sie **Benutzer hinzufügen** aus.

3. Gib den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.

4. Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten. Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt.  Wenn Benutzer eine Rollenzuweisung wünschen, finden sie die zu kontaktierenden globalen Administratoren unter **Benutzerverwaltung** durch Filtern nach „globaler Administrator“.

5. Wählen Sie **Hinzufügen** aus, um das Benutzerkonto zu erstellen. Bestätigen Sie die Details des Benutzers auf der nächsten Seite.

> [!IMPORTANT]  
> Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden. Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können. 

Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden. Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern.

## <a name="assign-user-roles"></a>Zuweisen von Benutzerrollen

Um im Partner Center arbeiten zu können, muss Ihnen eine Rolle zugewiesen sein.  Derzeit gibt es Rollen für Azure Active Directory-Mandanten, Cloud Solution Provider (CSP) und nicht auf AAD bezogene Rollen im Unternehmen. Ein einzelnes Unternehmen kann eine alle diese Rollen benötigen.

>[!Important]
>Benutzer müssen in Ihrem Mandanten aufgeführt sein, um auf das Partner Center zugreifen zu können. Rollenzuweisungen gewähren zusätzliche Zugriffsrechte.

## <a name="next-steps"></a>Nächste Schritte

- [Zuweisen von Rollen und Berechtigungen für Mitarbeiter, die im Partner Center arbeiten müssen](permissions-overview.md)
