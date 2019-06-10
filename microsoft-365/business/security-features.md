---
title: Funkcje bezpieczeństwa i zgodności Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Dowiedz się więcej o funkcjach zabezpieczeń, które pochodzą z Microsoft 365 Business.
ms.openlocfilehash: 54bac38ca3a60f88f848ec3ab8bdd8a7c0fabd54
ms.sourcegitcommit: ab04fea2765a63489d70b506f0e14303a5be16a0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34780784"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Funkcje bezpieczeństwa i zgodności Microsoft 365 Business

Microsoft 365 Business oferuje funkcje zabezpieczeń uproszczone do zapewnienia pomocy w ochronie danych na komputerach, telefonów i tabletek.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funkcje zabezpieczeń Centrum Microsoft 365 Business admin

![Transparent odsyłających do https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Można zarządzać wiele funkcji zabezpieczeń Microsoft 365 Business w Centrum administracyjnego, która pozwala na uproszczony sposób włączyć lub wyłączyć te funkcje. W Centrum administracyjnym można wykonać następujące czynności:
  
  
- [Ustawienia zarządzania aplikacji dla urządzeń Android lub iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Te ustawienia obejmują usunięcie plików z urządzenia nieaktywne po określonym czasie, system szyfrowania plików roboczych, wymaganie, że użytkownicy ustawić kod PIN, itp.
    
- [Ustawienia ochrony aplikacji dla urządzeń Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Te ustawienia mogą być stosowane do danych firmy na obu firmowych lub osobistymi urządzeniami.
    
- [Ustaw ustawienia ochrony urządzenia dla urządzeń Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Można włączyć szyfrowanie [funkcją BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) w celu ochrony danych w przypadku zgubienia lub kradzieży urządzenia i włączyć [Guard wykorzystać system Windows](https://go.microsoft.com/fwlink/p/?linkid=871404) zapewnia zaawansowaną ochronę przed szkodnika. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Jeśli urządzenie zostało utracone, skradzione, lub pracownik odejdzie z firmy, można zdalnie usunąć dane firmy.
    
- [Resetuj Windows 10 urządzenia do ustawień fabrycznych](reset-devices-to-factory-settings.md) . 
    
    Można zresetować urządzenia Windows 10 zawierające ustawienia ochrony urządzenia do nich stosowane.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Zaawansowane funkcje w programie Microsoft Business 365 dostępnych może pomóc chronić firmę przed zagrożeniami cyber i ochrona poufnych informacji.
  
- **[Office 365 zaawansowaną ochronę przed zagrożeniami](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Zaawansowane zagrożenia ochrony (ATP) pomaga w kompleksowej firmy przed atakami szkodnika przeznaczone do złamania pracownika lub informacji o klientach i zaawansowanych witryn wyłudzających informacje. Funkcje:
    
  - Zaawansowane analizy skanowania i zasilany AI załącznik do wykrycia i odrzucić niebezpieczne wiadomości.
    
  - Automatyczne sprawdza łącza w wiadomości e-mail do oceny, jeśli są one częścią wyłudzania informacji. To zapewnia bezpieczny dostęp do niebezpiecznych stron internetowych.

- **[W pełni możliwości Intune w portalu Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Uzyskiwanie dostępu do usługi Centrum administracyjnego w portalu Azure pozwala zdefiniować dodatkowe funkcje zabezpieczeń, takie jak zarządzanie urządzeniami MacOS, iPhone i android wraz z zaawansowane funkcje zarządzania urządzeniami w systemie Windows Intune nie są dostępne za pośrednictwem firmy Microsoft 365 Centrum admin biznesowych.
- **Sam [Dostępu warunkowego](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) , jak plan Azure AD P1**

    Dostępu warunkowego może pomóc chronić organizacji przed ryzykiem logowanie, próby dostępu z sieci nieoczekiwany lub ustawień regionalnych, prób dostępu do formularza typy urządzeń ryzykowne i tak dalej. Odmawia dostępu warunkowego, którego zasady są egzekwowane po zakończeniu pierwszego uwierzytelniania i używa sygnałów z pierwszego zdarzenia uwierzytelniania w celu określenia, jeśli prób uzyskania dostępu powinno zostać zatwierdzone, lub jest f więcej dowodów (na przykład drugi formularz identyfikacyjny) Wymagane.
    
## <a name="compliance-features"></a>Funkcje zgodności

Firmy Microsoft 365 subskrypcja zawiera funkcje ułatwiające Obsługa zgodności i normami.

- **[Omówienie zasady ochrony przed utratą danych](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    DLP można skonfigurować do automatycznego wykrywania poufnych informacji, takich jak numery kart kredytowych, numery ubezpieczenia społecznego, itp., aby uniemożliwić ich przypadkowe udostępnianie spoza firmy.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja Exchange Online — archiwum umożliwia wiadomości mają być archiwizowane łatwo z ciągłego tworzenia kopii zapasowych. Przechowuje wszystkie wiadomości e-mail użytkownika, w tym w przypadku, gdy są później potrzebne do odnajdowania lub przywrócenie usuniętych elementów. Ponadto można użyć zasad przechowywania różnych zachowanie danych poczty e-mail dla postępowania sądowego ładowni, zbierania elektronicznych materiałów dowodowych, lub zachowanie zgodności z wymaganiami.
    
- **[Ochrona informacji Azure](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Ułatwia ochronę informacji kontroli dostępu do poufnych informacji w wiadomości e-mail i dokumentów z formantów, takich jak "Nie do przodu" oraz "Nie Kopiuj." Można również sklasyfikować poufnych informacji jako "Poufne" i określić, jak informacje klasyfikowane są udostępniane poza i wewnątrz firmy. Szyfrowanie klasy korporacyjnej jest łatwy do zastosowania do poczty e-mail i dokumenty poufne informacje. Microsoft 365 Business zawiera wszystkie funkcje [Azure 1 Plan ochrony informacji](https://go.microsoft.com/fwlink/p/?linkid=871407). Można również zainstalować ochrony informacji Azure dodatek klienta dla aplikacji pakietu Office. Aby uzyskać więcej szczegółów zobacz [Podręcznik administratora programu ochrony informacji Azure klienta](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).

Te funkcje zabezpieczeń można zarządzać &amp; Centrum zgodności i Centrum administracyjnego programu Windows Intune. W czasie kontroli uproszczonej zostaną dodane do Centrum administracyjnego programu Microsoft 365 Business.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, gdzie sprzedawane Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć zabezpieczenia &amp; Centrum zgodności?
  
1. [Zaloguj się do programu Microsoft Business 365](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W nawigacji z lewej strony zlokalizuj **Admin gniazd produkcyjnych** i rozwiń ją. 
    
    ![W nawigacji w lewo w Centrum administracyjnym usługi Microsoft 365 wybierz Admin centrów.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz **zabezpieczeń &amp; zgodności** aby przejść do zabezpieczeń &amp; Centrum zgodności.