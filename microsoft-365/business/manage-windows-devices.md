---
title: Włączanie zarządzania przez platformę Microsoft 365 dla firm na urządzeniach z systemem Windows 10 przyłączanych do domeny
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Dowiedz się, jak w kilku krokach włączyć na platformie Microsoft 365 ochronę lokalnych urządzeń z systemem Windows 10 przyłącznych do usługi Active Directory.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407083"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Włączanie zarządzania przez usługę Microsoft 365 Business Premium dla urządzeń przyłączanych do domeny systemu Windows 10

Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, możesz zaimplementować urządzenia sprzężenia hybrydowego usługi **Azure AD.** Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i z usługą Azure Active Directory.

W tym klipie wideo opisano czynności, które należy wykonać w celu skonfigurowania tego ustawienia dla najbardziej typowego scenariusza, co opisano również w poniższych krokach.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Przed rozpoczęciem upewnij się, że wykonaj następujące czynności:
- Synchronizowanie użytkowników z usługą Azure AD za pomocą programu Azure AD Connect.
- Ukończ synchronizację jednostki organizacyjnej programu Azure AD Connect.
- Upewnij się, że wszyscy użytkownicy domeny, których synchronizujesz, mają licencje na usługę Microsoft 365 Business Premium.

Aby [uzyskać odpowiednie instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Weryfikowanie uprawnień mdm w usłudze Intune

Przejdź do Menedżera [punktów](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) końcowych i na stronie Usługi  Microsoft Intune wybierz pozycję Rejestracja **urządzeń,** a następnie na stronie Omówienie upewnij się, że zarządzanie **usługą MDM** to **Intune.**

- Jeśli **dla uprawnień mdm**  jest ustawiona wartość **Brak,** kliknij je, aby ustawić dla niego pozycję **Intune.**
- Jeśli zarządzanie **mdm** to usługa Microsoft Office  **365,** przejdź do strony Urządzenia Zarejestruj urządzenia i użyj okna dialogowego Dodawanie urzędu mdm po prawej stronie, aby dodać uprawnienia usługi Intune MDM (okno dialogowe Dodawanie urzędu zarządzania mdm jest dostępne tylko wtedy, gdy dla uprawnienia MDM ustawiono usługę Microsoft Office  >   365).    

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Sprawdzanie, czy w usłudze Azure AD włączono dołączanie do komputerów

- Przejdź do centrum administracyjnego i wybierz pozycję Azure Active Directory (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory nie jest widoczna) na liście <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Centra** administracyjne.  
- W centrum **administracyjnym usługi Azure Active Directory przejdź** do usługi Azure Active **Directory,** wybierz **pozycję Urządzenia,** a następnie **pozycję Ustawienia urządzenia.**
- Sprawdzanie,**czy użytkownicy mogą dołączać urządzenia do usługi Azure AD** 
    1. Aby włączyć wszystkich użytkowników, ustaw wartość **All (Wszystko).**
    2. Aby włączyć określonych użytkowników, ustaw opcję **Wybrano** w celu włączenia określonej grupy użytkowników.
        - Dodaj odpowiednich użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń.](../admin/create-groups/create-groups.md)
        - Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Sprawdzanie, czy w usłudze Azure AD włączono usługę MDM

- Przejdź do centrum administracyjnego i wybierz pozycję Zarządzanie punktami końcowymi (wybierz pozycję Pokaż wszystko, jeśli Menedżer punktów <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> końcowych jest niewidoczny)  
- W centrum **administracyjnym programu Microsoft Endpoint Manager** przejdź do pozycji Urządzenia **z** automatyczną rejestracją systemu  >  **Windows** w systemie  >  **Windows.**  >  
- Sprawdzanie, czy zakres użytkowników usługi MDM jest włączony.

    1. Aby zarejestrować wszystkie komputery, ustaw wartość Wszystko tak, aby wszystkie komputery użytkowników, które są sprzężeniami z usługą Azure AD, i nowe komputery, gdy użytkownicy dodają konto służbowe w systemie Windows. 
    2. Ustaw wartość **Niektórzy,** aby zarejestrować komputery określonej grupy użytkowników.
        -  Dodaj odpowiednich użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń.](../admin/create-groups/create-groups.md)
        -  Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.

## <a name="4-create-the-required-resources"></a>4. Tworzenie wymaganych zasobów 

Wykonywanie wymaganych zadań w celu skonfigurowania hybrydowego sprzężenia usługi [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki użyciu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) które znajduje się w module PowerShell programu [SecMgmt.](https://www.powershellgallery.com/packages/SecMgmt) Po wywołaniu tego polecenia cmdlet utworzy ono i skonfiguruje wymagany punkt połączenia usługi oraz zasady grupy.

Ten moduł można zainstalować, inicjując następujące polecenia z wystąpienia programu PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Zalecamy zainstalowanie tego modułu na serwerze Windows Server z uruchomionym programem Azure AD Connect.

Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Podczas wykonywania tego zadania będziesz potrzebować poświadczeń administratora globalnego usługi Microsoft 365 Business Premium. Gdy wszystko będzie gotowe do utworzenia zasobów, wywołaj następujące elementy:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Pierwsze polecenie nawiąze połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Połącz zasady grupy

1. W konsoli zasady grupy zarządzania (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, i wybierz z menu kontekstowego pozycję Połącz istniejący element *zasad* grupy.
2. Wybierz zasady utworzone w powyższym kroku, a następnie kliknij **przycisk OK.**

## <a name="get-the-latest-administrative-templates"></a>Pobierz najnowsze szablony administracyjne

Jeśli nie widzisz zasad Włącz automatyczną rejestrację mdm przy użyciu domyślnych poświadczeń usługi **Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego narzędzia ADMX dla systemu Windows 10 w wersji 1803 lub nowszej. Aby rozwiązać ten problem, wykonaj następujące czynności (Uwaga: najnowsza wersja pliku MDM.admx jest zgodna ze starszymi wersjami):

1.  Pobierz: [Szablony administracyjne (admx) dla systemu Windows 10 aktualizacja z października 2020 r. (20H2).](https://www.microsoft.com/download/102157)
2.  Zainstaluj pakiet na Kontroler domeny.
3.  W zależności od wersji szablonów administracyjnych przejdź do folderu: **C:\Program Files (x86)\Microsoft zasady grupy\Windows 10 October 2020 Update (20H2).**
4.  Zmień nazwę **folderu Definicje** zasad na powyższej ścieżce **na PolicyDefinitions.**
5.  Skopiuj folder **PolicyDefinitions** do udziału SYSVOL, który domyślnie znajduje się w folderze **C:\Windows\SYSVOL\domain\Policies.** 
    -   Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość zasadDefinitions.
6.  Jeśli masz kilka kontrolerów domen, poczekaj, aż system SYSVOL zreplikuje te zasady, aby były dostępne. Ta procedura będzie działać również w przypadku każdej przyszłej wersji szablonów administracyjnych.

W tym momencie powinno być możliwe wyświetlanie zasad Włącz automatyczną rejestrację mdm przy użyciu domyślnych dostępnych **poświadczeń usługi Azure AD.**
