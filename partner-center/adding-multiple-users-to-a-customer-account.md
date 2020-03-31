---
title: Erstellen mehrerer Benutzer für ein Kundenkonto | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in Partner Center hochladen.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: jasonwhowell
ms.author: jasonh
keywords: Stapelweises Hochladen, mehrere Benutzer einem Kundenkonto hinzufügen, Kunden eines Benutzers hinzufügen, stapelweises Hochladen der Benutzer des Kunden, Kundenkonto, Kunden des Benutzers, Benutzer
ms.localizationpriority: medium
ms.openlocfilehash: 499aff67d18b0d8f9fbaf098fecbab2d888d9ac7
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390369"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="67db2-104">Hinzufügen von mehreren Benutzern zu einem Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="67db2-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="67db2-105">**Gilt für:**</span><span class="sxs-lookup"><span data-stu-id="67db2-105">**Applies to**</span></span>

- <span data-ttu-id="67db2-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="67db2-106">Partner Center</span></span>

<span data-ttu-id="67db2-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="67db2-107">**Appropriate roles**</span></span>

- <span data-ttu-id="67db2-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="67db2-108">Global admin</span></span>

<span data-ttu-id="67db2-109">Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="67db2-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="67db2-110">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="67db2-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="67db2-111">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="67db2-111">Data file requirements</span></span>

<span data-ttu-id="67db2-112">Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="67db2-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="67db2-113">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="67db2-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="67db2-114">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="67db2-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="67db2-115">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="67db2-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="67db2-116">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="67db2-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="67db2-117">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="67db2-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="67db2-118">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="67db2-118">Enter only the data described below.</span></span> <span data-ttu-id="67db2-119">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="67db2-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="67db2-120">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="67db2-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="67db2-121">**Name der Spalte**</span><span class="sxs-lookup"><span data-stu-id="67db2-121">**Column name**</span></span> | <span data-ttu-id="67db2-122">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="67db2-122">**Description**</span></span>                                                              | <span data-ttu-id="67db2-123">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="67db2-123">**Limitation**</span></span>                             |
| <span data-ttu-id="67db2-124">Vorname</span><span class="sxs-lookup"><span data-stu-id="67db2-124">First name</span></span>      | <span data-ttu-id="67db2-125">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="67db2-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="67db2-126">Begrenzung von 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="67db2-126">50-character limit</span></span>                         |
| <span data-ttu-id="67db2-127">Nachname</span><span class="sxs-lookup"><span data-stu-id="67db2-127">Last name</span></span>       | <span data-ttu-id="67db2-128">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="67db2-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="67db2-129">Begrenzung von 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="67db2-129">50-character limit</span></span>                         |
| <span data-ttu-id="67db2-130">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="67db2-130">Display name</span></span>    | <span data-ttu-id="67db2-131">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="67db2-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="67db2-132">Begrenzung von 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="67db2-132">50-character limit</span></span>                         |
| <span data-ttu-id="67db2-133">E-Mail</span><span class="sxs-lookup"><span data-stu-id="67db2-133">Email</span></span>           | <span data-ttu-id="67db2-134">Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)</span><span class="sxs-lookup"><span data-stu-id="67db2-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="67db2-135">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen.</span><span class="sxs-lookup"><span data-stu-id="67db2-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="67db2-136">Statusupdate</span><span class="sxs-lookup"><span data-stu-id="67db2-136">Status update</span></span>   | <span data-ttu-id="67db2-137">Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="67db2-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="67db2-138">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="67db2-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="67db2-139">So erstellen Sie mehrere Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="67db2-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="67db2-140">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="67db2-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="67db2-141">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="67db2-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="67db2-142">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="67db2-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="67db2-143">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="67db2-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="67db2-144">Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.</span><span class="sxs-lookup"><span data-stu-id="67db2-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="67db2-145">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="67db2-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="67db2-146">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="67db2-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="67db2-147">Wählen Sie **Überprüfen**.</span><span class="sxs-lookup"><span data-stu-id="67db2-147">Select **Validate**.</span></span>

    <span data-ttu-id="67db2-148">**Hinweis**  Die meisten Fehler bei der Kontoerstellung werden durch Datendateiprobleme verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in der Datei.</span><span class="sxs-lookup"><span data-stu-id="67db2-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="67db2-149">Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="67db2-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="67db2-150">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="67db2-150">Select **Save**.</span></span>
10. <span data-ttu-id="67db2-151">Laden Sie die Informationen zum temporären Kennwort für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="67db2-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="67db2-152">**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="67db2-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="67db2-153">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="67db2-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="67db2-154">Neuen Benutzern werden automatisch die Berechtigungen **Can use licenses and services** zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="67db2-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



