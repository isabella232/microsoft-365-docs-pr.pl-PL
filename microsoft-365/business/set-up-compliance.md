---
title: Zwiększenie ochrony przed zagrożeniami dla usługi Microsoft 365 Business
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i zapewnić bezpieczeństwo poufnych informacji użytkownika i klientów.
ms.openlocfilehash: 4c8efc4ca96f2db7bc4d1592ad3fdc85dfb6b3b5
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550062"
---
# <a name="set-up-compliance-features"></a>Konfigurowanie funkcji zgodności

Twój microsoft 365 Business jest wyposażony w funkcje ochrony danych i urządzeń oraz pomagają chronić poufne informacje i klientów.

## <a name="set-up-dlp-features"></a>Konfigurowanie funkcji DLP

Zobacz [Tworzenie zasad DLP na podstawie szablonu,](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) aby na przykład jak skonfigurować zasady w celu ochrony przed danymi osobowymi (PI). 
  
DLP jest wyposażony w wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych. Na przykład Australia Financial Data, Canada Personal Information Act, U.S. Financial Data itd. Zobacz [Co szablony zasad DLP zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pełną listę. Wszystkie te szablony można włączyć podobnie do przykładu szablonu pii. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurowanie przechowywania poczty e-mail za pomocą usługi Exchange Online Archiving

 Funkcje licencji **na archiwizacje w usłudze Exchange Online** pomagają zachować standardy zgodności i standardy regulacyjne, zachowując zawartość wiadomości e-mail do zbierania elektronicznych materiałów dowodowych. Pomaga również zmniejszyć ryzyko, jeśli istnieje pozew i zapewnia sposób odzyskiwania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy. Można użyć blokady sporów sądowych, aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować.
  
**Blokada postępowania sądowego:** Można zachować całą zawartość skrzynki pocztowej, w tym usunięte elementy, umieszczając całą skrzynkę pocztową użytkownika w sporze sądowym. 
    
Aby zawiesić skrzynkę pocztową w postępowaniu sądowym, w Centrum administracyjnym:
    
1. W lewym nav przejdź do **użytkowników** \> **aktywnych użytkowników**.
    
2. Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić w zawieszeniu w postępowaniu sądowym. W okienku użytkownika rozwiń **pozycję Ustawienia poczty**, a obok pozycji Więcej **ustawień**wybierz pozycję Edytuj właściwości **programu Exchange**.
    
3. Na stronie skrzynki pocztowej użytkownika wybierz ** funkcje skrzynki pocztowej ** na lewym nawigacie, a następnie wybierz łącze **Włącz** w **obszarze Wstrzymywanie sporów**.
    
4. W oknie dialogowym **wstrzymania postępowania sądowego** można określić czas trwania wstrzymania postępowania sądowego w polu **Czas trwania wstrzymania postępowania sądowego.** Pozostaw puste pole, jeśli chcesz umieścić nieskończone przytrzymanie. Możesz również dodać notatki i skierować właściciela skrzynki pocztowej do witryny sieci Web, którą możesz wyjaśnić więcej na temat blokady postępowania sądowego. \>**Zapisz**.
    
**Retencja:** Można włączyć dostosowane zasady przechowywania, na przykład, aby zachować przez określony czas lub trwale usunąć zawartość na koniec okresu przechowywania. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Konfigurowanie etykiet czułości

Etykiety czułości są wyposażone w plan 1 usługi Azure Information Protection (AIP) i ułatwiają klasyfikowanie i opcjonalnie ochronę dokumentów i wiadomości e-mail, stosując etykiety. Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, w której użytkownicy otrzymują rekomendacje.

Aby skonfigurować etykiety czułości, wyświetl [klip wideo tworzenie etykiet czułości i zarządzanie nimi.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Ręczne instalowanie klienta usługi Azure Information Protection

Aby ręcznie zainstalować klienta AIP:

1. Pobierz **AzinfoProtection_UL.exe** z [centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Można sprawdzić, czy instalacja działała, wyświetlając dokument programu Word i upewniając się, że opcja **Czułość** jest dostępna na karcie **Narzędzia główne.**
<br/>![Z listy rozwijanej Karta ochrony w dokumencie programu Word.](../media/word-sensitivity.png)

Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
