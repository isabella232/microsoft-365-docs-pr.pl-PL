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
search.appverid:
- BCS160
- MET150
- MOE150
description: Dowiedz się, jak skonfigurować zasady dostępu warunkowego dla kampanii programu Microsoft 365.
ms.openlocfilehash: 1ef90bd77da43ded624d85cef9c7a33beec74345
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064620"
---
# <a name="set-up-conditional-access-policies"></a>Konfigurowanie zasad dostępu warunkowego

Zasady [dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dodają znaczne dodatkowe zabezpieczenia. Firma Microsoft udostępnia zestaw podstawowych zasad dostępu warunkowego, które są zalecane dla wszystkich klientów. Zasady linii bazowej to zestaw wstępnie zdefiniowanych zasad, które pomagają chronić organizacje przed wieloma typowymi atakami. Te typowe ataki mogą obejmować rozpylanie haseł, powtórki i wyłudzanie informacji.

Zasady te wymagają od administratorów i użytkowników wprowadzenia drugiej formy uwierzytelniania (nazywanej uwierzytelnianiem wieloskładnikowym lub protokołem MFA) po spełnieniu określonych warunków. Na przykład jeśli użytkownik loguje się z innego kraju, logowanie może być uznane za ryzykowne, a użytkownik musi podać dodatkową formę uwierzytelniania. 

Obecnie zasady linii bazowej obejmują następujące elementy:
- **Wymagaj usługi MFA dla administratorów** &ndash; Wymaga uwierzytelniania wieloskładnikowego dla najbardziej uprzywilejowanych ról administratora, w tym administratora globalnego.
- **Ochrona** &ndash; użytkownika końcowego Wymaga uwierzytelniania wieloskładnikowego dla użytkowników tylko wtedy, gdy logowanie jest ryzykowne. 
- **Blokuj starsze uwierzytelnianie** &ndash; Starsze aplikacje klienckie, a niektóre nowe aplikacje nie używają nowszych, bezpieczniejszych protokołów uwierzytelniania. Te starsze aplikacje mogą pomijać zasady dostępu warunkowego i uzyskać nieautoryzowany dostęp do środowiska. Ta zasada blokuje dostęp od klientów, którzy nie obsługują dostępu warunkowego. 
- **Wymagaj usługi MFA do zarządzania usługami** &ndash; Wymaga uwierzytelniania wieloskładnikowego w celu uzyskania dostępu do narzędzi do zarządzania, w tym witryny Azure portal (gdzie można skonfigurować zasady linii bazowej). 

Firma Microsoft zaleca włączenie wszystkich tych zasad planu bazowego. Po włączeniu tych zasad administratorzy i użytkownicy zostaną poproszeni o zarejestrowanie się w celu uwierzytelnienia multii-factor platformy Azure.

Aby uzyskać więcej informacji na temat tych zasad, zobacz [Co to są zasady linii bazowej?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Konfigurowanie zasad planu bazowego

1. Przejdź do [witryny Azure portal](https://portal.azure.com), a następnie przejdź do witryny Azure Active **Directory** \> **dostęp warunkowy**.
    
    Zasady linii bazowej są wyświetlane na stronie. <br/> <br/>
    ![Strona zawierająca listę zasad planu bazowego dostępu warunkowego.](../media/baslinepolicies.png)
1. Zobacz następujące szczegółowe instrukcje dla każdej zasady:

  - [Wymagaj usługi MFA dla administratorów](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Wymagaj usługi MFA dla użytkowników](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokowanie uwierzytelniania starszego](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Wymagaj usługi MFA do zarządzania usługami](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Można skonfigurować wiele dodatkowych zasad, takich jak wymaganie zatwierdzonych aplikacji klienckich. Aby uzyskać więcej informacji, zobacz [dokumentację dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/).
