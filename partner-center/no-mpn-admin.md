---
title: Was tun, wenn der einzige Administrator für Ihr MPN-Programm das Unternehmen verlassen hat?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie einen neuen MPN-Administrator finden oder Hilfe vom globalen Administrator Ihres Unternehmens erhalten. Außerdem erfahren Sie, wie Sie einen neuen globalen Partner Center hinzufügen.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151167"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Was tun, wenn der einzige Administrator für Ihr MPN-Programm das Unternehmen verlassen hat?

**Geeignete Rollen:** MPN-Partneradministrator| Kontoadministrator-| Globaler Administrator

Im folgenden Artikel werden drei typische Szenarien zur Vorgehensweise beschrieben, wenn Ihr MPN-Administrator das Unternehmen verlassen hat.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Szenario 1: MPN-Partneradministrator/Kontoadministrator hat das Unternehmen verlassen, aber es sind immer noch globale Administratoren im Konto.

In diesem Fall kann einer anderen Person im Unternehmen die Rolle eines MPN-Partneradministrators zugewiesen werden. So weisen Sie die Rolle eines bestimmten MPN-Partneradministrators/Kontoadministrators zu:

1. Melden Sie sich bei Partner Center-Konto mit Ihrem Arbeitskonto an (z. B. tom@contoso.com ).
1. Filtern Sie **auf der Seite** Benutzerverwaltung nach Globaler Administrator, um zu sehen, wer die globalen Administratoren für Ihr Unternehmen sind. 
1. Wenden Sie sich an einen der globalen Administratoren, und bitten Sie ihn, Ihnen die MPN-spezifische Rolle zu zuweisen, die Sie benötigen. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Szenario 2: MPN-Partneradministrator/Kontoadministrator hat das Unternehmen verlassen, und das Konto verfügt nicht über globale Administratoren. 

Wenn Sie zur  Seite Benutzerverwaltung wechseln und nach "Globaler Administrator" filtern, aber feststellen, dass es in Ihrem Unternehmen keinen globalen Administrator gibt, der Ihnen dabei helfen kann, die MPN-spezifische Rolle zu erhalten, führen Sie die folgenden Schritte aus:

1. Wechseln Sie [portal.azure.com](https://ms.portal.azure.com/), melden Sie sich mit Ihrem Arbeitskonto an (z. B. tom@contoso.com ). 
1. Wählen Sie **in der linken Menünavigationsleiste** die Option Hilfe und Support aus.
1. Wählen Sie auf der nächsten Seite im **Dropdownmenü** new Supportanfrage and **Technical Issue type** (Neuer Fehlertyp und Typ des technischen Problems) aus, fügen Sie alle zusätzlichen Details ein, und klicken Sie auf **Weiter: Lösungen.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Suchen sie den Administrator in Azure-Portal":::

4. Nachdem Sie die empfohlenen Lösungen auf der nächsten Seite überprüft haben, wählen Sie **Weiter: Details aus,** und füllen Sie die erforderlichen Felder aus.
1. Überprüfen und erstellen Sie die Supportanfrage.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Szenario 3: MPN-Partneradministrator/Kontoadministrator/Globaler Administrator hat das Unternehmen verlassen, und es gibt keine anderen Benutzer, die auf die Azure AD des Unternehmens zugreifen können. Dies ist ein vollständiger Zugriffsverlust.

Führen Sie die Schritte zur [Administratorübernahme](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) aus, um ein nicht verwaltetes Verzeichnis als Azure Active Directory Administrator zu übernehmen.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Sie sind nicht sicher, ob Ihre Firma bereits ein Geschäftskonto hat?

Wenn Sie nicht sicher sind, ob Ihr Unternehmen ein Geschäftskonto besitzt, können Sie das folgendermaßen überprüfen.

1. Melden Sie sich beim [Azure-Verwaltungsportal](https://ms.portal.azure.com)an.
2. Wählen Sie im linken Menü **Azure Active Directory** und dann **Domänennamen** aus.
Wenn Sie bereits ein Geschäftskonto haben, wird Ihr Domänenname aufgeführt.

>[!Note]
>Wenn Sie über ein aktives Abonnement für Microsoft Azure oder Office 365 verfügen, verfügen Sie bereits über ein Geschäftskonto, und Ihre Anmeldeinformationen sollten mit den Anmeldeinformationen übereinstimmen, die für den Zugriff auf diese Dienste verwendet werden.