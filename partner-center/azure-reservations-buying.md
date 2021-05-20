---
title: Erwerben von Microsoft Azure Reservierungen für Kunden
description: Erfahren Sie, wie Sie Azure-Reservierungen im Namen Ihrer Kunden in Partner Center erwerben. Listet auch Märkte auf, in denen Azure-Reservierungen nicht verfügbar sind.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149535"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Kaufen von Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center

**Geeignete Rollen:** Administrator-Agent-| Globale | | des Helpdesk-Agents | des Vertriebsmitarbeiters Benutzerverwaltungsadministrator

In diesem Artikel wird erläutert, wie Sie Azure-Reservierungen im Auftrag Ihrer Kunden in Partner Center erwerben. Außerdem werden Märkte identifiziert, in denen Azure-Reservierungen nicht verfügbar sind.
 
> [!NOTE]
> Dieser Artikel gilt nur für Partner im CSP-Programm (Cloud Solution Provider). Kunden, die andere Abonnementtypen verwenden (z. B. Abonnements mit nutzungsbasierter Bezahlung, Einzelabonnements, Microsoft-Kundenvereinbarung oder Enterprise Agreement Abonnements), sollten stattdessen [diese Dokumentation zu Azure-Reservierungen](/azure/cost-management-billing/reservations)lesen.

## <a name="before-you-begin"></a>Voraussetzungen

Lesen Sie die folgenden wichtigen Informationen, bevor Sie Azure-Reservierungen im Auftrag Ihrer Kunden kaufen. (Möchten Sie, dass Kunden ihre eigenen Azure-Reservierungen über ein vorheriges Azure-Abonnement erwerben können, das Sie für sie erworben haben? Weitere Informationen finden Sie unter [Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Wenn und wenn Ihr Kunde die neue Microsoft-Kundenvereinbarung signiert (siehe [Bestätigen der Kundenakzeptanz des Microsoft-Kundenvereinbarung](confirm-customer-agreement.md)), müssen Sie Azure-Reservierungen im Rahmen des Azure-Plans erwerben. Weitere Informationen finden Sie unter [Erwerben des Azure-Plans.](purchase-azure-plan.md)

- Kunden müssen bereits über ein aktives Azure-Abonnement verfügen, bevor Sie Reservierungen in deren Auftrag kaufen können.
  
- Kosten für Software-Abonnements für z.B. Azure SQL-Datenbank oder SUSE Linux-Software sind in den Reservierungspreisen von Azure nicht inbegriffen.

- Die kommerziellen Preise von Microsoft enthalten keine Steuern, es sei denn, Ihr Standort ist Brasilien. Wenn Ihr Standort Brasilien ist, sind im Handelspreis für Sie die entsprechenden Steuern inbegriffen.

- Vertriebs- und Helpdeskmitarbeiter müssen expliziten Zugriff auf das Azure-Abonnement erhalten, damit sie es im Azure-Portal kaufen und verwalten können und im Auftrag des Kunden Supportanfragen stellen können, einschließlich Umtausch und Rückerstattungen.  

- Wenn Sie ein indirekter Anbieter sind und Azure-Reservierungen über die Azure-Portal erwerben, wird der Partner of Record (indirekter Vertriebspartner) von dem ausgewählten Azure CSP Abonnement geerbt.

- Der Partner of Record für Azure-Reservierungen kann nach dem Kauf nicht mehr geändert werden. Sie können die vorhandene Reservierung stornieren und eine neue Reservierung mit dem neuen Partner of Record erwerben.

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

Führen Sie die folgenden Schritte aus, um Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center zu kaufen. (Möchten Sie, dass Kunden ihre eigenen Azure-Reservierungen über ein vorheriges Azure-Abonnement erwerben können, das Sie für sie erworben haben? Weitere Informationen finden Sie unter [Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben.)](give-customers-permission.md)

1. Wählen Sie im Menü „Partner Center” **Kunden** aus.  

2. Suchen Sie **auf der** Seite Kunden den Kunden, der Azure-Reservierungen erwerben möchte, und wählen Sie dann den Pfeil nach unten aus, um die Zeile des Kunden zu erweitern.  

3. Wählen Sie **Produkte hinzufügen** und dann **Azure** aus. 

    a. Wählen Sie in der Liste **Segment** das Marktsegment des Kunden aus.

    b. Wählen **Sie reservierungen** aus der Liste **Produkttyp** aus.

    c. Wählen Sie in der Liste **Reservierungstyp** den vom Kunden gewünschten Typ der Reservierung aus.

4. Azure-Reservierungen müssen einem aktiven Azure-Abonnement zugeordnet werden. Wählen Sie in der Liste Kundenabonnement das Abonnement des Kunden aus, dem Sie **Azure-Reservierungen hinzufügen** möchten. 

   >[!IMPORTANT]
   >Wenn der Kunde noch kein aktives Azure-Abonnement hat, wählen Sie **Azure aus,** um jetzt eines hinzuzufügen. 

5. Verwenden Sie die Filter, um Azure-Reservierungen auf virtuellen Computern zu finden, die die Anforderungen Ihres Kunden erfüllen.  

6. Nachdem Sie die Reservierungen gefunden haben, die Sie kaufen möchten, geben Sie die Anzahl der vom Kunden benötigten reservierten Instanzen in **Menge** ein, und wählen Sie dann **In den Einkaufswagen** aus.  

7. Wiederholen Sie die Schritte 5 und 6, bis Sie der Bestellung alle erforderlichen Elemente hinzugefügt haben. Klicken Sie auf **Überprüfen**, um sicherzustellen, dass Ihre Bestellung ordnungsgemäß ist.  

8. Auf der Seite **Bestellungen überprüfen** können Sie folgende Aktionen ausführen: 

    - Überprüfen oder Ändern der Menge der reservierten Instanzen

    - Wählen Sie den Bereich der Reservierung aus. Der Bereich der Reservierung kann ein Abonnement oder mehrere Abonnements (freigegebener Bereich) umfassen. Wenn Sie ein einzelnes Abonnement auswählen, gilt der Reservierungsrabatt nur für dieses Abonnement. Wenn Sie Freigegeben auswählen, wird der Reservierungsrabatt auf alle Abonnements im Abrechnungskontext des Kunden angewendet. 

      >[!NOTE] 
      >Wenn Sie sich dafür entscheiden, den Umfang der Reservierung auf ein einzelnes Azure-Abonnement zu beschränken, müssen Sie möglicherweise die vCPU-Kontingente des Abonnements erhöhen. Um das vCPU-Kontingent des Abonnements zu erhöhen, müssen Sie im Azure-Portal eine Supportanfrage stellen. Folgen Sie den Anweisungen [in diesem Thema](/azure/azure-supportability/resource-manager-core-quotas-request), um die Anfrage zu erstellen. 

      >[!NOTE]   
      >Wenn Ihr Kunde den Azure-Plan verwendet, wird **Bereich** auf Freigegeben **festgelegt.** 

    - Wenn Sie Anbieterpartner sind, wählen Sie den Vertriebspartner aus, den Sie mit dem Produkt verknüpfen möchten.
    
    - Wenn Ihre Azure-Reservierung die Option Abrechnungsplan unterstützt, können Sie die Abrechnungshäufigkeit im Dropdownmenü als monatlich auswählen. 
    - Wenn Ihre Azure-Reservierung die Option Abrechnungsplan nicht unterstützt, wird die Abrechnungshäufigkeit standardmäßig auf die einmalige Abrechnung festgelegt. 

9. Klicken Sie auf **Kaufen**, um die Bestellung zu erwerben. Die Details Ihrer Bestellung, einschließlich Ihrer Bestellnummer, werden auf der Seite **Bestätigen** angezeigt. Klicken Sie auf **Fertig**, und wechseln Sie zur Seite **Bestellverlauf**. 

10. Um die Reservierung des Kunden im Azure-Portal zu verwalten,  suchen Sie den Kunden auf der Seite Kunden, und wählen Sie dann den Pfeil nach unten aus, um die Zeile des Kunden zu erweitern. Wählen **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden in der Azure-Portal.

## <a name="next-steps"></a>Nächste Schritte

|**Informationen über**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Verwalten von Azure-Reservierungen in Partner Center | [Verwalten von Azure-Reservierungen in Partner Center](azure-reservations-manage.md)
|Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden   |[Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation   |
|Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben  | [Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben](give-customers-permission.md)  |