---
title: Erstellen von Benutzerkonten und Festlegen von Berechtigungen | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Der Administrator erstellt ein Benutzerkonto für jeden Partnermitarbeiter, der Zugriff auf Partner Center benötigt.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.author: evansma
Keywords: Rollen, Berechtigungen, Benutzer hinzufügen, Rolle zuweisen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 3829a18a78cb50797b7ca2bfd862c82d93d92248
ms.sourcegitcommit: f916aa2884239b205398c24d04d1f1dc41b63c2b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2019
ms.locfileid: "64667916"
---
# <a name="create-user-accounts-and-assign-permissions"></a>Erstellen von Benutzerkonten und Zuweisen von Berechtigungen

Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf das Partner Center benötigen. Diese Aufgaben müssen von einem Administrator für die Benutzerverwaltung, Kontoadministrator oder vom globalen Administrator durchgeführt werden. 


## <a name="add-a-new-user"></a>Hinzufügen eines neuen Benutzers

1. Klicken Sie im Partner Center rechts oben auf das Symbol **Einstellungen** und dann auf **Benutzerverwaltung**.

2.  Wählen Sie **Benutzer hinzufügen** aus.

3.  Geben Sie den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.

4.  Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten. Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt.  Wenn Benutzer eine Rollenzuweisung wünschen, finden sie die zu kontaktierenden Kontoadministratoren unter **Benutzerverwaltung** durch Filtern nach Kontoadministrator.

5.  Wählen Sie **Hinzufügen** aus, um das Benutzerkonto zu erstellen. Bestätigen Sie die Details des Benutzers auf der nächsten Seite.

> [!IMPORTANT]  
> Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden. Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können. 

Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden. Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern. 

> [!NOTE]  
>  Wenn der globale Administrator Ihr Unternehmen verlassen hat oder intern versetzt wurde und Sie einen neuen globalen Administrator hinzufügen müssen, müssen Sie im [MPN-Portal](https://partner.microsoft.com/support) eine Serviceanfrage stellen. Der Support-Mitarbeiter kann eine Heraufstufung eines Benutzers zum globalen Administrator beantragen, wenn der Antragsteller die benötigten persönlichen Identitätsinformationen sowie zusätzliche Informationen zu Ihrer Organisation bereitstellen kann.

## <a name="assign-user-roles"></a>Zuweisen von Benutzerrollen

Um im Partner Center arbeiten zu können, muss Ihnen eine Rolle zugewiesen sein.  Derzeit gibt es Rollen für Azure Active Directory-Mandanten, Cloud Solution Provider (CSP) und nicht auf AAD bezogene Rollen im Unternehmen. Ein einzelnes Unternehmen kann eine alle diese Rollen benötigen.

>[!Important]
>Benutzer müssen in Ihrem Mandanten aufgeführt sein, um auf das Partner Center zugreifen zu können. Rollenzuweisungen gewähren zusätzliche Zugriffsrechte.


**AAD-Mandantenrollen**:
- Globaler Administrator
- Benutzeradministrator

**CSP-Rollen**:
- Administratoragent
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



### <a name="find-your-global-admin"></a>Finden des globalen Administrators

Es kann vorkommen, dass ein Benutzer seine Rolle ändern lassen muss oder ein neuer Benutzer eine Zuweisung zu einer bestimmten Rolle wünscht.  
Um einen globalen Administrator zu finden, der Rollenänderungen vornehmen oder einem neuen Benutzer Rollen zuweisen kann, klicken Sie rechts oben im Partner Center auf das Symbol **Einstellungen**, wählen Sie **Benutzerverwaltung** aus, und filtern Sie nach „Globaler Administrator“. 







