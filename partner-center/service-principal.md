---
title: Azure AD-Dienstprinzipal | Partner Center
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hinzufügen eines Dienstprinzipals zu Ihrem Azure AD-Mandanten
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure-Plan, Dienstprinzipal, Azure AD-Anwendung
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010381"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal) in Partner Center

Sie können nun im Programm für den kommerziellen Marketplace in Partner Center eine Azure AD-Anwendung (Dienstprinzipal) als Benutzer in Ihrem Azure AD-Mandanten hinzufügen. (Dieser Schritt konnte zuvor im CPP-Konto (Cloud-Partnerportal) ausgeführt werden. Nach Ihrer Migration zu Partner Center ist das CPP-Konto jedoch schreibgeschützt.) Beachten Sie, dass der Dienstprinzipal mit der Azure AD-Anwendung identisch ist.

## <a name="add-an-azure-ad-application-service-principal"></a>Hinzufügen einer Azure AD-Anwendung (Dienstprinzipal)

1. Wählen Sie auf dem Partner Center-Dashboard **Einstellungen** und anschließend **Entwicklereinstellungen** aus.

2. Wählen Sie **Benutzer** und dann **Azure AD-Anwendungen hinzufügen** aus.

3. Wählen Sie eine vorhandene Azure AD-Anwendung aus, oder erstellen eine neue.

4. Geben Sie bei Erstellung einer neuen Azure AD-Anwendung die folgenden Informationen an:  
  
**Name**: Dies ähnelt dem Feld „Anzeigename“ im CPP.

**Antwort-URL**: Dies ist die URL, unter der sich Benutzer zur Verwendung Ihrer Azure AD-Anwendung anmelden können. 

**App-ID-URI**: Dies ist ein logischer Bezeichner für die Azure AD-App, der beim Senden einer Anforderung für einmaliges Anmelden an Azure AD angezeigt wird. 

**Sicherheitsrollen**: Die Rollen **Manager** (entspricht der Rolle „Besitzer“ im CPP) und **Entwickler** (entspricht der Rolle „Mitwirkender“ im CPP) gelten für das Programm für den kommerziellen Marketplace in Partner Center und können dieser Azure AD-Anwendung zugeordnet werden.  

Wenn Sie zur Erstellung in Partner Center **Speichern** auswählen, werden die Informationen auch mit dem CPP-System synchronisiert.  
