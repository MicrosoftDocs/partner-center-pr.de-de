---
title: Anmeldung bei Partner Center nicht möglich
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Beheben sie mögliche Ursachen, und erfahren Sie mehr über Lösungen, wenn Sie sich nicht bei Partner Center anmelden können. Erfahren Sie mehr über das Zurücksetzen von Kennwörtern, das Überprüfen von Rollen und das Überprüfen von Anmeldeinformationen.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818795"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Behandeln von Anmeldeproblemen für Partner Center

**Geeignete Rollen:** Alle Partner, die an Partner Center interessiert sind

Dieser Artikel enthält Lösungen für häufige Anmeldeprobleme bei Partner Center.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Sie haben Ihr Kennwort für Partner Center

Wenn Sie Ihr Kennwort vergessen haben und sich nicht bei Partner Center anmelden können, wenden Sie sich an den Support. Die entsprechende Kontaktperson finden Sie unter [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).

Wenn Sie MPN-Partner sind, bitten Sie Ihren globalen Administrator, ein neues Kennwort für Sie zu erstellen. Wenn Sie ein indirekter CSP-Vertriebspartner sind, bitten Sie Ihren indirekten Anbieter, einen neuen globalen Administrator für Sie in Ihrem Azure AD Mandanten zu erstellen oder ein neues Kennwort für Sie mit den delegierten Administratorrechten zu erstellen.

Weitere Informationen dazu, wie Sie Ihr Kennwort zurücksetzen und den Zugriff auf Ihr Arbeitskonto wiederherstellen können, finden Sie unter [Zurücksetzen Ihres Arbeits- oder Schulkennworts mithilfe von Sicherheitsinformationen.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Sie können die erwarteten Seiten oder Funktionen in Partner Center

Der Zugriff auf Seiten in Partner Center wird durch die Ihnen zugewiesenen Rollen gesteuert. Um zu überprüfen, welche Rollen Ihnen zugewiesen sind, klicken Sie in Partner Center auf das Symbol Einstellungen, wählen **Sie Kontoeinstellungen** und dann unter Kontoeinstellungen die Option **Benutzerverwaltung** aus. Geben Sie unter Suchen Ihren Namen ein, und zeigen Sie dann die Ergebnisse an.

Wenn Sie die erwarteten Kompetenzen, Kunden, Incentives oder Benutzer nicht anzeigen oder verwalten können, probieren Sie die folgenden Lösungen aus:

- Wenden Sie sich an Ihren globalen Administrator oder Kontoadministrator, um Zugriff auf die Funktionen von MPN, CSP und Empfehlungen zu erhalten. Weitere Informationen zu Rollen und den Aufgaben, die sie in Partner Center aktivieren, finden Sie unter [Zuweisen von Rollen & Berechtigungen zu Benutzern.](permissions-overview.md)
- Um Zugriff auf die Funktionen des kommerziellen Marketplace und der Windows & Xbox-, Office Store-, Microsoft Edge- und Hardwareentwicklerprogramme zu erhalten, wenden Sie sich an die Person mit der Rolle "Besitzer" oder "Manager" in Ihrer Organisation. Weitere Informationen zu Rollen und Berechtigungen finden Sie unter Verwalten eines Kontos im [kommerziellen Marketplace in Microsoft Partner Center.](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Sie können Ihr Angebot oder Ihre Vorteile nicht in der Partner Center

Vergewissern Sie sich, dass Sie die richtigen Anmeldeinformationen für die Anmeldung verwenden. Beispielsweise können Ihre geschäfts- und persönlichen Konten gleich aussehen (z. B. ), aber eines kann ein persönliches Konto sein, das Sie erstellt haben, und ein anderes kann ein Geschäftskonto sein, das in Ihrem Namen abc@contoso.com eingerichtet wurde. Wenn Sie in diesem Fall angemeldet sind, aber die erwarteten Funktionen im Zusammenhang mit MPN, CSP und kommerziellem Marketplace nicht anzeigen können, versuchen Sie, Ihr Geschäftskonto auszuwählen.

## <a name="next-steps"></a>Nächste Schritte

- [Kontoinformationen überprüfen](verification-responses.md)
- [Zurücksetzen meines Kennworts](reset-my-pasword.md)
- [Zurücksetzen eines Benutzerkennworts](reset-a-user-password.md)