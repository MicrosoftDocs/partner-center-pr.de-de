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
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528180"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="60da4-103">Hinzufügen mehrerer Benutzer zu einem Kundenkonto durch Erstellen einer CSV-Datei</span><span class="sxs-lookup"><span data-stu-id="60da4-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="60da4-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="60da4-104">**Applies to**</span></span>

- <span data-ttu-id="60da4-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="60da4-105">Partner Center</span></span>

<span data-ttu-id="60da4-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="60da4-106">**Appropriate roles**</span></span>

- <span data-ttu-id="60da4-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="60da4-107">Global admin</span></span>

<span data-ttu-id="60da4-108">Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="60da4-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="60da4-109">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="60da4-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="60da4-110">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="60da4-110">Data file requirements</span></span>

<span data-ttu-id="60da4-111">Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="60da4-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="60da4-112">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="60da4-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="60da4-113">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="60da4-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="60da4-114">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="60da4-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="60da4-115">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="60da4-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="60da4-116">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="60da4-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="60da4-117">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="60da4-117">Enter only the data described below.</span></span> <span data-ttu-id="60da4-118">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="60da4-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="60da4-119">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="60da4-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="60da4-120">**Spaltenname**</span><span class="sxs-lookup"><span data-stu-id="60da4-120">**Column name**</span></span> | <span data-ttu-id="60da4-121">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="60da4-121">**Description**</span></span>  | <span data-ttu-id="60da4-122">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="60da4-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="60da4-123">Vorname</span><span class="sxs-lookup"><span data-stu-id="60da4-123">First name</span></span>  | <span data-ttu-id="60da4-124">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="60da4-124">User's first name (optional field)</span></span>  | <span data-ttu-id="60da4-125">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="60da4-125">50-character limit</span></span>  |
| <span data-ttu-id="60da4-126">Nachname</span><span class="sxs-lookup"><span data-stu-id="60da4-126">Last name</span></span>  | <span data-ttu-id="60da4-127">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="60da4-127">User's last name (optional field)</span></span>  | <span data-ttu-id="60da4-128">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="60da4-128">50-character limit</span></span>  |
| <span data-ttu-id="60da4-129">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="60da4-129">Display name</span></span>    | <span data-ttu-id="60da4-130">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="60da4-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="60da4-131">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="60da4-131">50-character limit</span></span>                         |
| <span data-ttu-id="60da4-132">E-Mail</span><span class="sxs-lookup"><span data-stu-id="60da4-132">Email</span></span>   | <span data-ttu-id="60da4-133">Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)</span><span class="sxs-lookup"><span data-stu-id="60da4-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="60da4-134">Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen.</span><span class="sxs-lookup"><span data-stu-id="60da4-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="60da4-135">Statusaktualisierung</span><span class="sxs-lookup"><span data-stu-id="60da4-135">Status update</span></span>   | <span data-ttu-id="60da4-136">Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="60da4-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="60da4-137">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="60da4-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="60da4-138">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="60da4-138">Next steps</span></span>

- [<span data-ttu-id="60da4-139">Vorgehensweise beim Hinzufügen von mehreren Benutzern für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="60da4-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)