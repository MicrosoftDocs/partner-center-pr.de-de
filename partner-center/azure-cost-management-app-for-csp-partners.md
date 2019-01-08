---
title: Azure Cost Management von Cloudyn für CSP-Partner | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management von Cloudyn erfordert einen Zugriff über die Partner Center-API.
author: Janet
ms.author: janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995794"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>App zum Azure-Kostenmanagement für Azure CSP-Partner  

**Betrifft:**

-  Partner Center

[Weitere Informationen zu Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Vorbemerkungen
Bevor Sie Azure Cost Management verwenden können, sollten Sie die folgenden Anforderungen erfüllen:

- Sie sind Partner im Cloud Solution Provider-Programm.
- Sie haben die Möglichkeit, eine Partner Center-API-Web-App zu erstellen.

## <a name="overview"></a>Übersicht

Azure Cost Management von Cloudyn ist eine Web-App, mit dem Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können. Sie können die App über die Partner Center-API nutzen.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrieren Ihrer Web-App im Partner Center
Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie auf die Partner Center-API zugreifen. 
1.  Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.
2.  Wählen Sie aus dem **Partner Center**, **kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Klicken Sie im Abschnitt **Web-app** auf **Neue Web-App hinzufügen**.
<br> **Hinweis:**: Wenn Sie bereits zuvor eine Web-App erstellt haben, können Sie Schritt3 überspringen.
4.  Kopieren und speichern Sie die **Commerce-ID**-GUID und die **App-ID**-GUID für Ihre Web-App. Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.

## <a name="add-a-secret-key-to-your-app"></a>Hinzufügen eines geheimen Schlüssels zu Ihrer App
1. Wählen Sie in der Dropdownliste neben der **Schlüssel hinzufügen**-Schaltfläche eine Dauer von 1 oder 2Jahren aus.
2. Klicken Sie auf **Schlüssel hinzufügen**. 
3. Kopieren Sie und speichern Sie den Wert des geheimen Schlüssels. Sie benötigen diesen für die kostenlose 30-Tage-Testversion.<br>
   > [!NOTE]  
   > Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Ablaufdaten. Speichern Sie die Schlüsselwerte für die zukünftige Verwendung an einem sicheren Ort.

## <a name="next-steps"></a>Nächste Schritte
Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).
Zum Start der Testversion benötigen Sie folgende Informationen:
- Anmeldeinformationen für das Partner Center
- Commerce-ID-GUID
- App-ID-GUID
- Geheimer Anwendungsschlüssel
