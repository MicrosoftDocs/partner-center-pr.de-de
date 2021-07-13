---
title: Auszahlungs- und Steuerprofile in Partner Center
ms.topic: how-to
ms.date: 04/15/2021
description: Erstellen und verwalten Sie Ihr Auszahlungs- und Steuerprofil, damit Sie für Ihre Incentives-Arbeit bezahlt werden können. Umfasst das Erstellen, Verwalten und Verwenden verschiedener Profile.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684252"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Incentives-Auszahlungs- und Steuerprofilen in Partner Center

**Geeignete Rollen:** Incentivesadministrator | Kontoadministrator-| Globaler Administrator

Bevor Sie Zahlungen für Ihre Incentives-Programme für einen bestimmten MPN-Standort erhalten können, müssen Sie Ihre Registrierung abschließen, indem Sie ein gültiges Auszahlungs- und Steuerprofil mit dem Programm und MPN-Standort verknüpfen. Microsoft nutzt dieses Auszahlungs- und Steuerprofil zur Ausstellung von Zahlungen. Je nach Regeln des Incentives-Programms kann es Ihnen gestattet sein, für die Zahlung eine elektronische Banküberweisung oder eine Gutschrift zu nutzen. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Rollen, Währungen und mehrere Microsoft Incentive-Programme

Es ist wichtig, die unten angegebenen Informationen zu verstehen, bevor Sie mit Ihrem Auszahlungs- und Steuerprofil beginnen.

### <a name="roles-and-permissions"></a>Rollen und Berechtigungen

Sie müssen Incentiveadministrator sein, um Bank- und Steuerinformationen für Incentivezahlungen einzugeben. Wenn Sie MPN-/Kontoadministrator sind, können Sie sich selbst und/oder einen Kollegen als Incentives-Administrator zuweisen.

Wenn Sie Incentives-Administratorberechtigungen anfordern müssen, wenden Sie sich an Ihren MPN-Administrator oder globalen Administrator. Sie können herausfinden, wer in Ihrem Unternehmen über diese Rollen verfügt, indem Sie sich beim [Partner Center Dashboard](https://partner.microsoft.com/dashboard/)anmelden. Wählen Sie im **symbol Einstellungen** oben rechts die Option **Benutzerverwaltung** aus, und filtern Sie dann nach Globaler Administrator.

Incentives Benutzer können Incentive-Einnahmen und Zahlungsdetails und -berichte anzeigen, aber keine Bank- und Steuerdetails bearbeiten.

### <a name="choose-your-disbursement-currency"></a>Auswählen Ihrer Auszahlungswährung

Incentivezahlungen erfolgen in der Währung, die Sie beim Einrichten Ihres Zahlungsprofils ausgewählt haben. Die Zahlungen werden anhand eines Wechselkurses berechnet, der von Microsoft monatlich festgelegt wird. Sie sind für alle Wertänderungen aufgrund der ausgewählten Währung verantwortlich.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Verwenden verschiedener Profile für verschiedene Microsoft-Programme

Wenn Ihr Unternehmen in mehreren Incentiveprogrammen registriert ist, können Sie für alle dasselbe Zahlungskonto verwenden oder verschiedene Zahlungskonten für verschiedene Programme verwenden.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Auszahlungs- und Steuerprofilen im Partner Center

Die folgenden Abschnitte führen Sie durch das Erstellen und Verwalten von Zahlungs- und Steuerprofilen in Partner Center.

>[!IMPORTANT]
>Sie müssen Incentiveadministrator sein, um Zahlungs- und Steuerprofile in Partner Center zu erstellen oder zu verwalten. Incentiverollen müssen jedem MPN-Standort unter jedem Incentive-Programm zugewiesen werden. Weitere Informationen zum Hinzufügen von Incentive-Administratoren in Partner Center finden Sie unter [Erstellen von Benutzerkonten.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Zugreifen auf den Auszahlungs- und Steuerabschnitt in Partner Center

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) mit Ihrem Azure Active Directory-Konto (Azure AD) (Unternehmenskonto) oder der entsprechenden E-Mail-Adresse an, falls eine zugewiesen wurde.

   - Mehrere Domänen können innerhalb eines Azure AD Kontos registriert werden. Wenden Sie sich an Ihren globalen Administrator, um zu ermitteln, welche Domänen zugeordnet sind.
   - Wenn Sie sich nur mit der Domäne anmelden können @onmicrosoft.com und zusätzliche Domänen benötigen, wenden Sie sich an Ihren Kontoadministrator, um dem Azure AD Konto weitere Domänen hinzuzufügen.
   - Wenn Sie aufgefordert werden, **ein Arbeits-, Schul- oder Schulkonto** oder **ein persönliches Konto** auszuwählen, wählen Sie **Arbeits- oder Schulkonto** aus.

2. Wählen Sie das Zahnradsymbol aus, um das **menü Einstellungen** zu öffnen, und wählen Sie dann **Kontoeinstellungen** aus.

3. Wählen Sie im Menü **Kontoeinstellungen** die Option **Auszahlung und Steuern** aus.

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Zuweisen von Auszahlungs- und Steuerprofilen zu einzelnen Programmen

1. Melden Sie sich beim [Partner Center Dashboard](https://partner.microsoft.com/dashboard/)an, und wählen Sie dann das Zahnradsymbol aus, um das **menü Einstellungen** zu öffnen. 

2. Wählen Sie **Kontoeinstellungen** aus, erweitern Sie den **Abschnitt Auszahlung und Steuern,** und wählen Sie dann **Auszahlungs- und Steuerprofilzuweisung aus.** 
   
   Eine Liste der Programme wird angezeigt. Wählen Sie den Pfeil neben einem Programm aus, um Profildetails anzuzeigen. 

3. Wählen Sie im Dropdownmenü **Steuerprofil** das gewünschte Steuerprofil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet.  Wählen Sie im Popupfenster **Weiter** aus. Der Prozess zum Erstellen eines neuen Steuerprofils ist unten angegeben.

4. Wählen Sie **Zahlungsmethode** aus.

   - Wenn Sie **Electronic Bank Transfer** als Zahlungsmethode ausgewählt haben, wählen Sie das gewünschte Zahlungsprofil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet. Wählen Sie im Popupfenster Weiter aus. Der Prozess zum Erstellen eines neuen Zahlungsprofils wurde unten bereitgestellt.

   - Wenn Sie **Gutschrift** als Zahlungsmethode ausgewählt haben, schließen Sie die Überprüfung ab. Dadurch wird bestätigt, dass die sap-Nummer, auf die verwiesen wird, zu Ihrer Organisation gehört.

    >[!NOTE]
    >Wenn mehrere Microsoft-Geschäftsentitäten aufgeführt sind, müssen Sie für jede Entität ein Zahlungsprofil auswählen.

    >[!NOTE]
    >Die Verfügbarkeit der Zahlungsmethode hängt von den Regeln des Incentiveprogramms ab.

    - Wenn Die MPN-ID Ihres Standorts von einer lokalen Microsoft-Niederlassung für ein bestimmtes Incentiveprogramm bezahlt wird und die Gutschrift für LRD (Distributor mit begrenztem Risiko) als Zahlungsmethode zulässt, wird Ihr Zahlungsprofil mit der Zahlungsmethode LRD-Gutschrift vorab aufgefüllt. In der Zeile mit der Zahlungsmethode für die LRD-Gutschrift für das jeweilige Incentive-Programm und die MPN-ID des Standorts wird im Abschnitt Zahlungsprofil der Status **Bestätigt** oder **Überprüfung erforderlich** angezeigt.
    
       Wählen Sie **Überprüfung erforderlich** aus, um die Details der CSP-Mandanten-ID zu bestätigen und zu überprüfen, die dem STANDORT-MPN und der Zahlungsmethode zugeordnet sind, um die Gutschriftzahlung zu erhalten. Überprüfen Sie im Dialogfeld **Gutschriftendetails,** ob die CSP-Mandanten-ID und die angegebenen Details korrekt sind. Wenn Mehrere Mandanten-IDs angezeigt werden, wählen Sie die CSP-Mandanten-ID, für die Sie Zahlungen erhalten möchten, sorgfältig aus. Wählen Sie als Nächstes **Bestätigen** aus, um zu bestätigen, dass Ihre Unternehmensdetails korrekt sind und dass die Incentivezahlung an die von Ihnen ausgewählte CSP-Mandanten-ID erfolgen soll.
 
      Wenn als Status **Bestätigt** angezeigt wird, wurde die Zuweisung der CSP-Mandanten-ID abgeschlossen, und es ist keine weitere Aktion erforderlich. Sie können weiterhin Bestätigt auswählen, um die Details der Zuweisung anzuzeigen.
   
      In Ländern, in denen Partner explizit eine Steuerausnahme anfordern müssen, gibt es neben dem Steuerprofil im Steuerprofilabschnitt des Incentive-Programms und des MpN für Standorte eine Option zum Anwenden der Steuerausnahme. Wenn Sie dieses Kontrollkästchen aktivieren, werden Steuerausnahmevorteile auf Ihren Incentive-Gutschrifthinweis angewendet. 
   
      Derzeit ist die Zahlungsmethode LRD Credit Note nur für Partner aus Australien, Neuseeland und Kanada für das Microsoft Commerce Incentive-Programm verfügbar. Wenn Sie Direktabrechnungspartner oder indirekter Anbieter in diesen drei Ländern sind, die für das MCI-Programm registriert sind und die LRD-Gutschrift nicht als verfügbare Zahlungsmethode angezeigt wird, vergewissern Sie sich, dass Ihre Mandanten-ID dem entsprechenden MPN-Standortkonto des Partners zugeordnet ist. Weitere Informationen hierzu finden Sie unter [Aktualisieren Ihres Organisationsprofils.](update-your-partner-profile.md)

    
5. Wählen Sie **die Währung aus.**

6. Wenn Sie alle Zahlungsfelder ausgefüllt haben, wählen Sie **Übermitteln** aus.

## <a name="set-up-a-default-bank-profile"></a>Einrichten eines Standardbankprofils

Sie können Standardbankprofile einrichten und diese MPN-Standorten zuweisen. Diese Standardprofile werden von Microsoft für nachfolgende Registrierungen für die entsprechenden MPN-Standorte verwendet. 

1. Melden Sie sich beim [Partner Center Dashboard](https://partner.microsoft.com/dashboard/)an, und wählen Sie dann das Zahnradsymbol aus, um das **menü Einstellungen** zu   öffnen. 

2. Wählen Sie **Kontoeinstellungen** aus, erweitern Sie den Abschnitt **Auszahlung und Steuern,** und wählen Sie dann **Auszahlungs- und Steuerprofile aus.** 

3. Wählen Sie im Abschnitt **Zahlungsprofile** die Option **Standardprofile verwalten** aus. 

4. Um ein Standardbankprofil zu erstellen, wählen **Sie Standardbankprofil hinzufügen** aus. 

5. Wählen Sie ein Bankprofil aus der Liste der verfügbaren Bankprofile Ihres Unternehmens aus, wählen Sie die Währung aus, die mit diesem Bankprofil verwendet werden soll, und wählen Sie dann die Liste der MPN-Standorte aus, für die dieses Standardprofil gelten soll.

6. Wählen Sie **Fertig** aus, nachdem Sie die Auswahl abgeschlossen haben. Auf die Schaltfläche Fertig kann erst geklickt werden, nachdem alle erforderlichen Felder abgeschlossen wurden. 

>[!NOTE]
>Die gleiche Bank- und Währungspaarung kann auf mehrere Standorte angewendet werden. Wenn dem Standort-MPN einmal eine Standardprofil- und Währungskombination zugewiesen wurde, wird es für zukünftige Standardprofilzuweisungen nicht mehr in der Standortdropdownliste angezeigt. Wenn die Standardauswahl gelöscht wird, wird der Standort-MPN für zukünftige Standardprofilzuweisungen erneut angezeigt. Jede Kombination aus Bankprofil und Währung wird als eindeutige, bearbeitbare Zeile hinzugefügt.

7. Nachdem alle erforderlichen Änderungen hinzugefügt wurden, wählen Sie **Speichern** aus.  

## <a name="create-your-bank-profile"></a>Erstellen Ihres Bankprofils

Bankprofile werden auf Unternehmensebene erstellt. Dadurch kann ein Bankprofil über mehrere MPN-IDs und Incentive-Programme innerhalb eines Unternehmens hinweg zugewiesen werden. Es kann Ausnahmen geben, wenn das Bankprofil auf verschiedene Länder angewendet wird, da unterschiedliche Bank- und Steuerregeln gelten können.

>[!NOTE]
>Auf den folgenden Seiten sind Felder mit einem Sternchen erforderlich. Wenn Sie nicht wissen, was ein Feld ist, wählen Sie das Informationssymbol aus. 

1. Füllen Sie auf der Seite **Details** die folgenden Felder aus: **Profilname:** Geben Sie einen eindeutigen Namen ein, um dieses Zahlungsprofil zu identifizieren.
    **Speicherort des Bankkontos:** Das Land, in dem sich die Bank Ihres Unternehmens befindet.
    **Zahlungsmethode:** Die bevorzugte Zahlungsmethode für Partner Center ist die elektronische Bankübertragung.

2. Wählen Sie **Weiter** aus.

3. Geben Sie auf der Seite **Bankkonto** Ihre Informationen ein. Die auf dieser Seite angezeigten Felder variieren je nach Land. 

4. Wählen Sie **Weiter** aus.

5. Geben Sie auf der Seite **"12"** die entsprechenden Informationen ein. Dies ist die Person in Ihrem Unternehmen, an die sich die Bank wenden würde, wenn sie Ihr Konto besprechen muss.

6. Wenn die Felder abgeschlossen sind, wählen **Sie Fertig stellen** und dann **Bestätigen** aus, um Ihr Bankprofil zu erstellen.

Sie werden zur Seite **Auszahlungs- und Steuerprofile** umgeleitet. Der Status Ihres neuen Profils gibt Ausstehende **Microsoft-Überprüfung an,** bis die Überprüfung abgeschlossen ist. Dieser Vorgang kann bis zu 48 Stunden dauern. Sobald die Überprüfung abgeschlossen ist, wird der Profilstatus entweder **Genehmigt oder** Aktion **erforderlich angezeigt.** Wenn **Aktion erforderlich ist,** wiederholen Sie die obigen Schritte, und geben Sie die erforderlichen Informationen an. 

## <a name="create-your-tax-profile"></a>Erstellen Ihres Steuerprofils

Verwenden Sie das folgende Verfahren, um Microsoft die für Ihre Organisation erforderlichen Steuerinformationen zur Verfügung zu stellen. Die Seiten in diesem Abschnitt sind dynamisch und variieren je nach Land oder Region. Wenn Sie Hilfe bei der Identifizierung der richtigen Steuerinformationen benötigen, wenden Sie sich an die entsprechenden Behörden in Ihrem Land.

Für Partnerunternehmen in Nordamerika: Wenn Sie Informationen zum Ausfüllen der W8- oder W9-Formulare benötigen, werden Sie über die folgenden Adressen auf die IRS-Website übertragen:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Geben Sie nur Details für Ihr Unternehmen ein. Geben Sie niemals persönliche Details ein.

1. Füllen Sie **auf der Seite** Geschäftsprofil die erforderlichen Felder aus, und wählen Sie dann Weiter **aus.** 

2. Wählen Sie **auf der** Seite Setup die Option aus, die für Ihr Unternehmen gilt.

   - Wählen Sie die Option auf der linken Seite aus, wenn Ihr Unternehmen nur in die USA integriert ist oder wenn dieses Profil für eine Einzelperson gilt.
   - Wählen Sie die Option auf der rechten Seite aus, wenn Ihr Unternehmen außerhalb des USA ist, und wählen Sie dann Ihr Land/Ihre Region aus der Liste aus.

3. Wählen Sie **Weiter** aus. 

4. Geben Sie **auf der Seite Steuerstatus** die erforderlichen Informationen ein, und wählen Sie dann **Weiter aus.** Die Felder auf dieser Seite variieren je nach Land. Ihre Details. 

5. Geben Sie auf **der Seite Zusätzliche** Dokumentation die erforderlichen Felder ein, und wählen Sie Weiter **aus.** 

6. Wählen **Sie Durchsuchen** aus, um alle Dokumente hochzuladen, die für Ihr Land oder Ihre Region erforderlich sind. Wenn der Dokumentname angezeigt wird, wählen Sie **Hochladen.** 

7. Wenn Sie das Dokument entfernen müssen, wählen Sie **Entfernen aus.**

8. Klicken Sie zum Speichern und Fortfahren auf **Fertig stellen.**

9. Wählen **Sie in** der Popupmeldung Bestätigen aus. Sie werden zurück zur Einrichtungsseite **auszahlungs- und steuerlich** genommen.
 
## <a name="update-expired-tax-profiles"></a>Aktualisieren abgelaufener Steuerprofile

1. Melden Sie sich [beim Partner Center Dashboard](https://partner.microsoft.com/dashboard/)an, und wählen Sie dann das Zahnradsymbol aus, um das Menü **Einstellungen** öffnen.

1. Wählen **Sie Kontoeinstellungen** aus, erweitern Sie den Abschnitt **Auszahlung und** Steuern, und wählen Sie dann **Auszahlungs- und Steuerprofil aus.**

1. Wählen Sie **Steuerprofil aus.**

1. Überprüfen Sie die Spalte **Ablaufdatum,** und navigieren Sie zu dem Steuerprofil, das abgelaufen ist oder abläuft.

1. Wählen Sie **Bearbeiten** aus.

1. Aktualisieren Sie im Abschnitt "Steuerformular" die Steuerformulare, indem Sie die neuen Details bereitstellen. 

## <a name="next-steps"></a>Nächste Schritte

- [Häufig gestellte Fragen zu Auszahlungen und Steuern](payout-faq.yml)
