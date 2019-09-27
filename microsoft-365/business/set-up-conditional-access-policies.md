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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
description: Dowiedz się, jak skonfigurować zasady dostępu warunkowego dla kampanii firmy Microsoft 365.
ms.openlocfilehash: dbb5231032d2faef0a7ecb2734226b34290c70bf
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288620"
---
# <a name="set-up-conditional-access-policies"></a>Konfigurowanie zasad dostępu warunkowego

Zasady [dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodają substancjalne dodatkowe zabezpieczenia. Firma Microsoft udostępnia zestaw podstawowych zasad dostępu warunkowego, które są zalecane dla wszystkich klientów. Zasady bazowe to zestaw wstępnie zdefiniowanych zasad, które ułatwiają ochronę organizacji przed wieloma powszechną atakami. Te typowe ataki mogą zawierać spray do haseł, powtórki i phishing.

Te zasady wymagają, aby administratorzy i użytkownicy wprowadzali drugą formę uwierzytelniania (nazywanych uwierzytelnianiem wieloczynnikowym lub MFA) po spełnieniu określonych warunków. Na przykład jeśli użytkownik jest logowanie z innego kraju, logowanie może być uważane za ryzykowne i użytkownik musi podać dodatkową formę uwierzytelniania. 

Obecnie zasady bazowe są następujące:
- **Wymagaj MFA dla administratorów** — wymaga uwierzytelniania wieloskładnikowego dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.
- **Ochrona użytkownika końcowego** — wymaga uwierzytelniania wieloskładnikowego dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne. 
- **Blokowanie starszego uwierzytelniania** — starsze aplikacje klienckie i niektóre nowe aplikacje nie korzystają z nowszych, bezpieczniejszych protokołów uwierzytelniania. Te starsze aplikacje mogą pomijać zasady dostępu warunkowego i uzyskiwać nieautoryzowany dostęp do środowiska. Ta zasada blokuje dostęp od klientów, którzy nie obsługują dostępu warunkowego. 
- Wymagaj uwierzytelniania wieloskładnikowego **dla usługi zarządzania** — wymaga Multi-Factor Authentication dostępu do narzędzi do zarządzania, w tym portalu Azure (gdzie można skonfigurować zasady linii bazowej). 

Firma Microsoft zaleca włączenie wszystkich tych zasad linii bazowej. Po włączeniu tych zasad Administratorzy i użytkownicy będą monitowani o zarejestrowanie się w usłudze Azure Multii-Factor Authentication.

Aby uzyskać więcej informacji na temat tych zasad, zobacz [co to są zasady linii bazowej](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Konfigurowanie zasad bazowych

1. Przejdź do [witryny Azure Portal](https://portal.azure.com), a następnie przejdź do **usługi Azure Active Directory** \> **dostępu warunkowego**.
    
    Zasady linii bazowej są wyświetlane na stronie. <br/> <br/>
    ![Strona, która zawiera listę zasad bazowych dla dostępu warunkowego.](media/baslinepolicies.png)
1. Zapoznaj się z poniższymi szczegółowymi instrukcjami dotyczącymi poszczególnych zasad:

  - [Wymagaj uwierzytelniania MFA dla administratorów](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Wymagaj uwierzytelniania wieloskładnikowego dla użytkowników](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokowanie starszego uwierzytelniania](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Wymagaj uwierzytelniania MFA do zarządzania usługami](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Można skonfigurować wiele dodatkowych zasad, takich jak wymaganie zatwierdzonych aplikacji klienckich. Zobacz [dokumentację dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/) Aby uzyskać więcej informacji.