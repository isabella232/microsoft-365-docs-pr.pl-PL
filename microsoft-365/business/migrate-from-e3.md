---
title: Migrowanie do usługi Microsoft 365 Business z usługi Office 365 E3
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
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Dowiedz się, jak przenieść firmę do usługi Microsoft 365 Business Premium z usługi Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081881"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migracja z usługi Office 365 E3 do usługi Microsoft 365 Business Premium 

Usługa Microsoft 365 Business Premium ma wszystko, czego potrzebujesz dla małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami. Jeśli masz obecnie subskrypcję usługi Office 365 E3, ale nie masz więcej niż 300 pracowników, rozważ przejście na usługę Microsoft 365 Business Premium w celu uzyskania dodatkowych funkcji zabezpieczeń.

Migracja jest prosta: najpierw przełączasz licencje, a wszystkie dane i informacje o użytkowniku w bieżącej subskrypcji są zachowywane. Po migracji należy skonfigurować funkcje dodane w usłudze Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Różnice między office 365 E3 i Microsoft 365 Business Premium

W tej tabeli przedstawiono różnice między usłudze Microsoft 365 Business Premium a office 365 E3.

| Funkcja    | Pomoc techniczna w usłudze Microsoft 365 Business Premium    | Pomoc techniczna w usłudze Office 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Aplikacje pakietu Office<sup>1</sup>    | Aplikacje usługi Microsoft 365 dla firm    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje zwiększające produktywność w chmurze**        | | | 
| Usługa Exchange Online i Outlook    | Limit miejsca 50 GB na skrzynkę pocztową i nieograniczona archiwizacja w trybie online programu Exchange    | Limit miejsca 100 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online | 
| Zespołów    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z pakietem Office 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | Limit pojemności 1 TB na użytkownika    | Nieograniczony | 
| Yammer, SharePoint Online, Planner, Strumień    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z pakietem Office 365 E3](../media/check-mark.png) | 
| StaffHub ( StaffHub )    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z pakietem Office 365 E3](../media/check-mark.png) | 
| Menedżer klienta programu Outlook, MileIQ    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrona przed zagrożeniami**        | | | 
| Plan 1 zaawansowanej ochrony przed zagrożeniami usługi Office 365 | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | Nie jest dołączony, ale można go dodać na | 
| **Zarządzanie tożsamościami**        | | | 
| Samoobsługowe resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego platformy Azure (MFA), dostępu warunkowego, zapisywania haseł dla tożsamości lokalnych|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Zarządzanie urządzeniami i aplikacjami**        | | |
| Microsoft Intune, Windows AutoPilot|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktywacja komputera współdzielonego|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z pakietem Office 365 E3](../media/check-mark.png)| 
| Prawa do uaktualnienia do systemu Windows 10 Pro z licencji Win 7/8.1 Pro|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Ochrona informacji**        | | |
|Zapobieganie utracie danych w usłudze Office 365|    ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)|![W zestawie z pakietem Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, wymuszanie funkcji Bitlocker|![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)||
|Plan ochrony informacji platformy Azure 1, etykiety czułości|![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licencja dostępu klienta (prawa CAL)**|||
|Pakiet CAL dla przedsiębiorstw (Exchange, SharePoint, Skype)||![W zestawie z pakietem Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Wersja aplikacji pakietu Microsoft 365 Business Premium nie obejmuje aktywacji zbiorczej za pośrednictwem zasad grupy, telemetrii aplikacji, formantów aktualizacji, porównywania i uzyskiwania informacji o arkuszach kalkulacyjnych ani analizy biznesowej.

## <a name="migration"></a>Migracji

Aby przeprowadzić migrację subskrypcji, zobacz [Ręczne zmienianie planów,](../commerce/subscriptions/change-plans-manually.md) aby uzyskać instrukcje, jeśli chcesz przenieść tylko kilka osób do usługi Microsoft 365 Business Premium. Możesz również [automatycznie uaktualnić wszystkich](../commerce/subscriptions/upgrade-to-different-plan.md)lub współpracować z partnerem, aby przenieść subskrypcję E3 i licencje do subskrypcji Microsoft 365 Business Premium.
W poniższych sekcjach opisano zmiany, które należy wprowadzić, jeśli istnieją, i co można zrobić po migracji.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfiguracja i dane subskrypcji usługi Office 365 E3
Przed migracją nie trzeba wywdziałać żadnych zmian w bieżącej subskrypcji lub danych, co obejmuje:

- Konfiguracja subskrypcji, taka jak rekordy DNS i nazwy domen.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usług zwiększających produktywność i ich dane, takie jak usługi Teams, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.
- Aplikacje pakietu Office będą skalowane automatycznie. Nowoczesne licencjonowanie usługi Office 365 sprawdza przypisanie licencji użytkownika co 72 godziny i konwertuje aplikacje pakietu Office na wersję odpowiadającą subskrypcji użytkownika.

### <a name="windows-10"></a>Windows 10

Jeśli systemu Windows nie ma jeszcze aktualizacji programu Windows Pro Creator, [uaktualnij go do usługi Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurowanie zasad ochrony urządzeń i plików użytkowników

> [!NOTE]
> Jeśli skonfigurujesz zasady i urządzenia MDM usługi Office 365, te urządzenia będą wyświetlane na stronie **Urządzenia** w centrum administracyjnym usługi Microsoft 365. Wszystkie skonfigurowane zasady pojawią się na liście klasycznych zasad w [portalu usługi Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Po przypisaniu licencji do usługi Microsoft 365 Business Premium można rozpocząć ochronę urządzeń i plików użytkowników.

Jeśli uaktualniono wszystkich osób w organizacji do usługi Microsoft 365 Business Premium, na stronie głównej zostanie wyświetlony kreator konfiguracji i możesz wykonać czynności [kreatora konfigurowania usługi Microsoft 365 Business Premium w](set-up.md) krokach kreatora instalacji w celu ochrony plików i urządzeń przenośnych.

Możesz również wykonać następujące kroki na stronie Urządzenia:
  
1. W centrum administracyjnym w lewym urządzeniu nawigacyjnym przejdź do **pozycji Zasady urządzeń** \> **Policies**.
    
2. Na stronie **Zasady urządzenia** wybierz pozycję **Dodaj**.
    
3. W okienku **Dodawanie zasad** nadaj zasadom nazwę, a następnie wybierz **typ zasad** z listy rozwijanej. 
    
     Można skonfigurować zasady aplikacji do ochrony plików na urządzeniach z systemem Android i iPhone, a także w systemie Windows 10, a także skonfigurować zasady konfiguracji urządzeń dla firmowych urządzeń z systemem Windows 10. Szczegółowe informacje można znaleźć w następujących łączach:
    
  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Ustawianie ustawień ochrony urządzeń dla komputerów z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Po skonfigurowaniu zasad ty i twoi pracownicy możecie skonfigurować urządzenia:
    
  - Aby uzyskać instrukcje dotyczące urządzeń z systemem Windows dla urządzeń [z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium, zobacz Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
  - Aby uzyskać instrukcje dotyczące telefonów i telefonów iPhone z systemem Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business Premium.](set-up-mobile-devices.md) 

### <a name="threat-protection"></a>Ochrona przed zagrożeniami

Po migracji do usługi Microsoft 365 Business Premium masz usługę Office 365 ATP. Zobacz [Usługi Office 365 ATP,](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) aby uzyskać omówienie. Aby skonfigurować, zobacz [konfigurowanie bezpiecznych łączy ATP](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [konfigurowanie bezpiecznych załączników ATP](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)i [konfigurowanie programu ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Etykiety wrażliwości

Aby rozpocząć korzystanie z etykiet czułości, zobacz [Omówienie etykiet czułości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) oraz [tworzenie etykiet czułości i zarządzanie nimi](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) wideo.
