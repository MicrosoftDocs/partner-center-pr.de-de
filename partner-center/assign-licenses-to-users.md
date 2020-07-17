---
title: Verwalten von Benutzern in Kundenkonten
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Benutzerkonten für einen Kunden erstellen, Benutzerlizenzen hinzufügen oder entfernen, Benutzer Kennwörter zurücksetzen, Benutzerkonten löschen oder wiederherstellen.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 18b1fd689db84d20b62389841c5e5474d97ff1cb
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435959"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="1d9f4-103">Benutzer Verwaltungsaufgaben für Kundenkonten im Partner Center</span><span class="sxs-lookup"><span data-stu-id="1d9f4-103">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="1d9f4-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="1d9f4-104">**Applies to**</span></span>

- <span data-ttu-id="1d9f4-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="1d9f4-105">Partner Center</span></span>

<span data-ttu-id="1d9f4-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="1d9f4-106">**Appropriate roles**</span></span>

- <span data-ttu-id="1d9f4-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="1d9f4-107">Global admin</span></span>
- <span data-ttu-id="1d9f4-108">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="1d9f4-108">User management admin</span></span>
- <span data-ttu-id="1d9f4-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="1d9f4-109">Admin agent</span></span>
- <span data-ttu-id="1d9f4-110">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="1d9f4-110">Sales agent</span></span>
- <span data-ttu-id="1d9f4-111">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="1d9f4-111">Helpdesk agent</span></span>

<span data-ttu-id="1d9f4-112">Sie können neue Benutzer im Konto eines Kunden erstellen und löschen.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="1d9f4-113">Sie können auch ein oder mehrere Benutzerkonten wiederherstellen, die Sie zuvor innerhalb von 30 Tagen nach dem Löschvorgang gelöscht haben.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="1d9f4-114">Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).</span><span class="sxs-lookup"><span data-stu-id="1d9f4-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="1d9f4-115">Wenn Sie neue Abonnements für einen Kunden kaufen, sollte der Kunde eine Liste aller Benutzer erhalten, die Konten, die Benutzerberechtigungen und die von den einzelnen Benutzern benötigten Dienste benötigen.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="1d9f4-116">Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="1d9f4-117">Erstellen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="1d9f4-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="1d9f4-118">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1d9f4-119">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-119">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1d9f4-120">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-120">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="1d9f4-121">Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-121">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="1d9f4-122">**Speichern** Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-122">**Save** your changes.</span></span>

5. <span data-ttu-id="1d9f4-123">Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="1d9f4-124">Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-124">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="1d9f4-125">Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="1d9f4-126">Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="1d9f4-127">Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="1d9f4-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="1d9f4-128">Die folgenden Schritte gelten für das Hinzufügen oder Entfernen von Benutzerlizenzen für Microsoft-Produkte.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="1d9f4-129">Informationen zum Hinzufügen oder Entfernen von Benutzerlizenzen für Lizenz basierte Saas-Abonnements im kommerziellen Marketplace finden Sie unter [Hinzufügen oder Entfernen von Lizenzen für ein SaaS-Abonnement](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="1d9f4-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="1d9f4-130">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1d9f4-131">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-131">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1d9f4-132">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-132">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="1d9f4-133">Wählen Sie einen oder mehrere Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-133">Choose one or more users from the list.</span></span> <span data-ttu-id="1d9f4-134">Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese den Personen zuweisen möchten, die noch keine Lizenzen besitzen, können Sie mit der Option **Benutzer filtern nach …** die richtige Gruppe finden.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="1d9f4-135">Wählen Sie **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-135">Select **Manage licenses**.</span></span> <span data-ttu-id="1d9f4-136">Nehmen Sie Ihre Änderungen vor, und wählen Sie anschließend **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-136">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="1d9f4-137">Für [Azure Marketplace Produkte](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wird die Lizenz Zuweisung und-Aktivierung über den unabhängigen Software Hersteller (Independent Software Vendor, ISV) verwaltet, der das Produkt veröffentlicht hat.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="1d9f4-138">Zurücksetzen eines Benutzerkennworts für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="1d9f4-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="1d9f4-139">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1d9f4-140">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-140">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="1d9f4-141">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-141">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="1d9f4-142">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="1d9f4-143">Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-143">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="1d9f4-144">Senden Sie das neue temporäre Kennwort an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="1d9f4-145">Löschen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="1d9f4-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="1d9f4-146">Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-146">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="1d9f4-147">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="1d9f4-148">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-148">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="1d9f4-149">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="1d9f4-150">Wählen Sie unten auf dem Bildschirm die Option **Benutzerkonto löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-150">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="1d9f4-151">Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="1d9f4-152">Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="1d9f4-153">Wiederherstellen gelöschter Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="1d9f4-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="1d9f4-154">Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-154">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="1d9f4-155">Wählen Sie **Benutzer und Lizenzen**aus.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-155">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="1d9f4-156">Wählen Sie die Registerkarte **Gelöschte Benutzer ()** aus. Es sollte **(1)** oder größer sein, wenn gelöschte Benutzer wieder hergestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="1d9f4-157">Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-157">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="1d9f4-158">Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="1d9f4-159">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="1d9f4-159">Related topics</span></span>


[<span data-ttu-id="1d9f4-160">Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="1d9f4-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="1d9f4-161">Erstellen mehrerer Benutzer für ein Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="1d9f4-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)