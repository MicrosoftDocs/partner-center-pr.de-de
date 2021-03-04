---
title: Auszahlungs- und Steuerprofile in Partner Center
ms.topic: how-to
ms.date: 02/24/2021
description: Erstellen und verwalten Sie Ihr Auszahlungs-und Steuer Profil, damit Sie für Ihre Incentives kostenpflichtig sind. Umfasst das Erstellen, verwalten und Verwenden von unterschiedlichen Profilen.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ba8c1a811d66a5e6233f625c3981283341ea546c
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756587"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Auszahlungs-und Steuer Profilen für die Anreize im Partner Center


**Geeignete Rollen:**

- Incentiveadministrator
- Kontoadministrator
- Globaler Administrator

Bevor Sie Zahlungen für Ihre Incentives-Programme für einen bestimmten MPN-Standort erhalten können, müssen Sie Ihre Registrierung abschließen, indem Sie ein gültiges Auszahlungs- und Steuerprofil mit dem Programm und MPN-Standort verknüpfen. Microsoft nutzt dieses Auszahlungs- und Steuerprofil zur Ausstellung von Zahlungen. Je nach Regeln des Incentives-Programms kann es Ihnen gestattet sein, für die Zahlung eine elektronische Banküberweisung oder eine Gutschrift zu nutzen. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Rollen, Währungen und andere Microsoft-Programme

Es ist wichtig, die folgenden Informationen zu verstehen, bevor Sie mit Ihrem Auszahlungs-und Steuer Profil beginnen.

### <a name="roles-and-permissions"></a>Rollen und Berechtigungen

Sie müssen ein Administrator der Administrator sein, um Bank-und Steuerinformationen für Incentive-Zahlungen einzugeben. Wenn Sie ein MPN/Konto-Administrator sind, können Sie sich selbst und/oder einen Kollegen als Administrator für Administratoren zuweisen.

Wenn Sie Administrator Berechtigungen für Incentives anfordern müssen, wenden Sie sich an den MPN-Administrator oder den globalen Administrator. Sie können herausfinden, wer in Ihrem Unternehmen über diese Rollen verfügt, indem Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)anmelden. Wählen Sie oben rechts im Symbol " **Einstellungen** " die Option **Benutzerverwaltung** aus, und Filtern Sie dann nach globaler Administrator.

Incentives: Benutzer können die Informationen zu den Incentive-und Zahlungsdetails und-Berichten anzeigen, aber keine Bank-und Steuer Details bearbeiten.

### <a name="choose-your-disbursement-currency"></a>Wählen Sie Ihre Auszahlungs Währung aus.

In der Währung, die Sie beim Einrichten Ihres Zahlungs Profils ausgewählt haben, werden Incentive-Zahlungen erhoben. Zahlungen werden mit einem Exchange-Satz berechnet, der monatlich von Microsoft festgelegt wird. Aufgrund der ausgewählten Währung sind Sie für alle Änderungen am Wert verantwortlich.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Verwenden verschiedener Profile für verschiedene Microsoft-Programme

Wenn Ihr Unternehmen in mehreren Incentive-Programmen registriert ist, können Sie das gleiche Zahlungskonto für alle verwenden, oder Sie können unterschiedliche Zahlungskonten für verschiedene Programme verwenden.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Auszahlungs- und Steuerprofilen im Partner Center

In den folgenden Abschnitten werden die Schritte zum Erstellen und Verwalten von Zahlungs-und Steuer Profilen in Partner Center erläutert.

>[!IMPORTANT]
>Sie müssen ein Incentive-Administrator sein, um Zahlungs Profile in Partner Center zu erstellen oder zu verwalten. Incentive-Rollen müssen jedem MPN-Speicherort unter jedem Incentive-Programm zugewiesen werden. Weitere Informationen zum Hinzufügen von Incentive-Administratoren in Partner Center finden Sie unter [Erstellen von Benutzerkonten](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Zugriff auf den Abschnitt "Auszahlungs-und Steuer Berechtigung" im Partner Center

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) mit Ihrem Azure Active Directory (Azure AD)-Konto (Firmenkonto) oder der entsprechenden e-Mail-Adresse an, wenn eine zugewiesen wurde.

   - Mehrere Domänen können innerhalb eines Azure AD Kontos registriert werden. Wenden Sie sich an ihren globalen Administrator, um die zugeordneten Domänen zu ermitteln
   - Wenn Sie sich nur bei der Domäne anmelden können, wenden Sie sich an @onmicrosoft.com Ihren Konto Administrator, um dem Azure AD Konto zusätzliche Domänen hinzuzufügen.
   - Wenn Sie aufgefordert werden, Geschäfts-, **Schul** -oder unikonto oder **persönliches Konto** auszuwählen, wählen Sie Geschäfts- **oder Schul Konto** aus.

2. Wählen Sie das Zahnrad Symbol aus, um das Menü **Einstellungen** zu öffnen, und wählen Sie dann **Kontoeinstellungen** aus.

3. Wählen Sie im Menü **Kontoeinstellungen** die Option **Auszahlung und Steuern** aus. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Zuweisen von Auszahlungs-und Steuer Profilen zu einzelnen Programmen

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an, und wählen Sie das Zahnrad Symbol aus, um das Menü " **Einstellungen** " zu öffnen. 

2. Wählen Sie **Kontoeinstellungen** aus, erweitern Sie den **Abschnitt Auszahlung und Steuern**, und wählen Sie dann **Auszahlungs-und Steuer Profil Zuweisung** aus. 
   
   Eine Liste der Programme wird angezeigt. Wählen Sie den Pfeil neben einem Programm aus, um die Profildetails anzuzeigen. 

3. Wählen Sie im Dropdown Menü **Steuer Profil** das gewünschte Steuer Profil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet.  Wählen Sie im Popup Fenster fortsetzen aus. Der Prozess zum Erstellen eines neuen Steuer Profils wurde unten bereitgestellt.

4. Wählen Sie **Zahlungsmethode** aus.

   - Wenn Sie **Electronic Bank Transfer** als Zahlungsmethode ausgewählt haben, wählen Sie das gewünschte Zahlungsprofil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet. Wählen Sie im Popup Fenster fortsetzen aus. Der Prozess zum Erstellen eines neuen Zahlungs Profils wurde unten bereitgestellt.

   - Wenn Sie **Guthaben Hinweis** als Zahlungsmethode ausgewählt haben, schließen Sie die Überprüfung ab. Dadurch wird bestätigt, dass die referenzierte SAP-Nummer zu Ihrer Organisation gehört.

    >[!NOTE]
    >Wenn mehrere Microsoft-Geschäfts Entitäten aufgelistet sind, müssen Sie ein Zahlungsprofil für jede Entität auswählen.

    >[!NOTE]
    >Die Verfügbarkeit der Zahlungsmethode hängt von den Regeln des Incentive-Programms ab.

    - Wenn Ihre Speicherort-MPN-ID von einer lokalen Microsoft-Niederlassung für ein bestimmtes Incentive-Programm gezahlt wird und LRD-Guthaben (Limited Risk Distributor) als Zahlungsmethode zulässt, wird Ihr Zahlungsprofil mit der Zahlungsmethode für die LRD-Gutschrift vorab ausgefüllt. In der LRD-Gutschrift Zahlungsmethode für die entsprechende MPN-ID des Incentive-Programms und des Standorts wird die **Bestätigung** oder über **Prüfung** als Status im Abschnitt Zahlungsprofil angezeigt.
    
       Wählen Sie über **Prüfung erforderlich** aus, um die Details der CSP-Mandanten-ID zu bestätigen und zu überprüfen, die dem Speicherort MPN und der Zahlungsmethode zugeordnet sind, um die Zahlungs Notiz Überprüfen Sie im Dialogfeld **Details zum Kredit Hinweis** , ob die ID des CSP-Mandanten und die angegebenen Details richtig sind. Wenn Sie mehr als eine Mandanten-ID haben, wählen Sie die CSP-Mandanten-ID, für die Sie Zahlungen erhalten möchten, sorgfältig aus. Wählen Sie als nächstes bestätigen aus, um zu **bestätigen** , dass Ihre Unternehmens Details richtig sind, und dass die Incentive-Zahlung an die von Ihnen ausgewählte CSP-Mandanten-ID vorgenommen werden soll.
 
      Wenn der Status **bestätigt** angezeigt wird, wurde die Zuweisung der CSP-Mandanten-ID abgeschlossen, und es ist keine weitere Aktion erforderlich. Sie können weiterhin bestätigt auswählen, um die Details der Zuweisung anzuzeigen.
   
      In Ländern, in denen Partner explizit anfordern müssen, eine Steuerbefreiung anzuwenden, gibt es eine Option zum Anwenden von Steuer Ausnahmen neben dem Steuer Profil im Steuer Profilabschnitt des Incentive-Programms und des Standort-MPN. Wenn Sie dieses Kontrollkästchen aktivieren, werden die Vorteile der Tax-Ausnahme auf Ihre Incentive-Gutschrift 
   
      Diese Zahlungsmethode ist derzeit nur für die Partner von Australien, Neuseeland und Kanada für das Microsoft Commerce Incentive-Programm verfügbar. Wenn Sie ein direkter Rechnungs Partner oder indirekter Anbieter in diesen drei Ländern sind, die für das MCI-Programm registriert sind, und Sie keine LRD-Gutschrift als Zahlungsmethode sehen, vergewissern Sie sich, dass Ihre Mandanten-ID dem entsprechenden Partnerkonto für MPN-Speicherort zugeordnet ist. Weitere Informationen zu diesem Thema finden Sie unter Vorgehens [Weise beim Aktualisieren Ihres Organisations Profils](update-your-partner-profile.md).

    
5. Wählen Sie die **Währung** aus.

6. Wenn Sie alle Zahlungs Felder ausgefüllt haben, wählen Sie über **Mitteln** aus.


## <a name="create-your-bank-profile"></a>Erstellen Ihres Bank Profils

Bank Profile werden auf Organisationsebene erstellt. Dadurch kann ein Bankkonto in einer Organisation über mehrere MPN-IDs und Incentive-Programme hinweg zugewiesen werden. Möglicherweise gibt es Ausnahmen, wenn Sie das Banking-Profil auf verschiedene Länder anwenden, da ggf. andere Bank-und Steuerregeln gelten.

>[!NOTE]
>Auf den folgenden Seiten sind Felder mit einem Sternchen erforderlich. Wenn Sie nicht wissen, was ein Feld ist, wählen Sie das Informationssymbol aus. 

1. Füllen Sie auf der Seite **Details** die folgenden Felder aus: **Profilname:** geben Sie einen eindeutigen Namen ein, um dieses Zahlungsprofil zu identifizieren.
    **Speicherort des Bankkontos:** Das Land, in dem sich die Bank des Unternehmens befindet.
    **Zahlungsmethode:** Die bevorzugte Zahlungsmethode für Partner Center ist Electronic Bank Transfer.

2. Wählen Sie **Weiter** aus.

3. Geben Sie auf der Seite **Bankkonto** Ihre Informationen ein. Felder, die auf dieser Seite angezeigt werden, variieren je nach Land. 

4. Wählen Sie **Weiter** aus.

5. Geben Sie auf der Seite **Empfänger** die entsprechenden Informationen ein. Der Begünstigter ist die Person in Ihrem Unternehmen, die die Bank kontaktiert, wenn Sie Ihr Konto besprechen müssen.

6. Wenn die Felder abgeschlossen sind, klicken Sie auf **Fertig** stellen, und wählen Sie dann **bestätigen** aus, um das Bank Profil zu erstellen.

Sie werden auf die Seite " **Auszahlungs-und Steuer profile** " umgeleitet. Der Status Ihres neuen Profils reflektiert die **ausstehende Microsoft** -Überprüfung, bis die Überprüfung abgeschlossen ist. Dieser Vorgang kann bis zu 48 Stunden dauern. Nachdem die Überprüfung abgeschlossen ist, wird Ihr Profil Status entweder **genehmigt** oder **Aktion erforderlich** angezeigt. Wenn eine **Aktion erforderlich** ist, wiederholen Sie die obigen Schritte, um die erforderlichen Informationen bereitzustellen 

## <a name="create-your-tax-profile"></a>Steuer Profil erstellen

Mithilfe des folgenden Verfahrens können Sie Microsoft die für Ihre Organisation erforderlichen Steuerinformationen bereitstellen. Die Seiten in diesem Abschnitt sind dynamisch und variieren je nach Land oder Region. Wenn Sie Hilfe bei der Identifizierung der richtigen Steuerinformationen benötigen, wenden Sie sich an die entsprechenden Regierungsquellen in Ihrem Land.

Wenn Sie für Partnerunternehmen in Nordamerika Informationen zum Abschließen von W8-oder W9-Formularen benötigen, gelangen Sie mit den folgenden Adressen zur IRS-Website:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Geben Sie nur Details für Ihr Unternehmen ein. Geben Sie niemals persönliche Details ein.

1. Füllen Sie auf der Seite **Geschäftsprofil** die erforderlichen Felder aus, und klicken Sie dann auf **weiter**. 

2. Wählen Sie auf der Seite **Setup** die Option aus, die für Ihr Unternehmen gilt.

   - Wählen Sie die Option auf der linken Seite aus, wenn Ihr Unternehmen nur in den USA integriert ist, oder wenn dieses Profil für eine Person vorgesehen ist.
   - Wählen Sie die Option auf der rechten Seite aus, wenn Ihr Unternehmen außerhalb des USA integriert ist, und wählen Sie dann Ihr Land/Ihre Region aus der Liste aus.

3. Wählen Sie **Weiter** aus. 

4. Geben Sie auf der Seite " **Tax Status** " die erforderlichen Informationen ein, und klicken Sie dann auf **weiter**. Felder auf dieser Seite variieren je nach Land. Ihre Details. 

5. Wählen Sie auf der Seite **zusätzliche Dokumentation** die erforderlichen Felder aus, und wählen Sie **weiter** aus. 

6. Wählen Sie **Durchsuchen** aus, um alle von Ihrem Land oder Ihrer Region benötigten Dokumente hochzuladen. Wenn der Dokument Name angezeigt wird, wählen Sie **hochladen** aus. 

7. Wenn Sie das Dokument entfernen müssen, wählen Sie **Entfernen** aus.

8. Klicken Sie zum Speichern und Fortfahren auf **Fertig** stellen.

9. Wählen Sie in der Popup Meldung **bestätigen** aus. Sie gelangen zurück zur Seite " **Auszahlungs-und Steuereinrichtung** ".

## <a name="next-steps"></a>Nächste Schritte

- [Häufige Fragen zu Auszahlungen und Steuern](payout-faq.md)
