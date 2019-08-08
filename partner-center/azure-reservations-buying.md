---
title: Kaufen von Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden | Partner Center
ms.topic: article
ms.date: 03/15/2019
Description: Sie können Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center kaufen.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, verwalten, Abrechnung, kaufen
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 5d42c62c10d1717868b7b22f7a63ffc2311a3f70
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708774"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Kaufen von Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center 

**Gilt für**

-  Partner Center
-  Microsoft Azure-Portal
-  Partner im Cloud Solution Provider-Programm

## <a name="before-you-begin"></a>Vorbemerkungen

Lesen Sie die folgenden wichtigen Informationen, bevor Sie Azure-Reservierungen im Auftrag Ihrer Kunden kaufen.

-   Kunden müssen bereits über ein aktives Azure-Abonnement verfügen, bevor Sie Reservierungen in deren Auftrag kaufen können.
  
-   Kosten für Software-Abonnements für z.B. Azure SQL-Datenbank oder SUSE Linux-Software sind in den Reservierungspreisen von Azure nicht inbegriffen.

-   In den Handelspreisen von Microsoft für Sie sind keine Steuern inbegriffen, es sei denn, Sie haben Ihren Standort in Brasilien. Wenn Ihr Standort Brasilien ist, sind im Handelspreis für Sie die entsprechenden Steuern inbegriffen. 
 
-   Vertriebs- und Helpdeskmitarbeiter müssen expliziten Zugriff auf das Azure-Abonnement erhalten, damit sie es im Azure-Portal kaufen und verwalten können und im Auftrag des Kunden Supportanfragen stellen können, einschließlich Umtausch und Rückerstattungen.  

-   Wenn Sie mit einem indirekten Anbieter zusammenarbeiten und Azure-Reservierungen über das Azure-Portal erwerben, wird der eingetragene Partner (indirekte Händler) aus dem Azure-CSP-Abonnement übernommen, das Sie auswählen. 

-   Der eingetragene Partner für Azure-Reservierungen kann nach dem Kauf nicht geändert werden. Sie können die vorhandene Reservierung stornieren und beim eingetragenen Partner eine neue erwerben. 

-   Wenn ein Kunde ein Azure-Abonnement von Direct oder EA nach CSP übertragen möchte, werden Reservierungen nicht übertragen. 

## <a name="azure-reservations-unavailable-markets"></a>Azure-Reservierungen: Märkte ohne Verfügbarkeit

>[!IMPORTANT] 
>Azure-Reservierungen sind in den folgenden Märkten *nicht* verfügbar:  
>  
> | Märkte ohne Verfügbarkeit | &nbsp; | &nbsp; |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Ålandinseln                  | Grönland                         | Palau                                    |
> | Amerikanisch-Samoa                 | Grenada                           | Papua-Neuguinea                         |
> | Andorra                        | Guadeloupe                        | Pitcairninseln                         |
> | Anguilla                       | Guam                              | Réunion                                  |
> | Antarktis                     | Guernsey                          | Russische Föderation                       |
> | Antigua und Barbuda            | Guinea                            | Saba                                     |
> | Aruba                          | Guinea-Bissau                     | Saint Barthélemy                         |
> | Aserbeidschan                     | Guyana                            | St. Lucia                              |
> | Belarus                        | Haiti                             | Saint Martin                             |
> | Benin                          | Heard und McDonaldinseln | St. Pierre und Miquelon                |
> | Bhutan                         | Indien                             | St. Vincent und die Grenadinen         |
> | Bonaire                        | Isle of Man                       | Samoa                                    |
> | Bouvetinsel                  | Jan Mayen                         | San Marino                               |
> | Brazilien                         | Jersey                            | São Tomé und Príncipe                    |
> | Britisches Territorium im Indischen Ozean | Kasachstan                        | Seychellen                               |
> | Britische Jungferninseln         | Kiribati                          | Sierra Leone                             |
> | Burkina Faso                   | Republik Korea                | Sint Eustatius                           |
> | Burundi                        | Kosovo                            | Sint Maarten                             |
> | Kambodscha                       | Laos                              | Salomonen                          |
> | Zentralafrikanische Republik       | Lesotho                           | Somalia                                  |
> | Tschad                           | Liberia                           | Südgeorgien und die Südlichen Sandwichinseln |
> | China                          | Madagaskar                        | Südsudan                              |
> | Weihnachtsinsel               | Malawi                            | St. Helena, Ascension und Tristan da Cunha   |
> | Kokosinseln        | Malediven                          | Suriname                                 |
> | Komoren                        | Mali                              | Spitzbergen                                 |
> | Kongo                          | Marshallinseln                  | Swasiland                                |
> | Kongo, Demokratische Republik                    | Martinique                        | Taiwan                                   |
> | Cookinseln                   | Mauretanien                        | Timor-Leste                              |
> | Dschibuti                       | Mayotte                           | Togo                                     |
> | Dominica                       | Mikronesien                        | Tokelau                                  |
> | Äquatorialguinea              | Montserrat                        | Tonga                                    |
> | Eritrea                        | Mosambik                        | Turks- und Caicosinseln                 |
> | Falklandinseln               | Myanmar                           | Tuvalu                                   |
> | Französisch-Guyana                  | Nauru                             | USA Kleinere Amerikanische Überseeinseln                    |
> | Französisch-Polynesien               | Neukaledonien                     | Ukraine                                  |
> | Französische Süd- und Antarktisgebiete    | Niger                             | Vanuatu                                  |
> | Gabun                          | Niue                              | Vatikanstadt                             |
> | Gambia                         | Norfolkinsel                    | Wallis und Futuna                        |
> | Gibraltar                      | Nördliche Marianen          | Jemen                                    |
> |

## <a name="purchase-azure-reservations"></a>Kaufen von Azure-Reservierungen

Führen Sie die folgenden Schritte aus, um Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden im Partner Center zu kaufen.

1. Wählen Sie im Menü „Partner Center” **Kunden** aus.  

2. Suchen Sie auf der Seite **Kunden** den Kunden, der Azure-Reservierungen kaufen möchte. Klicken Sie dann den nach unten zeigenden Pfeil, um den Datensatz des Kunden zu erweitern.  

3. Wählen Sie **Produkte hinzufügen** und dann **Azure** aus. 

    a. Wählen Sie in der Liste **Segment** das Marktsegment des Kunden aus.

    b. Wählen Sie **Reservierungen** in der Liste **Typ** für Produkte aus.

    c. Wählen Sie in der Liste **Reservierungstyp** den vom Kunden gewünschten Typ der Reservierung aus.

4. Azure-Reservierungen müssen einem aktiven Azure-Abonnement zugeordnet werden. Wählen Sie in der Liste **Kundenabonnement** das Abonnement des Kunden aus, dem Sie Azure-Reservierungen hinzufügen möchten. 

   >[!IMPORTANT]
   >Wenn der Kunde bereits ein aktives Azure-Abonnement hat, wählen Sie **Onlinedienste** aus, um ein neues hinzuzufügen. 

5. Verwenden Sie die Filter, um Azure-Reservierungen für virtuelle Computer zu finden, die den Anforderungen Ihrer Kunden entsprechen.  

6. Nachdem Sie die Reservierungen gefunden haben, die Sie kaufen möchten, geben Sie die Anzahl der vom Kunden benötigten reservierten Instanzen in **Menge** ein, und wählen Sie dann **In den Einkaufswagen** aus.  

7. Wiederholen Sie die Schritte 5 und 6, bis Sie der Bestellung alle erforderlichen Elemente hinzugefügt haben. Klicken Sie auf **Überprüfen**, um sicherzustellen, dass Ihre Bestellung ordnungsgemäß ist.  

8. Auf der Seite **Bestellungen überprüfen** können Sie folgende Aktionen ausführen: 

    - Überprüfen oder Ändern der Menge der reservierten Instanzen

    - Auswählen des Reservierungsbereichs Der Reservierungsbereich kann ein Abonnement oder mehrere Abonnements (gemeinsam genutzter Bereich) umfassen. Wenn Sie ein einzelnes Abonnement auswählen, gilt der Reservierungsrabatt nur für dieses Abonnement. Wenn Sie die Option „Gemeinsam genutzt“ wählen, gilt der Reservierungsrabatt für alle Abonnements im Abrechnungskontext des Kunden. 

      >[!NOTE] 
      >Wenn Sie sich dafür entscheiden, den Umfang der Reservierung auf ein einzelnes Azure-Abonnement zu beschränken, müssen Sie möglicherweise die vCPU-Kontingente des Abonnements erhöhen. Um das vCPU-Kontingent des Abonnements zu erhöhen, müssen Sie im Azure-Portal eine Supportanfrage stellen. Folgen Sie den Anweisungen [in diesem Thema](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request), um die Anfrage zu erstellen.    

    - Wenn Sie Anbieterpartner sind, wählen Sie den Vertriebspartner aus, den Sie mit dem Produkt verknüpfen möchten.

9. Klicken Sie auf **Kaufen**, um die Bestellung zu erwerben. Die Details Ihrer Bestellung, einschließlich Ihrer Bestellnummer, werden auf der Seite **Bestätigen** angezeigt. Klicken Sie auf **Fertig**, und wechseln Sie zur Seite **Bestellverlauf**. 

10. Um die Reservierung des Kunden im Azure-Portal zu verwalten, suchen Sie den Kunden auf Ihrer Seite **Kunden**, und klicken Sie dann auf den nach unten gerichteten Pfeil, um den Datensatz des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um die Daten des Kunden im Azure-Portal zu öffnen.

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen
|**Weitere Informationen zu**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Verwalten von Azure-Reservierungen im Partner Center | [Verwalten von Azure-Reservierungen im Partner Center](azure-reservations-manage.md)
|Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden   |[Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Kaufen von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation
|

 


 
