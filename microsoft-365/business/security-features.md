---
title: Funkcje zabezpieczeń i zgodności programu Microsoft 365 Business Premium
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
description: Dowiedz się więcej o funkcjach zabezpieczeń dostępnych w systemie Microsoft 365 Business Premium, które pomagają chronić dane na komputerach, telefonach i tabletach.
ms.openlocfilehash: 587d80c27f867a387c901d23f4ec05f3c5905bf6
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48843493"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Funkcje zabezpieczeń i zgodności programu Microsoft 365 Business Premium

Program Microsoft 365 Business Premium oferuje uproszczone funkcje zabezpieczeń, które pomagają chronić dane na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-admin-center-security-features"></a>Funkcje zabezpieczeń centrum administracyjnego programu Microsoft 365

W centrum administracyjnym można zarządzać wieloma funkcjami zabezpieczeń programu Microsoft 365 Business Premium, co zapewnia uproszczony sposób włączania i wyłączania tych funkcji. W centrum administracyjnym możesz wykonać następujące czynności:
  
- [Ustawianie ustawień zarządzania aplikacjami dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Te ustawienia obejmują usuwanie plików z nieaktywnego urządzenia po określonym okresie, szyfrowanie plików służbowych wymagające użytkownikom ustawienia numeru PIN itd.
    
- [Ustawianie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Te ustawienia mogą być stosowane do danych firmowych zarówno na urządzeniach należących do firmy, jak i osobistych.
    
- [Ustawianie ustawień ochrony urządzeń dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Szyfrowanie [funkcji BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) można włączyć, aby chronić dane na wypadek, gdyby urządzenie zostało zgubione lub skradzione, i włączyć funkcję [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) , aby zapewnić zaawansowaną ochronę przed używaniem oprogramowania wymuszającego okup. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Możesz zdalnie wyczyścić dane firmy, jeśli urządzenie zostanie zgubione, skradzione lub pozostawiono firmie.
    
- [Przywróć ustawienia fabryczne urządzeń z systemem Windows 10](reset-devices-to-factory-settings.md) . 
    
    Możesz zresetować wszystkie urządzenia z systemem Windows 10, do których zastosowano ustawienia ochrony urządzeń.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

W programie Microsoft 365 Business Premium udostępniono zaawansowane funkcje ułatwiające ochronę firmy przed zagrożeniami związanymi z Cyber i ochroną poufnych informacji.
  
- **[Microsoft Defender dla Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Program Microsoft Defender dla Office 365 ułatwia ochronę Twojej firmy przed wyrafinowanymi atakami wyłudzania informacji i oprogramowania wymuszającego okup, mającymi na celu złamanie informacji o pracownikach lub klientach. Funkcje obejmują:
    
  - Zaawansowanego skanowania załączników i analizy z obsługą AI do wykrywania i odrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie łączy w wiadomości e-mail w celu oceny, czy są one częścią procedury wyłudzania informacji. Dzięki temu można bezpiecznie uzyskiwać dostęp do niebezpiecznych witryn internetowych.

- **[Pełne funkcje usługi Intune w portalu Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Uzyskiwanie dostępu do centrum administracyjnego usługi Intune w portalu Azure umożliwia konfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami MacOS, iPhone i urządzeniami z systemem Android oraz zaawansowane zarządzanie urządzeniami z systemem Windows, które nie są dostępne za pośrednictwem Centrum administracyjnego usługi Microsoft 365.
- **Taki sam [dostęp warunkowy](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) jak plan usługi Azure AD Premium w wersji P1**


    Dostęp warunkowy ułatwia ochronę organizacji przed ryzykiem logowania, próbuje uzyskać dostęp do nieoczekiwanych sieci lub ustawień regionalnych, próbuje uzyskać dostęp do różnych typów urządzeń z czynnikami ryzyka itd. Zasady dostępu warunkowego są wymuszane po zakończeniu pierwszego uwierzytelniania, a w celu określenia, czy próba uzyskania dostępu powinna zostać zatwierdzona, odrzucona lub jeśli jest wymagany (na przykład druga forma identyfikacji), są używane sygnały z pierwszego zdarzenia uwierzytelniania.

    Uwzględnione funkcje dostępu warunkowego są następujące:

    - Dostęp na podstawie nazwy użytkownika, grupy i roli
    - Dostęp [na podstawie aplikacji](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Dostęp na podstawie lokalizacji](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Zezwalaj na dostęp tylko z zaufanych zakresów IP lub określonych krajów 
    - Wymagaj uwierzytelniania wieloskładnikowego w programie Access
    - Blokowanie dostępu do aplikacji korzystających ze [starszych wersji uwierzytelniania](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Wymagaj aplikacji TP Użyj usługi [Intune App Protection](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Niestandardowe uwierzytelnianie, takie jak MFA z dostawcami innych firm, na przykład DUO.
   
    Inne funkcje:
    - Samoobsługowe [Resetowanie hasła](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) dla hybrydowej usługi Azure AD
    
## <a name="compliance-features"></a>Funkcje zgodności

Abonament Microsoft 365 Business Premium zawiera funkcje, które ułatwiają zachowanie zgodności i standardów wykonawczych.

- **[Omówienie zasad ochrony przed utratą danych](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (DLP). 
    
    Ustawienia DLP można skonfigurować w celu automatycznego wykrywania poufnych informacji, takich jak numery kart kredytowych, numerów PESEL i tak dalej, aby zapobiec przypadkowemu udostępnieniu poza firmą.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja archiwizowania usługi Exchange Online umożliwia łatwe archiwizowanie wiadomości za pomocą ciągłej kopii zapasowej danych. Umożliwia przechowywanie wszystkich wiadomości e-mail użytkownika, w tym elementów usuniętych, na wypadek, gdyby były one wymagane później do odnalezienia lub przywrócenia. Ponadto można korzystać z różnych zasad przechowywania w celu zachowania danych wiadomości e-mail dotyczących czynności sądowych, zbierania elektronicznych materiałów dowodowych lub spełniania wymagań dotyczących zgodności.
    
- **[Etykiety wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Pakiet Microsoft 365 Business Premium zawiera wszystkie funkcje [usługi Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Dzięki temu planowi można tworzyć **etykiety czułe** , które umożliwiają kontrolowanie dostępu do poufnych informacji w wiadomościach e-mail i dokumentach za pomocą formantów, takich jak "nie przesyłaj dalej" i "nie Kopiuj". Informacje poufne można także sklasyfikować jako "poufne" i określić sposób udostępniania informacji klasyfikowanych na zewnątrz i w firmie. W przypadku firm szyfrowanie jest łatwe w obsłudze w wiadomościach e-mail i dokumentach, aby zapewnić prywatność informacji. Możesz również zainstalować dodatek klienta usługi Azure Information Protection dla pakietu Office. Aby uzyskać więcej informacji, zobacz [Klient usługi Azure Information Protection Unified etykietowanie klientów](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Aby uzyskać etykiety wrażliwości, zainstaluj **AzInfoProtection_UL.exe**.

Tymi funkcjami można zarządzać w &amp; Centrum zgodności z zabezpieczeniami oraz w centrum administracyjnym usługi Intune. W czasie, gdy uproszczone kontrolki zostaną dodane do centrum administracyjnego usługi Microsoft 365.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których jest sprzedawany program Microsoft 365 Business Premium.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć &amp; Centrum zgodności zabezpieczeń?
  
1. [Zaloguj się do aplikacji Microsoft 365 Business Premium](https://portal.microsoft.com/) , korzystając z poświadczeń administratora. 
    
2. W lewym okienku nawigacji znajdź pozycję **centra administracyjne** i rozwiń ją. 
    
    ![W lewym obszarze nawigacyjnym w centrum administracyjnym usługi Microsoft 365 wybierz pozycję centra administracyjne.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz **pozycję &amp; zgodność zabezpieczeń** , aby przejść do &amp; Centrum zgodności z zabezpieczeniami.
