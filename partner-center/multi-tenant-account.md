---
title: Hinzufügen von Mandanten zu Ihrem Partner Center-Konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie mehrere Azure AD Mandanten in Ihrem Partner Center-Konto hinzufügen, konsolidieren oder verwalten und warum Sie dies tun möchten.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151201"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto


**Geeignete Rollen:** globale | Kontoadministrator

In diesem Artikel wird erläutert, wie Sie mehrere Azure Active Directory -Mandanten (Azure AD) für Ihr Unternehmen konsolidieren und diese dann ihrem Partner Center-Konto hinzufügen und verwalten. Dafür gibt es viele Gründe. Beispiel:

- Angenommen, Ihr Unternehmen Contoso hat ein anderes Unternehmen erworben: Fabrikam. Sie möchten, dass die beiden Unternehmen getrennt bleiben, aber die neuen Mitarbeiter in der Lage sein sollen, Partner Center zu verwenden. In diesem Fall ordnen Sie den Azure AD Mandanten des neuen Unternehmens Ihrem globalen Partnerkonto (PGA) zu. Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.

- Wenn Sie Ihr Unternehmen mit mehr als einem Mandanten (z. *B. contoso.com*, *contoso.uk* und *contoso.in*) ausführen, können Sie diese mithilfe von Mehrinstanzenfähigkeit im gleichen PC-Konto gruppieren.

- Wenn Die Richtlinien für Fusionen und Übernahmen erfordern, dass Sie mit Mandanten beider Unternehmen zusammenarbeiten, verwenden Sie sowohl die *constoso.com* als auch *fabrikam.com* Mandanten.

- Benutzer eines beliebigen Mandanten müssen in der Lage sein, Folgendes zu ermöglichen:
    * Greifen Sie auf Partner Center für Schulungen, digitale Downloads oder die McP-Zuordnung (Microsoft Certified Professional) zu.
    * Ihnen werden Partner Center Rollen zugewiesen, z. B. Microsoft Partner Network-Administrator (MPN) oder Incentives-Administrator.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Hinzufügen eines Azure AD Mandanten zu Ihrem Konto

1. Melden Sie sich als globaler Administrator bei [Microsoft Partner Center](https://partner.microsoft.com/dashboard)an.

1. Wählen Sie oben rechts **Einstellungen** aus, wählen Sie **Kontoeinstellungen** und dann **Mandanten aus.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot der Schaltfläche &quot;Zuordnen&quot; im Bereich &quot;profil&quot; Azure AD"::: 

1. Wählen Sie **Zuordnen** aus, und geben Sie dann den Mandanten an, den Sie zuordnen möchten.

1. Melden Sie sich an der Eingabeaufforderung als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und wählen Sie dann **Bestätigen aus.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot der Schaltfläche &quot;Bestätigen&quot; im Bereich &quot;Neue Azure AD bestätigen&quot;."::: 

   Nachdem Sie die Zuordnung bestätigt haben, wird die Meldung **Alle** festgelegt angezeigt. Um den neu hinzugefügten Mandanten anzeigen zu können, wählen **Sie Zur Mandantenverwaltung zurückkehren aus.** 
 
>[!NOTE]
>Sie können einen Mandanten nicht einem Konto zuordnen, wenn er bereits einem anderen Konto Partner Center ist.


## <a name="remove-a-tenant-from-your-account"></a>Entfernen eines Mandanten aus Ihrem Konto
 
1. Melden Sie sich als globaler Administrator bei [Microsoft Partner Center an.](https://partner.microsoft.com/dashboard)

1. Wählen Sie oben rechts das Symbol **Einstellungen** und dann **Kontoeinstellungen aus.**

1. Wählen Sie im linken Bereich **Mandanten aus.** Wählen **Sie unter Azure AD Mandanten verwalten** die Registerkarte **Partner** aus.
 
1. Klicken **Sie neben** dem Mandanten, dessen Zuordnung Sie entfernen möchten, auf Entfernen.

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot der aktuellen Mandantenzuordnungen und deren Links zum Entfernen":::

   Wie im vorherigen Screenshot  gezeigt, sind die Links entfernen für alle zugeordneten Mandanten aktiviert, mit Ausnahme des primären Mandanten und des Mandanten, bei dem Sie derzeit angemeldet sind. 

   > [!NOTE]   
   > Wenn Sie einen Mandanten entfernen, haben die Benutzer in diesem Mandanten keinen Zugriff mehr auf das Partner Center-Konto, und die Entfernung hat möglicherweise Auswirkungen auf Ihre Kompetenzen. 

## <a name="next-steps"></a>Nächste Schritte

- [Erstellen von Benutzerkonten](create-user-accounts-and-set-permissions.md)






