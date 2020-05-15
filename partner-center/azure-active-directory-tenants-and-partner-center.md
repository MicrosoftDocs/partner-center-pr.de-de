---
title: Arbeitskonten und Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, warum Sie ein Geschäftskonto benötigen, um ein Partner Center-Konto zu erstellen. Überprüfen Sie, ob Sie bereits über ein Geschäftskonto verfügen.
author: LauraBrenner
ms.author: labrenne
Keywords: Geschäftskonto, E-Mail-Adresse, Mandant, Azure-Mandant, Konto erstellen, Domänenname
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: e34eecb482df140a1a225d0d28460ef957701d59
ms.sourcegitcommit: af3ecd7f35e5bb3b87f5f683335c76e287f2a9b8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83369267"
---
# <a name="your-company-work-account-and-partner-center"></a>Das Geschäftskonto Ihrer Firma und Partner Center  

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator

## <a name="why-you-need-a-work-account"></a>Warum Sie ein Geschäftskonto benötigen

Microsoft setzt voraus, dass Sie das Geschäftskonto Ihres Unternehmens mit Ihrem neuen Partner Center-Konto verknüpfen. Der Link ermöglicht es Kontobenutzern, sich mit den Benutzernamen und Kennwörtern ihres Geschäftskontos bei Partner Center anzumelden.

## <a name="the-work-account-email-address"></a>Die E-Mail-Adresse des Geschäftskontos

Ihr Geschäftskonto oder Ihre geschäftliche E-Mail-Adresse ist die von Ihrem Unternehmen für Sie bereitgestellte E-Mail-Adresse. Eine E-Mail-Adresse des Geschäftskontos hat normalerweise das Format `you@yourcompany.com`. Persönliche E-Mail-Adressen, beispielsweise bei Hotmail, Gmail oder Yahoo, stellen keine geschäftliche E-Mail-Adresse dar und können nicht für Ihr Partner Center-Konto verwendet werden.

Wenn Sie mehr als eine gültige geschäftliche E-Mail-Adresse haben, verwenden Sie die Adresse, die dem Hauptsitz Ihres Unternehmens zugeordnet ist, statt der regionalen Abteilung. Verwenden Sie beispielsweise statt der `contoso.uk`-E-Mail-Adresse Ihre `contoso.com`-Adresse.

> [!NOTE]  
> Bevor Sie beschließen, ein vorhandenes Geschäftskonto zu verwenden, überlegen Sie, wie viele Benutzer des Kontos im Partner Center arbeiten müssen. Wenn das Konto Benutzer enthält, die nicht im Partner Center arbeiten müssen, erwägen Sie die Erstellung eines neuen Kontos nur für diese Benutzer.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Sie sind nicht sicher, ob Ihre Firma bereits ein Geschäftskonto hat?

Wenn Sie nicht genau wissen, ob Ihr Unternehmen ein Geschäftskonto hat, können Sie das mit den folgenden Schritten überprüfen. Mit einem aktiven Abonnement für Microsoft Azure oder Office 365 besitzen Sie bereits ein Geschäftskonto.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com) an.

2. Wählen Sie im Menü „Azure Active Directory“ und dann „Domänennamen“ aus.

3. Wenn Sie bereits ein Geschäftskonto haben, wird Ihr Domänenname aufgeführt.

Falls Ihr Unternehmen noch kein Geschäftskonto hat, können Sie eines während des Registrierungsprozesses erstellen.

Das folgende Diagramm enthält die Schritte für mehrere typische Szenarien:

- Ermitteln, ob Sie ein Geschäftskonto haben
- Ermitteln, wie Sie sich bei Ihrem Geschäftskonto anmelden
- Ermitteln, ob Sie ein neues Geschäftskonto erstellen müssen

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Besitzen Sie ein Geschäftskonto oder müssen Sie eins erstellen?":::

Weitere Informationen zum Hinzufügen von Domänen in Azure AD finden Sie unter [Hinzufügen oder Zuordnen einer Domäne in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain).

## <a name="about-microsoft-azure"></a>Informationen zu Microsoft Azure

Microsoft Azure ist eine öffentliche Cloudplattform, die Unternehmen zum Erstellen, Bereitstellen und Verwalten von Apps in einem globalen Netzwerk von durch Microsoft verwalteten Rechenzentren verwenden können. Unternehmen nutzen Azure zum Erstellen einer virtuellen IT-Infrastruktur mit virtuellen Funktionen oder Diensten anstelle von physischen Computern.

Wenn Sie ein Azure-Abonnement erwerben, mieten Sie im Wesentlichen einen dedizierten, sicheren Bereich in der öffentlichen Azure-Cloud. Dies ist dem Mieten eines Stockwerks in einem Bürogebäude für das physische Geschäft Ihres Unternehmens sehr ähnlich. Für den Eigentümer des Bürogebäudes ist Ihr Unternehmen ein Mieter.

Ein Azure-Geschäftskonto ist eine dedizierte und isolierte virtuelle Darstellung Ihres Unternehmens in der öffentlichen Azure-Cloud. Das Konto wird für Sie erstellt, wenn Sie einen Microsoft Cloud Service wie Azure, Microsoft Intune oder Office 365 abonnieren.

Das Geschäftskonto hostet Ihre Azure AD-Benutzer und die zugehörigen Informationen – Kennwörter, Profildaten, Berechtigungen usw. Zudem enthält das Geschäftskonto Gruppen, Anwendungen und andere Informationen, die ein Unternehmen und seine Sicherheit betreffen.
