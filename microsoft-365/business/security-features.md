---
title: Funkcje zabezpieczeń i zgodności usługi Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Dowiedz się więcej o funkcjach zabezpieczeń dosieciowych w usłudze Microsoft 365 Business.
ms.openlocfilehash: 0e1823374ec1843b6caa3f080393ca013302bf72
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593430"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Funkcje zabezpieczeń i zgodności usługi Microsoft 365 Business

Usługa Microsoft 365 Business oferuje uproszczone funkcje zabezpieczeń ułatwiające ochronę danych na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funkcje zabezpieczeń centrum administracyjnego usługi Microsoft 365 Business

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

W centrum administracyjnym można zarządzać wieloma funkcjami zabezpieczeń programu Microsoft 365 Business, które zapewniają uproszczony sposób wyłączeniu lub wyłączenia tych funkcji. W centrum administracyjnym można wykonać następujące czynności:
  
- [Ustawianie ustawień zarządzania aplikacjami dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Ustawienia te obejmują usuwanie plików z nieaktywnego urządzenia po określonym czasie, szyfrowanie plików służbowych, wymaganie, aby użytkownicy ustawiali kod PIN itd.
    
- [Ustawianie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Te ustawienia można zastosować do danych firmy zarówno na urządzeniach należących do firmy, jak i na urządzeniach będących własnością firmy.
    
- [Ustawianie ustawień ochrony urządzeń dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Można włączyć szyfrowanie [funkcji BitLocker,](https://go.microsoft.com/fwlink/p/?linkid=871405) aby chronić dane w przypadku utraty lub kradzieży urządzenia, a także włączyć [usługę Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) w celu zapewnienia zaawansowanej ochrony przed oprogramowaniem wymuszającym okup. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Możesz zdalnie wyczyścić dane firmy, jeśli urządzenie zostanie zgubione, skradzione lub pracownik opuści firmę.
    
- [Zresetuj urządzenia z systemem Windows 10 do ustawień fabrycznych](reset-devices-to-factory-settings.md) . 
    
    Można zresetować wszystkie urządzenia z systemem Windows 10, na których zastosowano ustawienia ochrony urządzenia.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Zaawansowane funkcje w usłudze Microsoft 365 Business są dostępne, aby chronić firmę przed zagrożeniami cybernetycznymi i chronić poufne informacje.
  
- **[Zaawansowana ochrona przed zagrożeniami w usłudze Office 365](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Zaawansowana ochrona przed zagrożeniami (ATP) pomaga chronić firmę przed wyrafinowanymi atakami phishingowymi i ransomware mającymi na celu naruszenie informacji o pracownikach lub klientach. Funkcje obejmują:
    
  - Zaawansowane skanowanie załączników i analiza z napędem AI w celu wykrywania i odrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie linków w wiadomości ach w wiadomościach e-mail w celu sprawdzenia, czy są one częścią systemu phishingu. Dzięki temu można bezpiecznie uzyskać dostęp do niebezpiecznych stron internetowych.

- **[Pełne możliwości usługi Intune w witrynie Azure portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Uzyskiwanie dostępu do centrum administracyjnego usługi Intune w witrynie Azure portal umożliwia skonfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami z systemem MacOS, iPhone i urządzenia mionem Android, a także zaawansowane zarządzanie urządzeniami dla systemu Windows, które nie są dostępne za pośrednictwem firmy Microsoft 365 Centrum administracyjne firmy.
- **Ten sam [dostęp warunkowy](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) co plan usługi Azure AD P1**


    Dostęp warunkowy może pomóc chronić organizację przed ryzykiem logowania, próbami dostępu z nieoczekiwanej sieci lub ustawień regionalnych, próbami dostępu z ryzykownych typów urządzeń itd. Zasady dostępu warunkowego są wymuszane po zakończeniu pierwszego uwierzytelniania i używa sygnałów z pierwszego zdarzenia uwierzytelniania, aby ustalić, czy próbowana odmowa dostępu powinna zostać zatwierdzona, odrzucona lub jeśli więcej dowodów (takich jak druga forma identyfikacji) jest wymagane.

    Zawarte funkcje dostępu warunkowego to:

    - Dostęp na podstawie nazwy użytkownika, grupy i roli
    - Dostęp [oparty na aplikacji](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Dostęp w zależności od lokalizacji](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  zezwalaj tylko na dostęp z zaufanych zakresów adresów IP lub określonych krajów 
    - Wymagaj pomocy w programie MFA w celu uzyskania dostępu
    - Blokowanie dostępu do aplikacji korzystających ze [starszego uwierzytelniania](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Wymagaj, aby aplikacje tp korzystały z [ochrony aplikacji Usługi Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Uwierzytelnianie niestandardowe, takie jak uwierzytelnianie wieloskładnikowe z dostawcami zewnętrznymi, na przykład DUO.
   
    Inne funkcje:
    - [Samoobsługowe resetowanie hasła](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) dla hybrydowej usługi Azure AD
    
## <a name="compliance-features"></a>Funkcje zgodności

Subskrypcja usługi Microsoft 365 Business zawiera funkcje ułatwiające zachowanie zgodności i standardów regulacyjnych.

- **[Omówienie zasad zapobiegania utracie danych](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    DLP można skonfigurować do automatycznego wykrywania poufnych informacji, takich jak numery kart kredytowych, numery ubezpieczenia społecznego itd., aby zapobiec ich nieumyślnemu udostępnianiu poza firmą.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja Exchange Online Archiving umożliwia łatwe archiwizowanie wiadomości za pomocą ciągłej kopii zapasowej danych. Przechowuje wszystkie wiadomości e-mail użytkownika, w tym usunięte elementy, na wypadek, gdyby były potrzebne później do odnajdowania lub przywracania. Ponadto można użyć różnych zasad przechowywania, aby zachować dane e-mail dla blokad sądowych, zbierania elektronicznych materiałów dowodowych lub spełniać wymagania dotyczące zgodności.
    
- **[Etykiety wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Usługa Microsoft 365 Business zawiera wszystkie funkcje [planu ochrony informacji platformy Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Za pomocą tego planu można utworzyć **etykiety czułości,** które umożliwiają kontrolowanie dostępu do poufnych informacji w wiadomościach e-mail i dokumentach, za pomocą kontrolek, takich jak "Nie przesyłaj dalej" i "Nie kopiuj". Można również sklasyfikować poufne informacje jako "poufne" i określić, w jaki sposób informacje niejawne mogą być udostępniane na zewnątrz i wewnątrz firmy. Szyfrowanie klasy korporacyjnej jest łatwe do zastosowania do poczty e-mail i dokumentów, aby zachować swoje informacje prywatne. Można również zainstalować dodatek klienta usługi Azure Information Protection dla aplikacji pakietu Office. Aby uzyskać więcej informacji, zobacz [Azure Information Protection ujednolicony klient etykietowania](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). W przypadku etykiet czułości zainstaluj **AzInfoProtection_UL.exe**.

Te funkcje można zarządzać &amp; w Centrum zgodności zabezpieczeń i w centrum administracyjnym usługi Intune. Z czasem uproszczone kontrolki zostaną dodane do centrum administracyjnego firmy Microsoft 365 Business.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których sprzedawany jest program Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć Centrum &amp; zgodności zabezpieczeń?
  
1. [Zaloguj się do usługi Microsoft 365 Business](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W lewej nav zlokalizuj **centra administracyjne** i rozwiń ją. 
    
    ![W lewym nav w centrum administracyjnym programu Microsoft 365 wybierz pozycję Centra administracyjne.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz ** &amp; pozycję Zgodność zabezpieczeń,** aby przejść do Centrum zgodności zabezpieczeń. &amp;
