---
title: rollenbasierter Partner Center Insights-Zugriff
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die spezifischen Rollen, die erforderlich sind, um Partner Center Insights-Berichte anzuzeigen. Dazu gehören die Rollen des Berichts-Viewers der Geschäftsleitung und des Berichts-Viewers.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb06a863218446b0e88b38af242b4dac044560c0
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565303"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="015d7-104">Rollenbasierte Zugriffssteuerung für das Partner Center Insights-Dashboard</span><span class="sxs-lookup"><span data-stu-id="015d7-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="015d7-105">**Geeignete Rollen:** globale | | des Administrator-Agents Berichts-Viewer-| Berichtanzeige der Geschäftsleitung</span><span class="sxs-lookup"><span data-stu-id="015d7-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="015d7-106">Das Insights-Dashboard verwendet zwei neue Rollen in Partner Center, um den Mitarbeiterzugriff auf die Berichte zu verwalten: Berichts-Viewer der Geschäftsleitung und Berichts-Viewer.</span><span class="sxs-lookup"><span data-stu-id="015d7-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="015d7-107">Benutzer in der Rolle "Berichts-Viewer der Geschäftsleitung" haben Zugriff auf alle Berichtsdatasets, während Benutzer in der Berichts-Viewer-Rolle keinen Zugriff auf vertrauliche Datasets wie Umsatz- und personenbezogene Daten von Kunden/Mitarbeitern haben.</span><span class="sxs-lookup"><span data-stu-id="015d7-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="015d7-108">Wie bei anderen Partner Center Rollen kann der globale Administrator oder der Kontoadministrator diesen Rollen auf der Seite Benutzerverwaltung Benutzer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="015d7-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="015d7-109">Die Rollen können für das gesamte Unternehmen oder für bestimmte MPN-Standorte (Microsoft Partner Network) gelten.</span><span class="sxs-lookup"><span data-stu-id="015d7-109">The roles can be applicable across the entire company or for specific Microsoft Partner Network (MPN) location(s).</span></span> <span data-ttu-id="015d7-110">Rollen, die für bestimmte MPN-Speicherorte zugewiesen sind, beschränken den Benutzer auf die Anzeige von Berichtsdaten, die nur den ausgewählten MPN-Speicherorten zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="015d7-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="015d7-111">Partner können einen oder mehrere Standorte aus der folgenden Ansicht auswählen.</span><span class="sxs-lookup"><span data-stu-id="015d7-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Zeigt standortspezifische Partner Center Insights-Rolleneinstellungen für Berichts-Viewer und Berichts-Viewer der Geschäftsleitung an.":::

>[!Note]
> <span data-ttu-id="015d7-113">Benutzer, die ab dem 20. Januar 2020 MPN-Partneradministratoren sind, werden automatisch der unternehmensweiten Rolle **Executive Report Viewer** für alle Standorte für diesen Mandanten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="015d7-113">Users who are MPN partner admins as of January 20, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="015d7-114">Diese Benutzer können daher ohne explizite Aktion des globalen Administrators oder Kontoadministrators auf die Berichte als Managerberichts-Viewer zugreifen. Die globalen Administratoren und Kontoadministratoren können die automatisch zugewiesenen Rollen dieser Benutzer überschreiben, um ihre Funktionen weiter zu erhöhen oder einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="015d7-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="015d7-115">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="015d7-115">Next steps</span></span>

- <span data-ttu-id="015d7-116">Erfahren Sie mehr über [Partner Center Insights](partner-center-insights.md) und die verschiedenen Berichte.</span><span class="sxs-lookup"><span data-stu-id="015d7-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
