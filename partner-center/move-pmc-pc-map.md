---
title: Wechsel von PMC zu Partner Center
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informieren Sie sich, welche Unterschiede PMC und Partner Center im Hinblick auf Verlängerungen, die Kontostruktur, die Anmeldung, Benutzerrollen, Kompetenzen und mehr aufweisen.
author: parthpandyaMSFT
ms.author: parthp
keywords: PMC, Migration, Wechsel zu Partner Center
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ac79b85d4278f6340d6997fc94151bc0cb404c3e
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390627"
---
# <a name="moving-from-partner-membership-center-pmc-to-partner-center"></a>Umstellung von Partner Membership Center (PMC) auf Partner Center

**Geeignete Rollen**
-    Globaler Administrator

Wir vereinfachen die Geschäftstätigkeit mit uns, indem wir eine einzelne Website (Partner Center) einführen, die als zentrale Anlaufstelle dient. Alle Aktivitäten, die du von Partner Membership Center (PMC) kennst, kannst du auch über das Dashboard in Partner Center ausführen. 

Darüber hinaus kannst du noch viele weitere Aufgaben erledigen – alles in einer einzigen Website. Die Begriffe und Features unterscheiden sich jedoch leicht. Mithilfe der Tour zum Dashboard sollten Sie unbedingt herausfinden, welche Funktion sich wo befindet.

Die folgende Tabelle zeigt einige der Unterschiede zwischen PMC und Partner Center.

## <a name="renewing-your-microsoft-partner-network--membership"></a>Aktualisieren der Microsoft Partner Network-Mitgliedschaft

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Verlängerungen begannen 90 Tage vor dem Jahrestag und mussten bis zum Jahrestag abgeschlossen sein.| Partner können einen bis 30 Tage nach dem Jahrestag verlängern.|

## <a name="account-structure"></a>Kontostruktur

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Hauptsitz und Filialstandorte wurden separat bewertet. Die Bewertung der Kompetenzen erfolgte auf lokaler Ebene.|Das globale Unternehmen einschließlich zugehöriger Filialstandorte – das Partner Global Account (PGA) –, wird als Ganzes bewertet. Leistungs- und Qualifikationsdaten werden auf PGA-Ebene aggregiert. Partner Center umfasst verschiedene Profilansichten für Programme, z. B. Partner- und Businessprofile für Empfehlungen und Marketing. Weitere Informationen findest du unter [Kontostruktur in Partner Center](account-structure.md).|

## <a name="sign-in"></a>Melden Sie sich

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Es konnten die Anmeldeinformationen sowohl für Microsoft-Konten (MSA) also auch für persönliche Konten (joe@outlook.com) verwendet werden.|Du musst die Anmeldeinformationen für dein Geschäftskonto verwenden (joe@joescompany.com). Weitere Informationen findest du unter [Das Geschäftskonto deines Unternehmens und Partner Center](azure-active-directory-tenants-and-partner-center.md).|

## <a name="user-roles"></a>Benutzerrollen

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Viele der PMC-Rollen werden in Partner Center nicht verwendet.|Dem Administrator, der den Wechsel zu Partner Center durchführt, werden automatisch die Rollen „MPN Admin“, „Account Admin“ und „Referrals Admin“ zugewiesen. Dann kann dieser Administrator andere Benutzer zu Benutzerrollen zuweisen.|
|Benutzer wurden auf Standortebene verwaltet.|Benutzer werden Unternehmensebene (PGA) verwaltet, nicht auf Standortebene. Die Rolle „Incentives Admin“ bildet eine Ausnahme, da diese auf Standortebene funktioniert.|
|   |Partner Center bietet zwei umfangreiche Rollensätze: die Rollen, die den Azure AD-Mandanten verwalten, und die Rollen, die die Geschäftstätigkeit des Unternehmens verwalten. Organisiere die Rollen so, dass sie für dein Unternehmen am meisten Sinn ergeben. Es kann eine Person für alles zuständig sein, oder mehreren Personen können verschiedene Rollen und Berechtigungen zugewiesen werden. Weitere Informationen findest du unter [Zuweisen von Rollen und Berechtigungen zu Benutzern](permissions-overview.md). 

## <a name="how-competencies-and-benefits-are-accounted-for"></a>Berücksichtigung der Kompetenzen und Vorteile

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Pro Standort zusammengefasst und verwaltet.|Die Vorteile, einschließlich der Vorteilsadministration, gelten für das gesamte Unternehmen, du kannst die Vorteile aber so verwalten, wie es für dein Unternehmen am günstigsten ist. |
|Additional Benefits Tool Kits (ABTKs) standen zur Verfügung, bis sie im Oktober 2018 eingestellt wurden.|Keine ABTKs. Ein MAPS pro Unternehmen, eine Silver-Kompetenz pro Unternehmen, eine Gold-Kompetenz pro Unternehmen.|
||MAPS kann erworben werden, sofern noch nicht vorhanden. Der MAPS-Besitz ist nicht an Kompetenzen gebunden.  
|Der Zugriff auf Vorteile erfolgte per Partner Digital Download (PDD). |Alle Vorteile sind im Partner Center verfügbar.|
|Kompetenzen und Vorteile waren auf mehrere Standorte aufgeteilt.|Kompetenzen und Vorteile aus allen Standorten sind auf Unternehmensebene (PGA) konsolidiert und bleiben bis zum Jahrestag erhalten. Zu diesem Zeitpunkt muss ein Neuerwerb oder eine Verlängerung auf Unternehmensebene erfolgen. Leistung und Fähigkeiten werden ebenso wie Kompetenzen global aggregiert.|
|Ansprüche aus Software Assurance-Vouchern wurden im Voucher Validation and Redemption-Tool (VVR) geltend gemacht.|Jetzt kannst du im Partner Center auf Software Assurance Training Vouchers (SATV) und/oder Deployed Planning Services (DPS) zugreifen und diese verwalten.  Das veraltete VRR-Tool wird am 1. Oktober 2019 außer Betrieb genommen.  |

## <a name="associating-mcp-ids-to-partner-center"></a>Zuordnen von MCP-IDs zu Partner Center

|**PMC**   |**Partner Center**   |
|-------------------------|:-------------------|
|Du kannst dieselbe MCP-ID mehreren Unternehmen zuordnen.| Einem einzelnen Partner Center-Konto kann nur eine MCP-ID zugeordnet werden. Du musst die Zuordnung manuell vornehmen. Wähle im Partner Center-Dashboard das Symbol für **Dein Konto** in der rechten Ecke des Dashboards aus, und wähle dann **Mein Profil** aus. Unter **Dein Learning** kannst du dein Microsoft Learning-Konto zuordnen und auch dein Microsoft-Konto mit Partner University verbinden.

## <a name="visual-studio-benefits-and-msa"></a>Visual Studio: Vorteile und MSA

|**PMC**   |**Partner Center**   |
|-----------------|:-----------------|
|Zuordnung von Visual Studio-Vorteilen zu einem MSA|Visual Studio-Vorteile, die MSAs zugeordnet sind, bleiben erhalten und gelten weiter.|
||MSA-Zuordnungen von Visual Studio werden nach der Verlängerung in Partner Center beibehalten.|
||In Partner Center kann ein Partner Geschäftskonten und Gastbenutzerkonten vom Typ MSA aus demselben Mandanten hinzufügen, in dem der Partner MPN-Administrator im Azure AD-Mandanten ist. Wenn der Partner globaler Administrator in mehreren Azure AD-Mandanten ist und all diese Mandanten demselben Partner Center-Konto zugeordnet sind, kann der Partner Benutzer aus all diesen Mandanten zu Visual Studio-Vorteilen und zu auf der Azure-Nutzung basierenden Zuordnungen hinzufügen. Ein MPN-Administrator oder globaler Administrator kann zwar Gastbenutzern nutzungsbasierte Visual Studio-Abonnements zuweisen, aber Gastbenutzer können sich nicht mit ihrem MSA bei Partner Center anmelden. Gastbenutzer können sich aber bei Azure und Visual Studio anmelden, um die ihnen zugewiesenen Vorteile zu überprüfen und zu nutzen. |

## <a name="programs-now-located-and-managed-in-partner-center"></a>In Partner Center befindliche und verwaltete Programme 

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|PDD  |Vorteile|
|CHIP, ICP, PIE | Incentives|
||Empfehlungen|
|Partner Insights| Analysen|
|Tool zur Gutscheinvalidierung und -einlösung (Voucher Validation and Redemption, VVR)| Tool zur Gutscheinvalidierung und -einlösung (Voucher Validation and Redemption, VVR)|
|           |Cloud Solution Provider-Programme|

Visual Studio-Vorteile, die MSAs zugeordnet sind, bleiben erhalten und gelten weiter. Sie werden auch nach der Verlängerung in Partner Center beibehalten. Wenn Sie jedoch nach der Migration zu Partner Center eine MSA-Zuordnung entfernen, kann diese Partner Center nicht erneut hinzugefügt werden.

In Partner Center kann ein Partner Geschäftskonten und Gastbenutzerkonten vom Typ MSA aus demselben Mandanten hinzufügen, in dem der Partner MPN-Administrator im Azure AD-Mandanten ist. Wenn der Partner globaler Administrator in mehreren Azure AD-Mandanten ist und all diese Mandanten demselben Partner Center-Konto zugeordnet sind, kann der Partner Benutzer aus all diesen Mandanten zu Visual Studio-Vorteilen und zu auf der Azure-Nutzung basierenden Zuordnungen hinzufügen.

Ein MPN-Administrator oder globaler Administrator kann zwar Gastbenutzern nutzungsbasierte Visual Studio-Abonnements zuweisen, aber Gastbenutzer können sich nicht mit ihrem MSA bei Partner Center anmelden. Gastbenutzer können sich aber bei Azure und Visual Studio anmelden, um die ihnen zugewiesenen Vorteile zu überprüfen und zu nutzen.
