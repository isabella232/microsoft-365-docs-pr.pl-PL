---
title: Konfigurowanie zasad dostępu warunkowego dla kampanii microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
description: Dowiedz się, jak skonfigurować zasady dostępu warunkowego dla kampanii usługi Microsoft 365, aby zwiększyć dodatkowe zabezpieczenia.
ms.openlocfilehash: be3ca0da3d27e3ec49f1227e4482cfd7fcaae8cb
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550082"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="e5411-103">Konfigurowanie zasad dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="e5411-103">Set up conditional access policies</span></span>

<span data-ttu-id="e5411-104">[Zasady dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodać znaczne dodatkowe zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="e5411-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="e5411-105">Firma Microsoft udostępnia zestaw podstawowych zasad dostępu warunkowego, które są zalecane dla wszystkich klientów.</span><span class="sxs-lookup"><span data-stu-id="e5411-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="e5411-106">Zasady bazowe to zestaw wstępnie zdefiniowanych zasad, które pomagają chronić organizacje przed wieloma typowymi atakami.</span><span class="sxs-lookup"><span data-stu-id="e5411-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="e5411-107">Te typowe ataki mogą obejmować rozpylanie haseł, powtórkę i wyłudzanie informacji.</span><span class="sxs-lookup"><span data-stu-id="e5411-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="e5411-108">Te zasady wymagają, aby administratorzy i użytkownicy włączyli drugą formę uwierzytelniania (nazywane uwierzytelnianiem wieloskładnikowym lub uwierzytelnianiem wieloskładnikowym), gdy spełnione są określone warunki.</span><span class="sxs-lookup"><span data-stu-id="e5411-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="e5411-109">Na przykład jeśli użytkownik loguje się z innego kraju, logowanie może być uznane za ryzykowne, a użytkownik musi podać dodatkową formę uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="e5411-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="e5411-110">Obecnie zasady bazowe obejmują następujące zasady:</span><span class="sxs-lookup"><span data-stu-id="e5411-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="e5411-111">**Wymagaj uwierzytelniania mfa dla administratorów** &ndash; Wymaga uwierzytelniania wieloskładnikowego dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="e5411-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="e5411-112">**Ochrona** &ndash; użytkowników końcowych Wymaga uwierzytelniania wieloskładnikowego dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne.</span><span class="sxs-lookup"><span data-stu-id="e5411-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="e5411-113">**Blokuj starsze uwierzytelnianie** &ndash; Starsze aplikacje klienckie i niektóre nowe aplikacje nie używają nowszych, bezpieczniejszych protokołów uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="e5411-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="e5411-114">Te starsze aplikacje mogą ominąć zasady dostępu warunkowego i uzyskać nieautoryzowany dostęp do środowiska.</span><span class="sxs-lookup"><span data-stu-id="e5411-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="e5411-115">Ta zasada blokuje dostęp od klientów, którzy nie obsługują dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="e5411-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="e5411-116">**Wymagaj uwierzytelniania mfa dla zarządzania usługami** &ndash; Wymaga uwierzytelniania wieloskładnikowego w celu uzyskania dostępu do narzędzi zarządzania, w tym do witryny Azure portal (w którym można skonfigurować zasady według planu bazowego).</span><span class="sxs-lookup"><span data-stu-id="e5411-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="e5411-117">Firma Microsoft zaleca włączenie wszystkich tych zasad bazowych.</span><span class="sxs-lookup"><span data-stu-id="e5411-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="e5411-118">Po włączeniu tych zasad administratorzy i użytkownicy zostaną poproszeni o zarejestrowanie się w celu uwierzytelniania multii-factor platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="e5411-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="e5411-119">Aby uzyskać więcej informacji na temat tych zasad, zobacz [Co to są zasady bazowe?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="e5411-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="e5411-120">Konfigurowanie zasad linii bazowej</span><span class="sxs-lookup"><span data-stu-id="e5411-120">Set up baseline policies</span></span>

1. <span data-ttu-id="e5411-121">Przejdź do [witryny Azure portal](https://portal.azure.com), a następnie przejdź do usługi Azure Active **Directory** \> **dostęp warunkowy**.</span><span class="sxs-lookup"><span data-stu-id="e5411-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="e5411-122">Zasady bazowe są wymienione na stronie.</span><span class="sxs-lookup"><span data-stu-id="e5411-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="e5411-123">![Strona zawierająca listę zasad bazowych dostępu warunkowego.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="e5411-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="e5411-124">Zapoznaj się z poniższymi szczegółowymi instrukcjami dotyczącymi poszczególnych zasad:</span><span class="sxs-lookup"><span data-stu-id="e5411-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="e5411-125">Wymaganie usługi MFA dla administratorów</span><span class="sxs-lookup"><span data-stu-id="e5411-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="e5411-126">Wymagaj usługi MFA dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="e5411-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="e5411-127">Blokowanie uwierzytelniania starszego</span><span class="sxs-lookup"><span data-stu-id="e5411-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="e5411-128">Wymaganie usługi MFA do zarządzania usługami</span><span class="sxs-lookup"><span data-stu-id="e5411-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="e5411-129">Można skonfigurować wiele dodatkowych zasad, takich jak wymaganie zatwierdzonych aplikacji klienckich.</span><span class="sxs-lookup"><span data-stu-id="e5411-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="e5411-130">Aby uzyskać więcej informacji, zobacz [dokumentację dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="e5411-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
