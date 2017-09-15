---
title: Azure Active Directory tenants and Partner Center | Partner Center
description: "To create a Partner Center account, your company must have an Azure Active Directory (Azure AD) tenant. Azure AD is Microsoft’s cloud-based directory and identity management service."
author: labrenne
robots: 
ms.openlocfilehash: ab16d167fc978d76c96fc6ef7c1b8eabe26a1ad5
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/07/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Azure Active Directory tenants and Partner Center  

**Applies to**

-  Partner Center

#<a name="why-you-need-an-azure-ad-tenant"></a>Why you need an Azure AD tenant

We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.

If your company already has an Azure AD tenant, you can link it to your Partner Center account. 

**Hinweis** Bevor Sie sich entschließen, einen vorhandenen Azure AD-Mandanten zu verwenden, bedenken Sie, wie viele Benutzer im Mandanten Partner Center verwenden müssen. If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.

Falls Ihr Unternehmen nicht bereits über einen Azure AD-Mandanten verfügt, können Sie während des Registrierungsprozesses kostenlos einen erstellen. Wählen Sie **Neuen Mandanten erstellen** auf der Seite **Bei Azure Active Directory anmelden**. 


## <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Sie sind nicht sicher, ob Ihre Firma bereits einen Azure AD-Mandanten besitzt?

If you’re not sure whether your company has an Azure AD tenant, follow these steps to check. Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.
1.  Sign in to the Azure admin portal at https://ms.portal.azure.com
2.  Select Azure Active Directory from the menu and then select Domain Names.
3.  Wenn Sie bereits einen Mandanten haben, wird Ihr Domänenname aufgeführt.

##<a name="using-an-existing-tenant"></a>Verwenden Sie einen vorhandenen Mandanten?

If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps. 

![Haben Sie einen Azure AD-Mandanten oder müssen Sie einen erstellen?](images/onboardingAADFlow.png)

Weitere Informationen zum Hinzufügen von Domänen in Azure AD finden Sie unter [Hinzufügen oder Zuweisen einer Domäne in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain).

# <a name="about-microsoft-azure"></a>Informationen zu Microsoft Azure

Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters. Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines. 

When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business. To the office building’s owner, your company is a tenant. 

An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365. 

Der Mandanten hostet die Azure AD-Benutzer und die Informationen zu ihnen – ihre Kennwörter, Profildaten, Berechtigungen usw. Der Mandant enthält darüber hinaus Gruppen, Anwendungen und andere Informationen, die ein Unternehmen und seine Sicherheit betreffen. 
