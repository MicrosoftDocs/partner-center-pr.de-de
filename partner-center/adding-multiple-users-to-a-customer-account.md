---
title: Hinzufügen mehrerer Benutzer für ein Kundenkonto
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen. Laden Sie eine Datendatei mit dem Dateiformat mit Komma getrennten Werten (CSV-Datei) in Partner Center hoch.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a9a94ac9d9022b33c7f909a258b66daa4312ad13
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436309"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="960df-104">Hinzufügen mehrerer Benutzer zu einem Kundenkonto: Hochladen einer Datendatei in Partner Center</span><span class="sxs-lookup"><span data-stu-id="960df-104">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="960df-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="960df-105">**Applies to**</span></span>

- <span data-ttu-id="960df-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="960df-106">Partner Center</span></span>

<span data-ttu-id="960df-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="960df-107">**Appropriate roles**</span></span>

- <span data-ttu-id="960df-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="960df-108">Global admin</span></span>

<span data-ttu-id="960df-109">Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="960df-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="960df-110">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="960df-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="960df-111">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="960df-111">Data file requirements</span></span>

<span data-ttu-id="960df-112">Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="960df-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="960df-113">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="960df-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="960df-114">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="960df-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="960df-115">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="960df-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="960df-116">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="960df-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="960df-117">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="960df-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="960df-118">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="960df-118">Enter only the data described below.</span></span> <span data-ttu-id="960df-119">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="960df-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="960df-120">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="960df-120">Enter the following data in the data file:</span></span>

| <span data-ttu-id="960df-121">**Spaltenname**</span><span class="sxs-lookup"><span data-stu-id="960df-121">**Column name**</span></span> | <span data-ttu-id="960df-122">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="960df-122">**Description**</span></span>  | <span data-ttu-id="960df-123">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="960df-123">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="960df-124">Vorname</span><span class="sxs-lookup"><span data-stu-id="960df-124">First name</span></span>  | <span data-ttu-id="960df-125">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="960df-125">User's first name (optional field)</span></span>  | <span data-ttu-id="960df-126">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="960df-126">50-character limit</span></span>  |
| <span data-ttu-id="960df-127">Nachname</span><span class="sxs-lookup"><span data-stu-id="960df-127">Last name</span></span>  | <span data-ttu-id="960df-128">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="960df-128">User's last name (optional field)</span></span>  | <span data-ttu-id="960df-129">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="960df-129">50-character limit</span></span>  |
| <span data-ttu-id="960df-130">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="960df-130">Display name</span></span>    | <span data-ttu-id="960df-131">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="960df-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="960df-132">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="960df-132">50-character limit</span></span>                         |
| <span data-ttu-id="960df-133">Email</span><span class="sxs-lookup"><span data-stu-id="960df-133">Email</span></span>   | <span data-ttu-id="960df-134">Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)</span><span class="sxs-lookup"><span data-stu-id="960df-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="960df-135">Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen.</span><span class="sxs-lookup"><span data-stu-id="960df-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="960df-136">Statusaktualisierung</span><span class="sxs-lookup"><span data-stu-id="960df-136">Status update</span></span>   | <span data-ttu-id="960df-137">Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="960df-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="960df-138">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="960df-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="960df-139">So erstellen Sie mehrere Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="960df-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="960df-140">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="960df-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="960df-141">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="960df-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="960df-142">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="960df-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="960df-143">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="960df-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="960df-144">Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.</span><span class="sxs-lookup"><span data-stu-id="960df-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="960df-145">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="960df-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="960df-146">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="960df-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="960df-147">Wählen Sie **Überprüfen** aus.</span><span class="sxs-lookup"><span data-stu-id="960df-147">Select **Validate**.</span></span>

    <span data-ttu-id="960df-148">**Hinweis**    Die meisten Fehler bei der Kontoerstellung werden durch Probleme mit der Datendatei verursacht, darunter fehlende Informationen, falsch formatierte oder doppelte e-Mail-Adressen oder zu viele Datensätze in der Datei.</span><span class="sxs-lookup"><span data-stu-id="960df-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="960df-149">Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="960df-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="960df-150">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="960df-150">Select **Save**.</span></span>
10. <span data-ttu-id="960df-151">Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="960df-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="960df-152">**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="960df-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="960df-153">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="960df-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="960df-154">Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="960df-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



