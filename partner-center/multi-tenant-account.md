---
title: Fügen Sie Ihrem Partner Center-Konto weitere Mandanten hinzu.
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verwalten mehrerer Mandanten über Ihr Partner Center-Konto
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846958"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator

Mit diesem Feature können Sie mehrere Mandanten für Ihr Unternehmen verwalten und sie in Ihrem Partner Center-Konto konsolidieren. Es gibt viele Gründe, warum Sie möglicherweise mehrere Azure AD Mandanten in Ihrem Partner Center-Konto verwalten müssen. Beispiel:

- Ihr Unternehmen kann ein anderes Unternehmen erwerben und möchten, dass die Mitarbeiter des neuen Unternehmens Partner Center verwenden können. Sie möchten jedoch, dass die beiden Unternehmen getrennt bleiben. In diesem Fall würden Sie den Azure AD Mandanten des neuen Unternehmens mit ihrem globalen Partner Konto (PGA) verknüpfen. Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.

- Wenn Sie über mehr als einen Mandanten verfügen, um Ihr Unternehmen auszuführen (z. b. contoso.com, contoso.uk, contoso.in), können Sie die mehr Instanzen Fähigkeit verwenden, um Sie mit dem gleichen PC-Konto zu verknüpfen.

- Bei Fusionen und Übernahmen müssen Sie mit mehr als einem Mandanten arbeiten (Wenn Contoso beispielsweise Fabrikam übernimmt), müssen Sie in der Lage sein, sowohl constoso.com als auch fabrikam.com entsprechende Mandanten zu verwenden.

- Benutzer von einem der Mandanten müssen folgende Aktionen ausführen können:
    1.  Access Partner Center für Schulungen, digitale Downloads, MCP-Zuordnung
    2.  Ihnen werden Partner Center-Rollen wie MPN admin, Incentive admin usw. zugewiesen.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Fügen Sie Ihrem Konto einen weiteren Azure AD Mandanten hinzu.

1. Melden Sie sich als globaler Administrator beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.
1. Wählen Sie auf dem Symbol " **Einstellungen** " die Option **Kontoeinstellungen** und dann Mandanten **aus.**
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Mandanten zuordnen"::: 

3. Wählen Sie **anderen AD** -Mandanten zuordnen aus, und geben Sie den Mandanten an, den Sie zuordnen möchten

1. Melden Sie sich als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und bestätigen Sie die Zuordnung. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zuordnen von Mandanten bestätigen"::: 

5. Nachdem Sie sich vergewissert haben, wird eine Benachrichtigung über den Hinweis " **alle** " angezeigt.  Wählen Sie **zur Mandanten Verwaltung zurückkehren aus,** damit der neu hinzugefügte Mandant aufgeführt wird. 
 

>[!NOTE]
>Sie können einem Konto keinen Mandanten zuordnen, wenn dieser bereits einem anderen Partner Center-Konto zugeordnet ist.

 
## <a name="next-steps"></a>Nächste Schritte

- [Hinzufügen von Benutzern](create-user-accounts-and-set-permissions.md)
