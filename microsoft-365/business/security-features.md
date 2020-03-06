---
title: Funkcje zabezpieczeń i zgodności z przepisami dotyczącymi usługi Microsoft 365 Business
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Dowiedz się więcej o funkcjach zabezpieczeń związanych z usługą Microsoft 365 Business, aby chronić dane na komputerach, telefonach i tabletach.
ms.openlocfilehash: eb92131cc937875615342b2b0d39c78d51a8a99f
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550042"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Funkcje zabezpieczeń i zgodności z przepisami dotyczącymi usługi Microsoft 365 Business

Usługa Microsoft 365 Business oferuje uproszczone funkcje zabezpieczeń ułatwiające ochronę danych na komputerach, telefonach i tabletach.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funkcje zabezpieczeń centrum administracyjnego usługi Microsoft 365 Business

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

W centrum administracyjnym można zarządzać wieloma funkcjami zabezpieczeń usługi Microsoft 365 Business, co zapewnia uproszczony sposób włączeniu lub wyłączeniu tych funkcji. W centrum administracyjnym można wykonać następujące czynności:
  
- [Ustaw ustawienia zarządzania aplikacjami dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Ustawienia te obejmują usuwanie plików z nieaktywnego urządzenia po określonym czasie, szyfrowanie plików roboczych, wymaganie, aby użytkownicy ustawili numer PIN itd.
    
- [Ustaw ustawienia ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Ustawienia te mogą być stosowane do danych firmy zarówno na urządzeniach należących do firmy, jak i na urządzeniach będących własnością firmy.
    
- [Ustaw ustawienia ochrony urządzeń dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Możesz włączyć [szyfrowanie funkcją BitLocker,](https://go.microsoft.com/fwlink/p/?linkid=871405) aby chronić dane w przypadku zgubienia lub kradzieży urządzenia, a także włączyć funkcję [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) w celu zapewnienia zaawansowanej ochrony przed oprogramowaniem wymuszającym okup. 
    
- [Usuwanie firmowych danych z urządzeń](remove-company-data.md)
    
    Możesz zdalnie wyczyścić dane firmy, jeśli urządzenie zostanie zgubione, skradzione lub pracownik opuści firmę.
    
- [Zresetuj urządzenia z systemem Windows 10 do ustawień fabrycznych](reset-devices-to-factory-settings.md) . 
    
    Możesz zresetować wszystkie urządzenia z systemem Windows 10, na których zastosowano ustawienia ochrony urządzeń.
    
## <a name="additional-security-features"></a>Dodatkowe funkcje zabezpieczeń 

Zaawansowane funkcje usługi Microsoft 365 Business pomagają chronić firmę przed zagrożeniami cybernetycznymi i chronić poufne informacje.
  
- **[Zaawansowana ochrona przed zagrożeniami usługi Office 365](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Zaawansowana ochrona przed zagrożeniami (ATP) pomaga chronić firmę przed wyrafinowanymi atakami typu phishing i ransomware mającymi na celu naruszenie informacji o pracownikach lub klientach. Funkcje obejmują:
    
  - Zaawansowane skanowanie załączników i analiza ai do wykrywania i wyrzucania niebezpiecznych wiadomości.
    
  - Automatyczne sprawdzanie linków w wiadomoście e-mail w celu sprawdzenia, czy są one częścią systemu wyłudzania informacji. Dzięki temu możesz bezpiecznie korzystać z niebezpiecznych stron internetowych.

- **[Pełne możliwości usługi Intune w witrynie Azure portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Uzyskiwanie dostępu do centrum administracyjnego usługi Intune w witrynie Azure portal umożliwia skonfigurowanie dodatkowych funkcji zabezpieczeń, takich jak zarządzanie urządzeniami z systemem MacOS, telefonem iPhone i urządzeniami z systemem Android, a także zaawansowane zarządzanie urządzeniami dla systemu Windows, które nie są dostępne za pośrednictwem firmy Microsoft 365 Centrum administracyjne dla firm.
- **Ten sam [dostęp warunkowy](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) jako plan usługi Azure AD P1**


    Dostęp warunkowy może pomóc chronić organizację przed ryzykiem logowania, uzyskać dostęp do prób z nieoczekiwanej sieci lub ustawień regionalnych, uzyskać dostęp do prób z ryzykownych typów urządzeń i tak dalej. Zasady dostępu warunkowego są wymuszane po zakończeniu pierwszego uwierzytelniania i używają sygnałów z pierwszego zdarzenia uwierzytelniania, aby ustalić, czy próba dostępu powinna zostać zatwierdzona, odrzucona lub czy więcej dowodów (na przykład druga forma identyfikacji) jest wymagane.

    Funkcje dostępu warunkowego są następujące:

    - Dostęp na podstawie nazwy użytkownika, grupy i roli
    - Dostęp [na podstawie aplikacji](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Dostęp w oparciu o lokalizację](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Zezwalaj tylko na dostęp z zaufanych zakresów adresów IP lub określonych krajów 
    - Wymagaj dostępu do pomocy mfa
    - Blokowanie dostępu do aplikacji korzystających z [starszego uwierzytelniania](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Wymagaj od aplikacji tp korzystania z [ochrony aplikacji usługi Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Uwierzytelnianie niestandardowe, takie jak uwierzytelnianie wieloskładnikowe u dostawców innych firm, na przykład DUO.
   
    Inne funkcje:
    - [Samoobsługowe resetowanie hasła](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) dla hybrydowej usługi Azure AD
    
## <a name="compliance-features"></a>Funkcje zgodności

Subskrypcja usługi Microsoft 365 Business zawiera funkcje ułatwiające zachowanie zgodności i standardów regulacyjnych.

- **[Omówienie zasad zapobiegania utracie danych](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    DLP można skonfigurować tak, aby automatycznie wykrywał poufne informacje, takie jak numery kart kredytowych, numery ubezpieczenia społecznego itd., aby zapobiec ich nieumyślnemu udostępnianiu poza firmą.
    
- **[Exchange Online  archiwum](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licencja na archiwizację w usłudze Exchange Online umożliwia łatwe archiwizowanie wiadomości za pomocą ciągłej kopii zapasowej danych. Przechowuje wszystkie wiadomości e-mail użytkownika, w tym usunięte elementy, na wypadek, gdyby były one potrzebne później do odnajdowania lub przywracania. Ponadto można użyć różnych zasad przechowywania, aby zachować dane poczty e-mail dla blokad sporów, zbierania elektronicznych materiałów dowodowych lub w celu spełnienia wymagań dotyczących zgodności.
    
- **[Etykiety wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Usługa Microsoft 365 Business zawiera wszystkie funkcje [planu ochrony informacji platformy Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Za pomocą tego planu można utworzyć **etykiety czułości,** które umożliwiają kontrolowanie dostępu do poufnych informacji w wiadomościach e-mail i dokumentach, z kontrolkami takimi jak "Nie przesyłaj dalej" i "Nie kopiuj". Można również sklasyfikować poufne informacje jako "poufne" i określić, w jaki sposób informacje niejawne mogą być udostępniane na zewnątrz i wewnątrz firmy. Szyfrowanie klasy korporacyjnej jest łatwe do zastosowania do poczty e-mail i dokumentów, aby zachować swoje informacje prywatne. Można również zainstalować dodatek klienta usługi Azure Information Protection dla aplikacji pakietu Office. Aby uzyskać więcej informacji, zobacz [Ujednolicony klient etykietowania usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). W przypadku etykiet czułości zainstaluj **plik AzInfoProtection_UL.exe**.

Te funkcje można zarządzać &amp; w Centrum zgodności zabezpieczeń i w centrum administracyjnym usługi Intune. Z czasem uproszczone formanty zostaną dodane do centrum administracyjnego usługi Microsoft 365 Business.
  
    
## <a name="faq"></a>Często zadawane pytania

 ### <a name="are-these-security-features-available-in-all-markets"></a>Czy te funkcje zabezpieczeń są dostępne na wszystkich rynkach?
  
Tak, te funkcje są dostępne na wszystkich rynkach, na których sprzedawany jest program Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak znaleźć Centrum &amp; zgodności zabezpieczeń?
  
1. [Zaloguj się do usługi Microsoft 365 Business](https://portal.microsoft.com/) przy użyciu poświadczeń administratora. 
    
2. W lewym nav znajdź **centra administracyjne** i rozwiń je. 
    
    ![W lewym nav w centrum administracyjnym usługi Microsoft 365 wybierz pozycję Centra administracyjne.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Wybierz ** &amp; pozycję Zgodność zabezpieczeń,** aby przejść do centrum zgodności zabezpieczeń. &amp;
