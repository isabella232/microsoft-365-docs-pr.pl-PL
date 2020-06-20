---
title: Zwiększenie ochrony przed zagrożeniami dla usługi Microsoft 365 Business Premium
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i zapewnić bezpieczeństwo poufnych informacji twoich i klientów.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785837"
---
# <a name="set-up-compliance-features"></a>Konfigurowanie funkcji zgodności

Usługa Microsoft 365 Business Premium jest wyposażona w funkcje ochrony danych i urządzeń oraz pomagają chronić poufne informacje użytkownika i klientów.

## <a name="set-up-dlp-features"></a>Konfigurowanie funkcji DLP

Zobacz [Tworzenie zasad DLP na podstawie szablonu,](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) aby uzyskać przykład na temat konfigurowania zasad w celu ochrony przed danymi umożliwiającymi identyfikację użytkownika. 
  
DLP jest wyposażony w wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych. Na przykład Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, itd. Zobacz, [co zawierają szablony zasad DLP,](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) aby uzyskać pełną listę. Wszystkie te szablony można włączyć podobnie jak przykład szablonu pii. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurowanie przechowywania poczty e-mail za pomocą archiwizacji usługi Exchange Online

 Funkcje licencji **Exchange Online Archiving** pomagają utrzymać zgodność i standardy regulacyjne, zachowując zawartość wiadomości e-mail do elektronicznego zbierania elektronicznych materiałów dowodowych. Pomaga również zmniejszyć ryzyko, jeśli istnieje pozew, i zapewnia sposób odzyskiwania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy. Za pomocą blokady postępowania sądowego można zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować.
  
**Wstrzymanie postępowania sądowego:** Można zachować całą zawartość skrzynki pocztowej, w tym usunięte elementy, umieszczając całą skrzynkę pocztową użytkownika w zawieszeniu w postępowaniu sądowym. 
    
Aby zawiesić skrzynkę pocztową w postępowaniu sądowym, w Centrum administracyjnym:
    
1. W lewej stronie nawigacyjnej przejdź do **strony Użytkownicy** \> **aktywni użytkownicy**.
    
2. Wybierz użytkownika, którego skrzynkę pocztową chcesz zawiesić w postępowaniu sądowym. W okienku użytkownika rozwiń pozycję **Ustawienia poczty**, a obok pozycji **Więcej ustawień**wybierz pozycję Edytuj właściwości **programu Exchange**.
    
3. Na stronie skrzynki pocztowej dla użytkownika wybierz ** funkcje skrzynki pocztowej ** na lewym polu nawigacyjnym, a następnie wybierz **łącze Włącz** w obszarze **Wstrzymanie postępowania sądowego**.
    
4. W oknie dialogowym **wstrzymanie postępowania sądowego** można określić czas trwania wstrzymania postępowania sądowego w polu **Czas trwania wstrzymania postępowania sądowego.** Pozostaw pole puste, jeśli chcesz umieścić nieskończone przytrzymanie. Możesz również dodać notatki i skierować właściciela skrzynki pocztowej do witryny sieci Web, która może być bardziej wyjaśniona na temat wstrzymania postępowania sądowego. \>**Zapisz**.
    
**Retencja:** Można włączyć dostosowane zasady przechowywania, na przykład, aby zachować przez określony czas lub usunąć zawartość trwale na koniec okresu przechowywania. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Konfigurowanie etykiet czułości

Etykiety czułości są wyposażone w plan 1 usługi Azure Information Protection (AIP) i ułatwiają klasyfikowanie i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety. Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki ręcznie przez użytkowników lub przy użyciu kombinacji, w której użytkownicy otrzymują rekomendacje.

Aby skonfigurować etykiety czułości, wyświetl [wideo tworzenie etykiet czułości i zarządzanie nimi.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Ręczne instalowanie klienta usługi Azure Information Protection

Aby ręcznie zainstalować klienta AIP:

1. Pobierz **AzinfoProtection_UL.exe** z [centrum pobierania Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Można sprawdzić, czy instalacja zadziałała, przeglądając dokument programu Word i upewniając się, że opcja **Czułość** jest dostępna na karcie **Narzędzia** główne.
<br/>![Karta Ochrony rozwijana w dokumencie programu Word.](../media/word-sensitivity.png)

Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
