---
title: Office 365 Partner Advisory-Microsoft 365 Voice in CSP | Partner Center
description: PSTN-Dienste in einigen Ländern unterliegen möglicherweise speziellen Steuer-und behördlichen Anforderungen, die sich auf die Auftrags-und Rechnungsstellung von Partnern auswirken können
ms.topic: article
ms.date: 11/04/2019
author: maggiepuccievans
ms.author: evansma
keywords: Office, O365, PSTN-Dienste, Steuern, Anforderungen, Rechnungen, Rechnungsstellung
ms.localizationpriority: medium
ms.openlocfilehash: b6359a49503237e72c8cffdb5758bdd418910306
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384813"
---
# <a name="office-365-partner-advisory-microsoft-365-voice-in-csp"></a>Office 365-Partner Beratung: Microsoft 365 Voice in CSP

**Gilt für**

- Partner Center  

Die Dienste für öffentliche Wechsel Telefonnetzwerke (PSTN) unterliegen möglicherweise speziellen Steuer-und behördlichen Anforderungen, die sich auf die Reihenfolge der Partner und die Rechnungsstellung auswirken können.  In den USA, Puerto Rico und Kanada unterliegen die Skype for Business-PSTN-und Microsoft 365 Voice-Dienste speziellen Steuer-und gesetzlichen Anforderungen. In den USA und Puerto Rico werden die PSTN-Dienste von Microsoft als Steuer inklusiv fest.  Eindeutige PSTN-Steuern und-Vorschriften wirken sich auf Office 365-Partner aus, die Microsoft 365 Voice-Produkte.  Wenn ein Partner einen Aufschlag auf den Preis eines PSTN-Diensts von Microsoft erhebt, ist er möglicherweise für die Berechnung und Abführung von Steuern und Gebühren für PSTN-Dienste verantwortlich.

## <a name="partner-recommendations"></a>Partner Empfehlungen

Informieren Sie sich bei Ihren Steuer- und Rechtsberatern über die Verantwortlichkeiten Ihres Unternehmens in Bezug auf Bestimmungen, Steuern und Gebühren für PSTN-Dienste und andere mögliche Verpflichtungen.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Rechnungs Präsentation und Vereinbarungs Datei für Partner

CSP-Rechnungen und CSP-Abstimmungs Dateien in den USA, Puerto Rico und Kanada, die Skype for Business-PSTN und Microsoft 365 Voice-Dienste enthalten, stellen separate Zeilen Elemente für die PSTN-und nicht-PSTN-Komponenten bereit.

Darüber hinaus wird für CSP-Rechnungen der folgende Fußnote angezeigt:

* Der angezeigte Preis ist eine Gebühr für Audiokonferenzen und das Aufrufen von Plan Diensten.  Alle anwendbaren Transaktionssteuern werden ausschließlich in Rechnung gestellt, mit Ausnahme des Umsatzes, der in der USA erfolgt.  In den USA ist der angezeigte Preis steuerlich inklusiv, da er eine Gebühr für den Aufruf Plan und die Audiokonferenz-Dienste sowie eine Gebühr für die Steuern und Gebühren enthält, die wir berechnen müssen.  Audiokonferenzen und Aufruf Plan Dienste werden vom Microsoft-Partner betreut, der zur Bereitstellung autorisiert ist.  Weitere Informationen finden Sie in der [Microsoft-Volumen Lizenzierung](https://go.microsoft.com/fwlink/?LinkId=690247) .

## <a name="reconciliation-file-example"></a>Beispiel für eine Abstimmungs Datei

Office 365 Enterprise E5 zeigt eine Abstimmungs Datei als zweizeilige Elemente mit identischen Namen und identischen IDs an, aber jedes einzelne Zeilen Element hat einen eindeutigen Einheitspreis (Beispiel: $28,40 und $2,00). Dies unterscheidet die Skype for Business PSTN Conferencing-Komponente vom Office 365-Angebot, sodass Sie Steuern korrekt anwenden können.

**Beispiel für Partner Abstimmung #1 (Spalten auswählen):**

|**Permanente Angebots-ID**|**Angebotsname**|**Startdatum des Abonnements**|**Enddatum des Abonnements**|**Startdatum der Abrechnung**|**Enddatum der Abrechnung**|**Typ der Abrechnung**|**Preis pro Einheit**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Gebühr für Zyklus   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Gebühr für Zyklus   |2,00   |

**Beispiel für Partner Abstimmung #2**

Microsoft 365 Business in Kanada verfügbare Sprache verfügt über zusätzliche PSTN-Komponenten, die auf der CSP-Rechnung konsolidiert werden (ähnlich wie bei Office 365 E5 werden zwei Zeilen Elemente angezeigt, eine für PSTN-Komponenten und die andere für nicht-PSTN-Komponenten).  In der CSP-Abstimmungs Datei für Microsoft 365 Business Voice werden alle zu debuggenden PSTN-Komponenten einzeln angezeigt (individuelle PSTN-Komponenten werden in nicht konsolidiert. CSV-oder API-Tool).  Die Summe der Bestelldetails und der in Rechnung gestellten Beträge für Kunden, die in der Abstimmungs Datei gefunden werden, entspricht der CSP-Rechnung.

## <a name="additional-resources"></a>Zusätzliche Ressourcen
Weitere Informationen finden Sie auf der [Microsoft 365 für Partner](https://drumbeat.office.com/Pages/home2016.aspx) Website.

