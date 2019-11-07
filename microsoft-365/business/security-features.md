---
title: Funkcje zabezpieczeń i zgodności firmy Microsoft 365 dla firm
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Dowiedz się więcej o funkcjach zabezpieczeń, które są wyposażone w Microsoft 365 Business.
ms.openlocfilehash: 5e295480b1a578ca26646a89d6a0a4183a15428d
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031450"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Funkcje zabezpieczeń i zgodności firmy Microsoft 365 dla firm

Firma Microsoft 365 Business oferuje uproszczone funkcje zabezpieczeń, które ułatwiają Zabezpieczanie danych na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funkcje zabezpieczeń Microsoft 365 Business Admin Center

[![Etykieta, aby poinformować, że centrum admin zmienia się i można znaleźć więcej szczegółów na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

W centrum administracyjnym można zarządzać wieloma funkcjami zabezpieczeń firmy Microsoft 365 Business, co pozwala na uproszczone Włączanie i wyłączanie tych funkcji. W centrum administracyjnym można wykonać następujące czynności:
  
  
- [Ustaw ustawienia zarządzania aplikacjami dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Ustawienia te obejmują usuwanie plików z nieaktywnego urządzenia po upływie ustawiowego okresu, szyfrowanie plików roboczych, wymaganie od użytkowników ustawienia kodu PIN itp.
    
- [Ustaw ustawienia ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Te ustawienia mogą być stosowane do danych firmowych na urządzeniach należących do firmy lub osobiście.
    
- [Ustaw ustawienia ochrony urządzenia dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Możesz włączyć szyfrowanie [funkcją BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) , aby chronić dane w przypadku zgubienia lub kradzieży urządzenia, a także włączyć funkcję [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) w celu zapewnienia zaawansowanej ochrony przed oprogramowaniem typu ransomware. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Można zdalnie wymazać dane firmy, jeśli urządzenie zostanie zgubione, skradzione lub pracownik opuści firmę.
    
- [Zresetuj urządzenia z systemem Windows 10 do ustawień fabrycznych](reset-devices-to-factory-settings.md) . 
    
    Można zresetować wszystkie urządzenia z systemem Windows 10, które mają zastosowane ustawienia ochrony urządzenia.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Zaawansowane funkcje firmy Microsoft 365 Business są dostępne, aby pomóc chronić firmę przed zagrożeniami cybernetycznymi i chronić poufne informacje.
  
- **[Office 365 Zaawansowana ochrona przed zagrożeniami](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Zaawansowana ochrona przed zagrożeniami (ATP) pomaga chronić firmę przed zaawansowanymi atakami typu phishing i Ransomware, które mają na celu złamanie zabezpieczeń danych pracowników lub klientów. Funkcje obejmują:
    
  - Zaawansowane Skanowanie załączników i analizy oparte na sztucznej inteligencji do wykrywania i odrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie linków w wiadomościach e-mail w celu oceny, czy są one częścią systemu phishingu. Dzięki temu można bezpiecznie uzyskiwać dostęp do niebezpiecznych witryn.

- **[Pełne możliwości usługi Intune w witrynie Azure Portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Uzyskiwanie dostępu do centrum administracyjnego usługi Intune w witrynie Azure Portal umożliwia konfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami z systemem MacOS, urządzeniami iPhone i Android oraz zaawansowane zarządzanie urządzeniami dla systemu Windows, które nie są dostępne za pośrednictwem programu Microsoft 365 centrum administracyjnego biznesu.
- **Ten sam [dostęp warunkowy](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) jako plan usługi Azure AD P1**

    Dostęp warunkowy może pomóc w ochronie organizacji przed ryzykiem logowania, próbami dostępu z nieoczekiwanej sieci lub ustawień regionalnych, próbami dostępu tworzą ryzykowne typy urządzeń itd. Zasady dostępu warunkowego są wymuszane po pierwszym uwierzytelnieniu i używa sygnałów z pierwszego zdarzenia uwierzytelniania w celu określenia, czy próba dostępu powinna być zatwierdzona, zaprzecza lub f więcej dowodu (np. druga forma identyfikacji) jest Wymagane.

    Dostępne są funkcje dostępu warunkowego:

    - Dostęp na podstawie nazwy użytkownika, grupy i roli
    - Dostęp [na podstawie aplikacji](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Dostęp na podstawie lokalizacji](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Zezwalaj tylko na dostęp z zaufanych zakresów adresów IP lub określonych krajów 
    - Wymagaj uwierzytelniania MFA dla dostępu
    - Blokowanie dostępu do aplikacji, które korzystają z [uwierzytelniania starszego](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Wymagaj aplikacji TP Użyj [ochrony aplikacji usługi Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Uwierzytelnianie niestandardowe, takie jak MFA z zewnętrznymi dostawcami, na przykład DUO.
   
    Inne funkcje:
    - [Samoobsługowe resetowanie hasła](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) dla hybrydowej usługi Azure AD
    
## <a name="compliance-features"></a>Funkcje zgodności

Subskrypcja Microsoft 365 Business obejmuje funkcje ułatwiające utrzymanie zgodności i standardów regulacyjnych.

- **[Omówienie zasad zapobiegania utracie danych](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Można skonfigurować DLP, aby automatycznie wykrywać poufne informacje, takie jak numery kart kredytowych, numery ubezpieczenia społecznego, itp., aby zapobiec ich przypadkowemu udostępnieniu poza firmą.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja Exchange Online Archiwizacja umożliwia łatwe archiwizowanie wiadomości przy użyciu ciągłej kopii zapasowej danych. Przechowuje wszystkie wiadomości e-mail użytkownika, w tym elementy usunięte, w przypadku, gdy są one potrzebne później do odnajdywania lub przywracania. Ponadto można użyć różnych zasad przechowywania, aby zachować dane poczty e-mail dla blokad sądowych, zbierania elektronicznych materiałów dowodowych lub w celu spełnienia wymagań dotyczących zgodności.
    
- **[Etykiety wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business zawiera wszystkie funkcje [usługi Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Dzięki temu planom można tworzyć **etykiety czułości**, które umożliwiają kontrolowanie dostępu do poufnych informacji w wiadomościach e-mail i dokumentach za pomocą kontrolek, takich jak "nie przesyłaj dalej" i "nie Kopiuj". Można również klasyfikować poufne informacje jako "poufne" i określać sposób, w jaki informacje niejawne mogą być udostępniane na zewnątrz i wewnątrz firmy. Szyfrowanie klasy korporacyjnej jest łatwe do zastosowania w przypadku poczty e-mail i dokumentów w celu zachowania prywatnych informacji. Można również zainstalować dodatek klienta usługi Azure Information Protection dla aplikacji pakietu Office. Aby uzyskać więcej informacji, zobacz [usługi Azure Information Protection Unified etykietowania klienta](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). W przypadku etykiet czułości należy zainstalować **AzInfoProtection_UL. exe**.

Te funkcje można zarządzać w centrum zgodności zabezpieczeń &amp; i centrum administracyjnego usługi Intune. Z biegiem czasu uproszczone formanty zostaną dodane do centrum administracyjnego Microsoft 365 Business.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których jest sprzedawana firma Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć centrum zgodności zabezpieczeń &amp; ?
  
1. [Zaloguj się do firmy Microsoft 365 Business](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W lewym NAV Zlokalizuj **centra administracyjne** i rozwiń go. 
    
    ![W lewej NAV w centrum administracyjnym Microsoft 365, wybierz centra administracyjne.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz **zgodność &amp; zabezpieczeń** , aby przejść do &amp; Centrum zgodności zabezpieczeń.
