---
title: Hinzufügen von Mandanten zu Ihrem Partner Center-Konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie mehrere Azure AD Mandanten in Ihrem Partner Center-Konto hinzufügen, konsolidieren oder verwalten, und erfahren Sie, warum Sie dies möglicherweise tun möchten.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124804"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto


**Geeignete Rollen**

- Globaler Administrator
- Kontoadministrator

In diesem Artikel wird erläutert, wie Sie mehrere Azure Active Directory Mandanten (Azure AD) für Ihr Unternehmen konsolidieren und diese dann in Ihrem Partner Center-Konto hinzufügen und verwalten. Hierfür gibt es viele Gründe. Beispiel:

- Nehmen wir beispielsweise an, dass Ihr Unternehmen, ". Sie möchten, dass die beiden Unternehmen getrennt bleiben, aber Sie möchten, dass die neuen Mitarbeiter Partner Center verwenden können. In diesem Fall ordnen Sie den Azure AD Mandanten des neuen Unternehmens Ihrem Partner-Global-Konto (PGA) zu. Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.

- Wenn Sie Ihr Unternehmen mit mehr als einem Mandanten ausführen (z. b. *contoso.com*, *contoso.uk* und *contoso.in*), können Sie die mehr Instanzen Fähigkeit verwenden, um Sie im gleichen PC-Konto zu gruppieren.

- Wenn die Richtlinien für Fusionen und Übernahmen Sie bei der Zusammenarbeit mit Mandanten beider Unternehmen benötigen, verwenden Sie die Mandanten *constoso.com* und *Fabrikam.com* .

- Benutzer eines beliebigen Mandanten müssen folgende Aktionen ausführen können:
    * Zugang zum Partner Center für Schulungen, digitale Downloads oder Microsoft Certified Professional-Zuordnungen (MCP).
    * Zugewiesenen Partner Center-Rollen wie Microsoft Partner Network (MPN) admin oder Incentive admin.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Fügen Sie Ihrem Konto einen Azure AD Mandanten hinzu.

1. Melden Sie sich als globaler Administrator bei [Microsoft Partner Center](https://partner.microsoft.com/dashboard)an.

1. Klicken Sie oben rechts auf **Einstellungen**, wählen Sie **Kontoeinstellungen** aus, und wählen Sie dann Mandanten **aus.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot der Schaltfläche &quot;zuordnen&quot; im Bereich &quot;Azure AD Profil&quot;."::: 

1. Wählen Sie **zuordnen** aus, und geben Sie dann den Mandanten an, den Sie zuordnen möchten.

1. Melden Sie sich an der Eingabeaufforderung als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und wählen Sie dann **bestätigen** aus. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot der Schaltfläche &quot;bestätigen&quot; im Bereich &quot;neue Azure AD Zuordnung bestätigen&quot;."::: 

   Nachdem Sie die Zuordnung bestätigt haben, wird eine **alle festgelegte** Meldung angezeigt. Um den neu hinzugefügten Mandanten anzuzeigen, wählen Sie **zur Mandanten Verwaltung zurückkehren** aus. 
 
>[!NOTE]
>Sie können einen Mandanten nicht mit einem Konto verknüpfen, wenn es bereits einem anderen Partner Center-Konto zugeordnet ist.


## <a name="remove-a-tenant-from-your-account"></a>Entfernen eines Mandanten aus Ihrem Konto
 
1. Melden Sie sich als globaler Administrator bei [Microsoft Partner Center](https://partner.microsoft.com/dashboard)an.

1. Klicken Sie in der oberen rechten Ecke auf das Symbol **Einstellungen** , und wählen Sie dann **Kontoeinstellungen** aus.

1. **Wählen Sie** im linken Bereich Mandanten aus. Wählen Sie unter **Azure AD Mandanten verwalten** die Registerkarte **Partner** aus.
 
1. Wählen Sie neben dem Mandanten, dessen Zuordnung Sie entfernen möchten, die Option **Entfernen** aus.

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot der aktuellen Mandanten Zuordnungen und ihrer Entfernungs Verknüpfungen.":::

   Wie im obigen Screenshot gezeigt, sind die **Entfernungs Entfernungs** Links für alle zugeordneten Mandanten aktiviert, mit Ausnahme des primären Mandanten und des Mandanten, bei dem Sie zurzeit angemeldet sind. 

   > [!NOTE]   
   > Wenn Sie einen Mandanten entfernen, haben die Benutzer in diesem Mandanten keinen Zugriff mehr auf das Partner Center-Konto, und die Entfernung wirkt sich möglicherweise auf ihre Kompetenzen aus. 

## <a name="next-steps"></a>Nächste Schritte

- [Erstellen von Benutzerkonten](create-user-accounts-and-set-permissions.md)






