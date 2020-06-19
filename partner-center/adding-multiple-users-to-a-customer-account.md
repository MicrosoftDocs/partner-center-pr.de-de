---
title: Hinzufügen mehrerer Benutzer für ein Kundenkonto
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen. Laden Sie eine Datendatei mit dem Dateiformat mit Komma getrennten Werten (CSV-Datei) in Partner Center hoch.
author: LauraBrenner
ms.author: labrenne
keywords: Massenupload, einem Kundenkonto mehrere Benutzer hinzufügen, Benutzer eines Kunden hinzufügen, Massenupload der Benutzer eines Kunden, Kundenkonto, Kundenbenutzer, Benutzer
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 09bb83b82cf1db78a54af9bab98a5cbdaa00c0d9
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991082"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="96add-105">Hinzufügen mehrerer Benutzer zu einem Kundenkonto: Hochladen einer Datendatei in Partner Center</span><span class="sxs-lookup"><span data-stu-id="96add-105">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="96add-106">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="96add-106">**Applies to**</span></span>

- <span data-ttu-id="96add-107">Partner Center</span><span class="sxs-lookup"><span data-stu-id="96add-107">Partner Center</span></span>

<span data-ttu-id="96add-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="96add-108">**Appropriate roles**</span></span>

- <span data-ttu-id="96add-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="96add-109">Global admin</span></span>

<span data-ttu-id="96add-110">Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="96add-110">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="96add-111">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="96add-111">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="96add-112">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="96add-112">Data file requirements</span></span>

<span data-ttu-id="96add-113">Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:</span><span class="sxs-lookup"><span data-stu-id="96add-113">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="96add-114">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="96add-114">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="96add-115">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="96add-115">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="96add-116">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="96add-116">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="96add-117">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="96add-117">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="96add-118">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="96add-118">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="96add-119">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="96add-119">Enter only the data described below.</span></span> <span data-ttu-id="96add-120">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="96add-120">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="96add-121">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="96add-121">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="96add-122">**Spaltenname**</span><span class="sxs-lookup"><span data-stu-id="96add-122">**Column name**</span></span> | <span data-ttu-id="96add-123">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="96add-123">**Description**</span></span>                                                              | <span data-ttu-id="96add-124">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="96add-124">**Limitation**</span></span>                             |
| <span data-ttu-id="96add-125">Vorname</span><span class="sxs-lookup"><span data-stu-id="96add-125">First name</span></span>      | <span data-ttu-id="96add-126">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="96add-126">User's first name (optional field)</span></span>                                           | <span data-ttu-id="96add-127">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="96add-127">50-character limit</span></span>                         |
| <span data-ttu-id="96add-128">Nachname</span><span class="sxs-lookup"><span data-stu-id="96add-128">Last name</span></span>       | <span data-ttu-id="96add-129">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="96add-129">User's last name (optional field)</span></span>                                            | <span data-ttu-id="96add-130">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="96add-130">50-character limit</span></span>                         |
| <span data-ttu-id="96add-131">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="96add-131">Display name</span></span>    | <span data-ttu-id="96add-132">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="96add-132">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="96add-133">Maximal 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="96add-133">50-character limit</span></span>                         |
| <span data-ttu-id="96add-134">E-Mail</span><span class="sxs-lookup"><span data-stu-id="96add-134">Email</span></span>           | <span data-ttu-id="96add-135">Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)</span><span class="sxs-lookup"><span data-stu-id="96add-135">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="96add-136">Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen.</span><span class="sxs-lookup"><span data-stu-id="96add-136">Each user must have a unique email address</span></span> |
| <span data-ttu-id="96add-137">Statusaktualisierung</span><span class="sxs-lookup"><span data-stu-id="96add-137">Status update</span></span>   | <span data-ttu-id="96add-138">Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="96add-138">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="96add-139">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="96add-139">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="96add-140">So erstellen Sie mehrere Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="96add-140">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="96add-141">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="96add-141">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="96add-142">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="96add-142">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="96add-143">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="96add-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="96add-144">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="96add-144">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="96add-145">Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.</span><span class="sxs-lookup"><span data-stu-id="96add-145">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="96add-146">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="96add-146">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="96add-147">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="96add-147">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="96add-148">Wählen Sie **Überprüfen** aus.</span><span class="sxs-lookup"><span data-stu-id="96add-148">Select **Validate**.</span></span>

    <span data-ttu-id="96add-149">**Hinweis**    Die meisten Fehler bei der Kontoerstellung werden durch Probleme mit der Datendatei verursacht, darunter fehlende Informationen, falsch formatierte oder doppelte e-Mail-Adressen oder zu viele Datensätze in der Datei.</span><span class="sxs-lookup"><span data-stu-id="96add-149">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="96add-150">Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="96add-150">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="96add-151">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="96add-151">Select **Save**.</span></span>
10. <span data-ttu-id="96add-152">Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="96add-152">Download the temporary password information for the users.</span></span>

<span data-ttu-id="96add-153">**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="96add-153">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="96add-154">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="96add-154">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="96add-155">Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="96add-155">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



