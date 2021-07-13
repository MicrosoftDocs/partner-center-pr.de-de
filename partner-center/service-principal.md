---
title: Azure AD-Dienstprinzipal
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie einen Dienstprinzipal zu Ihrem Azure AD-Mandanten hinzufügen. Dabei fügen Sie eine Azure AD-Anwendung (Dienstprinzipal) in Partner Center hinzu.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551553"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center

**Geeignete Rollen**: Globaler Administrator

Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Microsoft Azure Active Directory (Azure AD) Anwendung (Dienstprinzipal) als Benutzer in Ihrem Partner Center-Konto hinzufügen. (Dies war zuvor in Ihrem Cloud-Partnerportal Konto möglich). Nach der Migration zu Partner Center ist das CPP-Konto schreibgeschützt.)
 
>[!Note] 
>Der Dienstprinzipal ist mit der Azure AD-Anwendung identisch.

## <a name="add-an-azure-ad-application-service-principal"></a>Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal)

1. Wählen Sie auf dem Partner Center-Dashboard **Einstellungen** und anschließend **Entwicklereinstellungen** aus.

2. Wählen Sie **Benutzer** und dann **Azure AD-Anwendungen hinzufügen** aus.

3. Wählen Sie eine vorhandene Azure AD-Anwendung aus, oder erstellen eine neue.

4. Geben Sie bei Erstellung einer neuen Azure AD-Anwendung die folgenden Informationen an:  

   - **Antwort-URL**: Die URL, unter der sich Benutzer zur Verwendung Ihrer Azure AD-Anwendung anmelden können.

   - **App-ID-URI**: Ein logischer Bezeichner für die Azure AD-Anwendung, der beim Senden einer Anforderung für einmaliges Anmelden an Azure AD angezeigt wird.

   - **Sicherheitsrollen**: Die Rollen **Manager** (entspricht der Rolle „Besitzer“ im CPP) und **Entwickler** (entspricht der Rolle „Mitwirkender“ im CPP) gelten für das Programm für den kommerziellen Marketplace in Partner Center und können dieser Azure AD-Anwendung zugeordnet werden.  

## <a name="next-steps"></a>Nächste Schritte

- [Übersicht über den kommerziellen Marketplace im Partner Center](csp-commercial-marketplace-overview.md)