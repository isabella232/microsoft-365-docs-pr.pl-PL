---
title: Migrowanie do programu Microsoft 365 Business z pakietu Office 365 E3
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
description: Dowiedz się, jak przenieść firmę do witryny Microsoft 365 Business Premium z pakietu Office 365 E3.
ms.openlocfilehash: f3f3894a2a5cb69f9f91825d89db4f4b857fac5c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295295"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrowanie z pakietu Office 365 E3 do programu Microsoft 365 Business Premium 

Aplikacja Microsoft 365 Business Premium ma wszystko, czego potrzebujesz dla małych firm, łącząc aplikacje biurowe z najlepszą obsługą chmurek, korzystając z prostego zarządzania urządzeniami i zabezpieczeniami. Jeśli masz obecnie subskrypcję pakietu Office 365 E3, ale nie masz więcej niż 300 pracowników, pomyśl o przełączeniu się do Microsoft 365 Business Premium w celu uzyskania dodatkowych funkcji zabezpieczeń.

Migracja jest łatwa: najpierw przełączasz licencje i wszystkie dane oraz informacje o użytkowniku w bieżącej subskrypcji są zachowywane. Po przeprowadzeniu migracji musisz skonfigurować funkcje dodane w programie Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Różnice między pakietem Office 365 E3 a programem Microsoft 365 Business Premium

W poniższej tabeli przedstawiono różnice między programem Microsoft 365 Business Premium a pakietem Office 365 E3.

| Funkcja    | Pomoc techniczna w programie Microsoft 365 Business Premium    | Pomoc techniczna w pakiecie Office 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Aplikacje pakietu Office<sup>1</sup>    | Aplikacje Microsoft 365 dla firm    | Aplikacje Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje do pracy w chmurze**        | | | 
| Exchange Online i Outlook    | 50 GB limitu magazynowania na skrzynkę pocztową i funkcję archiwizacji usługi Exchange Online    | 100 GB limitu magazynowania na skrzynkę pocztową i funkcję archiwizacji usługi Exchange Online | 
| Teams    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w pakiecie Office 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | 1 TB limitu magazynowania na użytkownika    | Czas | 
| Yammer, SharePoint Online, Planner, Stream    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w pakiecie Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w pakiecie Office 365 E3](../media/check-mark.png) | 
| Program Outlook Customer Manager, MileIQ    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrona przed zagrożeniami**        | | | 
| Office 365 Advanced Threat Protection (ATP) plan 1 | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | Nieuwzględniona, ale można ją dodać | 
| **Zarządzanie tożsamościami**        | | | 
| Samoobsługowe resetowanie hasła dla kont hybrydowych usługi Azure Active Directory (MFA), usługi Azure Multi-Factor Authentication (MFA), dostęp warunkowy, Stornowanie hasła dla tożsamości lokalnych|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Zarządzanie urządzeniami i aplikacjami**        | | |
| Microsoft Intune, Windows dla autopilota|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktywacja na komputerze współużytkowanym|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w pakiecie Office 365 E3](../media/check-mark.png)| 
| Prawa do uaktualnienia do systemu Windows 10 Pro z licencji win 7/8.1 Pro|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Ochrona informacji**        | | |
|Ochrona przed utratą danych w pakiecie Office 365|    ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)|![Dostępne w pakiecie Office 365 E3](../media/check-mark.png)|
|Usługa Azure Information Protection Plan 1, egzekwowanie funkcji BitLocker|![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)||
|Usługa Azure Information Protection Plan 1, etykiety wrażliwości|![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licencja dostępu klienta (prawa CAL)**|||
|Pakiet licencji Enterprise CAL (Exchange, SharePoint, Skype)||![Dostępne w pakiecie Office 365 E3](../media/check-mark.png)|

<sup>1</sup> wersja aplikacji pakietu Office dla firm Microsoft 365 Business Premium nie obejmuje aktywacji zbiorczej za pośrednictwem zasad grupy, funkcji telemetrii, aktualizacji, porównywania arkuszy kalkulacyjnych i zapytań lub analizy biznesowej.

## <a name="migration"></a>Migracj

Aby przeprowadzić migrację subskrypcji, zobacz [ręczne zmienianie planów](../commerce/subscriptions/change-plans-manually.md) w celu uzyskania instrukcji, jeśli chcesz przenieść tylko kilka osób do programu Microsoft 365 Business Premium. Możesz również [automatycznie uaktualnić wszystkich użytkowników](../commerce/subscriptions/upgrade-to-different-plan.md)lub współpracować z partnerem, aby przenieść subskrypcję E3 i licencje na subskrypcję usługi Microsoft 365 Business Premium.
W poniższych sekcjach opisano zmiany, które należy wprowadzić, jeśli istnieją, oraz jakie czynności można wykonać po zakończeniu migracji.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfiguracja i dane subskrypcji pakietu Office 365 E3
Przed przeprowadzeniem migracji nie musisz robić żadnych zmian w bieżącym abonamentu ani danych, co obejmuje następujące funkcje:

- Konfiguracja subskrypcji, taka jak rekordy DNS i nazwy domen.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usług biurowych i ich dane, takie jak zespoły, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla firm i Notesy programu OneNote.
- Aplikacje pakietu Office będą skalowane automatycznie. Nowoczesne Licencjonowanie pakietu Office 365 sprawdzi przypisanie licencji użytkownika co 72 godzin i przekonwertuje aplikacje pakietu Office do wersji zgodnej z subskrypcją użytkownika.

### <a name="windows-10"></a>Windows 10

Jeśli system Windows nie jest jeszcze w witrynie Windows Pro Creator Update, [Uaktualnij go do aktualizacji Windows Pro Creators](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurowanie zasad ochrony urządzeń i plików użytkowników

> [!NOTE]
> Jeśli skonfigurujesz zasady i urządzenia usługi MDM pakietu Office 365, urządzenia te zostaną wyświetlone na stronie **urządzenia** w centrum administracyjnym usługi Microsoft 365. Wszystkie skonfigurowane zasady zostaną wyświetlone na liście zasad klasycznych w [portalu usługi Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Po przypisaniu licencji do programu Microsoft 365 Business Premium możesz rozpocząć ochronę urządzeń i plików użytkowników.

Jeśli wszystkie osoby w organizacji zostały uaktualnione do programu Microsoft 365 Business Premium, na stronie głównej pojawi się Kreator konfiguracji, a [w Kreatorze konfiguracji](set-up.md) zostanie wyświetlony 365 monit o ochronę plików i urządzeń przenośnych.

Możesz również wykonać te czynności na stronie urządzenia:
  
1. W centrum administracyjnym w lewym obszarze nawigacji przejdź do obszaru zasady **urządzeń** \> **Policies**.
    
2. Na stronie **zasady dotyczące urządzeń** wybierz pozycję **Dodaj**.
    
3. W okienku **Dodaj zasady** nadaj zasadom nazwę, a następnie wybierz **Typ zasad** z listy rozwijanej. 
    
     Możesz skonfigurować zasady aplikacji dotyczące ochrony plików na urządzeniach z systemem Android i iPhone oraz systemu Windows 10, a także skonfigurować zasady konfiguracji urządzeń dla urządzeń należących do systemu Windows 10. Aby uzyskać szczegółowe informacje, zobacz następujące linki:
    
  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Ustawianie ustawień ochrony urządzeń dla komputerów PC z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Po skonfigurowaniu zasad i pracownicy mogą konfigurować urządzenia:
    
  - Aby uzyskać instrukcje dotyczące urządzeń z systemem Windows, zobacz [Konfigurowanie urządzeń z systemem Windows dla programu Microsoft 365 Business Premium](set-up-windows-devices.md) . 
    
  - Zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników programu Microsoft 365 Business Premium](set-up-mobile-devices.md) , aby zapoznać się z instrukcjami dotyczącymi telefonów stacjonarnych i iPhone z systemem Android. 
  
### <a name="mailbox-size"></a>Rozmiar skrzynki pocztowej

Program Microsoft 365 Business Premium ma limit magazynowania 50 GB, ponieważ używa usługi Exchange Online (plan 1). Podczas migrowania do programu Microsoft 365 Business Premium, jeśli którykolwiek z użytkowników przekroczy 50 GB miejsca do magazynowania, zaleca się przypisanie tego użytkownika do planu 2 usługi Exchange Online i usunięcie planu Exchange Online (1), ponieważ nie można go przypisać.


### <a name="threat-protection"></a>Ochrona przed zagrożeniami

Po przeprowadzeniu migracji do programu Microsoft 365 Business Premium masz pakiet Office 365 ATP. Aby zapoznać się z omówieniem, zobacz [pakiet Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) . Aby skonfigurować konto, zobacz [Konfigurowanie bezpiecznych linków ATP](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [Konfigurowanie bezpiecznych załączników ATP](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)i [Konfigurowanie ATP — ochrona przed phishingiem](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Etykiety wrażliwości

Aby zacząć korzystać z etykiet wrażliwości, zobacz [Omówienie etykiet wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) oraz [Tworzenie zawartości i zarządzanie etykietami liter](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .
