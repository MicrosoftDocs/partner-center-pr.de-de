---
title: Gewinnen von Erkenntnissen mit Kundenaktivitätsprotokollen
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Aktivitätsprotokolle anzeigen und exportieren, um Einblicke in Kundenkontotransaktionen und andere kundenbezogene Partnerverwaltungsaktivitäten zu erhalten.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150589"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="0a541-103">Anzeigen oder Exportieren von Kundenaktivitätsprotokollen für weitere Einblicke in Kundentransaktionen</span><span class="sxs-lookup"><span data-stu-id="0a541-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="0a541-104">**Geeignete Rollen:** globale | Abrechnungsadministrator-| | des Benutzerverwaltungsadministrators | des Administrator-Agents | des Vertriebsmitarbeiters Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="0a541-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="0a541-105">Aktivitätsprotokolle enthalten Informationen zu Transaktionen und Partnerverwaltungsaktionen für Kunden.</span><span class="sxs-lookup"><span data-stu-id="0a541-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="0a541-106">Protokolle für Transaktionen bieten detaillierte Informationen zu Transaktionen, einschließlich zahlungspflichtiger Abonnements.</span><span class="sxs-lookup"><span data-stu-id="0a541-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="0a541-107">Sie können Aktivitätsprotokolle auch in eine mit Excel kompatible durch Trennzeichen getrennte Datei (.csv) exportieren.</span><span class="sxs-lookup"><span data-stu-id="0a541-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="0a541-108">Aktivitätsprotokolle enthalten Datensätze für Partneraktionen für Kundenkonten und Produkttransaktionen.</span><span class="sxs-lookup"><span data-stu-id="0a541-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="0a541-109">Sie können Aktivitätsprotokolle auch in eine CSV-Datei exportieren.</span><span class="sxs-lookup"><span data-stu-id="0a541-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="0a541-110">Anzeigen und Exportieren von Aktivitätsprotokollen</span><span class="sxs-lookup"><span data-stu-id="0a541-110">View and export activity logs</span></span>

1. <span data-ttu-id="0a541-111">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="0a541-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="0a541-112">Wähle im Menü **Kontoeinstellungen** die Option **Aktivitätsprotokoll** aus.</span><span class="sxs-lookup"><span data-stu-id="0a541-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="0a541-113">Wählen Sie mithilfe der Felder **Von** und **Bis** den Aktivitätsprotokollierungszeitraum aus.</span><span class="sxs-lookup"><span data-stu-id="0a541-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="0a541-114">Für den Export des Aktivitätsprotokolls wird standardmäßig der letzte Monat festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0a541-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="0a541-115">Jedes Aktivitätsprotokoll enthält einen Link zur Seite **Abonnements** des aufgeführten Kunden.</span><span class="sxs-lookup"><span data-stu-id="0a541-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="0a541-116">Wählen Sie für ein beliebiges Aktivitätsprotokoll den Pfeil nach unten, um Details zu einer protokollierten Aktion anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="0a541-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="0a541-117">Ein einzelnes Aktivitätsprotokoll kann eine große Menge von Daten enthalten, beispielsweise Daten zur Bestellung mehrerer Produkte.</span><span class="sxs-lookup"><span data-stu-id="0a541-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="0a541-118">Zu den Datenspalten des Protokolls gehören u. a.:</span><span class="sxs-lookup"><span data-stu-id="0a541-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="0a541-119">**Date-Time**: Datum und Uhrzeit der Aktion</span><span class="sxs-lookup"><span data-stu-id="0a541-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="0a541-120">**Affected customer**: Firmenname des Kunden</span><span class="sxs-lookup"><span data-stu-id="0a541-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="0a541-121">**Action**: die vom Kunden ausgeführte Aktion, z. B. „hat eine Empfehlung erstellt“</span><span class="sxs-lookup"><span data-stu-id="0a541-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="0a541-122">**Partner user**: der mit der Aktivität verknüpfte Partner</span><span class="sxs-lookup"><span data-stu-id="0a541-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="0a541-123">Wählen Sie **Exportprotokoll** aus, um die Abonnementdaten des Kunden in eine CSV-Datei zu kopieren und in den Standarddownloadordner auf Ihrem Computer hochzuladen.</span><span class="sxs-lookup"><span data-stu-id="0a541-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0a541-124">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0a541-124">Next steps</span></span>

- [<span data-ttu-id="0a541-125">Analysieren von Abonnements und Lizenzen zur Unterstützung von Geschäftsentscheidungen</span><span class="sxs-lookup"><span data-stu-id="0a541-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
