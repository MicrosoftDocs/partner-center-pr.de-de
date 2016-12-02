---
title: Erstellen von Benutzerkonten und Festlegen von Berechtigungen | Partner Center
description: "Der Administrator erstellt ein Benutzerkonto für jeden Partnermitarbeiter, der Zugriff auf Partner Center benötigt."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 19faea7877a7501b8761b58e084e33f77cf95752

---

# Erstellen von Benutzerkonten und Festlegen von Berechtigungen


Der Administrator erstellt ein Benutzerkonto für jeden Partnermitarbeiter, der Zugriff auf Partner Center benötigt. Diese Aufgaben müssen von einem Administrator durchgeführt werden, der über die Berechtigung **Globaler Administrator** oder **Benutzerverwaltungsadministrator** verfügt. Unter **Kontoeinstellungen** &gt; **Benutzerverwaltung** können Sie Konten hinzufügen und Berechtigungen festlegen bzw. aktualisieren.

**Hinzufügen eines neuen Benutzers**

1.  Wechseln Sie in Partner Center zum Menü „Dashboard“ &gt; **Kontoeinstellungen** &gt; **Benutzerverwaltung**.
2.  Wählen Sie **Benutzer hinzufügen**.

3.  Geben Sie den vollständigen Namen des Benutzers ein, und erstellen Sie eine eindeutige E-Mail-Adresse für den Benutzer.

4.  Wählen Sie den Typ des Agent- und Administratortyp aus. Partner Center verfügt über eine rollenbasierte Benutzeroberfläche, sodass die in diesem Schritt vorgenommene Auswahl die Ansicht des Benutzer so anpasst, dass nur die erforderlichen Funktionen angezeigt werden. Weitere Informationen dazu, welche Möglichkeiten Benutzer mit den jeweiligen Rollen haben, finden Sie unter [Festlegen von Benutzerberechtigungen](#setuserpermissions).

5.  Fügen Sie den Benutzer hinzu. Es wird ein Bestätigungsbildschirm mit einem temporären Kennwort für den neuen Anmeldenamen angezeigt. Sie müssen das Kennwort kopieren und an den neuen Benutzer senden. Nach Verlassen des Bildschirms ist es nicht mehr verfügbar. Wenn der Benutzer sich zum ersten Mal anmeldet, wird er zum Aktualisieren des Kennworts aufgefordert.

### <a href="" id="setuserpermissions"></a>Festlegen von Benutzerberechtigungen

Das Partner Center verfügt über eine rollenbasierte Benutzeroberfläche. Dies bedeutet, dass Sie die Ansicht des Benutzers so ändern können, dass nur die Funktionen angezeigt werden, die der Benutzer für seinen Aufgabenbereich benötigt. Sie müssen für jeden Benutzer zwei Einstellungen aktivieren:

-   Die **Agent**-Einstellung steuert, welche Art von Kundendaten und Microsoft-Informationen dem Benutzer angezeigt werden.

-   Die **Admin**-Einstellung bestimmt, inwieweit der Benutzer die Umgebung von Partner Center sowie alle anderen Microsoft-Dienste (Konten, Profile und Supportanfragen) steuern kann. Diese Einstellung hat auch Auswirkungen außerhalb von Partner Center: Ein Abrechnungsadministrator kann auf alle Rechnungen für alle Microsoft-Dienste zugreifen (auch auf solche, die sich nicht auf CSP beziehen), und ein globaler Administrator hat ebenfalls über CSP hinausgehenden Zugriff auf Benutzerkonten und Kundenkonten.

    Die Standardeinstellung muss immer **Keine Administrator** sein, es sei denn, der Benutzer benötigt diesen zusätzlichen Zugriff tatsächlich im Rahmen seiner Arbeit.

Die folgende Tabelle erläutert die gesamten Aktivitäten, die die einzelnen Rollen in Partner Center durchführen können.

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
<li><p>Beauftragter Administrator</p></li>
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
<li><p>Partnerschaft beantragen</p></li>
<li><p>Potenzielle Kunden verwalten</p></li>
<li><p>Kundenvertrag anzeigen</p></li>
<li><p>Vertragshändler registrieren</p></li>
</ul></td>
<td><ul>
<li><p>Supportanfragen für Dienste oder Partner Center erstellen</p></li>
<li><p>Supportanfragen lösen</p></li>
<li><p>Dienstintegrität anzeigen</p></li>
<li><p>Preise und Angebote anzeigen</p></li>
<li><p>Abrechnung</p></li>
<li><p>Beauftragter Administrator</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Helpdesk-Agent</strong></p></td>
<td><ul>
<li><p>Nach Kunden suchen und anzeigen</p></li>
<li><p>Kundendetails bearbeiten</p></li>
<li><p>Dienstintegrität und Dienstanfragen</p></li>
<li><p>Beauftragter Administrator</p></li>
</ul></td>
<td><ul>
<li><p>Partnerprofile anzeigen</p></li>
<li><p>Neuen Kundeneintrag erstellen</p></li>
<li><p>Rechnungsinformationen des Kunden bearbeiten</p></li>
<li><p>Abonnementverwaltung</p></li>
<li><p>Partnerschaft beantragen</p></li>
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

 

 

 






<!--HONumber=Nov16_HO4-->


