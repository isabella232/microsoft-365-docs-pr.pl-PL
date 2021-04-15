---
title: Migrowanie do usługi Microsoft 365 Business z usługi Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: f2b7962918186f4a1063c5a66596135c2972ec71
ms.sourcegitcommit: 07dea2aa98daf0c4086f8590375167830027c802
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/13/2021
ms.locfileid: "51750005"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrowanie z usługi Office 365 E3 do platformy Microsoft 365 Business Premium

Usługa Microsoft 365 Business Premium oferuje wszystko, czego potrzebujesz dla Twojej małej firmy, i łączy najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami. Jeśli obecnie masz subskrypcję usługi Office 365 E3, ale nie masz więcej niż 300 pracowników, rozważ przełączenie się do usługi Microsoft 365 Business Premium, aby uzyskać dostęp do dodatkowych funkcji zabezpieczeń.

Migracja jest łatwa: najpierw przełączasz licencje, a wszystkie dane i informacje o użytkownikach w bieżącej subskrypcji są zachowywane. Po zakończeniu migracji musisz skonfigurować funkcje dodawane do usługi Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Różnice między usługami Office 365 E3 i Microsoft 365 Business Premium

W poniższej tabeli przedstawiono różnice między usługami Microsoft 365 Business Premium i Office 365 E3.

| Funkcja    | Pomoc techniczna na platformy Microsoft 365 Business Premium    | Pomoc techniczna w usłudze Office 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Aplikacje pakietu Office<sup>1</sup>    | Aplikacje Microsoft 365 dla firm    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje zwiększające produktywność w chmurze**        | | | 
| Usługi Exchange Online i Outlook    | Limit miejsca do magazynowania 50 GB na skrzynkę pocztową i nieograniczona archiwum online usługi Exchange    | Limit miejsca do magazynowania 100 GB na skrzynkę pocztową i nieograniczona archiwum online usługi Exchange | 
| Teams    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do usługi Office 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | 1 TB miejsca do magazynowania na użytkownika    | Bez ograniczeń | 
| Yammer, SharePoint Online, Planner, Stream    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do usługi Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do usługi Office 365 E3](../media/check-mark.png) | 
| MileiQ    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrona przed zagrożeniami**        | | | 
| Defender dla usługi Office 365 (plan 1) | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | Nie dołączona, ale można ją dodać do | 
| **Zarządzanie tożsamościami**        | | | 
| Samodzielne resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego (MFA), dostępu warunkowego i zapisu haseł tożsamości lokalnych|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Zarządzanie urządzeniami i aplikacją**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktywacja na komputerze udostępnionym|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do usługi Office 365 E3](../media/check-mark.png)| 
| Prawa do uaktualnienia do systemu Windows 10 Pro z licencji Win 7/8.1 Pro|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Ochrona informacji**        | | |
|Ochrona przed utratą danych w usłudze Office 365|    ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)|![Dołączone do usługi Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, wymuszanie funkcji BitLocker|![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, Etykiety wrażliwości|![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licencja dostępu klienta (prawa calowe)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Dołączone do usługi Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Wersja aplikacji pakietu Office 365 Business Premium nie obejmuje aktywacji zbiorczej za pośrednictwem programu zasady grupy, telemetrii aplikacji, kontrolek aktualizacji, porównywania i ineksji arkuszy kalkulacyjnych ani analizy biznesowej.

## <a name="migration"></a>Migracja

Aby przeprowadzić migrację subskrypcji, [zobacz](../commerce/subscriptions/change-plans-manually.md) Ręczne zmienianie planów, aby uzyskać instrukcje dotyczące przenoszenia tylko kilku osób do usługi Microsoft 365 Business Premium. Możesz również [uaktualnić wszystkich](../commerce/subscriptions/upgrade-to-different-plan.md)automatycznie lub we współpracy z partnerem przenieść subskrypcję I licencje E3 do subskrypcji Microsoft 365 Business Premium.
W poniższych sekcjach opisano zmiany, które należy wprowadzić (o ile są) oraz czynności, które można wprowadzić po migracji.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfiguracja i dane subskrypcji Office 365 E3
Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:

- Konfiguracja subskrypcji, taka jak rekordy DNS i nazwy domen.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usługi zwiększającej produktywność i ich dane, takie jak usługa Teams, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.
- Aplikacje pakietu Office zostaną przeskalowane automatycznie. Nowoczesne licencjonowanie usługi Office 365 sprawdza przypisanie licencji użytkownika co 72 godziny i konwertuje aplikacje pakietu Office na wersję, która jest taka, jak subskrypcja użytkownika.

### <a name="windows-10"></a>Windows 10

Jeśli twój system Windows nie jest jeszcze w aktualizacji Windows Pro Creator, [uaktualnij go do wersji Windows Pro (aktualizacja dla twórców).](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurowanie zasad ochrony urządzeń i plików użytkowników

> [!NOTE]
> Jeśli skonfigurujsz zasady MDM i urządzenia usługi Office 365, będą one wymienione na stronie Urządzenia w centrum administracyjnym platformy Microsoft 365.  Wszystkie zasady, które skonfigurujsz, będą wyświetlane na liście zasad klasycznych w [portalu usługi Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Po przypisaniu licencji do usługi Microsoft 365 Business Premium możesz rozpocząć ochronę urządzeń i plików użytkowników.

Jeśli wszyscy w organizacji przeprowadzisz uaktualnienie do usługi Microsoft 365 Business Premium, na stronie głównej zostanie wyświetlony kreator konfiguracji i możesz wykonać kroki Konfigurowania usługi [Microsoft 365 Business Premium](set-up.md) w kreatorze konfiguracji w celu ochrony plików i urządzeń przenośnych.

Na stronie Urządzenia możesz również wykonać następujące czynności:
  
1. W centrum administracyjnym w lewym okienku narracji przejdź do **pozycji Zasady dotyczące** \> **urządzeń.**
    
2. Na stronie **Zasady dotyczące urządzeń** wybierz pozycję **Dodaj**.
    
3. W **okienku Dodaj** zasady nadaj zasadom nazwę, **a** następnie z listy rozwijanej wybierz typ zasad. 
    
     Możesz skonfigurować zasady aplikacji dotyczące ochrony plików na urządzeniach z systemem Android i iPhone, a także w systemie Windows 10, a także skonfigurować zasady konfiguracji urządzeń dla urządzeń z systemem Windows 10, których właścicielem jest firma. Aby uzyskać szczegółowe informacje, zobacz następujące linki:
    
  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Konfigurowanie ustawień ochrony urządzeń dla komputerów z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Po skonfigurowaniu zasad Ty i Twoi pracownicy możecie skonfigurować urządzenia:
    
  - Aby uzyskać instrukcje dotyczące urządzeń z systemem Windows, zobacz Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi [Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
  - Aby uzyskać instrukcje dotyczące telefonów iPhone z systemem Android, zobacz Konfigurowanie urządzeń przenośnych dla użytkowników usługi [Microsoft 365 Business Premium.](set-up-mobile-devices.md) 
  
### <a name="mailbox-size"></a>Rozmiar skrzynki pocztowej

Usługa Microsoft 365 Business Premium ma limit przestrzeni dyskowej 50 GB, ponieważ korzysta z usługi Exchange Online (plan 1). Podczas migracji do usługi Microsoft 365 Business Premium, jeśli którykolwiek z użytkowników przekracza 50 GB miejsca do magazynowania skrzynki pocztowej, zaleca się przypisanie temu użytkownikowi planu 2 usługi Exchange Online i usunięcie planu 1 usługi Exchange Online, ponieważ nie jest możliwe przypisanie obu tych skrzynek.


### <a name="threat-protection"></a>Ochrona przed zagrożeniami

Po zakończeniu migracji do usługi Microsoft 365 Business Premium masz program Defender dla usługi Office 365. Zobacz [Microsoft Defender dla Office 365,](../security/office-365-security/defender-for-office-365.md) aby uzyskać omówienie. Aby skonfigurować, zobacz Konfigurowanie bezpiecznych [linków,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [konfigurowanie](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)bezpiecznych załączników i konfigurowanie ochrony przed wyłudzaniem informacji w [usłudze Defender dla usługi Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Etykiety wrażliwości

Aby rozpocząć korzystanie z etykiet wrażliwości, zobacz [Omówienie etykiet wrażliwości](../compliance/sensitivity-labels.md) oraz tworzenie etykiet wrażliwości i zarządzanie nimi — [klip](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) wideo.
