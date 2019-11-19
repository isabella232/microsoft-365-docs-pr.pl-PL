---
title: Zwiększ ochronę przed zagrożeniami dla Microsoft 365 Business
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
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i etykietach poufnych danych.
ms.openlocfilehash: 6fae95e8c5e6d133e3163dbdfd3c09cfede11382
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715127"
---
# <a name="set-up-compliance-features"></a>Konfigurowanie funkcji zgodności

Twoja firma Microsoft 365 Business zawiera funkcje chroniące dane i urządzenia oraz pomagające w zabezpieczeniu poufnych informacji Twoich i Twoich klientów.

## <a name="set-up-dlp-features"></a>Konfigurowanie funkcji DLP

Zobacz [Tworzenie zasad DLP z szablonu](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) , aby zapoznać się z przykładem sposobu konfigurowania zasad w celu ochrony przed danymi osobowymi (PII). 
  
DLP zawiera wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych. Na przykład australijskie dane finansowe, kanadyjska ustawa o danych osobowych, dane finansowe Stanów Zjednoczonych itd. Zobacz [, jakie szablony zasad DLP zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pełną listę. Wszystkie te szablony można włączyć podobne do przykładu szablonu PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurowanie przechowywania poczty e-mail przy użyciu usługi Exchange Online archiwizacji

 Funkcje **programu Exchange Online archiwizowanie** licencji ułatwiają zachowanie zgodności i standardów regulacyjnych przez zachowanie zawartości poczty elektronicznej na potrzeby zbierania elektronicznych materiałów dowodowych. Pomaga również zmniejszyć ryzyko, jeśli jest pozew, i zapewnia sposób na odzyskanie danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy. Aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować, możesz użyć wstrzymania w postępowaniu sądowym.
  
**Sądowym:** Możesz zachować całą zawartość skrzynki pocztowej, w tym elementy usunięte, umieszczając całą skrzynkę pocztową użytkownika w postępowaniu sądowym. 
    
Aby umieścić skrzynkę pocztową w postępowaniu sądowym, w centrum administracyjnym:
    
1. W lewym NAV przejdź do **użytkowników** \> **aktywnych**użytkowników.
    
2. Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić w postępowaniu sądowym. W okienku użytkownika rozwiń **Ustawienia poczty**, a obok **więcej ustawień**wybierz **Edytuj właściwości programu Exchange**.
    
3. Na stronie skrzynki pocztowej dla użytkownika wybierz * * funkcje skrzynki pocztowej * * na lewej NAV, a następnie wybierz **Włącz** łącze w związku z **postępowaniem sądowym**.
    
4. W oknie dialogowym **wstrzymanie** w trakcie postępowania sądowego można określić czas trwania wstrzymania w **czasie trwania** postępowania sądowego. Pozostaw pole puste, jeśli chcesz umieścić nieskończoną zawieszone. Można również dodawać notatki i kierować właściciela skrzynki pocztowej do witryny sieci Web może być trzeba wyjaśnić więcej na temat wstrzymania postępowania sądowego. \>**Zapisać**.
    
**Zatrzymanie:** Można włączyć niestandardowe zasady przechowywania, na przykład, aby zachować określoną ilość czasu lub trwale usunąć zawartość na końcu okresu przechowywania. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Ustawianie etykiet czułości

Etykiety czułości pochodzą z planu 1 usługi Azure Information Protection (AIP) i ułatwiają klasyfikować i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety. Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub przy użyciu kombinacji, gdzie użytkownicy są podane zalecenia.

Aby skonfigurować etykiety czułości, zobacz [Tworzenie i zarządzanie etykietami czułości](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) wideo.



### <a name="install-the-azure-information-protection-client-manually"></a>Ręczne instalowanie klienta usługi Azure Information Protection

Aby ręcznie zainstalować klienta AIP:

1. Pobierz **AzinfoProtection_UL. exe** z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Można sprawdzić, czy instalacja zadziałało, przeglądając dokument programu Word i upewniając się, że opcja **czułość** jest dostępna na karcie **Narzędzia główne** .
<br/>![Karta ochrona listy rozwijanej w dokumencie programu Word.](media/word-sensitivity.png)

Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
