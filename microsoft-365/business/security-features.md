---
title: Funkcje zabezpieczeń i zgodności usługi Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Dowiedz się więcej o funkcjach zabezpieczeń, które są dostępne w p programie Microsoft 365 Business Premium, aby chronić dane na komputerach, telefonach i tabletach.
ms.openlocfilehash: d641fc66e27f3c5e0a7c8609e4fa25fac93d8561
ms.sourcegitcommit: 956176ed7c8b8427fdc655abcd1709d86da9447e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51052259"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Funkcje zabezpieczeń i zgodności usługi Microsoft 365 Business Premium

Usługa Microsoft 365 Business Premium oferuje uproszczone funkcje zabezpieczeń chroniące dane na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-admin-center-security-features"></a>Funkcje zabezpieczeń centrum administracyjnego platformy Microsoft 365

W centrum administracyjnym można zarządzać wieloma funkcjami zabezpieczeń platformy Microsoft 365 Business Premium, co zapewnia uproszczony sposób ich włączanie i wyłączanie. W centrum administracyjnym możesz wykonać następujące czynności:
  
- [Konfigurowanie ustawień zarządzania aplikacją dla urządzeń z systemem Android lub iOS.](app-protection-settings-for-android-and-ios.md) 
    
    Te ustawienia obejmują usuwanie plików z nieaktywnego urządzenia po upływie ustawionego okresu, szyfrowanie plików służbowych, wymaganie od użytkowników ustawienia numeru PIN itp.
    
- [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10.](protection-settings-for-windows-10-devices.md) 
    
    Te ustawienia można stosować do danych firmowych zarówno na urządzeniach należących do firmy, jak i na urządzeniach należących do firmy.
    
- [Konfigurowanie ustawień ochrony urządzeń dla urządzeń z systemem Windows 10.](protection-settings-for-windows-10-pcs.md) 
    
    Możesz włączyć szyfrowanie [BitLocker,](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) aby chronić dane w przypadku zgubienia lub kradzieży urządzenia, oraz włączyć [funkcję Windows Exploit Guard,](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) aby zapewnić zaawansowaną ochronę przed oprogramowaniem wymuszającym okup. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Jeśli urządzenie zostanie zgubione, skradzione lub pracownik opuści firmę, możesz zdalnie wyczyścić dane firmowe.
    
- [Zresetuj urządzenia z systemem Windows 10 do ustawień fabrycznych.](reset-devices-to-factory-settings.md) 
    
    Możesz zresetować dowolne urządzenia z systemem Windows 10, do których zastosowano ustawienia ochrony urządzeń.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Dostępne są zaawansowane funkcje usługi Microsoft 365 Business Premium, które pomagają chronić firmę przed cyberzagrożeniami i chronić poufne informacje.
  
- **[Microsoft Defender dla Office 365](../security/defender-365-security/defender-for-office-365.md)**
    
    Usługa Microsoft Defender dla usługi Office 365 pomaga chronić firmę przed zaawansowanymi atakami wyłudzającym informacji i oprogramowaniem wymuszającym okup przeznaczonymi do naruszenia informacji o pracownikach i klientach. Dostępne są następujące funkcje:
    
  - Zaawansowane skanowanie załączników i analiza wykorzystująca AI do wykrywania i odrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie łączy w wiadomości e-mail w celu sprawdzenia, czy są one częścią schematu wyłudzania informacji. Zapewnia to bezpieczny dostęp do niebezpiecznych witryn internetowych.

- **[Pełne możliwości usługi Intune w portalu Azure Portal](/mem/intune/fundamentals/what-is-intune)**
    
    Uzyskanie dostępu do centrum administracyjnego usługi Intune w portalu Azure umożliwia skonfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami MacOS, telefonami iPhone i urządzeniami z systemem Android, a także zaawansowane zarządzanie urządzeniami dla systemu Windows, które nie są dostępne za pośrednictwem centrum administracyjnego platformy Microsoft 365.
- **Taki [sam dostęp warunkowy](/azure/active-directory/conditional-access/overview) jak plan Azure AD Premium P1**


    Dostęp warunkowy pomaga chronić organizację przed ryzykiem logowania, dostępem do nieoczekiwanej sieci lub ustawień regionalnych, próbami dostępu przed ryzykowymi typami urządzeń itp. Zasady dostępu warunkowego są wymuszane po zakończeniu pierwszego uwierzytelniania i są w nim używane sygnały z pierwszego zdarzenia uwierzytelniania w celu określenia, czy próba dostępu powinna zostać zatwierdzona, odrzucona, czy też jest wymagany więcej dowodu (na przykład druga forma identyfikacji).

    Dostępne funkcje dostępu warunkowego:

    - Dostęp na podstawie nazwy użytkownika, grupy i roli
    - Program Access [oparty na aplikacji](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Dostęp na podstawie lokalizacji](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  zezwalaj na dostęp tylko z zaufanych zakresów adresów IP lub tylko z określonych krajów 
    - Wymaganie uwierzytelniania wieloskładnikowego dla dostępu
    - Blokowanie dostępu do aplikacji, które używają [starszego uwierzytelniania](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Wymaganie korzystania z ochrony [aplikacji w usłudze Intune](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Uwierzytelnianie niestandardowe, takie jak uwierzytelnianie MFA z dostawcami innych firm, na przykład DUO.
   
    Inne funkcje:
    - [Samodzielne resetowanie hasła dla](/azure/active-directory/authentication/concept-sspr-customization) hybrydowej usługi Azure AD
    
## <a name="compliance-features"></a>Funkcje zgodności

Subskrypcja usługi Microsoft 365 Business Premium zawiera funkcje, które ułatwiają zachowanie zgodności z przepisami i przepisami.

- **[Omówienie zasad ochrony przed utratą danych](../compliance/data-loss-prevention-policies.md)** (DLP). 
    
    Aby zapobiec przypadkowemu udostępnianiu informacji poza firmę, można skonfigurować zasady ochrony przed zagrożeniami, które mogą być poufne, takie jak numery kart kredytowych czy numery PESEL.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja na usługę Exchange Online Archiwum umożliwia łatwe archiwizowanie wiadomości przy użyciu ciągłej kopii zapasowej danych. Przechowuje ona wszystkie wiadomości e-mail użytkownika, w tym elementy usunięte, na wypadek, gdy będą one potrzebne później do odnajdowania lub przywrócenia. Ponadto możesz użyć różnych zasad przechowywania, aby zachować dane poczty e-mail na potrzeby sporu sądowego, zbierania elektronicznych materiałów dowodowych lub spełnienia wymagań dotyczących zgodności.
    
- **[Etykiety wrażliwości](../compliance/sensitivity-labels.md)**

   Usługa Microsoft 365 Business Premium zawiera wszystkie funkcje usługi [Azure Information Protection Plan 1.](https://go.microsoft.com/fwlink/p/?linkid=871407) W tym planie  możesz tworzyć etykiety wrażliwości, które umożliwiają kontrolowanie dostępu do informacji poufnych w wiadomościach e-mail i dokumentach, przy użyciu kontrolek, takich jak "Nie przesyłaj dalej" i "Nie kopiować". Możesz również klasyfikować informacje poufne jako "poufne" oraz określać, w jaki sposób można udostępniać sklasyfikowane informacje poza firmą i wewnątrz firmy. Szyfrowanie klasy korporacyjnej jest łatwe w obsłudze w wiadomościach e-mail i dokumentach w celu zabezpieczenia prywatnych informacji. Możesz również zainstalować dodatek klienta usługi Azure Information Protection dla aplikacji pakietu Office. Aby uzyskać więcej informacji, zobacz Ujednolicony klient etykiet usługi [Azure Information Protection.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) W przypadku etykiet wrażliwości zainstaluj **AzInfoProtection_UL.exe**.

Tymi funkcjami możesz zarządzać w Centrum &amp; zgodności zabezpieczeń i w centrum administracyjnym usługi Intune. Z czasem uproszczone kontrolki zostaną dodane do centrum administracyjnego platformy Microsoft 365.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których jest sprzedawana usługa Microsoft 365 Business Premium.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć Centrum zgodności &amp; zabezpieczeń?
  
1. [Zaloguj się do usługi Microsoft 365 Business Premium](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W lewym okienku wyszukiwania znajdź pozycję **Centra administracyjne** i rozwiń ją. 
    
    ![W lewym okienku narracji w centrum administracyjnym platformy Microsoft 365 wybierz pozycję Centra administracyjne.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz **pozycję Zgodność &amp; zabezpieczeń,** aby przejść do Centrum &amp; zgodności zabezpieczeń.
