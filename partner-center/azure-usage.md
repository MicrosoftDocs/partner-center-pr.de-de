---
title: Azure-VM-Größenanpassung für die maximale Reservierungs Nutzung
ms.topic: article
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie Sie die Größe eines virtuellen Computers (VM) mit den computinganforderungen ihrer Kunden skalimachen, wenn Sie Microsoft Azure Reservierungen für diese Computer erwerben.
author: BillLinzbach
ms.author: BillLi
keywords: Azure, Reservierungen, VM, verwalten, Nutzung, Größe
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 00da6723fc8aa4a5b3f1e0f747cb63acc1a504a8
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377654"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure VM-Größe für die maximale Reservierungsnutzung

**Zielgruppe**

- Partner Center
- Azure-Portal
- Partner im CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Ermitteln der VM-Größe für die Azure-Reservierung eines Kunden

Beim Kauf von Microsoft Azure Reservierungen im Auftrag ihrer Kunden müssen Sie einen virtuellen Computer (VM) auswählen, um die Anforderungen des Kunden zu erfüllen. Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:

- Azure-Nutzungs-API
- Das Azure-Portal
- Azure PowerShell
- Die API für Azure Resource Manager (ARM)

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen. Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet. Sie müssen die Reservierung nicht einem virtuellen Computer zuweisen.

>[!NOTE]
>Reservierungs Rabatte gelten nicht für klassische oder Werbe-VMS.

>[!IMPORTANT]
>Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API

1. Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.

2. Weitere Informationen finden Sie unter Ermitteln der [Auslastungs Datensätze eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Abrufen der VM-Größeninformationen im Microsoft Azure-Portal

1. Navigieren Sie im Partner Center zur Seite **Kunden**.

2. Suchen Sie den Kunden, der Azure-VM-Reservierungen erwerben möchte, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.

3. Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.

4. Suchen Sie auf der Detailseite des virtuellen Computers die Größe und Regions Informationen, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung in Partner Center zu erwerben.  

   :::image type="content" source="images/usage1.png" alt-text="Informationen zu Größe und Region auf der Detailseite":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell

Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten. 

:::image type="content" source="images/usage2.png" alt-text="VM-Standort und Größe":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API

1. Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).

    :::image type="content" source="images/usage3.png" alt-text="vmsize-Wert":::
    :::image type="content" source="images/usage4.png" alt-text="Location-Wert":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts

Nachdem Sie im Auftrag eines Kunden eine reservierte Azure-VM-Instanz erworben haben, wird der Rabatt für die Zahlung von VM-Speicherplatz im Voraus automatisch auf die virtuellen Computer angewendet, die den Attributen und der Menge der Kunden Reservierung entsprechen.

Mithilfe einer der folgenden Methoden können Sie die Reservierungs Nutzung des Kunden überprüfen und überprüfen, auf welche virtuellen Computer die Reservierungs Rabatte angewendet werden:

- Das Azure-Portal
- Azure-Nutzungs-API

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Überprüfen Sie die Reservierungs Nutzung des Kunden im Microsoft Azure-Portal

1. Navigieren Sie im Partner Center zur Seite **Kunden**.

2. Suchen Sie nach dem Kunden, dessen Reservierungs Rabatt und deren Nutzung Sie überprüfen möchten, und klicken Sie dann auf den Pfeil nach unten, um die Kundeninformationen zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.
3. Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.
4. Überprüfen Sie auf der Seite **Übersicht** das Auslastungs Diagramm der Reservierung, das anzeigt, wie viel der Reservierung auf virtuelle Computer angewendet wurde.

    >[!NOTE]
    >Nutzungsdaten können um bis zu 8 Stunden verzögert sein.

    a. Wenn die Nutzung der Reservierung 100% beträgt, erhält der Kunde alle möglichen Einsparungen, die der reservierte Kauf bereitstellen kann.
    b. Wenn die Nutzung der Reservierung 0% beträgt, wird der Rabatt nicht auf einen virtuellen Computer angewendet.
    c. Wenn die Reservierungs Nutzung zwischen 1% und 99% liegt, gibt es nicht genutzte Vorteile.

5. Um dieses Problem zu vermeiden, sollten Sie die richtige VM-Größe festlegen, um die computingressourcen der Kunden vor dem Erwerb zu unterstützen

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Überprüfen der Reservierungs Nutzung des Kunden mit der Azure-Nutzungs-API

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird. Vergleichen Sie Beispiel a mit Beispiel B, um zu erfahren, wie Sie die Reservierungs Nutzung eines Kunden überprüfen.

:::image type="content" source="images/usage5.png" alt-text="Beispiele für die Reservierungsnutzung":::

- Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.
- consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.
- ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.

Weitere Informationen finden Sie unter Ermitteln der [Auslastungs Datensätze eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung. Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet. Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen

|**Informationen über**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center   | [Kaufen von Azure-Reservierungen](azure-reservations-buying.md)
|Verwalten von Azure-Reservierungen in Partner Center | [Verwalten von Azure-Reservierungen in Partner Center](azure-reservations-manage.md)
|Erwerb von Azure-Reservierungen im Azure-Portal | [Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure-Reservierungen im Azure-Portal   | [Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation   |
|Erteilen von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von einem Abonnement zu erwerben, das Sie für Sie erworben haben. | [Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.](give-customers-permission.md)   |
