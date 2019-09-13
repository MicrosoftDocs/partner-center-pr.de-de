---
title: Microsoft Azure VM-Größe für die Verwendung der maximalen Reservierung | Partner Center
ms.topic: article
ms.date: 08/05/2019
Description: Wenn Sie Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden kaufen, müssen Sie einen virtuellen Computer (VM) auswählen, dessen Größe die Computing-Anforderungen des Kunden erfüllt.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, VM, verwalten, Nutzung, Größe
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 1c1c0170c5efd8abf2e1afb7bb6ef1dfac2b7e5b
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820192"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure VM-Größe für die maximale Reservierungsnutzung

**Gilt für**

- Partner Center
- Azure-Portal
- Partner im CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Bestimmen Sie die Größe des virtuellen Computers für die Reservierung eines Kunden in Azure 

Wenn Sie Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden kaufen, müssen Sie einen virtuellen Computer (VM) auswählen, dessen Größe die Computing-Anforderungen des Kunden erfüllt. Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:

- Azure-Nutzungs-API
- Das Azure-Portal
- Azure PowerShell
- Die API für Azure Resource Manager (ARM)

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen. Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet. Sie müssen die Reservierung keinem virtuellen Computer zuweisen.

>[!NOTE]
>Reservierungsrabatte gelten nicht für klassische virtuelle Computer oder für VM-Angebote.

>[!IMPORTANT]
>Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.

**Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API**

1. Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.
2. Weitere Informationen finden Sie unter [Abrufen der Nutzungseinträge eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).

**Abrufen der VM-Größeninformationen im Microsoft Azure-Portal**

1. Navigieren Sie im Partner Center zur Seite **Kunden**.
2. Suchen Sie den Kunden, der Azure VM-Reservierungen kaufen möchte, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um die Daten des Kunden im Azure-Portal zu öffnen.
3. Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.
4. Auf der Seite mit den Details des virtuellen Computers finden Sie Informationen zur Größe und Region (siehe unten). Verwenden Sie diese Informationen, um die Reservierung im Partner Center zu erwerben.  

    ![Informationen zu Größe und Region auf der Detailseite](images/usage1.png)

**Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell**

Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten. 

![VM-Standort und Größe](images/usage2.png)

**Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API**

1. Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. Der Aufruf gibt die Werte für **VmSize** und **Speicherort** wieder, wie unten dargestellt.

    ![vmsize-](images/usage3.png) Wert ![Speicherort Wert](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Überprüfen Sie die Azure-VM-Nutzung und den Reservierungsrabatt

Nach dem Erwerb einer Azure Reserved VM Instance im Auftrag eines Kunden wird der Rabatt für den im Voraus bezahlten VM-Speicherplatz automatisch auf die virtuellen Computer angewendet, die den Attributen und der Menge der Reservierung des Kunden entsprechen.

Überprüfen Sie die Reservierungsnutzung des Kunden und sehen Sie mithilfe einer der folgenden Methoden, auf welche virtuellen Computer der Reservierungsrabatt angewendet wird:

- Das Azure-Portal
- Azure-Nutzungs-API

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Überprüfen der Reservierungsnutzung des Kunden im Microsoft Azure-Portal

1. Navigieren Sie im Partner Center zur Seite **Kunden**.

2. Suchen Sie den Kunden, dessen Reservierungsrabatt und -nutzung Sie überprüfen möchten, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um die Daten des Kunden im Azure-Portal zu öffnen.
3. Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.
4. Überprüfen Sie auf der Seite **Übersicht** das Auslastungsdiagramm der Reservierung, das anzeigt, welcher Anteil der Reservierung auf die virtuellen Computer angewendet wurde.

    >[!NOTE]
    >Nutzungsdaten können um bis zu 8 Stunden verzögert sein.

    a. Wenn die Reservierungsauslastung 100 % beträgt, erhält Ihr Kunde alle möglichen Einsparungen, die der Kauf der Reservierung ermöglicht.
    b. Wenn die Reservierungsnutzung 0 % beträgt, wird kein Rabatt auf virtuelle Computer angewendet.
    c. Wenn die Reservierung zwischen 1 und 99 % beträgt, gibt es nicht verwendete Vorteile.

5. Um dies zu vermeiden, bestimmen Sie die richtige Größe der VM zur Unterstützung des Computingbedarfs des Kunden vor dem Kauf.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Überprüfen Sie die Reservierungsnutzung des Kunden mit der Azure-Nutzungs-API

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird. Vergleichen Sie Beispiel A mit Beispiel B, um die Reservierungsnutzung des Kunden zu überprüfen.

![Beispiele für die Reservierungsnutzung](images/usage5.png)

- Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.
- consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.
- ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.

Weitere Informationen finden Sie unter [Abrufen der Nutzungseinträge eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung. Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet. Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen

|**Weitere Informationen zu**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center   |[Kaufen von Azure-Reservierungen](azure-reservations-buying.md)
|Verwalten von Azure-Reservierungen in Partner Center | [Verwalten von Azure-Reservierungen in Partner Center](azure-reservations-manage.md)
|Erwerb von Azure-Reservierungen im Azure-Portal | [Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure-Reservierungen im Azure-Portal   |[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation
