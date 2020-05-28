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
description: Dowiedz się więcej o funkcjach zabezpieczeń oferowanych w usłudze Microsoft 365 Business Premium, które pomagają chronić dane na komputerach, telefonach i tabletach.
ms.openlocfilehash: 839b5481e27591e1762a0d8eb5623f279d6d22dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402719"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Funkcje zabezpieczeń i zgodności usługi Microsoft 365 Business Premium

Usługa Microsoft 365 Business Premium oferuje uproszczone funkcje zabezpieczeń ułatwiające ochronę danych na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-admin-center-security-features"></a>Funkcje zabezpieczeń centrum administracyjnego usługi Microsoft 365

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Możesz zarządzać wieloma funkcjami zabezpieczeń usługi Microsoft 365 Business Premium w centrum administracyjnym, co zapewnia uproszczony sposób włączania lub wyłączania tych funkcji. W centrum administracyjnym można wykonać następujące czynności:
  
- [Ustawianie ustawień zarządzania aplikacjami dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Ustawienia te obejmują usuwanie plików z nieaktywnego urządzenia po upływie określonego czasu, szyfrowanie plików służbowych, wymaganie od użytkowników ustawiania numeru PIN itd.
    
- [Ustawianie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Te ustawienia mogą być stosowane do danych firmy zarówno na urządzeniach należących do firmy, jak i na urządzeniach będących własnością użytkownika.
    
- [Ustawianie ustawień ochrony urządzeń dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Można włączyć szyfrowanie [funkcją BitLocker,](https://go.microsoft.com/fwlink/p/?linkid=871405) aby chronić dane w przypadku utraty lub kradzieży urządzenia, a także włączyć usługę [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) w celu zapewnienia zaawansowanej ochrony przed oprogramowaniem wymuszającym okup. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Można zdalnie wyczyścić dane firmy, jeśli urządzenie zostanie zgubione, skradzione lub pracownik opuści firmę.
    
- [Zresetuj ustawienia fabryczne urządzeń z systemem Windows 10.](reset-devices-to-factory-settings.md) 
    
    Można zresetować wszystkie urządzenia z systemem Windows 10, które mają zastosowane ustawienia ochrony urządzeń.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Zaawansowane funkcje usługi Microsoft 365 Business Premium są dostępne, aby chronić firmę przed zagrożeniami cybernetycznymi i chronić poufne informacje.
  
- **[Zaawansowana ochrona przed zagrożeniami usługi Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Zaawansowana ochrona przed zagrożeniami (ATP) pomaga chronić firmę przed zaawansowanymi atakami phishingowymi i ransomware, które mają na celu naruszenie informacji o pracownikach lub klientach. Funkcje obejmują:
    
  - Zaawansowane skanowanie załączników i analiza oparta na sztucznej inteligencji w celu wykrywania i odrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie linków w wiadomościach e-mail w celu oceny, czy są one częścią systemu wyłudzania informacji. Dzięki temu możesz mieć dostęp do niebezpiecznych witryn.

- **[Pełne możliwości usługi Intune w witrynie Azure portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Dostęp do centrum administracyjnego usługi Intune w witrynie Azure portal umożliwia skonfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami MacOS, telefonem iPhone i urządzeniami z systemem Android, a także zaawansowane zarządzanie urządzeniami dla systemu Windows, które nie są dostępne za pośrednictwem centrum administracyjnego usługi Microsoft 365.
- **Ten sam [dostęp warunkowy](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) jak plan usługi Azure AD Premium P1**


    Dostęp warunkowy może pomóc chronić organizację przed ryzykiem logowania, próbami dostępu z nieoczekiwanej sieci lub ustawień regionalnych, próbami dostępu z ryzykownych typów urządzeń i tak dalej. Zasady dostępu warunkowego są wymuszane po zakończeniu pierwszego uwierzytelniania i używają sygnałów z pierwszego zdarzenia uwierzytelniania, aby określić, czy próba dostępu powinna zostać zatwierdzona, odrzucona lub czy wymagana jest większa liczba dowodów (takich jak druga forma identyfikacji).

    Dostępne są następujące funkcje dostępu warunkowego:

    - Dostęp na podstawie nazwy użytkownika, grupy i roli
    - Dostęp [na podstawie aplikacji](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Dostęp na podstawie lokalizacji;](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  zezwalaj tylko na dostęp z zaufanych zakresów adresów IP lub określonych krajów 
    - Wymagaj usługi MFA, aby uzyskać dostęp
    - Blokowanie dostępu do aplikacji korzystających ze [starszego uwierzytelniania](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Wymaganie aplikacji tp używać [ochrony aplikacji usługi Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Uwierzytelnianie niestandardowe, takie jak uwierzytelnianie wieloskładnikowe z dostawcami zewnętrznymi, na przykład DUO.
   
    Inne funkcje:
    - [Samoobsługowe resetowanie hasła](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) dla hybrydowej usługi Azure AD
    
## <a name="compliance-features"></a>Funkcje zgodności

Subskrypcja usługi Microsoft 365 Business Premium zawiera funkcje, które pomagają zachować zgodność i standardy regulacyjne.

- **[Omówienie zasad zapobiegania utracie danych](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (DLP). 
    
    Można skonfigurować DLP do automatycznego wykrywania poufnych informacji, takich jak numery kart kredytowych, numery ubezpieczenia społecznego i tak dalej, aby zapobiec ich przypadkowemu udostępnieniu poza firmą.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja Exchange Online Archiving umożliwia łatwe archiwizowanie wiadomości za pomocą ciągłej kopii zapasowej danych. Przechowuje wszystkie wiadomości e-mail użytkownika, w tym usunięte elementy, w przypadku, gdy są one potrzebne później do odnajdowania lub przywracania. Ponadto można użyć różnych zasad przechowywania, aby zachować dane wiadomości e-mail do blokady sporów sądowych, zbieranie elektronicznych materiałów dowodowych lub w celu spełnienia wymagań dotyczących zgodności.
    
- **[Etykiety wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Usługa Microsoft 365 Business Premium zawiera wszystkie funkcje [planu ochrony informacji platformy Azure 1.](https://go.microsoft.com/fwlink/p/?linkid=871407) Za pomocą tego planu można utworzyć **etykiety czułości,** które umożliwiają kontrolowanie dostępu do poufnych informacji w wiadomościach e-mail i dokumentach, za pomocą formantów takich jak "Nie przesyłaj dalej" i "Nie kopiuj". Możesz również sklasyfikować poufne informacje jako "poufne" i określić, w jaki sposób informacje niejawne mogą być udostępniane na zewnątrz i wewnątrz firmy. Szyfrowanie klasy korporacyjnej jest łatwe do zastosowania do poczty e-mail i dokumentów, aby zachować prywatność informacji. Można również zainstalować dodatek klienta usługi Azure Information Protection dla aplikacji pakietu Office. Aby uzyskać więcej informacji, zobacz [Azure Information Protection ujednoliconego klienta etykietowania](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). W przypadku etykiet czułości zainstaluj **program AzInfoProtection_UL.exe**.

Te funkcje można zarządzać w &amp; Centrum zgodności zabezpieczeń i centrum administracyjnym usługi Intune. Z czasem uproszczone formanty zostaną dodane do centrum administracyjnego usługi Microsoft 365.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których jest sprzedawany program Microsoft 365 Business Premium.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć Centrum &amp; zgodności zabezpieczeń?
  
1. [Zaloguj się do usługi Microsoft 365 Business Premium](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W lewej lokalizacji nawigacyjnej znajdź **centra administracyjne** i rozwiń je. 
    
    ![W lewej aplikacji w centrum administracyjnym usługi Microsoft 365 wybierz pozycję Centra administracyjne.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz **pozycję &amp; Zgodność zabezpieczeń,** aby przejść do &amp; Centrum zgodności zabezpieczeń.
