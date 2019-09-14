---
title: Konfigurowanie zasad dostępu warunkowego dla kampanii firmy Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Dowiedz się, jak skonfigurować zasady dostępu warunkowego dla kampanii firmy Microsoft 365.
ms.openlocfilehash: 614e3a6e13a14114f40ecf87bf936d4165744503
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982386"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="9326a-103">Konfigurowanie zasad dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="9326a-103">Set up conditional access policies</span></span>

<span data-ttu-id="9326a-104">Zasady [dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodają substancjalne dodatkowe zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="9326a-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="9326a-105">Firma Microsoft udostępnia zestaw podstawowych zasad dostępu warunkowego, które są zalecane dla wszystkich klientów.</span><span class="sxs-lookup"><span data-stu-id="9326a-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="9326a-106">Zasady bazowe to zestaw wstępnie zdefiniowanych zasad, które ułatwiają ochronę organizacji przed wieloma powszechną atakami.</span><span class="sxs-lookup"><span data-stu-id="9326a-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="9326a-107">Te typowe ataki mogą zawierać spray do haseł, powtórki i phishing.</span><span class="sxs-lookup"><span data-stu-id="9326a-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="9326a-108">Te zasady wymagają, aby administratorzy i użytkownicy wprowadzali drugą formę uwierzytelniania (nazywanych uwierzytelnianiem wieloczynnikowym lub MFA) po spełnieniu określonych warunków.</span><span class="sxs-lookup"><span data-stu-id="9326a-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="9326a-109">Na przykład jeśli użytkownik jest logowanie z innego kraju, logowanie może być uważane za ryzykowne i użytkownik musi podać dodatkową formę uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="9326a-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="9326a-110">Obecnie zasady bazowe są następujące:</span><span class="sxs-lookup"><span data-stu-id="9326a-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="9326a-111">**Wymagaj MFA dla administratorów** — wymaga uwierzytelniania wieloskładnikowego dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="9326a-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="9326a-112">**Ochrona użytkownika końcowego** — wymaga uwierzytelniania wieloskładnikowego dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne.</span><span class="sxs-lookup"><span data-stu-id="9326a-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="9326a-113">**Blokowanie starszego uwierzytelniania** — starsze aplikacje klienckie i niektóre nowe aplikacje nie korzystają z nowszych, bezpieczniejszych protokołów uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="9326a-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="9326a-114">Te starsze aplikacje mogą pomijać zasady dostępu warunkowego i uzyskiwać nieautoryzowany dostęp do środowiska.</span><span class="sxs-lookup"><span data-stu-id="9326a-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="9326a-115">Ta zasada blokuje dostęp od klientów, którzy nie obsługują dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="9326a-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="9326a-116">Wymagaj uwierzytelniania wieloskładnikowego **dla usługi zarządzania** — wymaga Multi-Factor Authentication dostępu do narzędzi do zarządzania, w tym portalu Azure (gdzie można skonfigurować zasady linii bazowej).</span><span class="sxs-lookup"><span data-stu-id="9326a-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="9326a-117">Firma Microsoft zaleca włączenie wszystkich tych zasad linii bazowej.</span><span class="sxs-lookup"><span data-stu-id="9326a-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="9326a-118">Po włączeniu tych zasad Administratorzy i użytkownicy będą monitowani o zarejestrowanie się w usłudze Azure Multii-Factor Authentication.</span><span class="sxs-lookup"><span data-stu-id="9326a-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="9326a-119">Aby uzyskać więcej informacji na temat tych zasad, zobacz [co to są zasady linii bazowej](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="9326a-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="9326a-120">Konfigurowanie zasad bazowych</span><span class="sxs-lookup"><span data-stu-id="9326a-120">Set up baseline policies</span></span>

1. <span data-ttu-id="9326a-121">Przejdź do [witryny Azure Portal](https://portal.azure.com), a następnie przejdź do **usługi Azure Active Directory** \> **dostępu warunkowego**.</span><span class="sxs-lookup"><span data-stu-id="9326a-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="9326a-122">Zasady linii bazowej są wyświetlane na stronie.</span><span class="sxs-lookup"><span data-stu-id="9326a-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="9326a-123">![Strona, która zawiera listę zasad bazowych dla dostępu warunkowego.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="9326a-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="9326a-124">Zapoznaj się z poniższymi szczegółowymi instrukcjami dotyczącymi poszczególnych zasad:</span><span class="sxs-lookup"><span data-stu-id="9326a-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="9326a-125">Wymagaj uwierzytelniania MFA dla administratorów</span><span class="sxs-lookup"><span data-stu-id="9326a-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="9326a-126">Wymagaj uwierzytelniania wieloskładnikowego dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="9326a-126">Require MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="9326a-127">Blokowanie starszego uwierzytelniania</span><span class="sxs-lookup"><span data-stu-id="9326a-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="9326a-128">Wymagaj uwierzytelniania MFA do zarządzania usługami</span><span class="sxs-lookup"><span data-stu-id="9326a-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="9326a-129">Można skonfigurować wiele dodatkowych zasad, takich jak wymaganie zatwierdzonych aplikacji klienckich.</span><span class="sxs-lookup"><span data-stu-id="9326a-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="9326a-130">Zobacz [dokumentację dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/) Aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="9326a-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>