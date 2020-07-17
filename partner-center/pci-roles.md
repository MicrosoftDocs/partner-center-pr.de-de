---
title: Rollen basierter Zugriff auf Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informieren Sie sich über die spezifischen Rollen, die zum Anzeigen von Partner Center Insights-Berichten erforderlich sind Hierzu gehören die Rollen des Executive Report Viewer und der Berichts-Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a9df2b6f67ca4e825da2c273c82d7cd46763f1b
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436639"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="9d1ab-104">Rollenbasierte Zugriffs Steuerung für das Partner Center Insights-Dashboard</span><span class="sxs-lookup"><span data-stu-id="9d1ab-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="9d1ab-105">Das Insights-Dashboard verwendet zwei neue Rollen im Partner Center, um den Mitarbeiter Zugriff auf die Berichte-Executive Report Viewer und Report Viewer zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="9d1ab-106">Benutzer in der Rolle "Executive Report Viewer" haben Zugriff auf alle Berichts Datasets, während Benutzer in der Rolle "Berichts-Viewer" keinen Zugriff auf sensible Datasets haben, wie z. b. Umsatz und persönliche Daten von Kunden und Mitarbeitern.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="9d1ab-107">Wie bei anderen Partner Center-Rollen kann der globale Administrator oder der Konto Administrator diesen Rollen auf der Seite "Benutzerverwaltung" Benutzer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="9d1ab-108">Die Rollen können auf das gesamte Unternehmen oder auf bestimmte MPN-Orte angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="9d1ab-109">Rollen, die für bestimmte MPN-Orte zugewiesen werden, begrenzen den Benutzer für die Anzeige von Berichtsdaten, die nur den ausgewählten MPN-Orten zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="9d1ab-110">Partner können einen oder mehrere Standorte aus der folgenden Ansicht auswählen.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-110">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Rollen":::

>[!Note]
> <span data-ttu-id="9d1ab-112">Benutzer, die MPN-Administratoren seit dem 20. Januar 2020 sind, werden automatisch der unternehmensweiten **Executive Report Viewer** -Rolle für alle Standorte dieses Mandanten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-112">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="9d1ab-113">Diese Benutzer können auf die Berichte als Executive Report Viewer zugreifen, ohne dass für den globalen Administrator oder Konto Administrator eine explizite Aktion erforderlich ist. Die globalen Administratoren und Konto Administratoren können die automatisch zugewiesenen Rollen dieser Benutzer außer Kraft setzen, um ihre Funktionen weiter zu erhöhen oder einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9d1ab-114">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="9d1ab-114">Next steps</span></span>

- <span data-ttu-id="9d1ab-115">Erfahren Sie mehr über [Partner Center Insights](partner-center-insights.md) und die verschiedenen Berichte.</span><span class="sxs-lookup"><span data-stu-id="9d1ab-115">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
