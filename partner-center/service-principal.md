---
title: Azure AD-Dienstprinzipal
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie einen Dienstprinzipal zu Ihrem Azure AD-Mandanten hinzufügen. Dabei fügen Sie eine Azure AD-Anwendung (Dienstprinzipal) in Partner Center hinzu.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d75c5c7311feaa3ca53139f2abf2702035b1069
ms.sourcegitcommit: 2e206627323ff175c0e0d10646cdba80e9881891
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/29/2020
ms.locfileid: "87365756"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator

Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Azure AD-Anwendung (Dienstprinzipal) als Benutzer in Ihrem Partner Center-Konto hinzufügen. (Dies war zuvor in Ihrem Cloud-Partnerportal- oder CPP-Konto möglich. Nach der Migration zu Partner Center ist das CPP-Konto schreibgeschützt.)
 
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