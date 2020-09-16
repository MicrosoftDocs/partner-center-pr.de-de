---
title: Steuern und Gebühren für regionale PSTN-Dienste
description: Als Office 365-Partner, der Microsoft 365 Voice-Produkte verarbeitet, unterliegen Sie möglicherweise regionalen Steuern, Gebühren oder gesetzlichen Anforderungen für PSTN-Dienste.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "90594458"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionale Steuern, Bestimmungen für Public Switched Telefon Network (PZN)-Dienste

**Zielgruppe**

- Partner Center
- Office 365-Partner, die Microsoft 365 Voice-Produkte transagieren

**Geeignete Rollen**
-    Globaler Administrator
-    Benutzeradministrator
-    Administrator-Agent

Die Public Switched Telefon Network-Dienste (PSTN) unterliegen möglicherweise speziellen Steuer-und behördlichen Anforderungen, die sich auf die Reihenfolge der Partner und die Rechnungsstellung auswirken können. In der USA, einschließlich Puerto Rico, PSTN-Dienste, die Audiokonferenzen, Aufruf Pläne und Kommunikations Guthaben enthalten, gelten spezielle Steuer-und gesetzliche Anforderungen. In den USA und Puerto Rico werden die PSTN-Dienste von Microsoft als Steuer inklusiv fest.  Eindeutige PSTN-Steuern und-Vorschriften wirken sich auf Office 365-Partner aus, die Microsoft 365 Voice-Produkte.  Wenn ein Partner einen Aufschlag auf den Preis eines PSTN-Diensts von Microsoft erhebt, ist er möglicherweise für die Berechnung und Abführung von Steuern und Gebühren für PSTN-Dienste verantwortlich.

## <a name="partner-recommendations"></a>Partner Empfehlungen

Wenden Sie sich an Ihren Steuer-und Rechtsberater, um zu verstehen, wie sich Ihr Unternehmen in Bezug auf die Vorschriften, Steuern und Gebühren sowie andere potenzielle Verpflichtungen in Ihrem Unternehmen für die

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Rechnungs Präsentation und Vereinbarungs Datei für Partner

CSP-Rechnungen und CSP-Abstimmungs Dateien in den USA, Puerto Rico und Kanada, die Skype for Business-PSTN und Microsoft 365 Voice-Dienste enthalten, stellen separate Zeilen Elemente für die PSTN-und nicht-PSTN-Komponenten bereit.

Darüber hinaus wird für CSP-Rechnungen der folgende Fußnote angezeigt:

* Der angezeigte Preis ist eine Gebühr für Audiokonferenzen und das Aufrufen von Plan Diensten.  Alle anwendbaren Transaktionssteuern werden ausschließlich in Rechnung gestellt, mit Ausnahme des Umsatzes, der in der USA erfolgt.  In den USA ist der angezeigte Preis steuerlich inklusiv, da er eine Gebühr für den Aufruf Plan und die Audiokonferenz-Dienste sowie eine Gebühr für die Steuern und Gebühren enthält, die wir berechnen müssen.  Audiokonferenzen und Aufruf Plan Dienste werden vom Microsoft-Partner betreut, der zur Bereitstellung autorisiert ist.  Weitere Informationen finden Sie unter [Microsoft-Volumenlizenzierung](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Beispiel für eine Abstimmungs Datei

Office 365 Enterprise E5 zeigt eine Abstimmungs Datei als zweizeilige Elemente mit identischen Namen und identischen IDs an, aber jedes einzelne Zeilen Element hat einen eindeutigen Einheitspreis (Beispiel: $28,40 und $2,00). Dies unterscheidet die Skype for Business PSTN Conferencing-Komponente vom Office 365-Angebot, sodass Sie Steuern korrekt anwenden können.

**Beispiel für Partner Abstimmung #1 (Spalten auswählen):**

|**Permanente Angebots-ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Gebühr für Zyklus   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Gebühr für Zyklus   |2.00   |

**Beispiel für Partner Abstimmung #2**

Microsoft 365 Business in Kanada verfügbare Sprache verfügt über zusätzliche PSTN-Komponenten, die auf der CSP-Rechnung konsolidiert werden (ähnlich wie bei Office 365 E5 werden zwei Zeilen Elemente angezeigt, eine für PSTN-Komponenten und die andere für nicht-PSTN-Komponenten).  In der CSP-Abstimmungs Datei für Microsoft 365 Business Voice werden alle zu debuggenden PSTN-Komponenten einzeln angezeigt (individuelle PSTN-Komponenten werden in nicht konsolidiert. CSV-oder API-Tool).  Die Summe der Bestelldetails und der in Rechnung gestellten Beträge für Kunden, die in der Abstimmungs Datei gefunden werden, entspricht der CSP-Rechnung.

## <a name="additional-resources"></a>Zusätzliche Ressourcen
Weitere Informationen finden Sie auf der [Microsoft 365 für Partner](https://www.microsoft.com/microsoft-365/partners/) Website.

