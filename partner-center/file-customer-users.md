---
title: Felder für die CSV-Datei zum Importieren mehrerer Benutzer für ein Kundenkonto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Um einem Kundenkonto mehrere Benutzer hinzuzufügen, erstellen Sie eine csv-Datei (durch Komma getrennte Werte) mit entsprechenden Feldern.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150980"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="b48a5-103">Hinzufügen mehrerer Benutzer zu einem Kundenkonto durch Erstellen einer CSV-Datei</span><span class="sxs-lookup"><span data-stu-id="b48a5-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="b48a5-104">**Geeignete Rollen**: Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b48a5-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="b48a5-105">Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im durch Komma getrennten Wertdateiformat (CSV) in die Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b48a5-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="b48a5-106">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="b48a5-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="b48a5-107">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="b48a5-107">Data file requirements</span></span>

<span data-ttu-id="b48a5-108">Um dem Konto eines Kunden mithilfe des Massenuploadprozesses mehrere Benutzer hinzuzufügen, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="b48a5-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="b48a5-109">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="b48a5-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="b48a5-110">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="b48a5-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="b48a5-111">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="b48a5-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="b48a5-112">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="b48a5-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="b48a5-113">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="b48a5-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="b48a5-114">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="b48a5-114">Enter only the data described below.</span></span> <span data-ttu-id="b48a5-115">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="b48a5-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="b48a5-116">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="b48a5-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="b48a5-117">**Spaltenname**</span><span class="sxs-lookup"><span data-stu-id="b48a5-117">**Column name**</span></span> | <span data-ttu-id="b48a5-118">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="b48a5-118">**Description**</span></span>  | <span data-ttu-id="b48a5-119">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="b48a5-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="b48a5-120">Vorname</span><span class="sxs-lookup"><span data-stu-id="b48a5-120">First name</span></span>  | <span data-ttu-id="b48a5-121">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="b48a5-121">User's first name (optional field)</span></span>  | <span data-ttu-id="b48a5-122">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="b48a5-122">50-character limit</span></span>  |
| <span data-ttu-id="b48a5-123">Nachname</span><span class="sxs-lookup"><span data-stu-id="b48a5-123">Last name</span></span>  | <span data-ttu-id="b48a5-124">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="b48a5-124">User's last name (optional field)</span></span>  | <span data-ttu-id="b48a5-125">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="b48a5-125">50-character limit</span></span>  |
| <span data-ttu-id="b48a5-126">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b48a5-126">Display name</span></span>    | <span data-ttu-id="b48a5-127">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="b48a5-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="b48a5-128">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="b48a5-128">50-character limit</span></span>                         |
| <span data-ttu-id="b48a5-129">E-Mail</span><span class="sxs-lookup"><span data-stu-id="b48a5-129">Email</span></span>   | <span data-ttu-id="b48a5-130">Geschäftliche E-Mail-Adresse des Benutzers beim Kundenunternehmen (Pflichtfeld)</span><span class="sxs-lookup"><span data-stu-id="b48a5-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="b48a5-131">Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen.</span><span class="sxs-lookup"><span data-stu-id="b48a5-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="b48a5-132">Statusaktualisierung</span><span class="sxs-lookup"><span data-stu-id="b48a5-132">Status update</span></span>   | <span data-ttu-id="b48a5-133">Wird verwendet, um anzugeben, ob der neue Benutzerdatensatz erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b48a5-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="b48a5-134">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="b48a5-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="b48a5-135">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="b48a5-135">Next steps</span></span>

- [<span data-ttu-id="b48a5-136">Hinzufügen mehrerer Benutzer für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="b48a5-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)