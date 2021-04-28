---
title: Suchen nach Mandanten-ID, Domänenname, Benutzerobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie IDs im Azure-Portal finden– der Azure AD Mandanten-ID, des Domänennamens oder einer bestimmten Benutzerobjekt-ID einer Organisation. Einige Aufgaben benötigen diese Informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172250"
---
# <a name="locate-important-ids-for-a-user"></a>Suchen wichtiger IDs für einen Benutzer

**Geeignete Rollen**

- Globaler Administrator

In diesem Artikel wird beschrieben, wie Sie die [Azure-Portal](https://portal.azure.com/) verwenden, um die folgenden Informationen für einen Benutzer zu finden:

- Die Microsoft Azure Active Directory(Azure AD)-Mandanten-ID der Organisation oder des Unternehmens des Benutzers

- Der primäre Domänenname der Organisation oder des Unternehmens, die dem Azure AD Mandanten zugeordnet ist.

- Die Benutzerobjekt-ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Suchen der Microsoft Azure AD Mandanten-ID und des primären Domänennamens

Führen Sie diese Schritte aus, um die Azure AD Mandanten-ID oder den primären Domänennamen innerhalb des Azure-Portal zu finden. (Wenn Sie eine Mandanten-ID programmgesteuert suchen möchten, finden Sie weitere Informationen unter Suchen einer [Mandanten-ID mit PowerShell oder cli.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)

> [!NOTE]
> Die Mandanten-ID kann in verschiedenen Anwendungen oder Ressourcen als unterschiedliche Namen bezeichnet werden. Die Mandanten-ID kann beispielsweise als Verzeichnis-ID, Azure Active Directory Mandant (Azure AD), Microsoft-ID oder für bestimmte Berichte bezeichnet werden, sogar als *tenantguid*.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.

2. Wählen Sie die Menüoption **Azure Active Directory** aus.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zeigt Azure-Portal auswahl der option Azure Active Directory im Menü an.":::

3. Eine Azure Active Directory **Seite Übersicht** wird angezeigt. Um die Azure AD Mandanten-ID oder den primären Domänennamen zu finden, suchen Sie nach dem Feld **Mandanten-ID** und dem Feld **Primäre Domäne.** Diese Felder werden im Abschnitt Mandanteninformationen angezeigt.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zeigt die Seite Übersicht mit zwei hervorgehobenen Feldern an: Mandanten-ID und primärer Domänenname.":::

4. Sie finden die Mandanten-ID im Azure-Portal auf andere Weise. Wählen Sie die Menüoption **Azure Active Directory** aus. Navigieren Sie dann im Menü zum Abschnitt **Verwalten,** und wählen Sie **Eigenschaften** aus.

   Auf der Seite Eigenschaften wird auch die zugeordnete Mandanten-ID des Benutzers angezeigt.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Seite &quot;Eigenschaften&quot; mit hervorgehobenen Feld &quot;Mandanten-ID&quot;":::

## <a name="find-the-user-object-id"></a>Suchen der Benutzerobjekt-ID

Das Suchen des Domänennamens und der Mandanten-ID reicht möglicherweise nicht immer aus. Möglicherweise müssen Sie auch die bestimmte Objekt-ID ermitteln, die einem Benutzer zugewiesen ist. Führen Sie die folgenden Schritte aus, um die Objekt-ID eines Benutzers in der folgenden Azure-Portal:

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.

2. Wählen Sie die Menüoption **Azure Active Directory** aus.

3. Suchen Sie **im Menü** nach dem Abschnitt Verwalten, und wählen Sie dann **Benutzer aus.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zeigt Azure Active Directory mit hervorgehobener Option Benutzer an.":::

4. Geben Sie auf der Seite Benutzer den Namen des Benutzers in das Suchfeld ein.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zeigt die Seite Benutzer mit Suchfeld an, um nach einem bestimmten Benutzer zu suchen.":::

5. Wählen Sie den Namen des Benutzers aus, an dem er in der Liste angezeigt wird.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zeigt die Seite Benutzer an, auf der eine Zeile für den gesuchten Benutzer angezeigt wird.":::

6. Suchen Sie auf der Seite Profil des Benutzers nach dem Abschnitt Identität. Das Feld Objekt-ID wird hier mit der eindeutigen Objekt-ID des Benutzers angezeigt.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zeigt die Seite &quot;Benutzerprofil&quot; mit dem Abschnitt Identität und einem hervorgehobenen Feld für die Objekt-ID an.":::

## <a name="next-steps"></a>Nächste Schritte

- [Programmgesteuertes Suchen Ihrer Mandanten-ID mit PowerShell oder cli](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Weitere Informationen zu Benutzerprofilen in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Erfahren Sie, wie Partner Kundendetails in der Partner Center](see-your-customer-list.md)

