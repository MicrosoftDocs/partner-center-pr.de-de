---
title: 'Partner Center Insights: rollenbasierte Zugriffs Steuerung | Partner Center'
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bestimmte Rollen sind erforderlich, um Insights-Berichte anzuzeigen.
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI, Leistung, Kunden Erfolg, Messungen, Rollen
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945862"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="66ca8-104">Rollenbasierte Zugriffs Steuerung für das Insights-Dashboard</span><span class="sxs-lookup"><span data-stu-id="66ca8-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="66ca8-105">Das Insights-Dashboard verwendet zwei neue Rollen im Partner Center, um den Mitarbeiter Zugriff auf die Berichte-Executive Report Viewer und Report Viewer zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="66ca8-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="66ca8-106">Benutzer in der Rolle "Executive Report Viewer" haben Zugriff auf alle Berichts Datasets, während Benutzer in der Rolle "Berichts-Viewer" keinen Zugriff auf sensible Datasets haben, wie z. b. Umsatz und persönliche Daten von Kunden und Mitarbeitern.</span><span class="sxs-lookup"><span data-stu-id="66ca8-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="66ca8-107">Wie bei anderen Partner Center-Rollen kann der globale Administrator oder der Konto Administrator diesen Rollen auf der Seite "Benutzerverwaltung" Benutzer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="66ca8-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="66ca8-108">Die Rollen können auf das gesamte Unternehmen oder auf bestimmte MPN-Orte angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="66ca8-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="66ca8-109">Rollen, die für bestimmte MPN-Orte zugewiesen werden, begrenzen den Benutzer für die Anzeige von Berichtsdaten, die nur den ausgewählten MPN-Orten zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="66ca8-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="66ca8-110">Partner können einen oder mehrere Standorte aus der folgenden Ansicht auswählen.</span><span class="sxs-lookup"><span data-stu-id="66ca8-110">Partner can select one or multiple locations from the below view.</span></span>

![Rollen](images/pci/roles.png)

><span data-ttu-id="66ca8-112">Nebenbei Benutzer, die MPN-Administratoren seit dem 20. Januar 2020 sind, werden automatisch der unternehmensweiten Rolle "Executive Report Viewer" für alle Standorte dieses Mandanten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="66ca8-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="66ca8-113">Diese Benutzer können auf die Berichte als Executive Report Viewer zugreifen, ohne dass für den globalen Administrator oder Konto Administrator eine explizite Aktion erforderlich ist. Die globalen Administratoren und Konto Administratoren können die automatisch zugewiesenen Rollen dieser Benutzer außer Kraft setzen, um ihre Funktionen weiter zu erhöhen oder einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="66ca8-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>