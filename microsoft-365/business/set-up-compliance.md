---
title: Zwiększ ochronę przed zagrożeniami dla firmy Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i oznaczać poufne dane.
ms.openlocfilehash: 09619de03aafde37106fb3942890b457c488ad43
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593410"
---
# <a name="set-up-compliance-features"></a>Konfigurowanie funkcji zgodności

Firma Microsoft 365 Business jest wyposażona w funkcje chroniące dane i urządzenia oraz ułatwiające bezpieczeństwo poufnych informacji użytkownika i klientów.

## <a name="set-up-dlp-features"></a>Konfigurowanie funkcji DLP

Zobacz [Tworzenie zasad DLP z szablonu,](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) aby uzyskać przykład konfigurowania zasad chroniących przed danymi osobowymi (PII). 
  
DLP jest wyposażony w wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych. Na przykład Australia Financial Data, Canada Personal Information Act, U.S. Financial Data itd. Zobacz, [jakie szablony zasad DLP zawierają,](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) aby uzyskać pełną listę. Wszystkie te szablony można włączyć podobnie do przykładu szablonu interfejsu ii. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurowanie przechowywania wiadomości e-mail za pomocą archiwizacji online programu Exchange

 Funkcje licencji **usługi Exchange Online Archiving** pomagają zachować zgodność i standardy regulacyjne, zachowując zawartość wiadomości e-mail w celu zbierania elektronicznych materiałów dowodowych. Pomaga również zmniejszyć ryzyko, jeśli istnieje pozew, i zapewnia sposób odzyskiwania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy. Możesz użyć blokady sporów, aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować.
  
**Wstrzymanie postępowania sądowego:** Możesz zachować całą zawartość skrzynki pocztowej, w tym usunięte elementy, wstrzymując całą skrzynkę pocztową użytkownika. 
    
Aby zawiesić skrzynkę pocztową w sporze sądowym, w centrum administracyjnym:
    
1. W lewej nav przejdź do **użytkowników** \> **aktywnych użytkowników**.
    
2. Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić w sporze sądowym. W okienku użytkownika rozwiń **pozycję Ustawienia poczty,** a następnie pozycję **Więcej ustawień**wybierz pozycję Edytuj właściwości **programu Exchange**.
    
3. Na stronie skrzynki pocztowej użytkownika wybierz ** funkcje skrzynki pocztowej ** po lewej stronie naw, a następnie wybierz łącze **Włącz** w obszarze **Wstrzymaj postępowanie sądowe**.
    
4. W oknie dialogowym **wstrzymanie sporu** można określić czas trwania blokady sporu w polu Czas **trwania blokady sporu.** Pozostaw pole puste, jeśli chcesz umieścić nieskończone przytrzymanie. Możesz również dodawać notatki i kierować właściciela skrzynki pocztowej do witryny sieci Web, którą może być trudniej wyjaśnić na temat blokady sporów. \>**Zapisz**.
    
**Retencja:** Można włączyć dostosowane zasady przechowywania, na przykład, aby zachować przez określony czas lub trwale usunąć zawartość na koniec okresu przechowywania. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Konfigurowanie etykiet czułości

Etykiety czułości są wyposażone w plan 1 usługi Azure Information Protection (AIP) i pomagają klasyfikować i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety. Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, w której użytkownicy otrzymują rekomendacje.

Aby skonfigurować etykiety czułości, [wyświetlaj tworzenie i zarządzanie klipem wideo etykiet czułości.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Ręczne instalowanie klienta usługi Azure Information Protection

Aby ręcznie zainstalować klienta AIP:

1. Pobierz **AzinfoProtection_UL.exe** z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Instalację można sprawdzić, czy instalacja działała, wyświetlając dokument programu Word i upewniając się, że opcja **Czułość** jest dostępna na karcie **Narzędzia główne.**
<br/>![Rozwijanie listy rozwijanej karty Ochrona w dokumencie programu Word.](media/word-sensitivity.png)

Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
