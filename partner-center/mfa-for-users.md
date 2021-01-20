---
title: Einrichten von Benutzern mit mehrstufiger Authentifizierung
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie Mitarbeiter mit mehrstufiger Authentifizierung (MFA) einrichten.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182374"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="0e09c-103">Einrichten von Benutzern mit mehrstufiger Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="0e09c-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="0e09c-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="0e09c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0e09c-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="0e09c-105">Global admin</span></span>

<span data-ttu-id="0e09c-106">Mehr Sicherheitsmaßnahmen für den Datenschutz und eine höhere Sicherheit gehören zu unseren obersten Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="0e09c-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="0e09c-107">Wir wissen, dass die beste Verteidigung die Prävention ist und dass wir nur so stark sind wie unser schwächstes Glied.</span><span class="sxs-lookup"><span data-stu-id="0e09c-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="0e09c-108">Deshalb müssen alle in unserem Partnerumfeld handeln und sicherstellen, dass sie über angemessene Sicherheitsvorkehrungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="0e09c-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="0e09c-109">Es wird dringend empfohlen, dass alle Partner die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) für die Benutzer in ihrem Partnermandanten aktivieren.</span><span class="sxs-lookup"><span data-stu-id="0e09c-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="0e09c-110">Hinzufügen der mehrstufigen Authentifizierung für Benutzer</span><span class="sxs-lookup"><span data-stu-id="0e09c-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="0e09c-111">Sie müssen der globale Administrator für Ihr Unternehmen sein, um diese Aufgabe auszuführen.</span><span class="sxs-lookup"><span data-stu-id="0e09c-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="0e09c-112">Die mehrstufige Authentifizierung für Ihre Benutzer kann am einfachsten aktiviert werden, während Sie diese Ihrem Azure AD-Mandanten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="0e09c-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="0e09c-113">Melden Sie sich beim [Azure-Portal](https://portal.azure.com) an, und wechseln Sie dann zu **Benutzerverwaltung**.</span><span class="sxs-lookup"><span data-stu-id="0e09c-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="0e09c-114">Wählen Sie **Multi-Factor Authentication** aus.</span><span class="sxs-lookup"><span data-stu-id="0e09c-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="0e09c-115">Wählen Sie den zu aktivierenden Benutzer und dann **Aktivieren** aus.</span><span class="sxs-lookup"><span data-stu-id="0e09c-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="0e09c-116">Dadurch wird Multi-Factor Authentication für diesen Benutzer aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0e09c-116">This will enable MFA for this user.</span></span> <span data-ttu-id="0e09c-117">Aktiviert bedeutet, dass der Benutzer bei der ersten Anmeldung aufgefordert wird, die MFA-Überprüfung einzurichten.</span><span class="sxs-lookup"><span data-stu-id="0e09c-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="0e09c-118">Anschließend wird der Benutzer bei der Anmeldung aufgefordert, einen Code anzugeben, der ihm entweder per E-Mail oder SMS (je nach Einrichtung) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="0e09c-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Festlegen der Überprüfungsmethode":::

>[!NOTE]
><span data-ttu-id="0e09c-120">Sie können die Verwendung von Multi-Factor Authentication durch die Benutzer erzwingen, indem Sie die oben beschriebenen Schritte ausführen und dann **Erzwingen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="0e09c-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="0e09c-121">Weitere Informationen finden Sie unter [Aktivieren von Azure Multi-Factor Authentication für Einzelbenutzer zum Sichern von Anmeldeereignissen](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="0e09c-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="0e09c-122">Alle Benutzer sind zunächst  **Deaktiviert**.</span><span class="sxs-lookup"><span data-stu-id="0e09c-122">All users start out **Disabled**.</span></span> <span data-ttu-id="0e09c-123">Wenn Sie Benutzer für Azure Multi-Factor Authentication für Einzelbenutzer registrieren, ändert sich deren Status in  **Aktiviert**.</span><span class="sxs-lookup"><span data-stu-id="0e09c-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="0e09c-124">Wenn aktivierte Benutzer sich anmelden und den Registrierungsprozess abschließen, ändert sich der Status in  **Erzwungen**.</span><span class="sxs-lookup"><span data-stu-id="0e09c-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0e09c-125">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0e09c-125">Next steps</span></span>

- [<span data-ttu-id="0e09c-126">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="0e09c-126">Assign roles and permissions to users</span></span>](permissions-overview.md)