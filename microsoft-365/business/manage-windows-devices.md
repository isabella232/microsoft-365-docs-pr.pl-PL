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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564956"
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

## <a name="4-set-up-service-connection-point-scp"></a>4. Konfigurowanie punktu połączenia usługi (SCP)

Te kroki są [uproszczone z konfigurowania hybrydowego połączenia usługi Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Aby wykonać kroki, musisz użyć usługi Azure AD Connect i globalnych haseł administratora i administratora usługi Active Directory usługi Microsoft 365 Business Premium.

1.  Uruchom usługę Azure AD Connect, a następnie wybierz pozycję **Konfiguruj**.
2.  Na stronie **Zadania dodatkowe** wybierz pozycję **Konfiguruj opcje urządzenia**, a następnie wybierz pozycję **Dalej**.
3.  Na stronie **Przegląd** wybierz pozycję **Dalej**.
4.  Na stronie **Połącz z usługą Azure AD** wprowadź poświadczenia administratora globalnego dla usługi Microsoft 365 Business Premium.
5.  Na stronie **Opcje urządzenia** wybierz pozycję **Konfiguruj hybrydowe sprzężenie usługi Azure AD,** a następnie wybierz pozycję **Dalej**.
6.  Na stronie **SCP** dla każdego lasu, w którym ma być skonfigurowany protokół SCP usługi Azure AD Connect, wykonaj następujące kroki, a następnie wybierz przycisk **Dalej:**
    - Zaznacz pole obok nazwy lasu. Las powinien być twoją nazwą domeny usługi AD.
    - W kolumnie **Usługa uwierzytelniania** otwórz listy rozwijanej i wybierz pasującą nazwę domeny (powinna istnieć tylko jedna opcja).
    - Wybierz **pozycję Dodaj,** aby wprowadzić poświadczenia administratora domeny.  
7.  Na stronie **Systemy operacyjne Urządzenia** wybierz tylko urządzenia z systemem Windows 10 lub nowszym.
8.  Na stronie **Gotowe do skonfigurowania** wybierz pozycję **Konfiguruj**.
9.  Na stronie **Konfiguracja zakończona** wybierz pozycję **Zakończ**.


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a>5. Tworzenie obiektu zasad grupy dla rejestracji usługi Intune — metoda ADMX

Używać. admx pliku szablonu.

1.  Zaloguj się do serwera USŁUGI AD, wyszukaj i otwórz **zarządzanie**  >  **Tools**  >  **zasadami grupy**Narzędzia Menedżera serwera .
2.  Wybierz nazwę domeny w obszarze **Domeny** i kliknij prawym przyciskiem myszy **pozycję Obiekty zasad grupy,** aby wybrać pozycję **Nowy**.
3.  Nadaj nowemu obiektowi obiektu zasad grupy nazwę, na przykład "*Cloud_Enrollment*", a następnie wybierz **przycisk OK**.
4.  Kliknij prawym przyciskiem myszy nowy obiekt zasad grupy w obszarze **Obiekty zasad grupy** i wybierz polecenie **Edytuj**.
5.  W **Edytorze zarządzania zasadami grupy**przejdź do **strony Zasady konfiguracji komputera**  >  **Policies**  >  **Szablony administracyjne składników**systemu  >  **Windows**  >  **MDM**.
6. Kliknij prawym przyciskiem myszy **pozycję Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD,** a następnie wybierz pozycję **Włączone**  >  **OK**. Zamknij okno edytora.

> [!IMPORTANT]
> Jeśli zasady nie są widoczne **włącz automatyczne rejestrowanie mdm przy użyciu domyślnych poświadczeń usługi Azure AD,** zobacz [Pobieranie najnowszych szablonów administracyjnych](#get-the-latest-administrative-templates).

## <a name="6-deploy-the-group-policy"></a>6. Wdrażanie zasad grupy

1.  W Menedżerze serwera w obszarze **Domeny** > obiekty zasad grupy wybierz obiekt zasad grupy z kroku 3 powyżej, na przykład "Cloud_Enrollment".
2.  Wybierz kartę **Zakres** dla obiektu zasad grupy.
3.  Na karcie Zakres obiektu zasad grupy kliknij prawym przyciskiem myszy łącze do domeny w obszarze **Łącza**.
4.  Wybierz **opcję Wymuszone,** aby wdrożyć obiekt zasad grupy, a następnie **przycisk OK** na ekranie potwierdzenia.

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

