---
title: Microsoft 365 Business Premium funkcji zabezpieczeń i zgodności
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Dowiedz się więcej o funkcjach zabezpieczeń, które są dostępne w p Microsoft 365 Business Premium zabezpieczania danych na komputerach, telefonach i tabletach.
ms.openlocfilehash: 50b74ed18d641e8de38db3284c3ef3abf319825f4f7dbe02b6575f6c0fbc6f85
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53887583"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium funkcji zabezpieczeń i zgodności

Microsoft 365 Business Premium oferuje uproszczone funkcje zabezpieczeń chroniące dane na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-admin-center-security-features"></a>centrum administracyjne platformy Microsoft 365 funkcje zabezpieczeń

W centrum administracyjnym można zarządzać wieloma Microsoft 365 Business Premium zabezpieczeń, co zapewnia uproszczony sposób ich włączanie i wyłączanie. W centrum administracyjnym możesz wykonać następujące czynności:
  
- [Konfigurowanie ustawień zarządzania aplikacją dla urządzeń z systemem Android lub iOS.](app-protection-settings-for-android-and-ios.md) 
    
    Te ustawienia obejmują usuwanie plików z nieaktywnego urządzenia po upływie ustawionego okresu, szyfrowanie plików służbowych, wymaganie od użytkowników ustawienia numeru PIN itp.
    
- [Konfigurowanie ustawień ochrony aplikacji dla Windows 10 urządzeniach](protection-settings-for-windows-10-devices.md) . 
    
    Te ustawienia można stosować do danych firmowych zarówno na urządzeniach należących do firmy, jak i na urządzeniach należących do firmy.
    
- [Skonfiguruj ustawienia ochrony urządzeń dla Windows 10 urządzeniach.](protection-settings-for-windows-10-pcs.md) 
    
    Możesz włączyć szyfrowanie [BitLocker,](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) aby chronić dane w przypadku zgubienia lub kradzieży urządzenia, oraz włączyć funkcję [Windows Exploit Guard,](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) aby zapewnić zaawansowaną ochronę przed oprogramowaniem wymuszającym okup. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Jeśli urządzenie zostanie zgubione, skradzione lub pracownik opuści firmę, możesz zdalnie wyczyścić dane firmowe.
    
- [Zresetuj Windows 10, aby przywrócić ich ustawienia fabryczne.](reset-devices-to-factory-settings.md) 
    
    Możesz zresetować wszystkie Windows 10 urządzenia, do których zastosowano ustawienia ochrony urządzeń.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Dostępne są zaawansowane funkcje Microsoft 365 Business Premium, które pomagają chronić firmę przed cyberzagrożeniami i chronić poufne informacje.
  
- **[Program Microsoft Defender dla Office 365](../security/office-365-security/defender-for-office-365.md)**
    
    Usługa Microsoft Defender dla Office 365 chroni firmę przed zaawansowanymi atakami wyłudzania informacji i oprogramowania wymuszającego okup przeznaczonymi do naruszenia informacji o pracownikach i klientach. Dostępne są następujące funkcje:
    
  - Zaawansowane skanowanie załączników i analiza wykorzystująca AI do wykrywania i odrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie łączy w wiadomości e-mail w celu sprawdzenia, czy są one częścią schematu wyłudzania informacji. Zapewnia to bezpieczny dostęp do niebezpiecznych witryn internetowych.

- **[Pełne możliwości usługi Intune w portalu Azure Portal](/mem/intune/fundamentals/what-is-intune)**
    
    Dostęp do centrum administracyjnego usługi Intune w portalu Azure umożliwia skonfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami MacOS, iPhone i Android, oraz zaawansowane zarządzanie urządzeniami dla systemu Windows, które nie są dostępne za pośrednictwem usługi centrum administracyjne platformy Microsoft 365.
- **Taki [sam dostęp warunkowy,](/azure/active-directory/conditional-access/overview) jak Azure AD — wersja Premium P1 dostępu**


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

Subskrypcja Microsoft 365 Business Premium zawiera funkcje, które pomagają w utrzymaniu standardów zgodności z przepisami i przepisów prawa.

- **[Informacje na temat ochrony przed utratą danych)](../compliance/dlp-learn-about-dlp.md)** (DLP). 
    
    Aby zapobiec przypadkowemu udostępnianiu informacji poza firmę, można skonfigurować zasady ochrony przed zagrożeniami, które mogą być poufne, takie jak numery kart kredytowych czy numery PESEL.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online — archiwum umożliwia łatwe archiwizowanie wiadomości przy użyciu ciągłej kopii zapasowej danych. Przechowuje ona wszystkie wiadomości e-mail użytkownika, w tym elementy usunięte, na wypadek, gdy będą one potrzebne później do odnajdowania lub przywrócenia. Ponadto możesz użyć różnych zasad przechowywania, aby zachować dane poczty e-mail na potrzeby sporu sądowego, zbierania elektronicznych materiałów dowodowych lub spełnienia wymagań dotyczących zgodności.
    
- **[Etykiety wrażliwości](../compliance/sensitivity-labels.md)**

   Microsoft 365 Business Premium zawiera wszystkie funkcje usługi [Azure Information Protection Plan 1.](https://go.microsoft.com/fwlink/p/?linkid=871407) W tym planie  możesz tworzyć etykiety wrażliwości, które umożliwiają kontrolowanie dostępu do informacji poufnych w wiadomościach e-mail i dokumentach, przy użyciu kontrolek, takich jak "Nie przesyłaj dalej" i "Nie kopiować". Możesz również klasyfikować informacje poufne jako "poufne" oraz określać, w jaki sposób można udostępniać sklasyfikowane informacje poza firmą i wewnątrz firmy. Enterprise e-mail i dokumentów klasy korporacyjnej można łatwo stosować do wiadomości e-mail i dokumentów, aby zachować prywatne informacje. Możesz również zainstalować dodatek klienta usługi Azure Information Protection dla Office aplikacji. Aby uzyskać więcej informacji, zobacz Ujednolicony klient etykiet usługi [Azure Information Protection.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) W przypadku etykiet wrażliwości zainstaluj **AzInfoProtection_UL.exe**.

Tymi funkcjami możesz zarządzać w Centrum &amp; zgodności zabezpieczeń i w centrum administracyjnym usługi Intune. Z czasem uproszczone kontrolki zostaną dodane do centrum administracyjne platformy Microsoft 365.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których Microsoft 365 Business Premium są sprzedawane.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć Centrum zgodności &amp; zabezpieczeń?
  
1. [Zaloguj się Microsoft 365 Business Premium](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W lewym okienku wyszukiwania znajdź pozycję **Centra administracyjne** i rozwiń ją. 
    
    ![W lewym okienku narracji w centrum administracyjne platformy Microsoft 365 wybierz pozycję Centra administracyjne.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz **pozycję Zgodność &amp; zabezpieczeń,** aby przejść do Centrum &amp; zgodności zabezpieczeń.
