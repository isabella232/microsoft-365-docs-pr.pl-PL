---
title: Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączonych do domeny przez usługę Microsoft 365 dla firm
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
description: Dowiedz się, jak w kilku krokach umożliwić programowi Microsoft 365 ochronę lokalnych urządzeń z systemem Windows 10 połączonych z usługą Active Directory.
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533790"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączanym do domeny przez usługę Microsoft 365 Business Premium

Jeśli twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, można skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, można zaimplementować **urządzenia przyłączone do usługi Azure AD.** Te urządzenia są przyłączane zarówno do lokalnej usługi Active Directory, jak i usługi Azure Active Directory.

W tym klipie wideo opisano kroki dotyczące konfigurowania tego dla najbardziej typowych scenariuszy, który jest również szczegółowo opisany w kolejnych krokach.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Zanim zaczniesz, wykonaj następujące czynności:
- Synchronizowanie użytkowników z usługą Azure AD z usługą Azure AD Connect.
- Pełna synchronizacja jednostki organizacyjnej usługi Azure AD Connect(OU).
- Upewnij się, że wszyscy synchronizowani użytkownicy domeny mają licencje na usługę Microsoft 365 Business Premium.

Aby uzyskać [instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Sprawdź urząd MDM w usłudze Intune

Przejdź do portal.azure.com i w górnej części strony wyszukaj usługę Intune.
Na stronie Usługi Microsoft Intune wybierz pozycję **Rejestracja na urządzenia** i na stronie **Przegląd** upewnij się, że **urzędem MDM** jest **usługa Intune**.

- Jeśli **urząd MDM** to **Brak,** kliknij **urząd MDM,** aby ustawić go na **Intune**.
- Jeśli **urzędem MDM** jest **usługa Microsoft Office 365,** przejdź do urządzenia **Devices**  >  **Rejestruj urządzenia** i użyj okna dialogowego **Dodaj urząd MDM** po prawej stronie, aby dodać uprawnienia **MDM usługi Intune** (okno dialogowe **Dodaj urząd MDM** jest dostępne tylko wtedy, gdy **urząd MDM** jest ustawiony na usługę Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Sprawdź, czy usługa Azure AD jest włączona do łączenia komputerów

- Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> i wybierz pozycję Usługa Azure Active **Directory** (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory nie jest widoczna) na liście **Centra administracyjne.** 
- W **centrum administracyjnym usługi Azure Active Directory**przejdź do **usługi Azure Active Directory** , wybierz pozycję **Urządzenia,** a następnie **ustawienia urządzenia**.
- Sprawdź, czy**użytkownicy mogą dołączać urządzenia do usługi Azure AD** jest włączona 
    1. Aby włączyć wszystkich użytkowników, ustaw opcję **Wszystkie**.
    2. Aby włączyć określonych użytkowników, ustaw opcję **Wybrane,** aby włączyć określoną grupę użytkowników.
        - Dodaj żądanych użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń](../admin/create-groups/create-groups.md).
        - Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkownika mdm dla tej grupy zabezpieczeń.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Sprawdź, czy usługa Azure AD jest włączona dla usługi MDM

- Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> i wybierz pozycję **Endpoint Managemen**t (wybierz pozycję **Pokaż wszystko,** jeśli **Menedżer punktów końcowych** nie jest widoczny)
- W **centrum administracyjnym programu Microsoft Endpoint Manager**przejdź do **pozycji Urządzenia**Rejestracji systemu  >  **Windows**  >  **Windows Enrollment**  >  **Rejestracja automatyczna rejestracja**systemu .
- Sprawdź, czy zakres użytkownika MDM jest włączony.

    1. Aby zarejestrować wszystkie komputery, ustaw opcję **Wszystkie,** aby automatycznie rejestrować wszystkie komputery użytkowników, które są przyłączone do usługi Azure AD i nowe komputery, gdy użytkownicy dodają konto służbowe do systemu Windows.
    2. Ustaw na **Niektóre,** aby zarejestrować komputery określonej grupy użytkowników.
        -  Dodaj żądanych użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń](../admin/create-groups/create-groups.md).
        -  Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkownika mdm dla tej grupy zabezpieczeń.

## <a name="4-create-the-required-resources"></a>4. Tworzenie wymaganych zasobów 

Wykonywanie zadań wymaganych do [konfigurowania hybrydowego sprzężenia usługi Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki zastosowaniu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) znalezionego w module [Programu SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. Po wywołaniu tego polecenia cmdlet utworzy i skonfiguruje wymagany punkt połączenia usługi i zasady grupy.

Ten moduł można zainstalować, wywołując następujące z wystąpienia programu PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Zaleca się zainstalowanie tego modułu w systemie Windows Server z systemem Azure AD Connect.

Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Podczas wykonywania tego zadania potrzebne będą poświadczenia administratora globalnego usługi Microsoft 365 Business Premium. Gdy chcesz utworzyć zasoby, należy wywołać następujące kwestie:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Pierwsze polecenie nawiąza połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Połącz zasady grupy

1. W konsoli zarządzania zasadami grupy (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, a następnie wybierz polecenie *Połącz istniejący obiekt zasad grupy...* z menu kontekstowego.
2. Wybierz zasady utworzone w powyższym kroku, a następnie kliknij przycisk **OK**.

## <a name="get-the-latest-administrative-templates"></a>Pobierz najnowsze szablony administracyjne

Jeśli zasady nie są widoczne **Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego serwera ADMX dla systemu Windows 10, wersja 1803, wersja 1809 lub wersja 1903. Aby rozwiązać ten problem, wykonaj następujące kroki (Uwaga: najnowszy plik MDM.admx jest zgodny wstecz:

1.  Pobierz: [Szablony administracyjne (admx) dla systemu Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Zainstaluj pakiet na podstawowym kontrolerze domeny (PDC).
3.  Przejdź, w zależności od wersji do folderu: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.
4.  Zmień nazwę folderu **Definicje zasad** na powyższej ścieżce na **PolicyDefinitions**.
5.  Kopiuj folder **PolicyDefinitions** do **folderu C:\Windows\SYSVOL\domain\Policies**. 
    -   Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość policyDefinitions.
6.  Uruchom ponownie podstawowy kontroler domeny, aby zasady były dostępne. Ta procedura będzie działać dla każdej przyszłej wersji, jak również.

W tym momencie powinieneś być w stanie zobaczyć zasady **Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD** dostępne.
