---
title: Suchen von Mandanten-ID, Domänen Name, Benutzerobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie IDs in der Azure-Portal Azure AD Mandanten-ID, Domänen Name oder bestimmte Benutzerobjekt-ID des Unternehmens finden. Einige Aufgaben benötigen diese Informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360070"
---
# <a name="locate-important-ids-for-a-user"></a>Wichtige IDs für einen Benutzer suchen

In diesem Artikel wird beschrieben, wie Sie den [Azure-Portal](https://portal.azure.com/) verwenden, um die folgenden Informationen für einen Benutzer zu suchen:

- Die Microsoft Azure Active Directory-Mandanten-ID (Azure AD) der Organisation oder des Unternehmens des Benutzers

- Der primäre Domänen Name der Organisation oder des Unternehmens, die mit dem Azure AD Mandanten verknüpft ist.

- Die Benutzerobjekt-ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Suchen der Microsoft Azure AD Mandanten-ID und des primären Domänen Namens

Führen Sie diese Schritte aus, um die Azure AD Mandanten-ID oder den primären Domänen Namen innerhalb des Azure-Portal zu ermitteln. (Wenn Sie eine Mandanten-ID Programm gesteuert finden möchten, finden Sie weitere Informationen untersuchen der Mandanten- [ID mit PowerShell oder der CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)

> [!NOTE]
> Die Mandanten-ID kann in verschiedenen Anwendungen oder Ressourcen als unterschiedliche Namen bezeichnet werden. Beispielsweise kann die Mandanten-ID als Verzeichnis-ID, der Azure Active Directory (Azure AD)-Mandant, Microsoft-ID oder für bestimmte Berichte (auch *tenantguid* ) bezeichnet werden.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.

2. Wählen Sie die Menüoption **Azure Active Directory** aus.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zeigt, Azure-Portal die Azure Active Directory-Option im Menü ausgewählt wird.":::

3. Eine Azure Active Directory **Übersichts** Seite wird angezeigt. Wenn Sie die Azure AD Mandanten-ID oder den primären Domänen Namen ermitteln möchten, suchen Sie nach dem Feld Mandanten- **ID** und dem Feld **primäre Domäne** . Diese Felder werden im Abschnitt Mandanten Informationen angezeigt.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zeigt eine Übersichtsseite mit zwei markierten Feldern, der Mandanten-ID und dem primären Domänen Namen an.":::

4. Sie finden die Mandanten-ID in der Azure-Portal auf andere Weise. Wählen Sie die Menüoption **Azure Active Directory** aus. Suchen Sie anschließend im Menü den Abschnitt **Verwalten** , und wählen Sie **Eigenschaften** aus.

   Auf der Seite "Eigenschaften" wird auch die zugehörige Mandanten-ID des Benutzers angezeigt.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zeigt die Eigenschaften Seite mit hervorgehobenem Feld für Mandanten-ID.":::

## <a name="find-the-user-object-id"></a>Suchen der Benutzerobjekt-ID

Das Auffinden des Domänen Namens und der Mandanten-ID ist möglicherweise nicht immer ausreichend. Möglicherweise müssen Sie auch die spezifische Objekt-ID suchen, die einem Benutzer zugewiesen ist. Führen Sie die folgenden Schritte aus, um die Objekt-ID eines Benutzers in der Azure-Portal zu finden:

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.

2. Wählen Sie die Menüoption **Azure Active Directory** aus.

3. Suchen Sie im Menü den Abschnitt **Verwalten** , und wählen Sie dann **Benutzer** aus.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zeigt Azure Active Directory Menü mit hervorgehobener Option &quot;Benutzer&quot; an.":::

4. Geben Sie auf der Seite Benutzer den Namen des Benutzers in das Suchfeld ein.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zeigt die Seite &quot;Benutzer&quot; mit Suchfeld an, um nach einem bestimmten Benutzer zu suchen.":::

5. Wählen Sie den Namen des Benutzers aus, in dem er in der Liste angezeigt wird.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zeigt die Benutzerseite an, die eine Zeile für den gesuchten Benutzer anzeigt.":::

6. Suchen Sie auf der Profilseite des Benutzers den Abschnitt "Identität". Das Feld Objekt-ID wird hier mit der eindeutigen Objekt-ID des Benutzers angezeigt.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zeigt die Seite &quot;Benutzerprofil&quot; mit dem Identitäts Abschnitt und einem markierten Feld für die Objekt-ID an.":::

## <a name="next-steps"></a>Nächste Schritte

- [Programm gesteuertes ermitteln Ihrer Mandanten-ID mit PowerShell oder der CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Weitere Informationen zu Benutzerprofilen finden Sie unter Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Erfahren Sie, wie Partner Kunden Details in Partner Center sehen oder exportieren können.](see-your-customer-list.md)
