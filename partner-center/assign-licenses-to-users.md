---
title: Verwalten von Benutzern für Kundenkonten
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Verwalten von Benutzern für Ihre Kunden in Partner Center: Erstellen Von Benutzerkonten, Hinzufügen oder Entfernen von Benutzerlizenzen, Zurücksetzen von Kennwörtern und Löschen oder Wiederherstellen von Benutzerkonten.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149892"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="a54cd-103">Verwalten von Benutzern und Benutzerlizenzen für Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="a54cd-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="a54cd-104">**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="a54cd-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="a54cd-105">Sie können neue Benutzer im Konto eines Kunden erstellen und löschen.</span><span class="sxs-lookup"><span data-stu-id="a54cd-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="a54cd-106">Sie können auch ein oder mehrere Benutzerkonten wiederherstellen, die Sie zuvor innerhalb von 30 Tagen nach dem Löschen gelöscht haben.</span><span class="sxs-lookup"><span data-stu-id="a54cd-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="a54cd-107">Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).</span><span class="sxs-lookup"><span data-stu-id="a54cd-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="a54cd-108">Wenn Sie neue Abonnements für einen Kunden erwerben, sollte der Kunde Ihnen eine Liste aller Benutzer zur Verfügung stellen, die Konten benötigen, deren Benutzerberechtigungen und welche Dienste jeder Benutzer benötigt.</span><span class="sxs-lookup"><span data-stu-id="a54cd-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="a54cd-109">Im Abschnitt Benutzer  und **Lizenzen** der Registerkarte Kunde werden alle Benutzer angezeigt, die im Mandanten eines bestimmten Kunden erstellt wurden, einschließlich Der Benutzer, die Lizenzen von einem anderen CSP-Partner oder einem anderen Kaufkanal erworben haben.</span><span class="sxs-lookup"><span data-stu-id="a54cd-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="a54cd-110">Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.</span><span class="sxs-lookup"><span data-stu-id="a54cd-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="a54cd-111">Erstellen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="a54cd-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="a54cd-112">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="a54cd-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a54cd-113">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a54cd-114">Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.**</span><span class="sxs-lookup"><span data-stu-id="a54cd-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="a54cd-115">Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein.</span><span class="sxs-lookup"><span data-stu-id="a54cd-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="a54cd-116">**Speichern** Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="a54cd-116">**Save** your changes.</span></span>

5. <span data-ttu-id="a54cd-117">Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.</span><span class="sxs-lookup"><span data-stu-id="a54cd-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="a54cd-118">Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.</span><span class="sxs-lookup"><span data-stu-id="a54cd-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="a54cd-119">Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="a54cd-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="a54cd-120">Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.</span><span class="sxs-lookup"><span data-stu-id="a54cd-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="a54cd-121">Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="a54cd-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="a54cd-122">Die folgenden Schritte gelten für das Hinzufügen oder Entfernen von Benutzerlizenzen für Microsoft-Produkte.</span><span class="sxs-lookup"><span data-stu-id="a54cd-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="a54cd-123">Informationen zum Hinzufügen oder Entfernen von Benutzerlizenzen für lizenzbasierte SaaS-Abonnements im kommerziellen Marketplace finden Sie unter Hinzufügen oder Entfernen von Lizenzen [für ein SaaS-Abonnement.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="a54cd-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="a54cd-124">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="a54cd-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a54cd-125">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a54cd-126">Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.**</span><span class="sxs-lookup"><span data-stu-id="a54cd-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="a54cd-127">Wählen Sie einen oder mehrere Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-127">Choose one or more users from the list.</span></span> <span data-ttu-id="a54cd-128">Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese Personen zuweisen möchten, die noch nicht über diese verfügen, können Sie die Option Benutzer nach **filtern nach...** verwenden, um die richtige Gruppe zu finden.</span><span class="sxs-lookup"><span data-stu-id="a54cd-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="a54cd-129">Wählen Sie **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="a54cd-129">Select **Manage licenses**.</span></span> <span data-ttu-id="a54cd-130">Nehmen Sie Ihre Änderungen vor, und speichern **Sie dann**.</span><span class="sxs-lookup"><span data-stu-id="a54cd-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="a54cd-131">Bei [Azure Marketplace-Produkten](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wird die Lizenzzuweisung und -aktivierung durch den unabhängigen Softwarehersteller (Independent Software Vendor, ISV) verwaltet, der das Produkt veröffentlicht hat.</span><span class="sxs-lookup"><span data-stu-id="a54cd-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="a54cd-132">Zurücksetzen eines Benutzerkennworts für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="a54cd-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="a54cd-133">Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="a54cd-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a54cd-134">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a54cd-135">Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.**</span><span class="sxs-lookup"><span data-stu-id="a54cd-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="a54cd-136">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="a54cd-137">Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**.</span><span class="sxs-lookup"><span data-stu-id="a54cd-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="a54cd-138">Senden Sie das neue temporäre Kennwort an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="a54cd-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="a54cd-139">Löschen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="a54cd-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="a54cd-140">Wählen Sie **Partner Center** Menü Kunden **aus.**</span><span class="sxs-lookup"><span data-stu-id="a54cd-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="a54cd-141">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="a54cd-142">Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.**</span><span class="sxs-lookup"><span data-stu-id="a54cd-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="a54cd-143">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="a54cd-144">Wählen Sie unten auf dem Bildschirm die Option **Benutzerkonto löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="a54cd-145">Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden.</span><span class="sxs-lookup"><span data-stu-id="a54cd-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="a54cd-146">Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.</span><span class="sxs-lookup"><span data-stu-id="a54cd-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="a54cd-147">Wiederherstellen gelöschter Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="a54cd-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="a54cd-148">Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a54cd-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="a54cd-149">Wählen Sie **Benutzer und Lizenzen aus.**</span><span class="sxs-lookup"><span data-stu-id="a54cd-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="a54cd-150">Wählen Sie **die Registerkarte Gelöschte Benutzer ( )** aus. Er sollte **(1) oder höher** lesen, wenn gelöschte Benutzer wiederhergestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="a54cd-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="a54cd-151">Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="a54cd-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="a54cd-152">Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a54cd-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a54cd-153">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="a54cd-153">Next steps</span></span>

- [<span data-ttu-id="a54cd-154">Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="a54cd-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="a54cd-155">Erstellen mehrerer Benutzer für ein Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="a54cd-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)