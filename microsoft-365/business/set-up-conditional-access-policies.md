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
# <a name="set-up-conditional-access-policies"></a>Konfigurowanie zasad dostępu warunkowego

[Zasady dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodać znaczne dodatkowe zabezpieczenia. Firma Microsoft udostępnia zestaw podstawowych zasad dostępu warunkowego, które są zalecane dla wszystkich klientów. Zasady bazowe to zestaw wstępnie zdefiniowanych zasad, które pomagają chronić organizacje przed wieloma typowymi atakami. Te typowe ataki mogą obejmować rozpylanie haseł, powtórkę i wyłudzanie informacji.

Te zasady wymagają, aby administratorzy i użytkownicy włączyli drugą formę uwierzytelniania (nazywane uwierzytelnianiem wieloskładnikowym lub uwierzytelnianiem wieloskładnikowym), gdy spełnione są określone warunki. Na przykład jeśli użytkownik loguje się z innego kraju, logowanie może być uznane za ryzykowne, a użytkownik musi podać dodatkową formę uwierzytelniania. 

Obecnie zasady bazowe obejmują następujące zasady:
- **Wymagaj uwierzytelniania mfa dla administratorów** &ndash; Wymaga uwierzytelniania wieloskładnikowego dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.
- **Ochrona** &ndash; użytkowników końcowych Wymaga uwierzytelniania wieloskładnikowego dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne. 
- **Blokuj starsze uwierzytelnianie** &ndash; Starsze aplikacje klienckie i niektóre nowe aplikacje nie używają nowszych, bezpieczniejszych protokołów uwierzytelniania. Te starsze aplikacje mogą ominąć zasady dostępu warunkowego i uzyskać nieautoryzowany dostęp do środowiska. Ta zasada blokuje dostęp od klientów, którzy nie obsługują dostępu warunkowego. 
- **Wymagaj uwierzytelniania mfa dla zarządzania usługami** &ndash; Wymaga uwierzytelniania wieloskładnikowego w celu uzyskania dostępu do narzędzi zarządzania, w tym do witryny Azure portal (w którym można skonfigurować zasady według planu bazowego). 

Firma Microsoft zaleca włączenie wszystkich tych zasad bazowych. Po włączeniu tych zasad administratorzy i użytkownicy zostaną poproszeni o zarejestrowanie się w celu uwierzytelniania multii-factor platformy Azure.

Aby uzyskać więcej informacji na temat tych zasad, zobacz [Co to są zasady bazowe?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Konfigurowanie zasad linii bazowej

1. Przejdź do [witryny Azure portal](https://portal.azure.com), a następnie przejdź do usługi Azure Active **Directory** \> **dostęp warunkowy**.
    
    Zasady bazowe są wymienione na stronie. <br/> <br/>
    ![Strona zawierająca listę zasad bazowych dostępu warunkowego.](../media/baslinepolicies.png)
1. Zapoznaj się z poniższymi szczegółowymi instrukcjami dotyczącymi poszczególnych zasad:

  - [Wymaganie usługi MFA dla administratorów](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Wymagaj usługi MFA dla użytkowników](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokowanie uwierzytelniania starszego](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Wymaganie usługi MFA do zarządzania usługami](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Można skonfigurować wiele dodatkowych zasad, takich jak wymaganie zatwierdzonych aplikacji klienckich. Aby uzyskać więcej informacji, zobacz [dokumentację dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/).
