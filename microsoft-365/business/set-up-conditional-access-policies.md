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
# <a name="set-up-conditional-access-policies"></a>Konfigurowanie zasad dostępu warunkowego

Zasady [dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodać istota dodatkowe zabezpieczenia. Firma Microsoft udostępnia zestaw zasad dostępu warunkowego według planu bazowego, które są zalecane dla wszystkich odbiorców. Zasady według planu bazowego są zestaw wstępnie zdefiniowanych zasad, ułatwiających ochronę organizacji przed atakami wiele typowych. Te wspólne ataki mogą zawierać hasło spray, powtórzeń i witryn wyłudzających informacje.

Zasady te wymagają Administratorzy i użytkownicy mają wprowadzać drugą formę uwierzytelniania (nazywany uwierzytelnianie wieloskładnikowe lub MFA) po spełnieniu pewnych warunków. Na przykład jeśli użytkownik jest logowania z innego kraju, znak w mogłyby być uważane za ryzykowne i użytkownik musi podać dodatkowe formy uwierzytelniania. 

Obecnie według planu bazowego zasady są następujące:
- **Wymagają MFA dla grupy Administratorzy** — wymaga wieloczynnikowe uwierzytelnianie dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.
- **Ochrona użytkownika końcowego** — wymaga wieloczynnikowe uwierzytelnianie dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne. 
- **Starsze uwierzytelnianie bloku** — starsze aplikacje klienta i niektóre nowe aplikacje nie używaj protokoły uwierzytelniania nowsze, bardziej bezpieczne. Te starsze aplikacje można ominąć zasady dostępu warunkowego i uzyskać nieautoryzowany dostęp do środowiska. Ta zasada blokuje dostęp od klientów, które nie obsługują dostępu warunkowego. 
- **Wymagają MFA zarządzania serwisem** — wymaga wieloczynnikowe uwierzytelnianie dla dostępu do narzędzi do zarządzania, w tym portalu Azure (gdzie można skonfigurować zasady według planu bazowego). 

Microsoft zaleca, aby włączyć wszystkie te zasady według planu bazowego. Po te zasady są włączone, Administratorzy i użytkownicy pojawi się monit zarejestrować Azure Multii uwierzytelniania.

Aby uzyskać więcej informacji o tych zasadach zobacz [Co to są zasady planu bazowego](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Ustawianie zasad według planu bazowego

1. Przejdź do [portalu Azure](https://portal.azure.com), a następnie przejdź do **Usługi Active Directory Azure** \> **Dostępu warunkowego**.
    
    Zasady według planu bazowego są wymienione na stronie. <br/> <br/>
    ![Strona, która wyświetla listę zasad według planu bazowego dla dostępu warunkowego.](media/baslinepolicies.png)
1. Zobacz następujące szczegółowe instrukcje dla każdej zasady:

  - [Wymagane MFA dla grupy Administratorzy](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Reequire MFA dla użytkowników](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Starsze uwierzytelnianie bloku](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Wymagane MFA zarządzania serwisem](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Można skonfigurować wiele dodatkowych polityk, takich jak wymagające aplikacje klienta zatwierdzone. Zobacz [Warunkowego dostępu do dokumentacji](https://docs.microsoft.com/azure/active-directory/conditional-access/) , aby uzyskać więcej informacji.