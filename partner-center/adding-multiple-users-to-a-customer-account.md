---
title: Hinzufügen mehrerer Benutzer für ein Kundenkonto
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Um dem Konto eines Kunden mehrere Benutzer hinzuzufügen, laden Sie eine Datendatei in Partner Center mithilfe des csv-Dateiformats (durch Komma getrennte Werte) hoch.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150470"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="c88c9-103">Hochladen einer CSV-Datei von Benutzern in das Konto eines Kunden</span><span class="sxs-lookup"><span data-stu-id="c88c9-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="c88c9-104">**Geeignete Rollen**: Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="c88c9-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c88c9-105">Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im durch Komma getrennten Wertdateiformat (CSV) in die Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c88c9-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="c88c9-106">Erstellen der Datei mit Kundenbenutzern und Hochladen in das Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="c88c9-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="c88c9-107">Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten.</span><span class="sxs-lookup"><span data-stu-id="c88c9-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="c88c9-108">Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.</span><span class="sxs-lookup"><span data-stu-id="c88c9-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="c88c9-109">Informationen zum Importieren mehrerer Benutzer für ein Kundenkonto finden Sie unter Felder für [die CSV-Datei.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="c88c9-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="c88c9-110">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="c88c9-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="c88c9-111">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c88c9-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="c88c9-112">Wählen Sie die Registerkarte Benutzer **und Lizenzen des** Kunden und dann Benutzer hochladen **aus.**</span><span class="sxs-lookup"><span data-stu-id="c88c9-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="c88c9-113">Wählen Sie unter **Upload user info** die Option **Durchsuchen**.</span><span class="sxs-lookup"><span data-stu-id="c88c9-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="c88c9-114">Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="c88c9-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="c88c9-115">Wählen Sie **Überprüfen** aus.</span><span class="sxs-lookup"><span data-stu-id="c88c9-115">Select **Validate**.</span></span>

    <span data-ttu-id="c88c9-116">**Hinweis:** Der Großteil der Fehler bei der Kontoerstellung wird durch Datendateifehler verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in einer Datei.</span><span class="sxs-lookup"><span data-stu-id="c88c9-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="c88c9-117">Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="c88c9-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="c88c9-118">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="c88c9-118">Select **Save**.</span></span>
10. <span data-ttu-id="c88c9-119">Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.</span><span class="sxs-lookup"><span data-stu-id="c88c9-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="c88c9-120">Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, weil dies später nicht mehr möglich ist.</span><span class="sxs-lookup"><span data-stu-id="c88c9-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="c88c9-121">Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="c88c9-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="c88c9-122">Neuen Benutzern werden automatisch Berechtigungen von Kann Lizenzen und Dienste **verwenden zugewiesen.**</span><span class="sxs-lookup"><span data-stu-id="c88c9-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c88c9-123">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="c88c9-123">Next steps</span></span>

- [<span data-ttu-id="c88c9-124">Erteilen sie Kunden die Berechtigung, Partner Center eigene Produkte oder Dienste zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="c88c9-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
