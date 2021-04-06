---
title: Felder für CSV-Datei zum Importieren mehrerer Benutzer für ein Kundenkonto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wenn Sie einem Kundenkonto mehrere Benutzer hinzufügen möchten, erstellen Sie eine Datei mit Komma getrennten Werten (CSV-Datei) mit entsprechenden Feldern.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441420"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="71546-103">Hinzufügen mehrerer Benutzer zu einem Kundenkonto durch Erstellen einer CSV-Datei</span><span class="sxs-lookup"><span data-stu-id="71546-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="71546-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="71546-104">**Appropriate roles**</span></span>

- <span data-ttu-id="71546-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="71546-105">Global admin</span></span>

<span data-ttu-id="71546-106">Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="71546-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="71546-107">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="71546-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="71546-108">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="71546-108">Data file requirements</span></span>

<span data-ttu-id="71546-109">Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="71546-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="71546-110">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="71546-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="71546-111">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="71546-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="71546-112">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="71546-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="71546-113">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="71546-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="71546-114">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="71546-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="71546-115">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="71546-115">Enter only the data described below.</span></span> <span data-ttu-id="71546-116">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="71546-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="71546-117">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="71546-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="71546-118">**Spaltenname**</span><span class="sxs-lookup"><span data-stu-id="71546-118">**Column name**</span></span> | <span data-ttu-id="71546-119">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="71546-119">**Description**</span></span>  | <span data-ttu-id="71546-120">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="71546-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="71546-121">Vorname</span><span class="sxs-lookup"><span data-stu-id="71546-121">First name</span></span>  | <span data-ttu-id="71546-122">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="71546-122">User's first name (optional field)</span></span>  | <span data-ttu-id="71546-123">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="71546-123">50-character limit</span></span>  |
| <span data-ttu-id="71546-124">Nachname</span><span class="sxs-lookup"><span data-stu-id="71546-124">Last name</span></span>  | <span data-ttu-id="71546-125">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="71546-125">User's last name (optional field)</span></span>  | <span data-ttu-id="71546-126">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="71546-126">50-character limit</span></span>  |
| <span data-ttu-id="71546-127">`Display name`</span><span class="sxs-lookup"><span data-stu-id="71546-127">Display name</span></span>    | <span data-ttu-id="71546-128">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="71546-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="71546-129">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="71546-129">50-character limit</span></span>                         |
| <span data-ttu-id="71546-130">Email</span><span class="sxs-lookup"><span data-stu-id="71546-130">Email</span></span>   | <span data-ttu-id="71546-131">Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)</span><span class="sxs-lookup"><span data-stu-id="71546-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="71546-132">Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen.</span><span class="sxs-lookup"><span data-stu-id="71546-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="71546-133">Statusaktualisierung</span><span class="sxs-lookup"><span data-stu-id="71546-133">Status update</span></span>   | <span data-ttu-id="71546-134">Wird verwendet, um anzugeben, ob der neue Benutzerdaten Satz erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="71546-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="71546-135">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="71546-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="71546-136">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="71546-136">Next steps</span></span>

- [<span data-ttu-id="71546-137">Hinzufügen mehrerer Benutzer für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="71546-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)