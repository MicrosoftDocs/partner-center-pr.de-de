---
title: Hinzufügen mehrerer Benutzer für ein Kundenkonto
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wenn Sie dem Konto eines Kunden mehrere Benutzer hinzufügen möchten, laden Sie mithilfe des CSV-Datei Formats (Comma-Separated Value, CSV) eine Datendatei in das Partner Center hoch.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535740"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="5d539-103">Hochladen einer CSV-Datei von Benutzern in das Konto eines Kunden</span><span class="sxs-lookup"><span data-stu-id="5d539-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="5d539-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="5d539-104">**Applies to**</span></span>

- <span data-ttu-id="5d539-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="5d539-105">Partner Center</span></span>

<span data-ttu-id="5d539-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="5d539-106">**Appropriate roles**</span></span>

- <span data-ttu-id="5d539-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="5d539-107">Global admin</span></span>

<span data-ttu-id="5d539-108">Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in das Partner Center hochladen.</span><span class="sxs-lookup"><span data-stu-id="5d539-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="5d539-109">Erstellen der Datei von Kunden Benutzern und Hochladen in das Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="5d539-109">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="5d539-110">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="5d539-110">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="5d539-111">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="5d539-111">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="5d539-112">Weitere Informationen finden [Sie Unterfelder für CSV-Datei, um mehrere Benutzer für ein Kundenkonto zu importieren](file-customer-users.md).</span><span class="sxs-lookup"><span data-stu-id="5d539-112">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="5d539-113">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="5d539-113">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="5d539-114">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="5d539-114">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="5d539-115">Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.</span><span class="sxs-lookup"><span data-stu-id="5d539-115">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="5d539-116">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="5d539-116">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="5d539-117">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="5d539-117">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="5d539-118">Wählen Sie **Überprüfen** aus.</span><span class="sxs-lookup"><span data-stu-id="5d539-118">Select **Validate**.</span></span>

    <span data-ttu-id="5d539-119">**Hinweis**    Die meisten Fehler bei der Kontoerstellung werden durch Probleme mit der Datendatei verursacht, darunter fehlende Informationen, falsch formatierte oder doppelte e-Mail-Adressen oder zu viele Datensätze in der Datei.</span><span class="sxs-lookup"><span data-stu-id="5d539-119">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="5d539-120">Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="5d539-120">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="5d539-121">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="5d539-121">Select **Save**.</span></span>
10. <span data-ttu-id="5d539-122">Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="5d539-122">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="5d539-123">Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, weil dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="5d539-123">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="5d539-124">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="5d539-124">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="5d539-125">Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="5d539-125">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="5d539-126">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="5d539-126">Next steps</span></span>

- [<span data-ttu-id="5d539-127">Erteilen Sie Kunden eine Berechtigung im Partner Center, um Ihre eigenen Produkte oder Dienste zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="5d539-127">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
