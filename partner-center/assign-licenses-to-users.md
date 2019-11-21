---
title: Benutzerverwaltungsaufgaben für Kundenkonten | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to create user accounts for a customer, add or remove user licenses, reset user passwords, delete user accounts or restore them.
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: MaggiePucciEvans
ms.author: evansma
Keywords: Kundenverwaltung, Konto, Konto erstellen, Lizenzen, Lizenz zuweisen Benutzerverwaltung, Kennwort, Kennwort zurücksetzen, Kennwort ändern
ms.localizationpriority: medium
ms.openlocfilehash: fb2e616a6bf7dbfa5072ff1617dc37ad76831b8c
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253345"
---
# <a name="user-management-tasks-for-customer-accounts"></a>Benutzerverwaltungsaufgaben für Kundenkonten

**Zielgruppe**

- Partner Center

You can create and delete new users in a customer's account. You can also restore one or more user accounts that you previously deleted within 30 days of the deletion. Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).

When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.  

Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Erstellen von Benutzerkonten für einen Kunden

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie im Kundenmenü **Benutzer und Lizenzen**.

4. Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein. **Speichern** Sie Ihre Änderungen.

5. Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.

6. Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.

7. Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen. Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden

The following steps apply to adding or removing user licenses for Microsoft products. To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie im Kundenmenü **Benutzer und Lizenzen**.

4. Wählen Sie einen oder mehrere Benutzer aus der Liste aus. Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese den Personen zuweisen möchten, die noch keine Lizenzen besitzen, können Sie mit der Option **Benutzer filtern nach …** die richtige Gruppe finden.

5. Wählen Sie **Lizenzen verwalten**. Nehmen Sie Ihre Änderungen vor, und wählen Sie anschließend **Speichern**.

> [!NOTE]
> For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Zurücksetzen eines Benutzerkennworts für einen Kunden

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3.  Wählen Sie im Kundenmenü **Benutzer und Lizenzen**. Wählen Sie den Benutzer aus der Liste aus.

4.  Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**. 

5.  Senden Sie das neue temporäre Kennwort an den Benutzer.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Löschen von Benutzerkonten für einen Kunden

1.  Wählen Sie **Kunden** im Menü **Partner Center** aus. Wählen Sie den Kunden aus der Liste aus.

2.  Wählen Sie im Kundenmenü **Benutzer und Lizenzen**. Wählen Sie den Benutzer aus der Liste aus.

3.  Wählen Sie am unteren Bildschirmrand **Benutzerkonto löschen**.

Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden. Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Wiederherstellen gelöschter Benutzerkonten

1.  Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.

2.  Wählen Sie **Benutzer und Lizenzen**.

3.  Wählen Sie die Registerkarte **Gelöschte Benutzer ( )** . Sie sollte mindestens **(1)** anzeigen, wenn gelöschte Benutzer vorhanden sind, die wiederhergestellt werden können.

4.  Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.

    Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.

## <a name="related-topics"></a>Verwandte Themen


[Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer](bulk-license-provisioning-for-multiple-users.md)

[Erstellen mehrerer Benutzer für ein Kundenkonto](adding-multiple-users-to-a-customer-account.md)