---
title: Konfigurowanie zasad dostępu warunkowego dla kampanii usługi Microsoft 365
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Dowiedz się, jak skonfigurować zasady dostępu warunkowego dla kampanii usługi Microsoft 365, aby dodać znaczne dodatkowe zabezpieczenia.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470652"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="adbbf-103">Konfigurowanie zasad dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="adbbf-103">Set up conditional access policies</span></span>

<span data-ttu-id="adbbf-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="adbbf-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="adbbf-105">[Zasady dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodać znaczne dodatkowe zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="adbbf-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="adbbf-106">Firma Microsoft udostępnia zestaw bazowych zasad dostępu warunkowego, które są zalecane dla wszystkich klientów.</span><span class="sxs-lookup"><span data-stu-id="adbbf-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="adbbf-107">Zasady bazowe to zestaw wstępnie zdefiniowanych zasad, które pomagają chronić organizacje przed wieloma typowymi atakami.</span><span class="sxs-lookup"><span data-stu-id="adbbf-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="adbbf-108">Te typowe ataki mogą obejmować rozpylanie hasła, powtarzanie i wyłudzanie informacji.</span><span class="sxs-lookup"><span data-stu-id="adbbf-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="adbbf-109">Te zasady wymagają od administratorów i użytkowników wprowadzenia drugiej formy uwierzytelniania (nazywanej uwierzytelnianiem wieloskładnikowym lub uwierzytelniania wieloskładnikowego), gdy spełnione są określone warunki.</span><span class="sxs-lookup"><span data-stu-id="adbbf-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="adbbf-110">Na przykład jeśli użytkownik loguje się z innego kraju, logowanie może być uznane za ryzykowne, a użytkownik musi podać dodatkową formę uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="adbbf-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="adbbf-111">Obecnie zasady linii bazowej są następujące:</span><span class="sxs-lookup"><span data-stu-id="adbbf-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="adbbf-112">**Wymagaj usługi MFA dla administratorów** &ndash; Wymaga uwierzytelniania wieloskładnikowego dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="adbbf-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="adbbf-113">**Ochrona użytkowników końcowych** &ndash; Wymaga uwierzytelniania wieloskładnikowego dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne.</span><span class="sxs-lookup"><span data-stu-id="adbbf-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="adbbf-114">**Blokowanie uwierzytelniania** &ndash; starszego Starsze aplikacje klienckie i niektóre nowe aplikacje nie używają nowszych, bezpieczniejszych protokołów uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="adbbf-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="adbbf-115">Te starsze aplikacje mogą pomijać zasady dostępu warunkowego i uzyskać nieautoryzowany dostęp do środowiska.</span><span class="sxs-lookup"><span data-stu-id="adbbf-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="adbbf-116">Ta zasada blokuje dostęp od klientów, którzy nie obsługują dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="adbbf-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="adbbf-117">**Wymagaj usługi MFA do zarządzania usługami** &ndash; Wymaga uwierzytelniania wieloskładnikowego w celu uzyskania dostępu do narzędzi do zarządzania, w tym witryny Azure Portal (w której można skonfigurować zasady linii bazowej).</span><span class="sxs-lookup"><span data-stu-id="adbbf-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="adbbf-118">Firma Microsoft zaleca włączenie wszystkich tych zasad bazowych.</span><span class="sxs-lookup"><span data-stu-id="adbbf-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="adbbf-119">Po włączeniu tych zasad administratorzy i użytkownicy zostaną poproszeni o zarejestrowanie się w celu uwierzytelniania wieloskładnikowego platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="adbbf-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="adbbf-120">Aby uzyskać więcej informacji na temat tych zasad, zobacz [Co to są zasady bazowe?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="adbbf-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="adbbf-121">Konfigurowanie zasad planu bazowego</span><span class="sxs-lookup"><span data-stu-id="adbbf-121">Set up baseline policies</span></span>

1. <span data-ttu-id="adbbf-122">Przejdź do [witryny Azure Portal](https://portal.azure.com), a następnie przejdź do **usługi Azure Active Directory** \> **Conditional Access**.</span><span class="sxs-lookup"><span data-stu-id="adbbf-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="adbbf-123">Zasady linii bazowej są wymienione na stronie.</span><span class="sxs-lookup"><span data-stu-id="adbbf-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="adbbf-124">![Strona zawierająca listę zasad planu bazowego dostępu warunkowego.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="adbbf-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="adbbf-125">Zobacz następujące instrukcje dotyczące każdej zasady:</span><span class="sxs-lookup"><span data-stu-id="adbbf-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="adbbf-126">Wymagaj usługi MFA dla administratorów</span><span class="sxs-lookup"><span data-stu-id="adbbf-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="adbbf-127">Wymagaj usługi MFA dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="adbbf-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="adbbf-128">Blokowanie uwierzytelniania starszego</span><span class="sxs-lookup"><span data-stu-id="adbbf-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="adbbf-129">Wymagaj usługi MFA do zarządzania usługami</span><span class="sxs-lookup"><span data-stu-id="adbbf-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="adbbf-130">Można skonfigurować wiele dodatkowych zasad, takich jak wymaganie zatwierdzonych aplikacji klienckich.</span><span class="sxs-lookup"><span data-stu-id="adbbf-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="adbbf-131">Aby uzyskać więcej informacji, zobacz [dokumentację dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="adbbf-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
