---
title: Verwalten von Benutzern für Kundenkonten
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Verwalten von Benutzern für Ihre Kunden im Partner Center: Erstellen von Benutzerkonten, hinzufügen oder Entfernen von Benutzerlizenzen, Zurücksetzen von Kenn Wörtern und löschen oder Wiederherstellen von Benutzerkonten.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756075"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="994cf-103">Verwalten von Benutzern und Benutzerlizenzen für Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="994cf-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="994cf-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="994cf-104">**Appropriate roles**</span></span>

- <span data-ttu-id="994cf-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="994cf-105">Global admin</span></span>
- <span data-ttu-id="994cf-106">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="994cf-106">User management admin</span></span>
- <span data-ttu-id="994cf-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="994cf-107">Admin agent</span></span>


<span data-ttu-id="994cf-108">Sie können neue Benutzer im Konto eines Kunden erstellen und löschen.</span><span class="sxs-lookup"><span data-stu-id="994cf-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="994cf-109">Sie können auch ein oder mehrere Benutzerkonten wiederherstellen, die Sie zuvor innerhalb von 30 Tagen nach dem Löschvorgang gelöscht haben.</span><span class="sxs-lookup"><span data-stu-id="994cf-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="994cf-110">Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).</span><span class="sxs-lookup"><span data-stu-id="994cf-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="994cf-111">Wenn Sie neue Abonnements für einen Kunden kaufen, sollte der Kunde eine Liste aller Benutzer erhalten, die Konten, die Benutzerberechtigungen und die von den einzelnen Benutzern benötigten Dienste benötigen.</span><span class="sxs-lookup"><span data-stu-id="994cf-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="994cf-112">Im Abschnitt **Benutzer und Lizenzen** der Registerkarte **Kunde** werden alle Benutzer angezeigt, die im Mandanten eines bestimmten Kunden erstellt wurden, einschließlich der Benutzer, die über Lizenzen verfügen, die von einem anderen CSP-Partner oder einem anderen Einkaufskanal erworben wurden</span><span class="sxs-lookup"><span data-stu-id="994cf-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="994cf-113">Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.</span><span class="sxs-lookup"><span data-stu-id="994cf-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="994cf-114">Erstellen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="994cf-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="994cf-115">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="994cf-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="994cf-116">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="994cf-117">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="994cf-118">Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein.</span><span class="sxs-lookup"><span data-stu-id="994cf-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="994cf-119">**Speichern** Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="994cf-119">**Save** your changes.</span></span>

5. <span data-ttu-id="994cf-120">Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.</span><span class="sxs-lookup"><span data-stu-id="994cf-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="994cf-121">Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.</span><span class="sxs-lookup"><span data-stu-id="994cf-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="994cf-122">Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="994cf-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="994cf-123">Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.</span><span class="sxs-lookup"><span data-stu-id="994cf-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="994cf-124">Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="994cf-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="994cf-125">Die folgenden Schritte gelten für das Hinzufügen oder Entfernen von Benutzerlizenzen für Microsoft-Produkte.</span><span class="sxs-lookup"><span data-stu-id="994cf-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="994cf-126">Informationen zum Hinzufügen oder Entfernen von Benutzerlizenzen für Lizenz basierte Saas-Abonnements im kommerziellen Marketplace finden Sie unter [Hinzufügen oder Entfernen von Lizenzen für ein SaaS-Abonnement](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="994cf-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="994cf-127">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="994cf-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="994cf-128">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="994cf-129">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="994cf-130">Wählen Sie einen oder mehrere Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-130">Choose one or more users from the list.</span></span> <span data-ttu-id="994cf-131">Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese den Personen zuweisen möchten, die noch keine Lizenzen besitzen, können Sie mit der Option **Benutzer filtern nach …** die richtige Gruppe finden.</span><span class="sxs-lookup"><span data-stu-id="994cf-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="994cf-132">Wählen Sie **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="994cf-132">Select **Manage licenses**.</span></span> <span data-ttu-id="994cf-133">Nehmen Sie Ihre Änderungen vor, und wählen Sie anschließend **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="994cf-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="994cf-134">Für [Azure Marketplace Produkte](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wird die Lizenz Zuweisung und-Aktivierung über den unabhängigen Software Hersteller (Independent Software Vendor, ISV) verwaltet, der das Produkt veröffentlicht hat.</span><span class="sxs-lookup"><span data-stu-id="994cf-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="994cf-135">Zurücksetzen eines Benutzerkennworts für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="994cf-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="994cf-136">Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="994cf-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="994cf-137">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="994cf-138">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="994cf-139">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="994cf-140">Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**.</span><span class="sxs-lookup"><span data-stu-id="994cf-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="994cf-141">Senden Sie das neue temporäre Kennwort an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="994cf-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="994cf-142">Löschen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="994cf-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="994cf-143">Wählen Sie im **Partner Center** -Menü die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="994cf-144">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="994cf-145">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="994cf-146">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="994cf-147">Wählen Sie unten auf dem Bildschirm die Option **Benutzerkonto löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="994cf-148">Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden.</span><span class="sxs-lookup"><span data-stu-id="994cf-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="994cf-149">Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.</span><span class="sxs-lookup"><span data-stu-id="994cf-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="994cf-150">Wiederherstellen gelöschter Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="994cf-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="994cf-151">Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="994cf-152">Wählen Sie **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="994cf-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="994cf-153">Wählen Sie die Registerkarte **Gelöschte Benutzer ()** aus. Es sollte **(1)** oder größer sein, wenn gelöschte Benutzer wieder hergestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="994cf-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="994cf-154">Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="994cf-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="994cf-155">Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="994cf-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="994cf-156">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="994cf-156">Next steps</span></span>

- [<span data-ttu-id="994cf-157">Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="994cf-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="994cf-158">Erstellen mehrerer Benutzer für ein Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="994cf-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)