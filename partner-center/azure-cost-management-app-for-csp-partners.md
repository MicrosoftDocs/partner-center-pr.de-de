---
title: Azure Cost Management von Cloudyn für CSP-Partner | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Azure Cost Management von Cloudyn erfordert einen Zugriff über die Partner Center-API.
author: Janet
ms.author: janet
Keywords: Azure Cost Management-app, Verwalten von Kosten, web-apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 14b94e94c349fa142cb6bd37ed4ca94f7a9397b6
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134670"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>App zum Azure-Kostenmanagement für Azure CSP-Partner  

**Gilt für**

-  Partner Center

[Informationen Sie weitere zu Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Vorbemerkungen
Bevor Sie Azure Cost Management verwenden können, sollten Sie die folgenden Anforderungen erfüllen:

- Sie sind Partner im Cloud-Lösungsanbieter-Programm.
- Sie haben die Möglichkeit, eine Partner Center-API-Web-App zu erstellen.

## <a name="overview"></a>Übersicht

Cloudyn ist eine Web-app, die Ihnen die Möglichkeit zum Nachverfolgen und verwalten, wie viel Ihre Kunden Azure und die Kosten für diese Nutzung verwenden. Sie können die App über die Partner Center-API nutzen.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrieren Ihrer Web-App im Partner Center
Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie auf die Partner Center-API zugreifen. 
1.  Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.
2.  Von der **Partner Center**Option **Kontoeinstellungen** &gt;  **[App-Verwaltung](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Klicken Sie im Abschnitt **Web-app** auf **Neue Web-App hinzufügen**.
<br> **Hinweis**: Wenn Sie zuvor eine Web-app erstellt haben, können Sie Schritt 3 überspringen.
4.  Kopieren und speichern Sie die **Commerce-ID**-GUID und die **App-ID**-GUID für Ihre Web-App. Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.

## <a name="add-a-secret-key-to-your-app"></a>Hinzufügen eines geheimen Schlüssels zu Ihrer App
1. Wählen Sie in der Dropdownliste neben der **Schlüssel hinzufügen**-Schaltfläche eine Dauer von 1 oder 2 Jahren aus.
2. Klicken Sie auf **Schlüssel hinzufügen**. 
3. Kopieren Sie und speichern Sie den Wert des geheimen Schlüssels. Sie benötigen diesen für die kostenlose 30-Tage-Testversion.<br>
   > [!NOTE]  
   > Der geheime Anwendungsschlüssel sind wie Kennwörter mit einer längeren Gültigkeitsdauer. Speichern Sie die Schlüsselwerte für die zukünftige Verwendung an einem sicheren Ort.

## <a name="next-steps"></a>Nächste Schritte
Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).
Zum Start der Testversion benötigen Sie folgende Informationen:
- Anmeldeinformationen für das Partner Center
- Commerce-ID-GUID
- App-ID-GUID
- Geheimer Anwendungsschlüssel
