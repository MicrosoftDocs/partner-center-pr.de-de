---
title: Suchen der Mandanten-ID, des Domänennamens, der Benutzerobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie IDs im Azure-Portal suchen– die Azure AD Mandanten-ID, den Domänennamen oder die spezifische Benutzerobjekt-ID einer Organisation. Einige Aufgaben benötigen diese Informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150861"
---
# <a name="locate-important-ids-for-a-user"></a>Suchen wichtiger IDs für einen Benutzer

**Geeignete Rollen**: Globaler Administrator

In diesem Artikel wird beschrieben, wie Sie [die](https://portal.azure.com/) Azure-Portal verwenden, um die folgenden Informationen für einen Benutzer zu finden:

- Die Microsoft Azure Active Directory (Azure AD) Mandanten-ID der Organisation oder des Unternehmens des Benutzers

- Der primäre Domänenname der Organisation oder des Unternehmens, die dem Azure AD zugeordnet ist

- Die Benutzerobjekt-ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Suchen der Microsoft Azure AD Mandanten-ID und des primären Domänennamens

Führen Sie die folgenden Schritte aus, um die Azure AD Mandanten-ID oder den primären Domänennamen in der Azure-Portal. (Wenn Sie eine Mandanten-ID programmgesteuert suchen möchten, finden Sie weitere Informationen unter Suchen der [Mandanten-ID mit PowerShell oder cli.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)

> [!NOTE]
> Die Mandanten-ID kann in verschiedenen Anwendungen oder Ressourcen als unterschiedliche Namen bezeichnet werden. Beispielsweise kann die Mandanten-ID als Verzeichnis-ID, der Azure Active Directory-Mandant (Azure AD), die Microsoft-ID oder für bestimmte Berichte, sogar *als tenantguid,* bezeichnet werden.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.

2. Wählen Sie die Menüoption **Azure Active Directory** aus.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zeigt Azure-Portal, wie Sie die Azure Active Directory im Menü auswählen.":::

3. Eine Azure Active Directory **Seite Übersicht** wird angezeigt. Um die Azure AD Mandanten-ID oder den primären Domänennamen zu finden, suchen Sie nach dem Feld **Mandanten-ID** und dem Feld **Primäre** Domäne. Diese Felder werden im Abschnitt Mandanteninformationen angezeigt.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zeigt die Seite Übersicht mit zwei hervorgehobenen Feldern an: Mandanten-ID und primärer Domänenname.":::

4. Sie können die Mandanten-ID in der Azure-Portal auf einige andere Arten finden. Wählen Sie die Menüoption **Azure Active Directory** aus. Suchen Sie dann im Menü **nach dem** Abschnitt Verwalten, und wählen Sie **Eigenschaften aus.**

   Auf der Seite Eigenschaften wird auch die zugeordnete Mandanten-ID des Benutzers angezeigt.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zeigt die Seite Eigenschaften mit hervorgehobenen Feld Mandanten-ID an.":::

## <a name="find-the-user-object-id"></a>Suchen der Benutzerobjekt-ID

Es reicht möglicherweise nicht immer aus, nur den Domänennamen und die Mandanten-ID zu finden. Möglicherweise müssen Sie auch die bestimmte Objekt-ID suchen, die einem Benutzer zugewiesen ist. Führen Sie die folgenden Schritte aus, um die Objekt-ID eines Benutzers im Azure-Portal zu suchen:

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.

2. Wählen Sie die Menüoption **Azure Active Directory** aus.

3. Suchen Sie im Menü den Abschnitt **Verwalten,** und wählen Sie dann **Benutzer** aus.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zeigt Azure Active Directory Menü mit hervorgehobener Option Benutzer an.":::

4. Geben Sie auf der Seite Benutzer den Namen des Benutzers in das Suchfeld ein.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zeigt die Seite Benutzer mit suchfeld an, um nach einem bestimmten Benutzer zu suchen.":::

5. Wählen Sie den Namen des Benutzers aus, an dem er in der Liste angezeigt wird.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zeigt die Seite Benutzer an, auf der eine Zeile für den gesuchten Benutzer angezeigt wird.":::

6. Suchen Sie den Abschnitt Identität auf der Seite Profil des Benutzers. Das Feld Objekt-ID wird hier mit der eindeutigen Objekt-ID des Benutzers angezeigt.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zeigt die Seite Benutzerprofil mit dem Abschnitt Identität und einem hervorgehobenen Feld für Objekt-ID an.":::

## <a name="next-steps"></a>Nächste Schritte

- [Programmgesteuertes Suchen Ihrer Mandanten-ID mit PowerShell oder cli](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Weitere Informationen zu Benutzerprofilen in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Erfahren Sie, wie Partner Kundendetails in Partner Center anzeigen oder exportieren können.](see-your-customer-list.md)

