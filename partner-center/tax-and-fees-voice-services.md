---
title: Steuern und Gebühren für regionale PSTN-Dienste
description: Als Office 365-Partner, der Microsoft 365 Voice-Produkte abwickelt, unterliegen Sie möglicherweise regionalen Steuern, Gebühren oder gesetzlichen Anforderungen für PSTN-Dienste.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854722"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionale Steuern, Bestimmungen für PTSN-Dienste (Public Switched Telephone Network)

**Geeignete Rollen:** globale | Benutzeradministrator-| Administrator-Agent

PsTN-Dienste (Public Switched Telephone Network) in einigen Ländern unterliegen möglicherweise besonderen Steuer- und gesetzlichen Anforderungen, die sich auf die Bestellung und Rechnungsstellung von Partnern auswirken können. In der USA, einschließlich Rico Rico, unterliegen PSTN-Dienste, die Audiokonferenzen, Anrufpläne und Kommunikationsguthaben umfassen, besonderen Steuer- und gesetzlichen Anforderungen. In den USA und Rico Rico vergünstigt Microsoft PSTN-Dienste als steuerlich inbegriffen.  Eindeutige PSTN-Steuern und -Vorschriften wirken sich auf Office 365-Partner aus, die Microsoft 365 Voice-Produkte tätigen.  Wenn ein Partner einen Aufschlag auf den Preis eines PSTN-Diensts von Microsoft erhebt, ist er möglicherweise für die Berechnung und Abführung von Steuern und Gebühren für PSTN-Dienste verantwortlich.

## <a name="partner-recommendations"></a>Partnerempfehlungen

Wenden Sie sich an Ihre Steuer- und Rechtsabteilung, um die Verantwortung Ihrer Organisation in Bezug auf die Regulierung von PSTN-Diensten, Steuern und Gebühren und andere potenzielle Haftungen zu verstehen.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Rechnungspräsentation und Partnerabstimmungsdatei

CSP-Rechnungen und CSP-Abstimmungsdateien in den USA, Rico Rico und Kanada, die Skype for Business PSTN und Microsoft 365 Voice-Dienste enthalten, stellen separate Positionen für die PSTN- und Nicht-PSTN-Komponenten bereit.

Darüber hinaus wird auf CSP-Rechnungen die folgende Fußnote angezeigt:

* Der angezeigte Preis ist eine Gebühr für Audiokonferenzen und Anrufplandienste.  Alle anwendbaren Transaktionssteuern werden ausschließlich dem angezeigten Betrag in Rechnung gestellt, mit Ausnahme der Verkäufe innerhalb der USA.  In den USA ist der angezeigte Preis steuerlich inbegriffen, da er eine Gebühr für den Anrufplan und die Audiokonferenzdienste sowie eine Gebühr für die Steuern und Gebühren enthält, die wir in Rechnung stellen müssen.  Audiokonferenz- und Anrufplandienste werden vom Microsoft-Partner bedient, der für die Bereitstellung autorisiert ist.  Weitere Informationen finden Sie unter [Microsoft-Volumenlizenzierung](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Beispiel für eine Abstimmungsdatei

Office 365 Enterprise E5 zeigt in der Abstimmungsdatei zwei Zeilenelemente mit identischen Namen und identischen IDs an, aber jedes Zeilenelement hat einen eindeutigen Einzelpreis (Beispiel: 28,40 USD und 2,00 USD). Dies unterscheidet die Skype for Business PSTN Conferencing-Komponente vom Office 365-Angebot, sodass Sie Steuern korrekt anwenden können.

**Beispiel für Partnerabstimmung #1 (Spalten auswählen):**

|**Permanente Angebots-ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Gebühr für Zyklus   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Gebühr für Zyklus   |2.00   |

**Beispiel für partnerabstimmung #2**

Microsoft 365 Business Voice in Kanada verfügt über zusätzliche PSTN-Komponenten, die auf der CSP-Rechnung konsolidiert werden (ähnlich wie bei Office 365 E5 werden zwei Zeilenelemente angezeigt: eine für PSTN-Komponenten und die andere für Nicht-PSTN-Komponenten).  In der CSP-Abstimmungsdatei für Microsoft 365 Business Voice werden alle PSTN-Komponenten einzeln angezeigt (einzelne PSTN-Komponenten werden nicht in konsolidiert). CSV- oder API-Tool).  Die Summe der Bestelldetails und abgerechneten Beträge für Kunden, die in der Abstimmungsdatei gefunden wurden, entspricht der CSP-Rechnung.

## <a name="additional-resources"></a>Weitere Ressourcen
Weitere Informationen finden Sie auf der Website [Microsoft 365 für Partner.](https://www.microsoft.com/microsoft-365/partners/)

