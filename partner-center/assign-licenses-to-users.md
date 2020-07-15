---
title: Verwalten von Benutzern in Kundenkonten
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Benutzerkonten für einen Kunden erstellen, Benutzerlizenzen hinzufügen oder entfernen, Benutzer Kennwörter zurücksetzen, Benutzerkonten löschen oder wiederherstellen.
author: BillLinzbach
ms.author: BillLi
Keywords: Kundenverwaltung, Konto, Konto erstellen, Lizenzen, Lizenz zuweisen Benutzerverwaltung, Kennwort, Kennwort zurücksetzen, Kennwort ändern
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 57d5a91fda593b47d6e22b3682d0072b256ae655
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377684"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="bfd8a-104">Benutzer Verwaltungsaufgaben für Kundenkonten im Partner Center</span><span class="sxs-lookup"><span data-stu-id="bfd8a-104">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="bfd8a-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="bfd8a-105">**Applies to**</span></span>

- <span data-ttu-id="bfd8a-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="bfd8a-106">Partner Center</span></span>

<span data-ttu-id="bfd8a-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="bfd8a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="bfd8a-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="bfd8a-108">Global admin</span></span>
- <span data-ttu-id="bfd8a-109">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="bfd8a-109">User management admin</span></span>
- <span data-ttu-id="bfd8a-110">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="bfd8a-110">Admin agent</span></span>
- <span data-ttu-id="bfd8a-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="bfd8a-111">Sales agent</span></span>
- <span data-ttu-id="bfd8a-112">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="bfd8a-112">Helpdesk agent</span></span>

<span data-ttu-id="bfd8a-113">Sie können neue Benutzer im Konto eines Kunden erstellen und löschen.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-113">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="bfd8a-114">Sie können auch ein oder mehrere Benutzerkonten wiederherstellen, die Sie zuvor innerhalb von 30 Tagen nach dem Löschvorgang gelöscht haben.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-114">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="bfd8a-115">Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).</span><span class="sxs-lookup"><span data-stu-id="bfd8a-115">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="bfd8a-116">Wenn Sie neue Abonnements für einen Kunden kaufen, sollte der Kunde eine Liste aller Benutzer erhalten, die Konten, die Benutzerberechtigungen und die von den einzelnen Benutzern benötigten Dienste benötigen.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-116">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="bfd8a-117">Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-117">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="bfd8a-118">Erstellen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="bfd8a-118">Create user accounts for a customer</span></span>

1. <span data-ttu-id="bfd8a-119">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="bfd8a-120">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-120">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="bfd8a-121">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-121">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="bfd8a-122">Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-122">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="bfd8a-123">**Speichern** Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-123">**Save** your changes.</span></span>

5. <span data-ttu-id="bfd8a-124">Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-124">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="bfd8a-125">Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-125">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="bfd8a-126">Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-126">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="bfd8a-127">Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-127">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="bfd8a-128">Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="bfd8a-128">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="bfd8a-129">Die folgenden Schritte gelten für das Hinzufügen oder Entfernen von Benutzerlizenzen für Microsoft-Produkte.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-129">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="bfd8a-130">Informationen zum Hinzufügen oder Entfernen von Benutzerlizenzen für Lizenz basierte Saas-Abonnements im kommerziellen Marketplace finden Sie unter [Hinzufügen oder Entfernen von Lizenzen für ein SaaS-Abonnement](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="bfd8a-130">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="bfd8a-131">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-131">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="bfd8a-132">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-132">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="bfd8a-133">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-133">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="bfd8a-134">Wählen Sie einen oder mehrere Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-134">Choose one or more users from the list.</span></span> <span data-ttu-id="bfd8a-135">Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese den Personen zuweisen möchten, die noch keine Lizenzen besitzen, können Sie mit der Option **Benutzer filtern nach …** die richtige Gruppe finden.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-135">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="bfd8a-136">Wählen Sie **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-136">Select **Manage licenses**.</span></span> <span data-ttu-id="bfd8a-137">Nehmen Sie Ihre Änderungen vor, und wählen Sie anschließend **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-137">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="bfd8a-138">Für [Azure Marketplace Produkte](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wird die Lizenz Zuweisung und-Aktivierung über den unabhängigen Software Hersteller (Independent Software Vendor, ISV) verwaltet, der das Produkt veröffentlicht hat.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-138">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="bfd8a-139">Zurücksetzen eines Benutzerkennworts für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="bfd8a-139">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="bfd8a-140">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-140">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="bfd8a-141">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-141">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="bfd8a-142">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="bfd8a-143">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-143">Choose the user from the list.</span></span>

4.  <span data-ttu-id="bfd8a-144">Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-144">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="bfd8a-145">Senden Sie das neue temporäre Kennwort an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-145">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="bfd8a-146">Löschen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="bfd8a-146">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="bfd8a-147">Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-147">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="bfd8a-148">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-148">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="bfd8a-149">Wählen Sie im Menü des Kunden die Option **Users and licenses** (Benutzer und Lizenzen) aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-149">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="bfd8a-150">Wählen Sie den Benutzer in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-150">Choose the user from the list.</span></span>

3.  <span data-ttu-id="bfd8a-151">Wählen Sie unten auf dem Bildschirm die Option **Benutzerkonto löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-151">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="bfd8a-152">Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-152">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="bfd8a-153">Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-153">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="bfd8a-154">Wiederherstellen gelöschter Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="bfd8a-154">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="bfd8a-155">Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-155">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="bfd8a-156">Wählen Sie **Benutzer und Lizenzen**aus.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-156">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="bfd8a-157">Wählen Sie die Registerkarte **Gelöschte Benutzer ()** aus. Es sollte **(1)** oder größer sein, wenn gelöschte Benutzer wieder hergestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-157">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="bfd8a-158">Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-158">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="bfd8a-159">Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="bfd8a-159">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="bfd8a-160">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="bfd8a-160">Related topics</span></span>


[<span data-ttu-id="bfd8a-161">Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="bfd8a-161">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="bfd8a-162">Erstellen mehrerer Benutzer für ein Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="bfd8a-162">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)