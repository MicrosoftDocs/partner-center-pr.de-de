---
title: Erstellen mehrerer Benutzer für ein Kundenkonto | Partner Center
description: Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in Partner Center hochladen.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: Stapelweises Hochladen, mehrere Benutzer einem Kundenkonto hinzufügen, Kunden eines Benutzers hinzufügen, stapelweises Hochladen der Benutzer des Kunden, Kundenkonto, Kunden des Benutzers, Benutzer
ms.localizationpriority: medium
ms.openlocfilehash: e7a5e7f9c0cebf81373c500dd3a552710fcf845a
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876970"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="2bc39-104">Hinzufügen von mehreren Benutzern zu einem Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="2bc39-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="2bc39-105">Betrifft</span><span class="sxs-lookup"><span data-stu-id="2bc39-105">Applies to</span></span>**

-  <span data-ttu-id="2bc39-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="2bc39-106">Partner Center</span></span>

<span data-ttu-id="2bc39-107">Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in Partner-Dashboard hochladen.</span><span class="sxs-lookup"><span data-stu-id="2bc39-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Dashboard.</span></span> <span data-ttu-id="2bc39-108">Sie können eine Beispieldatendatei aus dem Partner-Dashboard herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.</span><span class="sxs-lookup"><span data-stu-id="2bc39-108">You can download a sample data file from the Partner Dashboard and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="2bc39-109">Anforderungen an die Datendatei</span><span class="sxs-lookup"><span data-stu-id="2bc39-109">Data file requirements</span></span>


<span data-ttu-id="2bc39-110">Damit Sie mit dem Massenupload mehrere Benutzer zum Konto eines Kunden hinzufügen können, müssen die folgenden Voraussetzungen erfüllt sein:</span><span class="sxs-lookup"><span data-stu-id="2bc39-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="2bc39-111">Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.</span><span class="sxs-lookup"><span data-stu-id="2bc39-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="2bc39-112">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.</span><span class="sxs-lookup"><span data-stu-id="2bc39-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="2bc39-113">Sie können bis zu 100Datensätze gleichzeitig hochladen.</span><span class="sxs-lookup"><span data-stu-id="2bc39-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="2bc39-114">Wenn Sie mehr als 100Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.</span><span class="sxs-lookup"><span data-stu-id="2bc39-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="2bc39-115">Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.</span><span class="sxs-lookup"><span data-stu-id="2bc39-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="2bc39-116">Geben Sie nur die unten beschriebenen Daten ein.</span><span class="sxs-lookup"><span data-stu-id="2bc39-116">Enter only the data described below.</span></span> <span data-ttu-id="2bc39-117">Zusätzliche Daten führen zu einem Uploadfehler.</span><span class="sxs-lookup"><span data-stu-id="2bc39-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="2bc39-118">Geben Sie die folgenden Daten in die Datendatei ein:</span><span class="sxs-lookup"><span data-stu-id="2bc39-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="2bc39-119">Name der Spalte</span><span class="sxs-lookup"><span data-stu-id="2bc39-119">Column name</span></span>** | **<span data-ttu-id="2bc39-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bc39-120">Description</span></span>**                                                              | **<span data-ttu-id="2bc39-121">Einschränkung</span><span class="sxs-lookup"><span data-stu-id="2bc39-121">Limitation</span></span>**                             |
| <span data-ttu-id="2bc39-122">Vorname</span><span class="sxs-lookup"><span data-stu-id="2bc39-122">First name</span></span>      | <span data-ttu-id="2bc39-123">Vorname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="2bc39-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="2bc39-124">Begrenzung von 50Zeichen</span><span class="sxs-lookup"><span data-stu-id="2bc39-124">50-character limit</span></span>                         |
| <span data-ttu-id="2bc39-125">Nachname</span><span class="sxs-lookup"><span data-stu-id="2bc39-125">Last name</span></span>       | <span data-ttu-id="2bc39-126">Nachname des Benutzers (optionales Feld)</span><span class="sxs-lookup"><span data-stu-id="2bc39-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="2bc39-127">Begrenzung von 50Zeichen</span><span class="sxs-lookup"><span data-stu-id="2bc39-127">50-character limit</span></span>                         |
| <span data-ttu-id="2bc39-128">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="2bc39-128">Display name</span></span>    | <span data-ttu-id="2bc39-129">Der im Partner-Dashboard angezeigte Name (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="2bc39-129">Name displayed in the Partner Dashboard (required field)</span></span>                            | <span data-ttu-id="2bc39-130">Begrenzung von 50Zeichen</span><span class="sxs-lookup"><span data-stu-id="2bc39-130">50-character limit</span></span>                         |
| <span data-ttu-id="2bc39-131">E-Mail</span><span class="sxs-lookup"><span data-stu-id="2bc39-131">Email</span></span>           | <span data-ttu-id="2bc39-132">Geschäftliche E-Mail-Adresse des Benutzers beim Kundenunternehmen (erforderliches Feld)</span><span class="sxs-lookup"><span data-stu-id="2bc39-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="2bc39-133">Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen.</span><span class="sxs-lookup"><span data-stu-id="2bc39-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="2bc39-134">Statusupdate</span><span class="sxs-lookup"><span data-stu-id="2bc39-134">Status update</span></span>   | <span data-ttu-id="2bc39-135">Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="2bc39-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="2bc39-136">\*\*Keine Angabe\*\*</span><span class="sxs-lookup"><span data-stu-id="2bc39-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="2bc39-137">So erstellen Sie mehrere Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="2bc39-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="2bc39-138">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="2bc39-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="2bc39-139">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="2bc39-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="2bc39-140">Wählen Sie im Menü **Dashboard** die Option **Kunden**, und wählen Sie anschließend einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="2bc39-140">From the **Dashboard** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="2bc39-141">Wählen Sie **Upload users**.</span><span class="sxs-lookup"><span data-stu-id="2bc39-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="2bc39-142">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="2bc39-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="2bc39-143">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="2bc39-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="2bc39-144">Wählen Sie **Überprüfen**.</span><span class="sxs-lookup"><span data-stu-id="2bc39-144">Select **Validate**.</span></span>

    <span data-ttu-id="2bc39-145">**Hinweis:** Der Großteil der Fehler bei der Kontoerstellung wird durch Datendateifehler verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in einer Datei.</span><span class="sxs-lookup"><span data-stu-id="2bc39-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="2bc39-146">Wählen Sie nach der Überprüfung der Datei durch das Partner-Dashboard den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="2bc39-146">After the Partner Dashboard validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="2bc39-147">Wählen Sie **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="2bc39-147">Select **Save**.</span></span>
9.  <span data-ttu-id="2bc39-148">Laden Sie die Informationen zum temporären Kennwort für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="2bc39-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="2bc39-149">**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="2bc39-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="2bc39-150">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="2bc39-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="2bc39-151">Neue Benutzer werden automatisch Berechtigungen **use Licenses and Services** zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="2bc39-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



