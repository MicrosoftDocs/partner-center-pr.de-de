---
title: Erstellen von Benutzerkonten und Festlegen von Berechtigungen | Partner Center
description: "Der Administrator erstellt ein Benutzerkonto für jeden Partnermitarbeiter, der Zugriff auf Partner Center benötigt."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: 920f4590f94fbcc382286b206b532fcb204166be
ms.sourcegitcommit: b8146a4a959ef26efc09ead1788ff5e264ae121e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/25/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Erstellen von Benutzerkonten und Zuweisen von Berechtigungen

**Betrifft**

-  Partner Center

Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf Partner Center benötigen. Diese Aufgaben müssen von einem Administrator durchgeführt werden, der über die Berechtigungen eines Benutzerverwaltungsadministrators verfügt. 

## <a name="add-a-new-user"></a>Hinzufügen eines neuen Benutzers

1. Wählen Sie im Menü **Dashboard** **Kontoeinstellungen > Benutzerverwaltung**.

2.  Wählen Sie **Benutzer hinzufügen**.

3.  Geben Sie den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.

4.  Wählen Sie den Agent- und Administratortyp aus. Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt. Weitere Informationen dazu, welche Möglichkeiten Benutzer mit den jeweiligen Rollen haben, finden Sie unter [Zuweisen von Benutzerberechtigungen](#assignuserpermissions).

5.  Wählen Sie **Hinzufügen**, um das Benutzerkonto zu erstellen. Bestätigen Sie die Details des Benutzers auf der nächsten Seite.

>**Wichtig**<br>
Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden. Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können. <br>

>Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden. Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern.    


### <a href="" id="assignuserpermissions"></a>Zuweisen von Benutzerberechtigungen

Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt. 

Sie müssen für jeden Benutzer zwei Berechtigungsstufen auswählen:

-   Agent-Berechtigungen steuern, welche Art von Kundendaten und Kontoinformationen der Benutzer anzeigen und ändern kann.

-   Administratorberechtigungen steuern die Ebene des Zugriffs, über den der Benutzer für Partner Center-Funktionen verfügt. Diese Einstellung hat auch Auswirkungen außerhalb von Partner Center: Ein Abrechnungsadministrator kann auf alle Rechnungen für alle Microsoft-Dienste zugreifen (auch auf solche, die sich nicht auf CSP beziehen), und ein globaler Administrator hat ebenfalls über CSP hinausgehenden Zugriff auf Benutzerkonten und Kundenkonten.

>**Wichtig** Die Standardeinstellung sollten immer **No admin** sein, es sei denn, der Benutzer benötigt diesen zusätzlichen Zugriff tatsächlich im Rahmen seiner Arbeit.

In der folgende Tabelle wird erläutert, welche Möglichkeiten Benutzer mit den jeweiligen Rollen in Partner Center haben.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rolle im Partner Center</strong></p></td>
<td><p><strong>Was diese Rolle kann</strong></p></td>
<td><p><strong>Was diese Rolle nicht kann</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Administratoragent</strong></p></td>
<td><ul>
<li><p>Kundenverwaltung</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Dienstintegrität und Serviceanfragen für Kunden</p></li>
<li><p>Delegierte Administratorrechte anfordern</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
<li><p>Im Auftrag eines Kunden verwalten</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
<td><ul>
<li><p>Benutzerverwaltung</p></li>
<li><p>Serviceanfragen für Partner Center</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Vertriebsbeauftragter</strong></p></td>
<td><ul>
<li><p>Kundenverwaltung</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Supportanfragen anzeigen</p></li>
<li><p>Beantragen einer Partnerschaft mit einem Kunden</p></li>
<li><p>Potenzielle Kunden verwalten</p></li>
<li><p>Kundenvertrag anzeigen</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
<td><ul>
<li><p>Serviceanfragen für Probleme mit Partner Center erstellen</p></li>
<li><p>Supportanfragen lösen</p></li>
<li><p>Dienstintegrität anzeigen</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
<li><p>Im Auftrag eines Kunden verwalten</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Helpdesk-Agent</strong></p></td>
<td><ul>
<li><p>Nach Kunden suchen und anzeigen</p></li>
<li><p>Kundendetails bearbeiten</p></li>
<li><p>Dienstintegrität</p></li>
<li><p>Anfordern von Support im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office365-Abonnements sein.)</p></li>
<li><p>Verwalten von Abonnements und Diensten im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office365-Abonnements sein.)</p></li>
</ul></td>
<td><ul>
<li><p>Partnerprofile anzeigen</p></li>
<li><p>Neues Kundenkonto erstellen</p></li>
<li><p>Rechnungsinformationen des Kunden bearbeiten</p></li>
<li><p>Abonnements verwalten</p></li>
<li><p>Beantragen einer Partnerschaft mit einem Kunden</p></li>
<li><p>Potenzielle Kunden verwalten</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Kundenvertrag anzeigen</p></li>
<li><p>Abrechnung</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
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
<td></td>
</tr>
<tr class="even">
<td><p><strong>Abrechnungsadministrator</strong></p></td>
<td><ul>
<li><p>Zugriff auf alle Rechnungen von Microsoft mit allen Berechtigungen</p></li>
<li><p>Verträge, Preislisten und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Benutzerverwaltungsadministrator</strong></p></td>
<td><ul>
<li><p>Benutzer anzeigen, erstellen und verwalten</p></li>
<li><p>Alle Partnerprofile anzeigen</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

 

 

 



