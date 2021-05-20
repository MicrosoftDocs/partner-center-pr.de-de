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
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Verwalten von Benutzern und Benutzerlizenzen für Kundenkonten 

**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Administrator-Agent


Sie können neue Benutzer im Konto eines Kunden erstellen und löschen. Sie können auch ein oder mehrere Benutzerkonten wiederherstellen, die Sie zuvor innerhalb von 30 Tagen nach dem Löschen gelöscht haben. Die vorherigen Abonnementzuweisungen des Benutzers werden ebenfalls wiederhergestellt (vorausgesetzt, die vorherigen Zuweisungen sind verfügbar).

Wenn Sie neue Abonnements für einen Kunden erwerben, sollte der Kunde Ihnen eine Liste aller Benutzer zur Verfügung stellen, die Konten benötigen, deren Benutzerberechtigungen und welche Dienste jeder Benutzer benötigt.  

>[!NOTE]
>Im Abschnitt Benutzer  und **Lizenzen** der Registerkarte Kunde werden alle Benutzer angezeigt, die im Mandanten eines bestimmten Kunden erstellt wurden, einschließlich Der Benutzer, die Lizenzen von einem anderen CSP-Partner oder einem anderen Kaufkanal erworben haben.

Sie können [Abonnements gleichzeitig mehreren Benutzern zuweisen](bulk-license-provisioning-for-multiple-users.md), indem Sie die Namen mithilfe einer [Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) importieren.

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Erstellen von Benutzerkonten für einen Kunden

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.**

4. Klicken Sie für jeden Benutzer auf **Benutzer hinzufügen**, und geben Sie die Informationen, einschließlich Berechtigungen und Lizenzen, ein. **Speichern** Sie die Änderungen.

5. Notieren Sie den Benutzernamen und das temporäre Kennwort, um diese an den Benutzer zu senden.

6. Wenn Sie mehrere Benutzer hinzufügen, befolgen Sie die Anweisungen unter **Hinzufügen eines weiteren Benutzers**.

7. Sie können auch mehrere Benutzer gleichzeitig über [den Import einer Excel-kompatiblen CSV-Datei](adding-multiple-users-to-a-customer-account.md) hinzufügen. Sie können warten, bis Sie mit dem gesamten Satz fertig sind, bevor Sie die Namen und Kennwörter auf dem Bestätigungsbildschirm per E-Mail senden oder ausdrucken.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Hinzufügen oder Entfernen von Benutzerlizenzen für einen Kunden

Die folgenden Schritte gelten für das Hinzufügen oder Entfernen von Benutzerlizenzen für Microsoft-Produkte. Informationen zum Hinzufügen oder Entfernen von Benutzerlizenzen für lizenzbasierte SaaS-Abonnements im kommerziellen Marketplace finden Sie unter Hinzufügen oder Entfernen von Lizenzen [für ein SaaS-Abonnement.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.**

4. Wählen Sie einen oder mehrere Benutzer aus der Liste aus. Wenn der Kunde beispielsweise gerade neue Lizenzen erworben hat und Sie diese Personen zuweisen möchten, die noch nicht über diese verfügen, können Sie die Option Benutzer nach **filtern nach...** verwenden, um die richtige Gruppe zu finden.

5. Wählen Sie **Lizenzen verwalten**. Nehmen Sie Ihre Änderungen vor, und speichern **Sie dann**.

> [!NOTE]
> Bei [Azure Marketplace-Produkten](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wird die Lizenzzuweisung und -aktivierung durch den unabhängigen Softwarehersteller (Independent Software Vendor, ISV) verwaltet, der das Produkt veröffentlicht hat.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Zurücksetzen eines Benutzerkennworts für einen Kunden

1. Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

2. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

3. Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.** Wählen Sie den Benutzer in der Liste aus.

4. Wählen Sie am unteren Bildschirmrand **Kennwort zurücksetzen**. 

5. Senden Sie das neue temporäre Kennwort an den Benutzer.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Löschen von Benutzerkonten für einen Kunden

1. Wählen Sie **Partner Center** Menü Kunden **aus.** Wählen Sie den Kunden in der Liste aus.

2. Wählen Sie im Kundenmenü Benutzer **und Lizenzen aus.** Wählen Sie den Benutzer in der Liste aus.

3. Wählen Sie unten auf dem Bildschirm die Option **Benutzerkonto löschen** aus.

Wenn Sie dieses Konto wiederherstellen müssen, finden Sie es auf der Registerkarte **Gelöschte Benutzer** in der Liste **Benutzer und Lizenzen** des Kunden. Sie haben zum Wiederherstellen eines gelöschten Benutzers 30 Tage Zeit.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Wiederherstellen gelöschter Benutzerkonten

1. Wählen Sie im Menü **Partner Center** die Option **Kunden** und dann einen Kunden in der Liste aus.

2. Wählen Sie **Benutzer und Lizenzen aus.**

3. Wählen Sie **die Registerkarte Gelöschte Benutzer ( )** aus. Er sollte **(1) oder höher** lesen, wenn gelöschte Benutzer wiederhergestellt werden können.

4. Aktivieren Sie das Kontrollkästchen von mindestens einem gelöschten Benutzer, und wählen Sie **Wiederherstellen**.

    Alle ausgewählten Benutzerkonten werden erneut auf der Seite **Benutzer und Lizenzen** angezeigt.

## <a name="next-steps"></a>Nächste Schritte

- [Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer](bulk-license-provisioning-for-multiple-users.md)

- [Erstellen mehrerer Benutzer für ein Kundenkonto](adding-multiple-users-to-a-customer-account.md)