---
title: Azure Cost Management von cloudyn für CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die cloudyn-Web-App registrieren und einen geheimen Schlüssel für diese in Partner Center verwenden, damit Sie die APP verwenden können, um die Azure-Nutzung und die Kosten des Kunden zu verfolgen.
author: aparnagkrishnan
ms.author: aparnag
Keywords: Azure Cost Management-App, Kostenmanagement, Web-Apps
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 521501f9a979c0993d299ab30443168408656a44
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390447"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Verfolgen Sie die Azure-Nutzung und die Kosten des Kunden mit der Azure Cost Management-APP für CSP-Partner  

**Zielgruppe**

- Partner Center
- Partner im Cloud Solution Provider-Programm

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent

[Weitere Informationen zu Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Voraussetzungen
Bevor Sie Azure Cost Management verwenden können, müssen Sie die folgenden Anforderungen erfüllen:

- Sie sind Partner im Cloud Solution Provider-Programm.
- Sie haben die Fähigkeit, eine Partner Center-API-Web-App zu erstellen.

## <a name="overview"></a>Übersicht

Cloudyn ist eine Web-App, mit der Sie die Azure-Nutzung Ihrer Kunden und die Kosten dieser Nutzung nachverfolgen und verwalten können. Sie können die App über die Partner Center-API nutzen.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrieren Ihrer Web-App im Partner Center
Wenn Sie eine Azure Active Directory-Web-App im Partner Center registrieren, können Sie den Zugriff auf die Partner Center-API aktivieren. 
1.  Melden Sie sich beim [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) mit einem [globalen Administratorkonto oder Administrator-Agentkonto](create-user-accounts-and-set-permissions.md) an.
2.  Wählen Sie im **Partner Center**nacheinander **Kontoeinstellungen** &gt; **[App-Verwaltung](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** aus.
3.  Klicken Sie im Abschnitt **Web-App** auf **Neue Web-App hinzufügen**.
<br> **Hinweis**: Wenn Sie zuvor eine Web-App erstellt haben, können Sie Schritt 3 überspringen.
4.  Kopieren und speichern Sie die GUIDs für **Commerce-ID**und **App-ID** für Ihre Web-App. Sie benötigen beide IDs für die 30-tägige kostenlose Testversion der Azure Cost Management-App.

## <a name="add-a-secret-key-to-your-app"></a>Hinzufügen eines geheimen Schlüssels zu Ihrer App
1. Wählen Sie in der Dropdownliste neben der Schaltfläche **Schlüssel hinzufügen**eine Dauer von 1 oder 2 Jahren aus.
2. Klicken Sie auf **Schlüssel hinzufügen**. 
3. Kopieren und speichern Sie den Wert des geheimen Schlüssels. Sie benötigen diesen für die kostenlose 30-Tage-Testversion.<br>
   > [!NOTE]  
   > Die geheimen Anwendungsschlüssel sind wie Kennwörter mit längeren Laufzeiten. Speichern Sie den Schlüsselwert für die künftige Verwendung an einem sicheren Ort.

## <a name="next-steps"></a>Nächste Schritte
Starten Sie mit einer [kostenlosen 30-Tage-Testversion](https://go.microsoft.com/fwlink/?linkid=857895).
Zum Start der Testversion benötigen Sie folgende Informationen:
- Anmeldeinformationen für Partner Center
- Commerce-ID-GUID
- App-ID-GUID
- Wert des geheimen Anwendungsschlüssels
