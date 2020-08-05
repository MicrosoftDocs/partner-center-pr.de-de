---
title: Erstellen und Verwalten von Auszahlungs- und Steuerprofilen im Partner Center
ms.topic: how-to
ms.date: 06/29/2020
description: Bevor Sie für Ihre Incentives bezahlt werden können, müssen Sie Ihre Auszahlungs-und Steuer Profile erstellen.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 3e7424ff1329d9c2bf13e9a6c4181c312396e073
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/04/2020
ms.locfileid: "87546041"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a>Auszahlungs- und Steuerprofile in Partner Center

Gilt für:

- Partner Center

Bevor Sie Zahlungen für Ihre Incentives-Programme für einen bestimmten MPN-Standort erhalten können, müssen Sie Ihre Registrierung abschließen, indem Sie ein gültiges Auszahlungs- und Steuerprofil mit dem Programm und MPN-Standort verknüpfen. Microsoft nutzt dieses Auszahlungs- und Steuerprofil zur Ausstellung von Zahlungen. Je nach Regeln des Incentives-Programms kann es Ihnen gestattet sein, für die Zahlung eine elektronische Banküberweisung oder eine Gutschrift zu nutzen. 

Geeignete Rollen:

- Incentiveadministrator
- Abrechnungsadministrator
- Globaler Administrator

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Erstellen und Verwalten von Auszahlungs- und Steuerprofilen im Partner Center

In den folgenden Abschnitten werden die Schritte zum Erstellen und Verwalten von Zahlungs-und Steuer Profilen in Partner Center erläutert.

>[!IMPORTANT]
>Sie müssen ein Incentive-Administrator sein, um Zahlungs Profile in Partner Center zu erstellen oder zu verwalten. Incentive-Rollen müssen jedem MPN-Speicherort unter jedem Incentive-Programm zugewiesen werden. Weitere Informationen zum Hinzufügen von Incentive-Administratoren in Partner Center finden Sie unter [Hinzufügen von Incentive-Benutzern oder-Administratoren in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Zugriff auf den Abschnitt "Auszahlungs-und Steuer Berechtigung" im Partner Center

1. Melden Sie sich bei Partner Center mithilfe Ihres Aad-Kontos (Firmenkonto) oder der entsprechenden e-Mail-Adresse an, wenn eine zugewiesen wurde. 

   - Mehrere Domänen können innerhalb eines Aad-Kontos registriert werden. Wenden Sie sich an ihren globalen Administrator, um die zugeordneten Domänen zu ermitteln
   - Wenn Sie sich nur bei der Domäne anmelden können, wenden Sie sich an **@onmicrosoft.com** Ihren Konto Administrator, um dem AAD-Konto zusätzliche Domänen hinzuzufügen.
   - Wenn Sie aufgefordert werden, Geschäfts- **oder Schul Konto** oder **persönliches Konto**auszuwählen, wählen Sie Geschäfts- **oder Schul Konto**aus.

2. Wählen Sie das Zahnrad Symbol aus, um das Menü **Einstellungen** zu öffnen, und wählen Sie dann **Partner Einstellungen**aus.

3. Wählen Sie im Menü **Kontoeinstellungen** die Option **Auszahlung und Steuern**aus. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Zuweisen von Auszahlungs-und Steuer Profilen zu einzelnen Programmen

1. Wählen Sie im Partner Center das Zahnrad Symbol aus, um das Menü " **Einstellungen** " zu öffnen. 

2. Wählen Sie **Partner Einstellungen**aus, erweitern Sie den **Abschnitt Auszahlung und Steuern**, und wählen Sie dann **Auszahlungs-und Steuer Profil Zuweisung**aus. 
   
   Eine Liste der Programme wird angezeigt. Wählen Sie den Pfeil neben einem Programm aus, um die Profildetails anzuzeigen. 

3. Wählen Sie im Dropdown Menü **Steuer Profil** das gewünschte Steuer Profil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet.  Wählen Sie im Popup Fenster fortsetzen aus. Der Prozess zum Erstellen eines neuen Steuer Profils wurde unten bereitgestellt.

4. Wählen Sie **Zahlungsmethode**aus.

   - Wenn Sie **Electronic Bank Transfer** as Payment Method ausgewählt haben, wählen Sie in der Dropdown Liste Payment Profile das gewünschte Zahlungsprofil aus, oder wählen Sie die Option zum Erstellen eines neuen Profils aus. Wenn Sie die Option zum Erstellen eines neuen Profils auswählen, werden Sie entsprechend umgeleitet.  Wählen Sie im Popup Fenster fortsetzen aus. Der Prozess zum Erstellen eines neuen Zahlungs Profils wurde unten bereitgestellt.

   - Wenn Sie **Guthaben Hinweis** als Zahlungsmethode ausgewählt haben, führen Sie die Überprüfung aus, um zu bestätigen, dass die referenzierte SAP-Nummer zu Ihrer Organisation gehört.

    >[!NOTE]
    >Wenn mehrere Microsoft-Geschäfts Entitäten aufgelistet sind, müssen Sie ein Zahlungsprofil für jede Entität auswählen.

    >[!NOTE]
    >Die Verfügbarkeit der Zahlungsmethode hängt von den Regeln des Incentive-Programms ab.
    
5. Wählen Sie die **Währung**aus.

6. Wenn Sie alle Zahlungs Felder ausgefüllt haben, wählen Sie über **Mitteln**aus.

## <a name="create-your-bank-profile"></a>Erstellen Ihres Bank Profils

Bank Profile werden auf Organisationsebene erstellt, sodass das gleiche Bank Profil über mehrere MPN-IDs und Incentive-Programme innerhalb einer Organisation hinweg zugewiesen werden kann. Möglicherweise gibt es Ausnahmen, wenn Sie das Banking-Profil auf verschiedene Länder anwenden, da ggf. andere Bank-und Steuerregeln gelten.

>[!NOTE]
>Auf den folgenden Seiten sind Felder mit einem Sternchen erforderlich. Wenn Sie nicht wissen, was ein Feld ist, wählen Sie das Informationssymbol aus. 

1. Füllen Sie auf der Seite **Details** die folgenden Felder aus: **Profilname:** geben Sie einen eindeutigen Namen ein, um dieses Zahlungsprofil zu identifizieren.
    **Speicherort des Bankkontos:** Das Land, in dem sich die Bank des Unternehmens befindet.
    **Zahlungsmethode:** Die bevorzugte Zahlungsmethode ist für Partner Center Electronic Bank Transfer.

2. Wählen Sie **Weiter** aus.

3. Geben Sie auf der Seite **Bankkonto** Ihre Informationen ein. Felder, die auf dieser Seite angezeigt werden, variieren je nach Land. 

4. Wählen Sie **Weiter** aus.

5. Geben Sie auf der Seite **Empfänger** die entsprechenden Informationen ein. Der Begünstigter ist die Person in Ihrem Unternehmen, die die Bank kontaktiert, wenn Sie Ihr Konto besprechen müssen.

6. Wenn die Felder abgeschlossen sind, klicken Sie auf **Fertig**stellen, und wählen Sie dann **bestätigen** aus, um das Bank Profil zu erstellen.

Sie werden auf die Seite " **Auszahlungs-und Steuer profile** " umgeleitet. Der Status Ihres neuen Profils reflektiert die **ausstehende Microsoft** -Überprüfung, bis die Überprüfung abgeschlossen ist. Dies kann bis zu 48 Stunden dauern. Nachdem die Überprüfung abgeschlossen ist, wird Ihr Profil Status entweder **genehmigt** oder **Aktion erforderlich**angezeigt. Wenn eine **Aktion erforderlich**ist, wiederholen Sie die obigen Schritte, um die erforderlichen Informationen bereitzustellen 

## <a name="create-your-tax-profile"></a>Steuer Profil erstellen

Mithilfe des folgenden Verfahrens können Sie Microsoft die für Ihre Organisation erforderlichen Steuerinformationen bereitstellen. Die Seiten in diesem Abschnitt sind dynamisch und unterscheiden sich je nach Land oder Region. Wenn Sie Hilfe bei der Identifizierung der richtigen Steuerinformationen benötigen, wenden Sie sich an die entsprechenden Regierungsquellen in Ihrem Land.

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

## <a name="payout-and-tax-profile-faqs"></a>FAQs zu Auszahlungs-und Steuer Profilen

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a>Warum muss ich meine Auszahlungs-und/oder Steuer Details angeben?

Um die Auszahlungen für Microsoft Incentive-Programme zu erhalten, müssen Sie die Registrierung durchführen, indem Sie gültige Auszahlungs-und Steuer Details angeben. Eine Registrierung gilt nur, wenn das von Ihnen bereitgestellte Auszahlungs-und Steuer Profil von Microsoft überprüft wird.

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a>Gewusst wie wissen, dass ich meine Auszahlungs-und/oder Steuer Details angeben oder aktualisieren muss?

Alle Partner, die sich in einem neuen Incentive-Programm anmelden, müssen gültige Auszahlungs-und Steuer Details angeben, um die Registrierung abzuschließen.

Sie müssen möglicherweise auch aktualisierte Informationen bereitstellen, wenn sich die Regeln für das Incentive-Programm ändern oder wenn Aspekte des Profils ablaufen oder veraltet sind. Wenn dies der Fall ist, wird auf der Übersichtsseite der Status **Aktion erforderlich – Update Bank und/oder Steuer Profil**angezeigt.

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a>Wie kann ich meine Auszahlungs- und/oder Steuerdetails bereitstellen/aktualisieren?

Ausführliche Informationen zum Aktualisieren von Zahlungs-und Steuer Details in Partner Center finden Sie unter [Erstellen und Verwalten von Bank-und Steuer Profilen in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center) .

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>Warum sehe ich meine Registrierungen nicht, wenn ich mein Auszahlungs- und Steuerprofil zuweise?

Nur Incentives-Administratoren für Ihren MPN-Standort können Auszahlungs- und Steuerprofile erstellen oder verwalten. Möglicherweise verfügen Sie nicht über die entsprechenden Berechtigungen, oder Sie sind mit einem Konto angemeldet, das nicht über diese Berechtigungen verfügt. Wenden Sie sich zwecks Verwaltung der Berechtigungen für Bank und Steuern an den Administrator Ihrer Organisation.

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a>Wo kann ich die Auszahlungs- und Steuerprofile für meine Organisation sehen, die ich nutzen kann?

Verwenden Sie das folgende Verfahren, um Auszahlungs-und Steuer Profile anzuzeigen:

1. Melden Sie sich bei Partner Center an.

2. Wählen Sie das Zahnradsymbol zum Öffnen des Menüs **Einstellungen** aus.

3. Wählen Sie **Partner Einstellungen**aus.

4. Wählen Sie unter **Kontoeinstellungen** die Option **Auszahlung und Steuer** und dann **Auszahlungs- und Steuerprofil** aus. Sie sehen alle vorhandenen Zahlungs- und Steuerprofile mit Status und Bearbeitungsmöglichkeiten.

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>Meine Organisation ist an mehreren Incentive-Programmen beteiligt. Muss ich mein Zahlungs-und Steuer Profil mehrmals bereitstellen?

Bei Zahlungsprofilen liegt es in der Regel an Ihnen. Zahlungsprofile werden auf Organisationsebene erstellt, was es ermöglicht, dass dasselbe Bankprofil mehreren MPN-IDs und Incentives-Programmen innerhalb einer Organisation zugewiesen werden kann. In den meisten Fällen können Sie entweder ein vorhandenes Profil wieder verwenden oder ein neues erstellen.

Es kann jedoch Ausnahmen geben, wenn Sie Ihr Bankprofil verschiedenen Ländern oder Regionen zuordnen, da möglicherweise lokale Bank- oder Steuervorschriften gelten.

Für einen MPN-Standort erstellte Steuerprofile werden wiederverwendet und automatisch ausgefüllt, wenn derselbe MPN-Standort an einem anderen Incentives-Programm teilnimmt. Es kann jedoch Ausnahmen geben. Beispielsweise können die Auszahlungsregeln eines neuen Incentives-Programms zusätzliche Details zum Steuerprofil erfordern.  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>Ich kann mich nur bei meiner @onmicrosoft.com Domäne anmelden. Wie sollte ich vorgehen?

Bitten Sie Ihren Kontoadministrator, dem AAD-Konto zusätzliche Domänen hinzuzufügen.
