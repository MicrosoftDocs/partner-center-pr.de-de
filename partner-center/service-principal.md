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
ms.openlocfilehash: 9d0507b684b213e6da5f48a250e6e61f395fd52a
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436429"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center

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
