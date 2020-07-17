---
title: Microsoft Azure Reservierungen für Kunden kaufen
ms.topic: article
ms.date: 06/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie Sie Azure-Reservierungen im Namen Ihrer Kunden im Partner Center erwerben oder erwerben.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a8f9193d7bb383b602acc8092b159401ab0785d5
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435769"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Kaufen von Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center

**Zielgruppe**

- Partner Center
- Microsoft Azure-Portal
- Partner im CSP

**Geeignete Rollen**

- Administrator-Agent
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

## <a name="before-you-begin"></a>Voraussetzungen

Lesen Sie die folgenden wichtigen Informationen, bevor Sie Azure-Reservierungen im Auftrag Ihrer Kunden kaufen. (Möchten Sie, dass Kunden ihre eigenen Azure-Reservierungen von einem früheren Azure-Abonnement erwerben können, das Sie für Sie erworben haben? Weitere Informationen finden [Sie unter Erteilen von Kunden Berechtigungen zum erwerben ihrer eigenen Azure-Reservierungen](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Wenn Ihr Kunde den neuen Microsoft-Kundenvertrag signiert hat (siehe [bestätigen der kundenannahme des Microsoft-Kunden Vertrags](confirm-customer-agreement.md)), müssen Sie Azure-Reservierungen im Azure-Plan erwerben. Weitere Informationen finden Sie unter [Purchase Azure-Plan](purchase-azure-plan.md).

- Kunden müssen bereits über ein aktives Azure-Abonnement verfügen, bevor Sie Reservierungen in deren Auftrag kaufen können.
  
- Kosten für Software-Abonnements für z.B. Azure SQL-Datenbank oder SUSE Linux-Software sind in den Reservierungspreisen von Azure nicht inbegriffen.

- Die kommerziellen Preise von Microsoft für Sie umfassen keine Steuern, es sei denn, Ihr Standort ist Brasilien. Wenn Ihr Standort Brasilien ist, sind im Handelspreis für Sie die entsprechenden Steuern inbegriffen.

- Vertriebs- und Helpdeskmitarbeiter müssen expliziten Zugriff auf das Azure-Abonnement erhalten, damit sie es im Azure-Portal kaufen und verwalten können und im Auftrag des Kunden Supportanfragen stellen können, einschließlich Umtausch und Rückerstattungen.  

- Wenn Sie ein indirekter Anbieter sind und Azure-Reservierungen über den Azure-Portal erwerben, wird der Partner of Record (indirekter Reseller) vom Azure CSP-Abonnement geerbt, das Sie ausgewählt haben.

- Der Partner von Record für Azure-Reservierungen kann nach dem Kauf nicht geändert werden. Sie können die vorhandene Reservierung Abbrechen und einen neuen mit dem neuen Partner of Record erwerben.

- Wenn ein Kunde ein Azure-Abonnement von Direct oder EA nach CSP übertragen möchte, werden Reservierungen nicht übertragen.

## <a name="azure-reservations-unavailable-markets"></a>Azure-Reservierungen: Märkte ohne Verfügbarkeit

> [!IMPORTANT]
> Azure-Reservierungen sind in den folgenden Märkten **nicht** verfügbar:  
>  
> **Nicht verfügbare Märkte (in alphabetischer Reihenfolge)**
>
> |A bis Gi   | Gr bis Pal  | Pap bis Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Ålandinseln     | Grönland     | Papua-Neuguinea     |
> | Amerikanisch-Samoa     | Grenada     | Pitcairninseln     |
> | Andorra     | Guadeloupe     | Réunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktis     | Guernsey     | Saint Barthélemy   |
> | Antigua und Barbuda       | Guinea     | St. Lucia   |
> | Aruba       | Guinea-Bissau     | Saint Martin   |
> | Aserbaidschan       | Guyana     | St. Pierre und Miquelon   |
> | Benin     | Haiti       | St. Vincent und die Grenadinen     |
> | Bhutan     | Heard und McDonaldinseln       | Samoa     |
> | Bonaire     | Isle of Man     | San Marino     |
> | Bouvetinsel     | Jan Mayen     | São Tomé und Príncipe   |
> | Britisches Territorium im Indischen Ozean       | Jersey     | Seychellen   |
> | Britische Jungferninseln     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosovo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kambodscha     | Lesotho     | Salomonen     |
> | Zentralafrikanische Republik     | Liberia     | Somalia     |
> | Tschad     | Madagaskar     | Südgeorgien und die Südlichen Sandwichinseln     |
> | China     | Malawi     | Südsudan     |
> | Weihnachtsinsel     | Malediven     | St. Helena, Ascension und Tristan da Cunha     |
> | Kokosinseln     | Mali     | Suriname     |
> | Komoren     | Marshallinseln     | Spitzbergen     |
> | Kongo     | Martinique     | Swasiland     |
> | Kongo, Demokratische Republik     | Mauretanien     | Timor-Leste   |
> | Cookinseln     | Mayotte     | Togo   |
> | Dschibuti     | Mikronesien     | Tokelau   |
> | Dominica     | Montserrat     | Tonga   |
> | Äquatorialguinea     | Mosambik     | Turks- und Caicosinseln   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Falklandinseln     | Nauru     | USA Kleinere Amerikanische Überseeinseln   |
> | Französisch-Guyana     | Neukaledonien     | Vanuatu   |
> | Französisch-Polynesien     | Niger     | Vatikanstadt   |
> | Französische Süd- und Antarktisgebiete     | Niue     | Wallis und Futuna   |
> | Gabun     | Norfolkinsel     | Jemen   |
> | Gambia     | Nördliche Marianen     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Kaufen von Azure-Reservierungen

Führen Sie die folgenden Schritte aus, um Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center zu kaufen. (Möchten Sie, dass Kunden ihre eigenen Azure-Reservierungen von einem früheren Azure-Abonnement erwerben können, das Sie für Sie erworben haben? Weitere Informationen finden [Sie unter Erteilen von Kunden Berechtigungen zum erwerben ihrer eigenen Azure-Reservierungen](give-customers-permission.md).)

1. Wählen Sie im Menü „Partner Center” **Kunden** aus.  

2. Suchen Sie auf der Seite " **Kunden** " den Kunden, der Azure-Reservierungen erwerben möchte, und klicken Sie dann auf den Pfeil nach unten, um die Zeile des Kunden zu erweitern.  

3. Wählen Sie **Produkte hinzufügen** und dann **Azure** aus. 

    a) Wählen Sie in der Liste **Segment** das Marktsegment des Kunden aus.

    b) Wählen Sie **Reservierungen** in der Liste **Produkttyp** aus.

    c. Wählen Sie in der Liste **Reservierungstyp** den vom Kunden gewünschten Typ der Reservierung aus.

4. Azure-Reservierungen müssen einem aktiven Azure-Abonnement zugeordnet werden. Wählen Sie in der Liste **Kunden Abonnement** das Abonnement des Kunden aus, dem Sie Azure-Reservierungen hinzufügen möchten. 

   >[!IMPORTANT]
   >Wenn der Kunde nicht bereits über ein aktives Azure-Abonnement verfügt, wählen Sie **Azure** aus, um es jetzt hinzuzufügen. 

5. Verwenden Sie die Filter, um nach Azure-Reservierungen auf virtuellen Computern zu suchen, die die Anforderungen Ihres Kunden erfüllen.  

6. Nachdem Sie die Reservierungen gefunden haben, die Sie kaufen möchten, geben Sie die Anzahl der vom Kunden benötigten reservierten Instanzen in **Menge** ein, und wählen Sie dann **In den Einkaufswagen** aus.  

7. Wiederholen Sie die Schritte 5 und 6, bis Sie alle erforderlichen Elemente der Bestellung hinzugefügt haben. Klicken Sie auf **Überprüfen**, um sicherzustellen, dass Ihre Bestellung ordnungsgemäß ist.  

8. Auf der Seite **Bestellungen überprüfen** können Sie folgende Aktionen ausführen: 

    - Überprüfen oder Ändern der Menge der reservierten Instanzen

    - Wählen Sie den Bereich der Reservierung aus. Der Reservierungsbereich kann ein Abonnement oder mehrere Abonnements (frei gegebener Bereich) abdecken. Wenn Sie ein einzelnes Abonnement auswählen, gilt der Reservierungsrabatt nur für dieses Abonnement. Wenn Sie Shared auswählen, wird der Reservierungs Rabatt auf alle Abonnements innerhalb des Abrechnungs Kontexts des Kunden angewendet. 

      >[!NOTE] 
      >Wenn Sie sich dafür entscheiden, den Umfang der Reservierung auf ein einzelnes Azure-Abonnement zu beschränken, müssen Sie möglicherweise die vCPU-Kontingente des Abonnements erhöhen. Um das vCPU-Kontingent des Abonnements zu erhöhen, müssen Sie im Azure-Portal eine Supportanfrage stellen. Folgen Sie den Anweisungen [in diesem Thema](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request), um die Anfrage zu erstellen. 

      >[!NOTE]   
      >Wenn sich Ihr Kunde im Azure-Plan befindet, wird der Gültigkeits **Bereich** auf " **Shared**" festgelegt. 

    - Wenn Sie Anbieterpartner sind, wählen Sie den Vertriebspartner aus, den Sie mit dem Produkt verknüpfen möchten.
    
    - Wenn Ihre Azure-Reservierung die Option Abrechnungsplan unterstützt, können Sie im Dropdown Menü die Abrechnungs Häufigkeit als monatlich auswählen. 
    - Wenn Ihre Azure-Reservierung die Option Abrechnungsplan nicht unterstützt, wird für die Abrechnungs Häufigkeit standardmäßig die einmalige Abrechnung verwendet. 

9. Klicken Sie auf **Kaufen**, um die Bestellung zu erwerben. Die Details Ihrer Bestellung, einschließlich Ihrer Bestellnummer, werden auf der Seite **Bestätigen** angezeigt. Klicken Sie auf **Fertig**, und wechseln Sie zur Seite **Bestellverlauf**. 

10. Um die Reservierung des Kunden im Azure-Portal zu verwalten, finden Sie den Kunden auf Ihrer **Kunden** Seite, und klicken Sie dann auf den Pfeil nach unten, um die Zeile des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen
|**Informationen über**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Verwalten von Azure-Reservierungen in Partner Center | [Verwalten von Azure-Reservierungen in Partner Center](azure-reservations-manage.md)
|Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden   |[Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation   |
|Erteilen von Kunden Berechtigungen zum erwerben ihrer eigenen Azure-Reservierungen  | [Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.](give-customers-permission.md)  |
