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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389515"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator

Es gibt viele Gründe, warum Sie möglicherweise mehrere Azure AD Mandanten in Ihrem Partner Center-Konto verwalten müssen. Beispielsweise kann Ihr Unternehmen ein anderes Unternehmen erwerben und möchten, dass die Mitarbeiter des neuen Unternehmens Partner Center verwenden können. Sie möchten jedoch, dass die beiden Unternehmen getrennt bleiben. In diesem Fall würden Sie den Azure AD Mandanten des neuen Unternehmens Ihrem Partner-globalen Konto (PNG) zuordnen. Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.

## <a name="add-another-azure-ad-tenant-to-your-account"></a>Fügen Sie Ihrem Konto einen weiteren Azure AD Mandanten hinzu.

1. Melden Sie sich als globaler Administrator beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.
1. Wählen Sie auf dem Symbol " **Einstellungen** " die Option **Kontoeinstellungen** und dann Mandanten **aus.**
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="Mandanten zuordnen"::: 

3. Wählen Sie **anderen AD** -Mandanten zuordnen aus, und geben Sie den Mandanten an, den Sie zuordnen möchten

1. Melden Sie sich als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und bestätigen Sie die Zuordnung. 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="Zuordnen von Mandanten bestätigen"::: 

5. Nachdem Sie sich vergewissert haben, wird eine Benachrichtigung über den Hinweis " **alle** " angezeigt.  Wählen Sie **zur Mandanten Verwaltung zurückkehren aus,** damit der neu hinzugefügte Mandant aufgeführt wird.
 
## <a name="next-steps"></a>Nächste Schritte

- [Hinzufügen von Benutzern](create-user-accounts-and-set-permissions.md)
