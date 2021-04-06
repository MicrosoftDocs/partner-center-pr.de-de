---
title: Was ist zu tun, wenn der einzige Administrator für Ihr MPN-Programm das Unternehmen verlassen hat?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, was Sie tun müssen, um einen neuen MPN-Administrator zu finden oder Hilfe vom globalen Administrator Ihres Unternehmens zu erhalten. Erfahren Sie außerdem, wie Sie einen neuen globalen Administrator für Partner Center hinzufügen.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3702ebd5a9421036a053a9a142a2f40d3e488137
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441998"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Was ist zu tun, wenn der einzige Administrator für Ihr MPN-Programm das Unternehmen verlassen hat?

**Geeignete Rollen**

- MPN-Partneradministrator
- Kontoadministrator
- Globaler Administrator

Der folgende Artikel führt Sie durch drei typische Szenarien, in denen beschrieben wird, was geschehen soll, wenn Ihr MPN-Administrator das Unternehmen verlassen hat.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Szenario 1: der MPN-Partner Administrator/-Konto Administrator hat das Unternehmen verlassen, aber es sind noch globale Administratoren im Konto vorhanden.

In diesem Fall kann eine andere Person im Unternehmen der Rolle MPN-Partner Administrator zugewiesen werden. Um der Rolle einer bestimmten MPN-Partner Administrator-/kontoadministratorrolle zugewiesen zu werden:

1. Melden Sie sich mit Ihrem Geschäftskonto bei Ihrem Partner Center-Konto an (z tom@contoso.com . b.).
1. Über den Filter der **Benutzer Verwaltungs** Seite auf dem globalen Administrator, um zu sehen, wer die globalen Administratoren für Ihr Unternehmen sind. 
1. Wenden Sie sich an einen der globalen Administratoren, und bitten Sie ihn, Ihnen die MPN-spezifische Rolle zuzuweisen, die Sie benötigen. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Szenario 2: der MPN-Partner Administrator/-Konto Administrator hat das Unternehmen verlassen, und es sind keine globalen Administratoren im Konto vorhanden. 

Wenn Sie zur Seite " **Benutzerverwaltung** " wechseln und nach "globaler Administrator" filtern, aber feststellen, dass es keinen globalen Administrator in Ihrem Unternehmen gibt, der Ihnen helfen kann, die MPN-spezifische Rolle zu erhalten, führen Sie die folgenden Schritte aus:

1. Wechseln Sie zu [Portal.Azure.com](https://ms.portal.azure.com/), melden Sie sich mit Ihrem Geschäftskonto an (z tom@contoso.com . b.). 
1. Wählen Sie in der linken Menü Navigationsleiste die Option **Hilfe und Support** aus.
1. Wählen Sie auf der nächsten Seite im Dropdown Menü die Option **neu Supportanfrage** und **technischer** Problemtyp aus, fügen Sie weitere Details ein, und klicken Sie auf weiter **: Lösungen.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Admin in Azure-Portal suchen":::

4. Nachdem Sie die empfohlenen Lösungen auf der nächsten Seite überprüft haben, wählen Sie **Weiter: Details** aus, und füllen Sie die erforderlichen Felder aus.
1. Überprüfen und erstellen Sie die Supportanfrage.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Szenario 3: MPN-Partner Administrator/Konto Administrator/globaler Administrator hat das Unternehmen verlassen, und es gibt keine anderen Benutzer, die auf die Azure AD des Unternehmens zugreifen können. Dies ist ein kompletter Verlust des Zugriffs.

Befolgen Sie die Schritte für die [Administrator Übernahme](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) , um ein nicht verwaltetes Verzeichnis als Azure Active Directory Administrator zu übernehmen.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Sie sind nicht sicher, ob Ihre Firma bereits ein Geschäftskonto hat?

Wenn Sie nicht sicher sind, ob Ihr Unternehmen ein Geschäftskonto besitzt, können Sie das folgendermaßen überprüfen.

1. Melden Sie sich beim [Azure-Verwaltungs Portal](https://ms.portal.azure.com)an.
2. Wählen Sie im linken Menü **Azure Active Directory** aus, und wählen Sie dann **Domänen Namen** aus.
Wenn Sie bereits ein Geschäftskonto haben, wird Ihr Domänenname aufgeführt.

>[!Note]
>Wenn Sie über ein aktives Abonnement für Microsoft Azure oder Office 365 verfügen, verfügen Sie bereits über ein Geschäftskonto, und die Anmelde Informationen müssen mit den Anmelde Informationen identisch sein, die für den Zugriff auf diese Dienste verwendet werden.