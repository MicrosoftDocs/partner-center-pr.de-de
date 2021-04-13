---
title: Anmeldung beim Partner Center nicht möglich.
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Behandeln Sie mögliche Ursachen, und erfahren Sie mehr über Lösungen, wenn Sie sich nicht bei Partner Center anmelden können. Weitere Informationen zum Zurücksetzen von Kenn Wörtern, überprüfen von Rollen und Überprüfen von Anmelde Informationen.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266570"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Problembehandlung bei Anmelde Problemen für Partner Center

**Geeignete Rollen**

- Alle Partner, die an Partner Center interessiert sind

Dieser Artikel enthält Lösungen für häufige Anmeldeprobleme für Partner Center.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Sie haben Ihr Kennwort für Partner Center vergessen.

Wenn Sie Ihr Kennwort vergessen haben und sich nicht bei Partner Center anmelden können, wenden Sie sich an den Support. Finden Sie den entsprechenden Kontakt zum [Support für Geschäftsprodukte](/microsoft-365/admin/contact-support-for-business-products).

Wenn Sie ein MPN-Partner sind, wenden Sie sich an ihren globalen Administrator, um ein neues Kennwort für Sie zu erstellen. Wenn Sie ein indirekter CSP-Reseller sind, bitten Sie den indirekten Anbieter, einen neuen globalen Administrator für Sie in Ihrem Azure AD Mandanten zu erstellen, oder erstellen Sie ein neues Kennwort für Sie, indem Sie die delegierten Administratorrechte verwenden.

Weitere Informationen dazu, wie Sie Ihr Kennwort zurücksetzen und wieder Zugriff auf Ihr Geschäftskonto erhalten, finden Sie unter [Zurücksetzen Ihres Geschäfts-oder Schul Kennworts mithilfe von Sicherheitsinformationen](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Sie können die erwarteten Seiten oder Funktionen im Partner Center nicht anzeigen oder verwalten.

Der Zugriff auf Seiten im Partner Center wird durch die zugewiesenen Rollen gesteuert. Wählen Sie im Partner Center das Symbol Einstellungen aus, wählen Sie **Kontoeinstellungen** aus, und wählen Sie dann Unterkonto Einstellungen die Option **Benutzerverwaltung** aus, um zu überprüfen, welche Rollen Ihnen zugewiesen sind. Geben Sie in suchen Ihren Namen ein, und zeigen Sie die Ergebnisse an.

Wenn Sie die von Ihnen erwarteten Kompetenzen, Kunden, Anreize oder Benutzer nicht anzeigen oder verwalten können, versuchen Sie es mit den folgenden Lösungen:

- Wenden Sie sich an ihren globalen Administrator oder Konto Administrator, um Zugriff auf die Funktionen von MPN, CSP und Referenzen zu erhalten. Weitere Informationen zu Rollen und den Aufgaben, die Sie in Partner Center aktivieren, finden Sie unter [Zuweisen von Rollen & Berechtigungen für Benutzer](permissions-overview.md).
- Wenden Sie sich an die Person in der Rolle "Besitzer" oder "Manager" in Ihrer Organisation, um Zugriff auf die Funktionen des kommerziellen Marketplace und der Windows & Xbox, Office Store, Microsoft Edge und Hardware Entwickler Programme zu erhalten. Weitere Informationen zu Rollen und Berechtigungen finden Sie unter [Verwalten eines kommerziellen Marketplace-Kontos im Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Sie können Ihr Angebot oder Ihre Vorteile nicht in Partner Center sehen.

Vergewissern Sie sich, dass Sie die richtigen Anmelde Informationen für die Anmeldung verwenden. Ihre geschäftlichen und persönlichen Konten können z. b. identisch sein (z. b. abc@contoso.com ), aber ein persönliches Konto, das Sie erstellt haben, und ein anderes können ein Geschäftskonto sein, das in Ihrem Namen eingerichtet ist. Wenn Sie in diesem Fall angemeldet sind, aber keine erwarteten Funktionen anzeigen können, die sich auf MPN, CSP, kommerzieller Marketplace beziehen, können Sie versuchen, Ihr Geschäftskonto auszuwählen.

## <a name="next-steps"></a>Nächste Schritte

- [Kontoinformationen überprüfen](verification-responses.md)
- [Zurücksetzen meines Kennworts](reset-my-pasword.md)
- [Zurücksetzen eines Benutzerkennworts](reset-a-user-password.md)