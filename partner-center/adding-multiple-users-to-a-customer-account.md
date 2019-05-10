---
title: Erstellen mehrerer Benutzer für ein Kundenkonto | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in Partner Center hochladen.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: Massenupload, einem Kundenkonto mehrere Benutzer hinzufügen, Benutzer eines Kunden hinzufügen, Massenupload der Benutzer eines Kunden, Kundenkonto, Kundenbenutzer, Benutzer
ms.localizationpriority: medium
ms.openlocfilehash: b113736330b201ed6a4d1c6b8915e844b80fe5d5
ms.sourcegitcommit: f916aa2884239b205398c24d04d1f1dc41b63c2b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2019
ms.locfileid: "64668148"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="e9b8f-104">Hinzufügen von mehreren Benutzern zu einem Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="e9b8f-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="e9b8f-105">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="e9b8f-105">**Applies to**</span></span>

-  <span data-ttu-id="e9b8f-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e9b8f-106">Partner Center</span></span>

<span data-ttu-id="e9b8f-107">Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="e9b8f-108">Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="e9b8f-109">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="e9b8f-109">Data file requirements</span></span>


<span data-ttu-id="e9b8f-110">Damit Sie mit dem Massenupload mehrere Benutzer zum Konto eines Kunden hinzufügen können, müssen die folgenden Voraussetzungen erfüllt sein:</span><span class="sxs-lookup"><span data-stu-id="e9b8f-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="e9b8f-111">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="e9b8f-112">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="e9b8f-113">Sie können bis zu 100 Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="e9b8f-114">Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="e9b8f-115">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="e9b8f-116">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-116">Enter only the data described below.</span></span> <span data-ttu-id="e9b8f-117">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="e9b8f-118">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="e9b8f-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="e9b8f-119">**Spaltenname**</span><span class="sxs-lookup"><span data-stu-id="e9b8f-119">**Column name**</span></span> | <span data-ttu-id="e9b8f-120">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="e9b8f-120">**Description**</span></span>                                                              | <span data-ttu-id="e9b8f-121">**Einschränkung**</span><span class="sxs-lookup"><span data-stu-id="e9b8f-121">**Limitation**</span></span>                             |
| <span data-ttu-id="e9b8f-122">Vorname</span><span class="sxs-lookup"><span data-stu-id="e9b8f-122">First name</span></span>      | <span data-ttu-id="e9b8f-123">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="e9b8f-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="e9b8f-124">Begrenzung von 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="e9b8f-124">50-character limit</span></span>                         |
| <span data-ttu-id="e9b8f-125">Nachname</span><span class="sxs-lookup"><span data-stu-id="e9b8f-125">Last name</span></span>       | <span data-ttu-id="e9b8f-126">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="e9b8f-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="e9b8f-127">Begrenzung von 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="e9b8f-127">50-character limit</span></span>                         |
| <span data-ttu-id="e9b8f-128">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="e9b8f-128">Display name</span></span>    | <span data-ttu-id="e9b8f-129">Der im Partner Center angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="e9b8f-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="e9b8f-130">Begrenzung von 50 Zeichen</span><span class="sxs-lookup"><span data-stu-id="e9b8f-130">50-character limit</span></span>                         |
| <span data-ttu-id="e9b8f-131">E-Mail</span><span class="sxs-lookup"><span data-stu-id="e9b8f-131">Email</span></span>           | <span data-ttu-id="e9b8f-132">Geschäftliche E-Mail-Adresse des Benutzers beim Kundenunternehmen (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="e9b8f-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="e9b8f-133">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="e9b8f-134">Statusupdate</span><span class="sxs-lookup"><span data-stu-id="e9b8f-134">Status update</span></span>   | <span data-ttu-id="e9b8f-135">Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="e9b8f-136">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="e9b8f-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="e9b8f-137">So erstellen Sie mehrere Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="e9b8f-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="e9b8f-138">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="e9b8f-139">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="e9b8f-140">Wählen Sie im Menü **Partner Center** die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="e9b8f-141">Wählen Sie **Upload users**.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="e9b8f-142">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="e9b8f-143">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="e9b8f-144">Wählen Sie **Überprüfen**.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-144">Select **Validate**.</span></span>

    <span data-ttu-id="e9b8f-145">**Hinweis**  Die meisten Fehler bei der Kontoerstellung werden durch Datendateiprobleme verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in der Datei.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="e9b8f-146">Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="e9b8f-147">Wählen Sie **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-147">Select **Save**.</span></span>
9.  <span data-ttu-id="e9b8f-148">Laden Sie die Informationen zum temporären Kennwort für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="e9b8f-149">**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, weil dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="e9b8f-150">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="e9b8f-151">Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e9b8f-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



