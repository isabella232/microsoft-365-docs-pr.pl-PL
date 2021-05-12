---
title: Migrowanie do Microsoft 365 Business z Office 365 E3
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
description: Dowiedz się, jak przenieść firmę do Microsoft 365 Business Premium z Office 365 E3.
ms.openlocfilehash: 990ca8bdae979f1efb8a60a3460add2953a51892
ms.sourcegitcommit: 68383240ef7a673d5f28e2ecfab9f105bf1d8c8f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/11/2021
ms.locfileid: "52327175"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrowanie z Office 365 E3 do Microsoft 365 Business Premium

Microsoft 365 Business Premium wszystko, czego potrzebujesz dla swojej małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami. Jeśli obecnie masz subskrypcję Office 365 E3, ale nie masz więcej niż 300 pracowników, rozważ przełączenie się do usługi Microsoft 365 Business Premium w celu uwzględnienia dodatkowych funkcji zabezpieczeń.

Migracja jest łatwa: najpierw przełączasz licencje, a wszystkie dane i informacje o użytkownikach w bieżącej subskrypcji są zachowywane. Po migracji musisz skonfigurować funkcje, które są dodawane w programie Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Różnice między Office 365 E3 a Microsoft 365 Business Premium

W poniższej tabeli przedstawiono różnice między Microsoft 365 Business Premium a Office 365 E3.

| Funkcja    | Pomoc techniczna w Microsoft 365 Business Premium    | Pomoc techniczna w Office 365 E3 |
|:-------|:-----|:-----|
| **Lokalnie**        | | |
| Office aplikacji<sup>1</sup>    | Aplikacje Microsoft 365 dla firm    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw |
| **Aplikacje zwiększające produktywność w chmurze**        | | |
| Exchange Online i Outlook    | 50 GB miejsca do magazynowania na skrzynkę pocztową i nieograniczona liczba Exchange Online — archiwum    | 100 GB miejsca do magazynowania na skrzynkę pocztową i nieograniczona liczba Exchange Online — archiwum |
| Teams    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | 1 TB miejsca do magazynowania na użytkownika    | Bez ograniczeń | 
| Yammer, SharePoint Online, Planner, Stream    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png) |
| **Ochrona przed zagrożeniami**        | | |
| Defender dla Office 365 Plan 1 | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | Nie dołączona, ale można ją dodać do |
| **Zarządzanie tożsamościami**        | | |
| Samodzielne resetowanie hasła dla kont Azure Active Directory hybrydowych (Azure AD), uwierzytelnianie wieloskładnikowe (MFA), dostęp warunkowy, funkcja zapisu hasła dla tożsamości lokalnych|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| **Zarządzanie urządzeniami i aplikacją**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktywacja na komputerze udostępnionym|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png)| 
| Prawa do uaktualnienia do Windows 10 Pro z licencji win 7/8.1 Pro Windows|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    ||
| **Ochrona informacji**        | | |
|Office 365 Ochrona przed utratą danych|    ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)|![Dołączona do Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, funkcja BitLocker wymuszanie|![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, Etykiety wrażliwości|![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licencja dostępu klienta (prawa calowe)**|||
|Enterprise Cal Suite (Exchange, SharePoint, Skype)||![Dołączona do Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 Business Premium pakietu Office nie obejmuje aktywacji zbiorczej za pośrednictwem usługi zasady grupy, telemetrii aplikacji, kontrolek aktualizacji, porównywania i ineksji arkuszy kalkulacyjnych ani analizy biznesowej.

## <a name="migration"></a>Migracja

Aby przeprowadzić migrację subskrypcji, [zobacz](../commerce/subscriptions/change-plans-manually.md) Ręczne zmienianie planów, aby uzyskać instrukcje dotyczące przenoszenia tylko kilku osób do Microsoft 365 Business Premium. Możesz również [uaktualnić wszystkich automatycznie](../commerce/subscriptions/upgrade-to-different-plan.md)lub we współpracy z partnerem przenieść Twoją subskrypcję I licencje E3 do subskrypcji Microsoft 365 Business Premium subskrypcji.
W poniższych sekcjach opisano zmiany, które należy wprowadzić (o ile są) oraz czynności, które można wprowadzić po migracji.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 Dane i konfiguracja subskrypcji E3
Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:

- Konfiguracja subskrypcji, taka jak rekordy DNS i nazwy domen.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usługi zwiększającej produktywność i ich dane, takie Teams, Exchange Online pocztowe, SharePoint online, OneDrive dla Firm foldery i OneNote notesy.
- Office aplikacja skaluje się automatycznie. Office 365 nowoczesne licencjonowanie sprawdza przypisanie licencji użytkownika co 72 godziny i konwertuje aplikacje Office na wersję, która jest taka, jak subskrypcja użytkownika.

### <a name="windows-10"></a>Windows 10

Jeśli Twoje Windows nie są jeszcze w aktualizacji Windows Pro, uaktualnij je do Windows Pro [dla twórców.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurowanie zasad ochrony urządzeń i plików użytkowników

> [!NOTE]
> Jeśli skonfigurujesz zasady Office 365 mdM, te urządzenia będą wyświetlane  na stronie Urządzenia w centrum administracyjnym usługi Microsoft 365. Wszystkie zasady, które skonfigurujsz, będą wyświetlane na liście zasad klasycznych w [portalu usługi Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Po przypisaniu licencji do Microsoft 365 Business Premium możesz rozpocząć ochronę urządzeń i plików użytkowników.

Jeśli wszystkie osoby w organizacji zostały uaktualnione do programu Microsoft 365 Business Premium, na stronie głównej zostanie wyświetlony kreator konfiguracji, który może wykonać instrukcje Konfigurowanie usługi [Microsoft 365 Business Premium](set-up.md) w kreatorze konfiguracji w celu ochrony plików i urządzeń przenośnych.

Na stronie Urządzenia możesz również wykonać następujące czynności:
  
1. W centrum administracyjnym w lewym okienku narracji przejdź do **pozycji Zasady dotyczące** \> **urządzeń.**

2. Na stronie **Zasady dotyczące urządzeń** wybierz pozycję **Dodaj**.

3. W **okienku Dodaj** zasady nadaj zasadom nazwę, **a** następnie z listy rozwijanej wybierz typ zasad.

     Możesz skonfigurować zasady aplikacji do ochrony plików na urządzeniach z systemami Android i iPhone, a także Windows 10, a także dla firmowych urządzeń Windows 10 urządzeniach. Aby uzyskać szczegółowe informacje, zobacz następujące linki:

  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md)

  - [Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10](protection-settings-for-windows-10-devices.md)

  - [Konfigurowanie ustawień ochrony urządzeń dla Windows 10 PC](protection-settings-for-windows-10-pcs.md)
  
4. Po skonfigurowaniu zasad Ty i Twoi pracownicy możecie skonfigurować urządzenia:

  - Zobacz [Konfigurowanie Windows dla Microsoft 365 Business Premium,](set-up-windows-devices.md) aby uzyskać instrukcje dotyczące Windows urządzeniach. 

  - Zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business Premium,](set-up-mobile-devices.md) aby uzyskać instrukcje dotyczące telefonów iPhone i telefonów z systemem Android. 
  
### <a name="mailbox-size"></a>Rozmiar skrzynki pocztowej

Microsoft 365 Business Premium ma limit przestrzeni dyskowej 50 GB, ponieważ korzysta z Exchange Online Plan 1. Jeśli podczas migracji do programu Microsoft 365 Business Premium żaden z użytkowników przekracza 50 GB miejsca do magazynowania skrzynki pocztowej, zaleca się przypisanie temu użytkownikowi planu Exchange Online 2 i usunięcie planu Exchange Online Plan 1, ponieważ nie jest możliwe przypisanie obu tych wartości.

### <a name="threat-protection"></a>Ochrona przed zagrożeniami

Po zakończeniu migracji do programu Microsoft 365 Business Premium masz już programu Defender for Office 365. Aby [uzyskać omówienie Office 365](../security/office-365-security/defender-for-office-365.md) zobacz Program Microsoft Defender, aby uzyskać więcej informacji. Aby to skonfigurować, zobacz konfigurowanie linków Sejf [,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [konfigurowanie](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)załączników Sejf i konfigurowanie ochrony przed wyłudzaniem informacji w programie Defender dla [systemu Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Etykiety wrażliwości

Aby rozpocząć korzystanie z etykiet wrażliwości, zobacz [Omówienie etykiet wrażliwości](../compliance/sensitivity-labels.md) oraz tworzenie etykiet wrażliwości i zarządzanie nimi — [klip](../business-video/create-sensitivity-labels.md) wideo.
