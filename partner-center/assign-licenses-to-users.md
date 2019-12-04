---
title: Benutzerverwaltungsaufgaben für Kundenkonten | Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Benutzerkonten für einen Kunden erstellen, Benutzerlizenzen hinzufügen oder entfernen, Benutzer Kennwörter zurücksetzen, Benutzerkonten löschen oder wiederherstellen.
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: MaggiePucciEvans
ms.author: evansma
Keywords: Kundenverwaltung, Konto, Konto erstellen, Lizenzen, Lizenz zuweisen Benutzerverwaltung, Kennwort, Kennwort zurücksetzen, Kennwort ändern
ms.localizationpriority: medium
ms.openlocfilehash: cd1b32a0ceb133f9513263f56a7d1e2e98dde3c5
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721358"
---
# <a name="user-management-tasks-for-customer-accounts"></a><span data-ttu-id="09db1-104">Benutzerverwaltungsaufgaben für Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="09db1-104">User management tasks for customer accounts</span></span>

<span data-ttu-id="09db1-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="09db1-105">**Applies to**</span></span>

- <span data-ttu-id="09db1-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="09db1-106">Partner Center</span></span>

<span data-ttu-id="09db1-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="09db1-107">**Appropriate roles**</span></span>

- <span data-ttu-id="09db1-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="09db1-108">Global admin</span></span>
- <span data-ttu-id="09db1-109">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="09db1-109">User management admin</span></span>
- <span data-ttu-id="09db1-110">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="09db1-110">Admin agent</span></span>
- <span data-ttu-id="09db1-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="09db1-111">Sales agent</span></span>
- <span data-ttu-id="09db1-112">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="09db1-112">Helpdesk agent</span></span>

<span data-ttu-id="09db1-113">Sie können neue Benutzer im Konto eines Kunden erstellen und löschen.</span><span class="sxs-lookup"><span data-stu-id="09db1-113">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="09db1-114">Sie können auch ein oder mehrere Benutzerkonten wiederherstellen, die Sie zuvor innerhalb von 30 Tagen nach dem Löschvorgang gelöscht haben.</span><span class="sxs-lookup"><span data-stu-id="09db1-114">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="09db1-115">Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).</span><span class="sxs-lookup"><span data-stu-id="09db1-115">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="09db1-116">Wenn Sie neue Abonnements für einen Kunden kaufen, sollte der Kunde eine Liste aller Benutzer erhalten, die Konten, die Benutzerberechtigungen und die von den einzelnen Benutzern benötigten Dienste benötigen.</span><span class="sxs-lookup"><span data-stu-id="09db1-116">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="09db1-117">Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.</span><span class="sxs-lookup"><span data-stu-id="09db1-117">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="09db1-118">Erstellen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="09db1-118">Create user accounts for a customer</span></span>

1. <span data-ttu-id="09db1-119">Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="09db1-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="09db1-120">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-120">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="09db1-121">Wählen Sie im Kundenmenü **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-121">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="09db1-122">Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein.</span><span class="sxs-lookup"><span data-stu-id="09db1-122">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="09db1-123">**Speichern** Sie Ihre Änderungen.</span><span class="sxs-lookup"><span data-stu-id="09db1-123">**Save** your changes.</span></span>

5. <span data-ttu-id="09db1-124">Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.</span><span class="sxs-lookup"><span data-stu-id="09db1-124">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="09db1-125">Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.</span><span class="sxs-lookup"><span data-stu-id="09db1-125">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="09db1-126">Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="09db1-126">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="09db1-127">Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.</span><span class="sxs-lookup"><span data-stu-id="09db1-127">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="09db1-128">Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="09db1-128">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="09db1-129">Die folgenden Schritte gelten für das Hinzufügen oder Entfernen von Benutzerlizenzen für Microsoft-Produkte.</span><span class="sxs-lookup"><span data-stu-id="09db1-129">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="09db1-130">Informationen zum Hinzufügen oder Entfernen von Benutzerlizenzen für Lizenz basierte Saas-Abonnements im kommerziellen Marketplace finden Sie unter [Hinzufügen oder Entfernen von Lizenzen für ein SaaS-Abonnement](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="09db1-130">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="09db1-131">Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="09db1-131">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="09db1-132">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-132">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="09db1-133">Wählen Sie im Kundenmenü **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-133">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="09db1-134">Wählen Sie einen oder mehrere Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-134">Choose one or more users from the list.</span></span> <span data-ttu-id="09db1-135">Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese den Personen zuweisen möchten, die noch keine Lizenzen besitzen, können Sie mit der Option **Benutzer filtern nach …** die richtige Gruppe finden.</span><span class="sxs-lookup"><span data-stu-id="09db1-135">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="09db1-136">Wählen Sie **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="09db1-136">Select **Manage licenses**.</span></span> <span data-ttu-id="09db1-137">Nehmen Sie Ihre Änderungen vor, und wählen Sie anschließend **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="09db1-137">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="09db1-138">Für [Azure Marketplace Produkte](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wird die Lizenz Zuweisung und-Aktivierung über den unabhängigen Software Hersteller (Independent Software Vendor, ISV) verwaltet, der das Produkt veröffentlicht hat.</span><span class="sxs-lookup"><span data-stu-id="09db1-138">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="09db1-139">Zurücksetzen eines Benutzerkennworts für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="09db1-139">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="09db1-140">Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="09db1-140">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="09db1-141">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-141">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="09db1-142">Wählen Sie im Kundenmenü **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="09db1-143">Wählen Sie den Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-143">Choose the user from the list.</span></span>

4.  <span data-ttu-id="09db1-144">Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-144">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="09db1-145">Senden Sie das neue temporäre Kennwort an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="09db1-145">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="09db1-146">Löschen von Benutzerkonten für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="09db1-146">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="09db1-147">Wählen Sie **Kunden** im Menü **Partner Center** aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-147">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="09db1-148">Wählen Sie den Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-148">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="09db1-149">Wählen Sie im Kundenmenü **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-149">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="09db1-150">Wählen Sie den Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-150">Choose the user from the list.</span></span>

3.  <span data-ttu-id="09db1-151">Wählen Sie am unteren Bildschirmrand **Benutzerkonto löschen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-151">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="09db1-152">Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden.</span><span class="sxs-lookup"><span data-stu-id="09db1-152">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="09db1-153">Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.</span><span class="sxs-lookup"><span data-stu-id="09db1-153">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="09db1-154">Wiederherstellen gelöschter Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="09db1-154">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="09db1-155">Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="09db1-155">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="09db1-156">Wählen Sie **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-156">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="09db1-157">Wählen Sie die Registerkarte **Gelöschte Benutzer ( )** . Sie sollte mindestens **(1)** anzeigen, wenn gelöschte Benutzer vorhanden sind, die wiederhergestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="09db1-157">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="09db1-158">Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="09db1-158">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="09db1-159">Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="09db1-159">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="09db1-160">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="09db1-160">Related topics</span></span>


[<span data-ttu-id="09db1-161">Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="09db1-161">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="09db1-162">Erstellen mehrerer Benutzer für ein Kundenkonto</span><span class="sxs-lookup"><span data-stu-id="09db1-162">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)