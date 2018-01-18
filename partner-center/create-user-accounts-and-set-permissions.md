---
title: Erstellen von Benutzerkonten und Festlegen von Berechtigungen | Partner Center
description: "Der Administrator erstellt ein Benutzerkonto für jeden Partnermitarbeiter, der Zugriff auf Partner Center benötigt."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
Keywords: roles, permissions,add user, assign role, admin, agent,
ms.openlocfilehash: 4345db8cf8e383edbb58c269a3b0a948eade9d65
ms.sourcegitcommit: 628443b08dde9d2f02553b46e669504c620c3da4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/21/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Erstellen von Benutzerkonten und Zuweisen von Berechtigungen

**Betrifft**

-  Partner Center

Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf Partner Center benötigen. Diese Aufgaben müssen von einem Administrator durchgeführt werden, der über die Berechtigungen eines Benutzerverwaltungsadministrators verfügt. 

>**Hinweis:**<br> Sie haben nun die Möglichkeit, im Partner Center drei neue Rollen zur Verwaltung Ihres Unternehmens zuzuweisen: MPN-Administrator, Administrator für das Unternehmensprofil und Administrator für Empfehlungen. Weiter unten finden Sie unter „Zuweisen von Benutzerberechtigungen” Details zu jeder Rolle.


## <a name="add-a-new-user"></a>Hinzufügen eines neuen Benutzers

1. Wählen Sie im Menü **Dashboard** **Kontoeinstellungen > Benutzerverwaltung**.

2.  Wählen Sie **Benutzer hinzufügen**.

3.  Geben Sie den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.

4.  Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten. Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt. Weiter unten finden Sie nähere Informationen zu den Berechtigungen jeder Rolle.

5.  Wählen Sie **Hinzufügen**, um das Benutzerkonto zu erstellen. Bestätigen Sie die Details des Benutzers auf der nächsten Seite.

>**Wichtig**<br>
Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden. Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können. 

Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden. Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern. 



## <a name="assign-user-permissions"></a>Zuweisen von Benutzerberechtigungen

Der Zugriff auf Partner Center ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt. 

Für jeden Benutzer müssen Sie mindestens eine Berechtigungsstufe zuweisen. Eine dieser Stufen kann die Standardstufe **Verwaltet das Konto Ihrer Organisation als** sein. Wenn Sie einem Benutzer keine Rolle zuweisen, kann er das Partner Center nicht verwenden.

-   Agent-Berechtigungen steuern, welche Art von Kundendaten und Kontoinformationen der Benutzer anzeigen und ändern kann.

-   Administratorberechtigungen steuern die Ebene des Zugriffs, über den der Benutzer für Partner Center-Funktionen verfügt. Diese Einstellung hat auch Auswirkungen außerhalb von Partner Center: Ein Abrechnungsadministrator kann auf alle Rechnungen für alle Microsoft-Dienste zugreifen (auch auf solche, die sich nicht auf CSP beziehen), und ein globaler Administrator hat ebenfalls über CSP hinausgehenden Zugriff auf Benutzerkonten und Kundenkonten.

Die allgemeine Kategorien für Rollen sind: 

- Administrator-Rollen
- Agent-Rollen
- Incentives-Rollen
- Empfehlungs- und Marketing-Rollen

Innerhalb jeder dieser allgemeinen Kategorien kann ein Benutzer nur eine Rolle besitzen, aber derselbe Benutzer kann auch Rollen in den anderen allgemeinen Kategorien erhalten. 

>**Wichtig** Wenn ein Benutzer keine bestimmte Rolle benötigt, übernehmen Sie die Standardeinstellung für **Verwaltet das Konto Ihrer Organisation als**. Jedem Benutzer muss mindestens eine Rolle zugewiesen werden, damit er im Partner Center arbeiten kann.

In der folgende Tabelle wird erläutert, welche Möglichkeiten Benutzer mit den jeweiligen Rollen in Partner Center haben. Berücksichtigen Sie bei der Zuweisung von Rollen, welche Aufgabe ein Benutzer in Ihrer Organisation ausführt. Sie können z.B. den globalen Administrator als Administratoragent einsetzten. Und die für das Marketing zuständige Person könnte auch die Verwaltung des Unternehmensprofils übernehmen.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rolle im Partner Center</strong></p></td>
<td><p><strong>Berechtigungen dieser Rolle</strong></p></td>
</tr>
<tr class="odd">
<td><p><strong>Globaler Administrator</strong></p></td>
<td><ul>
<li><p>Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</p></li>
<li><p>Supportanfragen für Partner Center erstellen</p></li>
<li><p>Verträge, Preislisten und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
<li><p>Partnerbenutzer anzeigen, erstellen und verwalten</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Abrechnungsadministrator</strong></p></td>
<td><ul>
<li><p>Zugriff auf alle Rechnungen von Microsoft mit allen Berechtigungen</p></li>
<li><p>Verträge, Preislisten und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Benutzerverwaltungsadministrator</strong></p></td>
<td><ul>
<li><p>Benutzer anzeigen, erstellen und verwalten</p></li>
<li><p>Alle Partnerprofile anzeigen</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrator für das Unternehmensprofil</strong></p></td>
<td><ul>
<li><p>Anzeigen, Erstellen und Verwalten des Unternehmensprofils </p></li>
<li><p>Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</p></li>
</ul></td>
<tr class="odd">
<td><p><strong>Administrator für Empfehlungen </strong></p></td>
<td><ul>
<li><p>Anzeigen, Erstellen und Verwalten von Unternehmensprofilen</p></li>
<li><p>Empfangen und Verwalten von Empfehlungen</p></li>
<li><p>Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrator für MPN-Partner</strong></p></td>
<td><ul>
<li><p>Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</p></li>
<li><p>Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</p></li>
<li><p>Anzeigen der Daten und Fähigkeiten von Benutzern</p></li>
<li><p>Anzeigen von Kompetenzen</p></li>
<li><p>Anzeigen und Verwalten von Vorteilen</p></li>
<li><p>Anzeigen und Kaufen von MPN-Angeboten</p></li>
<li><p>Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrator für Benutzerverwaltung</strong></p></td>
<td><ul>
<li><p>Anzeigen, erstellen und verwalten von Benutzern</p></li>
<li><p>Anzeigen aller Partnerprofile</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administratoragent</strong></p></td>
<td><ul>
<li><p>Kundenverwaltung</p></li>
<li><p>Liste der Geräte zu Partner Center hinzufügen</p></li>
<p><li>Erstellen und Anwenden von Profilen auf Geräte</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Dienstintegrität und Serviceanfragen für Kunden</p></li>
<li><p>Delegierte Administratorrechte anfordern</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
<li><p>Im Auftrag eines Kunden verwalten</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Vertriebsbeauftragter</strong></p></td>
<td><ul>
<li><p>Kundenverwaltung</p></li>
<li><p>Liste der Geräte zu Partner Center hinzufügen</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Supportanfragen anzeigen</p></li>
<li><p>Beantragen einer Partnerschaft mit einem Kunden</p></li>
<li><p>Potenzielle Kunden verwalten</p></li>
<li><p>Kundenvertrag anzeigen</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Helpdesk-Agent</strong></p></td>
<td><ul>
<li><p>Nach Kunden suchen und anzeigen</p></li>
<li><p>Kundendetails bearbeiten</p></li>
<li><p>Unterstützten der Lösung von Kunden bei Problemen mit der Abrechnung oder der Abonnementverwaltung</p></li>
<li><p>Anfordern von Support im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office365-Abonnements sein.)</p></li>
<li><p>Verwalten von Abonnements und Diensten im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office365-Abonnements sein.)</p></li>
</ul></td>
</tr>
 

 

 



