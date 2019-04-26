---
title: Erstellen von Benutzerkonten und Festlegen von Berechtigungen (Partner Center im Betrieb über 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: So erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf Partner Center benötigen.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: a96c7fedacbb177c93ae19c5ff4f1a241905be4b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132372"
---
# <a name="create-user-accounts-and-set-permissions"></a>Erstellen von Benutzerkonten und Festlegen von Berechtigungen


**Gilt für**

-   Partner Center-Betreiber ist 21Vianet


Erstellen Sie Benutzerkonten für Ihre Mitarbeiter, die Aufgaben auf Partner Center ausführen müssen. Nur globale oder Management Benutzeradministratoren können Hinzufügen von Benutzern und Zuweisen von Rollen. In **Kontoeinstellungen** &gt; **benutzerverwaltung**, Sie können Benutzerkonten hinzufügen und zuweisen oder Ändern von Berechtigungen.

**Hinzufügen eines neuen Benutzers**

1.  Wechseln Sie im Partner Center, um das dashboardmenü &gt; **Kontoeinstellungen** &gt; **benutzerverwaltung**.

2.  Wählen Sie **Benutzer hinzufügen**.

3.  Geben Sie die vollständigen Namen und die eindeutige e-Mail-Adresse des Benutzers.

4.  Wählen Sie die Rolle und die Zugriffsebene des Mitarbeiters. Partner Center-Zugriff und Berechtigungen basieren auf Rollen, denen können Sie die spezifischen Aufgaben zu steuern, die jeder Mitarbeiter ausführen können. Weitere Informationen zu den Optionen jeder Rolle finden Sie unter [Festlegen von Benutzerberechtigungen](#setuserpermissions).

5.  Wählen Sie **Hinzufügen**, um das Benutzerkonto zu erstellen. Die Seite "Bestätigung" angezeigt wird, Berechtigungen und die Anmeldung Informationen, einschließlich der ein temporäres Kennwort des neuen Benutzers anzeigen.

    >**Wichtig**<br>Wenn neue Benutzer zum Partner Center zum ersten Mal anmelden, müssen sie sich mit ihren temporären Kennwort anmelden. Achten Sie darauf, notieren Sie sich das neue Kennwort des Benutzers temporäre, sodass Sie es später noch mal senden können. Sie wird nicht auf diese Informationen erneut zugreifen können. 

### <a href="" id="setuserpermissions"></a>Die Benutzerberechtigungen festlegen

Zugriff auf Partner Center ist rollenbasiert, was bedeutet, dass Sie die Benutzeransicht, um anzuzeigen, nur die Features und Funktionen, die ein Benutzer benötigt, um bestimmte Aufgaben beschränken können. Sie müssen für jeden Benutzer zwei Einstellungen aktivieren:

-   Die **Agent** Einstellung bestimmt, welche Art von Daten von Kunden und Unternehmen dem Benutzer angezeigt werden kann.

-   Die **Admin** Einstellung wird festgelegt, inwieweit der Benutzer auf Partner Center-Features, Funktionen und Daten hat zugreifen. 

    >**Hinweis**<br>Die Standardeinstellung muss **keine Admin** in den meisten Fällen nur, wenn der Mitarbeiter Berechtigungen für bestimmte administrative Aufgaben erfordert.

####<a name="partner-center-roles-and-associated-permissions"></a>Partner Center-Rollen und Berechtigungen

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>-Rolle im Partner Center</strong></p></td>
<td><p><strong>Was sie tun können</strong></p></td>
<td><p><strong>Was sie nicht möglich</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Administrator-Agents</strong></p></td>
<td><ul>
<li><p>Kundenverwaltung</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Dienstintegrität für den Zugriff für Kunden</p></li>
<li><p>Delegierte Administratorberechtigungen anfordern</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Anzeigen und Herunterladen von Rechnungen und kontenabstimmungsdateien</p></li>
<li><p>Im Auftrag eines Kunden verwalten</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
<td><ul>
<li><p>Benutzerverwaltung</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Handelsvertreter</strong></p></td>
<td><ul>
<li><p>Kundenverwaltung</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Beantragen einer Vertriebspartnerschaft mit einem Kunden</p></li>
<li><p>Kundenvertrag anzeigen</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
<td><ul>
<li><p>Erstellen von Supportanfragen mit 21Vianet für Probleme mit Diensten oder Partner Center</p></li>
<li><p>Dienstintegrität anzeigen</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Anzeigen und Herunterladen von Rechnungen und kontenabstimmungsdateien</p></li>
<li><p>Im Auftrag eines Kunden verwalten</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Helpdesk-Agent</strong></p></td>
<td><ul>
<li><p>Suchen Sie nach Kunden und die Kundendetails anzeigen</p></li>
<li><p>Kundendetails bearbeiten</p></li>
<li><p>Dienstintegrität für den Zugriff für Kunden</p></li>
<li><p>Im Auftrag eines Kunden verwalten</p></li>
</ul></td>
<td><ul>
<li><p>Partnerprofile anzeigen</p></li>
<li><p>Neues Kundenkonto erstellen</p></li>
<li><p>Bearbeiten Sie die Abrechnungsinformationen des Kunden</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Beantragen einer Vertriebspartnerschaft mit einem Kunden</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Kundenvertrag anzeigen</p></li>
<li><p>Anzeigen und Herunterladen von Rechnungen und kontenabstimmungsdateien</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Global admin</strong></p></td>
<td><ul>
<li><p>Können alle Konten und Dienste mit vollständigen Berechtigungen zugreifen.</p></li>
<li><p>Erstellen von Supportanfragen mit 21Vianet für Partner Center-Probleme</p></li>
<li><p>Verträge, Preislisten und Angebote anzeigen</p></li>
<li><p>Anzeigen und Herunterladen von Rechnungen und kontenabstimmungsdateien</p></li>
<li><p>Anzeigen, erstellen und Verwalten von Benutzern für Ihr Unternehmen</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Abrechnungsadministrator</strong></p></td>
<td><ul>
<li><p>Können alle Rechnungen und kontenabstimmungsdateien mit vollständigen Berechtigungen zugreifen.</p></li>
<li><p>Verträge, Preislisten und Angebote anzeigen</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Benutzerverwaltungsadministrator</strong></p></td>
<td><ul>
<li><p>Anzeigen, erstellen und Verwalten von Benutzern für Ihr Unternehmen</p></li>
<li><p>Alle Partnerprofile anzeigen</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

