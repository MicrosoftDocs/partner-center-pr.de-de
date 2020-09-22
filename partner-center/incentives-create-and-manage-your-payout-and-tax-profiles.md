---
title: Auszahlungs- und Steuerprofile in Partner Center
ms.topic: how-to
ms.date: 09/11/2020
description: Erstellen und verwalten Sie Ihr Auszahlungs-und Steuer Profil, damit Sie für Ihre Incentives kostenpflichtig sind.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: de143ecfae1b803e0743a28db5cda5ae9a3d5f2d
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999314"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Auszahlungs-und Steuer Profilen für die Anreize im Partner Center

**Gilt für:**

- Partner Center

**Geeignete Rollen:**

- Incentiveadministrator
- Abrechnungsadministrator
- Globaler Administrator

Bevor Sie Zahlungen für Ihre Incentives-Programme für einen bestimmten MPN-Standort erhalten können, müssen Sie Ihre Registrierung abschließen, indem Sie ein gültiges Auszahlungs- und Steuerprofil mit dem Programm und MPN-Standort verknüpfen. Microsoft nutzt dieses Auszahlungs- und Steuerprofil zur Ausstellung von Zahlungen. Je nach Regeln des Incentives-Programms kann es Ihnen gestattet sein, für die Zahlung eine elektronische Banküberweisung oder eine Gutschrift zu nutzen. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Rollen, Währungen und andere Microsoft-Programme

Es ist wichtig, die folgenden Informationen zu verstehen, bevor Sie mit Ihrem Auszahlungs-und Steuer Profil beginnen.

### <a name="roles-and-permissions"></a>Rollen und Berechtigungen

Sie müssen ein Administrator der Administrator sein, um Bank-und Steuerinformationen für Incentive-Zahlungen einzugeben. Wenn Sie ein MPN/Konto-Administrator sind, können Sie sich selbst und/oder einen Kollegen als Administrator für Administratoren zuweisen.

Wenn Sie Administrator Berechtigungen für Incentives anfordern müssen, wenden Sie sich an den MPN-Administrator oder den globalen Administrator. Sie können herausfinden, wer in Ihrem Unternehmen über diese Rollen verfügt, indem Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)anmelden. Wählen Sie oben rechts im Symbol " **Einstellungen** " die Option **Benutzerverwaltung** aus, und Filtern Sie dann nach globaler Administrator.

Incentives: Benutzer können die Informationen zu den Incentive-und Zahlungsdetails und-Berichten anzeigen, aber keine Bank-und Steuer Details bearbeiten.

### <a name="choose-your-disbursement-currency"></a>Wählen Sie Ihre Auszahlungs Währung aus.

Standardmäßig werden in der lokalen Währung der einzelnen Entitäten Incentives-Zahlungen durchgeführt. Während der Profil Einrichtung können Sie eine andere Währung angeben. Zahlungen werden mit einem Exchange-Satz berechnet, der monatlich von Microsoft festgelegt wird. Aufgrund der ausgewählten Währung sind Sie für alle Änderungen am Wert verantwortlich.

### <a name="bank-and-tax-information-and-other-programs"></a>Bank-und Steuerinformationen und andere Programme

Geben Sie die unten beschriebenen Informationen an, selbst wenn Microsoft Ihre Bank Daten bereits für Zahlungen verwendet. Dies trägt dazu bei, den Datenschutz und die Sicherheit der Daten Ihres Unternehmens sicherzustellen, da das Kopieren Ihres Profils in das neue Tool vertrauliche Informationen verfügbar machen kann. Diese Vorgehensweise ist auch eine gute Möglichkeit, um sicherzustellen, dass die Daten komplett und korrekt sind.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Verwenden verschiedener Profile für verschiedene Microsoft-Programme

Im Einzelhandel können Zahlungen für jedes der fünf Einzelhandels Incentive-Programme auf dasselbe Bankkonto übertragen werden. Alternativ können Sie auswählen, dass die Einzelhandel-Xbox-Zahlungen in einem Bankkonto durchlaufen werden, während der Einzelhandel an ein anderes Bankkonto gezahlt wird.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Auszahlungs- und Steuerprofilen im Partner Center

In den folgenden Abschnitten werden die Schritte zum Erstellen und Verwalten von Zahlungs-und Steuer Profilen in Partner Center erläutert.

>[!IMPORTANT]
>Sie müssen ein Incentive-Administrator sein, um Zahlungs Profile in Partner Center zu erstellen oder zu verwalten. Incentive-Rollen müssen jedem MPN-Speicherort unter jedem Incentive-Programm zugewiesen werden. Weitere Informationen zum Hinzufügen von Incentive-Administratoren in Partner Center finden Sie unter [Erstellen von Benutzerkonten](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Zugriff auf den Abschnitt "Auszahlungs-und Steuer Berechtigung" im Partner Center

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) mit Ihrem Azure Active Directory (Azure AD)-Konto (Firmenkonto) oder der entsprechenden e-Mail-Adresse an, wenn eine zugewiesen wurde.

   - Mehrere Domänen können innerhalb eines Azure AD Kontos registriert werden. Wenden Sie sich an ihren globalen Administrator, um die zugeordneten Domänen zu ermitteln
   - Wenn Sie sich nur bei der Domäne anmelden können, wenden Sie sich an @onmicrosoft.com Ihren Konto Administrator, um dem Azure AD Konto zusätzliche Domänen hinzuzufügen.
   - Wenn Sie aufgefordert werden, Geschäfts-, **Schul** -oder unikonto oder **persönliches Konto**auszuwählen, wählen Sie Geschäfts- **oder Schul Konto**aus.

2. Wählen Sie das Zahnrad Symbol aus, um das Menü **Einstellungen** zu öffnen, und wählen Sie dann **Partner Einstellungen**aus.

3. Wählen Sie im Menü **Kontoeinstellungen** die Option **Auszahlung und Steuern**aus. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Zuweisen von Auszahlungs-und Steuer Profilen zu einzelnen Programmen

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an, und wählen Sie das Zahnrad Symbol aus, um das Menü " **Einstellungen** " zu öffnen. 

2. Wählen Sie **Partner Einstellungen**aus, erweitern Sie den **Abschnitt Auszahlung und Steuern**, und wählen Sie dann **Auszahlungs-und Steuer Profil Zuweisung**aus. 
   
   Eine Liste der Programme wird angezeigt. Wählen Sie den Pfeil neben einem Programm aus, um die Profildetails anzuzeigen. 

3. Wählen Sie im Dropdown Menü **Steuer Profil** das gewünschte Steuer Profil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet.  Wählen Sie im Popup Fenster fortsetzen aus. Der Prozess zum Erstellen eines neuen Steuer Profils wurde unten bereitgestellt.

4. Wählen Sie **Zahlungsmethode**aus.

   - Wenn Sie **Electronic Bank Transfer** als Zahlungsmethode ausgewählt haben, wählen Sie das gewünschte Zahlungsprofil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet. Wählen Sie im Popup Fenster fortsetzen aus. Der Prozess zum Erstellen eines neuen Zahlungs Profils wurde unten bereitgestellt.

   - Wenn Sie **Guthaben Hinweis** als Zahlungsmethode ausgewählt haben, schließen Sie die Überprüfung ab. Dadurch wird bestätigt, dass die referenzierte SAP-Nummer zu Ihrer Organisation gehört.

    >[!NOTE]
    >Wenn mehrere Microsoft-Geschäfts Entitäten aufgelistet sind, müssen Sie ein Zahlungsprofil für jede Entität auswählen.

    >[!NOTE]
    >Die Verfügbarkeit der Zahlungsmethode hängt von den Regeln des Incentive-Programms ab.
    
5. Wählen Sie die **Währung**aus.

6. Wenn Sie alle Zahlungs Felder ausgefüllt haben, wählen Sie über **Mitteln**aus.

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

6. Wenn die Felder abgeschlossen sind, klicken Sie auf **Fertig**stellen, und wählen Sie dann **bestätigen** aus, um das Bank Profil zu erstellen.

Sie werden auf die Seite " **Auszahlungs-und Steuer profile** " umgeleitet. Der Status Ihres neuen Profils reflektiert die **ausstehende Microsoft** -Überprüfung, bis die Überprüfung abgeschlossen ist. Dieser Vorgang kann bis zu 48 Stunden dauern. Nachdem die Überprüfung abgeschlossen ist, wird Ihr Profil Status entweder **genehmigt** oder **Aktion erforderlich**angezeigt. Wenn eine **Aktion erforderlich**ist, wiederholen Sie die obigen Schritte, um die erforderlichen Informationen bereitzustellen 

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

5. Wählen Sie auf der Seite **zusätzliche Dokumentation** die erforderlichen Felder aus, und wählen Sie **weiter**aus. 

6. Wählen Sie **Durchsuchen** aus, um alle von Ihrem Land oder Ihrer Region benötigten Dokumente hochzuladen. Wenn der Dokument Name angezeigt wird, wählen Sie **hochladen**aus. 

7. Wenn Sie das Dokument entfernen müssen, wählen Sie **Entfernen**aus.

8. Klicken Sie zum Speichern und Fortfahren auf **Fertig**stellen.

9. Wählen Sie in der Popup Meldung **bestätigen** aus. Sie gelangen zurück zur Seite " **Auszahlungs-und Steuereinrichtung** ".

## <a name="next-steps"></a>Nächste Schritte

- [Häufig gestellte Fragen zu den Incentivezahlungen und Steuerprofilen](incentives-payout-tax-profile-faqs.md)
