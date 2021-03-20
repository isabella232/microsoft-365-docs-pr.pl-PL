---
title: Włączanie zarządzania przez platformę Microsoft 365 dla firm dla urządzeń przyłącznych do domeny systemu Windows 10
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
description: Dowiedz się, jak w kilku krokach włączyć ochronę lokalnych urządzeń z systemem Windows 10 przyłączanych do usługi Active Directory na platformie Microsoft 365.
ms.openlocfilehash: 82d4ac3f1d6aba9489f9ea153de3a3d2083b47ec
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913199"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Włączanie zarządzania przez usługę Microsoft 365 Business Premium dla urządzeń przyłączanych do domeny systemu Windows 10

Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, możesz zaimplementować urządzenia sprzężenia **hybrydowego usługi Azure AD.** Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i z usługą Azure Active Directory.

W tym klipie wideo opisano kroki, które należy wykonać w celu skonfigurowania tego najbardziej typowego scenariusza, a także szczegółowo opisano w poniższych krokach.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Przed rozpoczęciem upewnij się, że wykonaj następujące czynności:
- Zsynchronizowanie użytkowników z usługą Azure AD za pomocą programu Azure AD Connect.
- Ukończ synchronizację jednostek organizacyjnych usługi Azure AD Connect.
- Upewnij się, że wszyscy użytkownicy domeny, których synchronizujesz, mają licencje na usługę Microsoft 365 Business Premium.

Aby [uzyskać odpowiednie instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Weryfikowanie urzędu zarządzania usługą MDM w usłudze Intune

Przejdź do Menedżera [punktów końcowych](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) i na stronie Microsoft  Intune wybierz pozycję Rejestracja urządzeń **,** a następnie na stronie Omówienie upewnij się, że uprawnienia **MDM** to **Intune.**

- Jeśli **dla uprawnienia MDM jest** ustawiona wartość **Brak,** kliknij uprawnienia **MDM,** aby ustawić dla niego pozycję **Intune.**
- Jeśli uprawnienia **MDM** to usługa Microsoft Office  **365,** przejdź do strony Urządzenia Zarejestruj urządzenia i użyj okna dialogowego Dodawanie urzędu zarządzania mdM po prawej stronie, aby dodać uprawnienia usługi Intune MDM (okno dialogowe Dodawanie urzędu zarządzania mdm jest dostępne tylko wtedy, gdy dla uprawnienia MDM ustawiono usługę Microsoft Office  >   365).    

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Sprawdź, czy włączono usługę Azure AD, aby dołączać do komputerów

- Przejdź do centrum administracyjnego w miejscu i wybierz pozycję Azure Active Directory (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory jest niewidoczna) na liście <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Centra** administracyjne.  
- W centrum **administracyjnym usługi Azure Active Directory przejdź** do pozycji Azure Active **Directory** , wybierz **pozycję Urządzenia,** a następnie **pozycję Ustawienia urządzenia.**
- Sprawdzanie,**czy użytkownicy mogą dołączać do urządzeń w usłudze Azure AD** 
    1. Aby włączyć wszystkich użytkowników, ustaw wartość **Wszystkie.**
    2. Aby włączyć określonych użytkowników, ustaw wartość **Wybrani,** aby włączyć konkretną grupę użytkowników.
        - Dodaj do grupy zabezpieczeń żądanych użytkowników domeny zsynchronizowanych w [usłudze](../admin/create-groups/create-groups.md)Azure AD.
        - Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Sprawdzanie, czy usługa Azure AD jest włączona dla usługi MDM

- Przejdź do centrum administracyjnego w i <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> wybierz pozycję Zarządzanie  **punktami** końcowymi t (zaznacz pole wyboru Pokaż **wszystko,** jeśli menedżer punktów końcowych nie jest widoczny)
- W centrum **administracyjnym programu Microsoft Endpoint Manager** przejdź do pozycji Urządzenia **Rejestracja** automatyczna systemu Windows Rejestracja  >    >    >  **automatyczna systemu** Windows.
- Sprawdź, czy jest włączony zakres użytkowników usługi MDM.

    1. Aby zarejestrować wszystkie komputery, ustaw wartość Wszystkie w celu automatycznego zarejestrowania wszystkich komputerów użytkowników przyłącznych do usługi Azure AD i nowych komputerów, gdy użytkownicy dodają konto służbowe do systemu Windows. 
    2. Ustaw wartość **Some** (Niektóre), aby zarejestrować komputery określonej grupy użytkowników.
        -  Dodaj do grupy zabezpieczeń żądanych użytkowników domeny zsynchronizowanych w [usłudze](../admin/create-groups/create-groups.md)Azure AD.
        -  Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.

## <a name="4-create-the-required-resources"></a>4. Tworzenie wymaganych zasobów 

Wykonywanie wymaganych zadań w celu skonfigurowania hybrydowego sprzężenia usługi [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki użyciu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) w module [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. Wywoływanie tego polecenia cmdlet spowoduje utworzenie i skonfigurowanie wymaganego punktu połączenia usługi oraz zasad grupy.

Ten moduł można zainstalować, odwołując się do następującego wystąpienia programu PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Zalecane jest zainstalowanie tego modułu na serwerze Windows Server z uruchomionym programem Azure AD Connect.

Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Podczas wykonywania tego zadania będziesz potrzebować poświadczeń administratora globalnego usługi Microsoft 365 Business Premium. Gdy wszystko będzie gotowe do utworzenia zasobów, wywołaj następujące kwestie:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Pierwsze polecenie nawiązuje połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Połącz zasady grupy

1. W konsoli zasady grupy zarządzania (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, i wybierz z menu kontekstowego pozycję Połącz istniejący element *zasad* grupy.
2. Wybierz zasady utworzone w powyższym kroku, a następnie kliknij przycisk **OK.**

## <a name="get-the-latest-administrative-templates"></a>Pobierz najnowsze szablony administracyjne

Jeśli nie widzisz zasad Włącz automatyczną rejestrację mdM przy użyciu domyślnych poświadczeń usługi **Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego narzędzia ADMX dla systemu Windows 10 w wersji 1803 lub nowszej. Aby rozwiązać ten problem, wykonaj następujące czynności (Uwaga: najnowsza wersja pliku MDM.admx jest zgodna z poprzednimi wersjami):

1.  Pobierz: Szablony administracyjne (admx) dla systemu Windows 10 z października [2020 r. Aktualizacja (20H2)](https://www.microsoft.com/download/102157).
2.  Zainstaluj pakiet na Kontroler domeny.
3.  Przejdź do folderu w zależności od wersji szablonów administracyjnych: **C:\Program Files (x86)\Microsoft zasady grupy\Windows 10 October 2020 Update (20H2)**.
4.  Zmień nazwę **folderu Definicje** zasad na powyższej ścieżce do **folderu Definicje Zasad.**
5.  Skopiuj folder **PolicyDefinitions** do udziału SYSVOL, domyślnie znajdujący się w folderze **C:\Windows\SYSVOL\domain\Policies.** 
    -   Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość PolaOkreślenia Zasad.
6.  Jeśli masz kilka kontrolerów domeny, poczekaj, aż narzędzie SYSVOL zreplikuje te zasady, które będą dostępne. Ta procedura będzie działać również w przypadku każdej przyszłej wersji szablonów administracyjnych.

Na tym etapie powinny być dostępne zasady Włącz automatyczną rejestrację **w usłudze MDM przy użyciu domyślnych dostępnych poświadczeń usługi Azure AD.**