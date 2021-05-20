---
title: Azure-VM-Größe für die maximale Reservierungsnutzung
description: Erfahren Sie, wie Sie die Größe eines virtuellen Computers (VM) an die Computinganforderungen Ihrer Kunden anpassen, wenn Microsoft Azure Reservierungen für sie erwerben.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149450"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure VM-Größe für die maximale Reservierungsnutzung

**Geeignete Rollen:** Administrator-Agent| Vertriebs-Agent

In diesem Artikel wird erläutert, wie Sie die Größe eines virtuellen Computers (VM) an die Computinganforderungen Ihrer Kunden anpassen, wenn Microsoft Azure reservierungen erwerben.
 
> [!NOTE]
> Dieser Artikel gilt nur für Partner im Cloud Solution Provider -Programm (CSP). Kunden, die andere Arten von Abonnements verwenden (z. B. nutzungsbasierte Bezahlung, Einzelabonnements, Microsoft-Kundenvereinbarung- oder Enterprise Agreement-Abonnements), sollten stattdessen diese Dokumentation zu Azure-Reservierungen [lesen.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Ermitteln der VM-Größe für die Azure-Reservierung eines Kunden

Beim Kauf Microsoft Azure Reservierungen im Auftrag Ihrer Kunden müssen Sie einen virtuellen Computer (VM) auswählen, der die Computinganforderungen des Kunden erfüllt. Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:

- Azure-Nutzungs-API
- Das Azure-Portal
- Azure PowerShell
- Die API für Azure Resource Manager (ARM)

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen. Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet. Sie müssen die Reservierung nicht einem virtuellen Computer zuweisen.

>[!NOTE]
>Reservierungsrabatte gelten nicht für klassische oder Werbe-VMs.

>[!IMPORTANT]
>Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API

1. Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.

2. Weitere Informationen finden Sie unter [Abrufen der Nutzungsdatensätze](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) eines Kunden für Azure in der [Partner Center-API.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Abrufen der VM-Größeninformationen im Microsoft Azure-Portal

1. Navigieren Sie im Partner Center zur Seite **Kunden**.

2. Suchen Sie den Kunden, der Azure-VM-Reservierungen erwerben möchte, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern. Wählen **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden in der Azure-Portal.

3. Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.

4. Suchen Sie auf der Detailseite des virtuellen Computers die Informationen zu Größe und Region, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung im Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Informationen zu Größe und Region auf der Detailseite":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell

Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten. 

:::image type="content" source="images/usage2.png" alt-text="VM-Standort und Größe":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API

1. Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).

    :::image type="content" source="images/usage3.png" alt-text="vmSize-Wert":::
    :::image type="content" source="images/usage4.png" alt-text="Location-Wert":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts

Nachdem Sie eine reservierte Azure-VM-Instanz im Auftrag eines Kunden erwerben, wird der Rabatt für die Vorauszahlung für VM-Speicherplatz automatisch auf die virtuellen Computer angewendet, die mit den Attributen und der Menge der Reservierung des Kunden übereinstimmen.

Sie können die Reservierungsnutzung des Kunden überprüfen und mithilfe einer der folgenden Methoden überprüfen, auf welche virtuellen Computer die Reservierungsrabatte angewendet werden:

- Das Azure-Portal
- Azure-Nutzungs-API

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Überprüfen Sie die Reservierungsnutzung des Kunden im Microsoft Azure-Portal

1. Navigieren Sie im Partner Center zur Seite **Kunden**.

2. Suchen Sie den Kunden, dessen Reservierungsrabatt und Nutzung Sie überprüfen möchten, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.
3. Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.
4. Überprüfen Sie auf der Seite **Übersicht** das Auslastungsdiagramm der Reservierung, das anzeigt, wie viel der Reservierung auf virtuelle Computer angewendet wurde.

    >[!NOTE]
    >Nutzungsdaten können um bis zu 8 Stunden verzögert sein.

    a. Wenn die Auslastung der Reservierung 100 % beträgt, erhält Ihr Kunde alle möglichen Einsparungen, die der Reservierungskauf bieten kann.
    b. Wenn die Nutzung der Reservierung 0 % beträgt, wird der Rabatt nicht auf virtuelle Computer angewendet.
    c. Wenn die Nutzung der Reservierung zwischen 1 % und 99 % liegt, gibt es nicht genutzte Vorteile.

5. Um diese Situation zu vermeiden, bestimmen Sie die richtige Größe des virtuellen Computers, um die Computinganforderungen des Kunden zu unterstützen, bevor Sie den Kauf tätigen.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Überprüfen der Reservierungsnutzung des Kunden mit der Azure-Nutzungs-API

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird. Vergleichen Sie Beispiel A mit Beispiel B, um zu sehen, wie Sie die Reservierungsnutzung eines Kunden überprüfen.

:::image type="content" source="images/usage5.png" alt-text="Beispiele für die Reservierungsnutzung":::

- Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.
- consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.
- ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.

Weitere Informationen finden Sie unter [Abrufen der Nutzungsdatensätze eines Kunden für Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API.](/partner-center/develop/)

>[!IMPORTANT]
>Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung. Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet. Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="next-steps"></a>Nächste Schritte

|**Informationen über**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center   | [Kaufen von Azure-Reservierungen](azure-reservations-buying.md)
|Verwalten von Azure-Reservierungen in Partner Center | [Verwalten von Azure-Reservierungen in Partner Center](azure-reservations-manage.md)
|Erwerb von Azure-Reservierungen im Azure-Portal | [Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure-Reservierungen im Azure-Portal   | [Verwalten von reservierten VM-Instanzen](/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation   |
|Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen über ein Abonnement zu erwerben, das Sie für sie erworben haben. | [Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben](give-customers-permission.md)   |