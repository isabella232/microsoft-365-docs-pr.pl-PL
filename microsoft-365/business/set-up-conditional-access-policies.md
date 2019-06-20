---
title: Konfigurowanie zasad dostępu warunkowego dla kampanii Microsoft 365
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
description: Informacje o sposobie konfigurowania zasad dostępu warunkowego dla kampanii 365 Microsoft.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086377"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="c6d23-103">Konfigurowanie zasad dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="c6d23-103">Set up conditional access policies</span></span>

<span data-ttu-id="c6d23-104">Zasady [dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodać istota dodatkowe zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="c6d23-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="c6d23-105">Firma Microsoft udostępnia zestaw zasad dostępu warunkowego według planu bazowego, które są zalecane dla wszystkich odbiorców.</span><span class="sxs-lookup"><span data-stu-id="c6d23-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="c6d23-106">Zasady według planu bazowego są zestaw wstępnie zdefiniowanych zasad, ułatwiających ochronę organizacji przed atakami wiele typowych.</span><span class="sxs-lookup"><span data-stu-id="c6d23-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="c6d23-107">Te wspólne ataki mogą zawierać hasło spray, powtórzeń i witryn wyłudzających informacje.</span><span class="sxs-lookup"><span data-stu-id="c6d23-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="c6d23-108">Zasady te wymagają Administratorzy i użytkownicy mają wprowadzać drugą formę uwierzytelniania (nazywany uwierzytelnianie wieloskładnikowe lub MFA) po spełnieniu pewnych warunków.</span><span class="sxs-lookup"><span data-stu-id="c6d23-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="c6d23-109">Na przykład jeśli użytkownik jest logowania z innego kraju, znak w mogłyby być uważane za ryzykowne i użytkownik musi podać dodatkowe formy uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="c6d23-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="c6d23-110">Obecnie według planu bazowego zasady są następujące:</span><span class="sxs-lookup"><span data-stu-id="c6d23-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="c6d23-111">**Wymagają MFA dla grupy Administratorzy** — wymaga wieloczynnikowe uwierzytelnianie dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="c6d23-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="c6d23-112">**Ochrona użytkownika końcowego** — wymaga wieloczynnikowe uwierzytelnianie dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne.</span><span class="sxs-lookup"><span data-stu-id="c6d23-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="c6d23-113">**Starsze uwierzytelnianie bloku** — starsze aplikacje klienta i niektóre nowe aplikacje nie używaj protokoły uwierzytelniania nowsze, bardziej bezpieczne.</span><span class="sxs-lookup"><span data-stu-id="c6d23-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="c6d23-114">Te starsze aplikacje można ominąć zasady dostępu warunkowego i uzyskać nieautoryzowany dostęp do środowiska.</span><span class="sxs-lookup"><span data-stu-id="c6d23-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="c6d23-115">Ta zasada blokuje dostęp od klientów, które nie obsługują dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="c6d23-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="c6d23-116">**Wymagają MFA zarządzania serwisem** — wymaga wieloczynnikowe uwierzytelnianie dla dostępu do narzędzi do zarządzania, w tym portalu Azure (gdzie można skonfigurować zasady według planu bazowego).</span><span class="sxs-lookup"><span data-stu-id="c6d23-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="c6d23-117">Microsoft zaleca, aby włączyć wszystkie te zasady według planu bazowego.</span><span class="sxs-lookup"><span data-stu-id="c6d23-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="c6d23-118">Po te zasady są włączone, Administratorzy i użytkownicy pojawi się monit zarejestrować Azure Multii uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="c6d23-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="c6d23-119">Aby uzyskać więcej informacji o tych zasadach zobacz [Co to są zasady planu bazowego](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="c6d23-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="c6d23-120">Ustawianie zasad według planu bazowego</span><span class="sxs-lookup"><span data-stu-id="c6d23-120">Set up baseline policies</span></span>

1. <span data-ttu-id="c6d23-121">Przejdź do [portalu Azure](https://portal.azure.com), a następnie przejdź do **Usługi Active Directory Azure** \> **Dostępu warunkowego**.</span><span class="sxs-lookup"><span data-stu-id="c6d23-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="c6d23-122">Zasady według planu bazowego są wymienione na stronie.</span><span class="sxs-lookup"><span data-stu-id="c6d23-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="c6d23-123">![Strona, która wyświetla listę zasad według planu bazowego dla dostępu warunkowego.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="c6d23-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="c6d23-124">Zobacz następujące szczegółowe instrukcje dla każdej zasady:</span><span class="sxs-lookup"><span data-stu-id="c6d23-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="c6d23-125">Wymagane MFA dla grupy Administratorzy</span><span class="sxs-lookup"><span data-stu-id="c6d23-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="c6d23-126">Reequire MFA dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="c6d23-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="c6d23-127">Starsze uwierzytelnianie bloku</span><span class="sxs-lookup"><span data-stu-id="c6d23-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="c6d23-128">Wymagane MFA zarządzania serwisem</span><span class="sxs-lookup"><span data-stu-id="c6d23-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="c6d23-129">Można skonfigurować wiele dodatkowych polityk, takich jak wymagające aplikacje klienta zatwierdzone.</span><span class="sxs-lookup"><span data-stu-id="c6d23-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="c6d23-130">Zobacz [Warunkowego dostępu do dokumentacji](https://docs.microsoft.com/azure/active-directory/conditional-access/) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="c6d23-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>