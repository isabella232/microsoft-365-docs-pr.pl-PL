---
title: Konfigurowanie usługi Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować usługę Microsoft 365 Business.
ms.openlocfilehash: c370a5b3fd735e704eea56ac1079bb2e5dad4c4b
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594274"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurowanie programu Microsoft 365 Business w kreatorze konfiguracji

Ten klip wideo zawiera omówienie konfiguracji usługi Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i konfigurowanie zasad

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Kupując usługę Microsoft 365 Business, możesz użyć domeny, której jesteś właścicielem, lub kupić ją podczas [rejestracji.](sign-up.md)

- Jeśli zakupiono nową domenę podczas rejestracji, domena jest skonfigurowana i możesz przejść do [dodaj użytkowników i przypisujesz licencje](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu personalizacji logowania

1. Zaloguj się do [centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu globalnych poświadczeń administratora. 

2. Wybierz **pozycję Przejdź do konfiguracji,** aby uruchomić kreatora.

    ![Wybierz przejdź do konfiguracji.](media/gotosetupinadmincenter.png)

3. Na stronie **Instalowanie aplikacji pakietu Office** można opcjonalnie zainstalować aplikacje na własnym komputerze.
    
4. W kroku **Dodawanie domeny** wprowadź nazwę domeny, której chcesz użyć (np. contoso.com).

    > [!IMPORTANT]
    > Jeśli domena została zakupiona podczas rejestracji, nie zobaczysz tutaj **kroku Dodaj domenę.** Przejdź do [dodaj użytkowników.](#add-users-and-assign-licenses)

    ![Zrzut ekranu przedstawiający stronę Personalizowanie logowania.](media/adddomain.png)

    
4. Wykonaj czynności kreatora tworzenia [rekordów DNS u dowolnego dostawcy hostingu DNS usługi Office 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) który weryfikuje domenę. Jeśli znasz hosta domeny, zobacz również [instrukcje dotyczące hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jeśli dostawcą usług hostingowych jest godaddy lub inny host z [włączoną funkcją łączenia domen,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)proces jest łatwy i zostaniesz automatycznie poproszony o zalogowanie się i wpuszczenie firmy Microsoft do uwierzytelnienia w Twoim imieniu.

    ![Na stronie GoDaddy Confirm Access wybierz pozycję Autoryzowania.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

Możesz dodać użytkowników w kreatorze, ale możesz też [dodawać użytkowników później](add-users-m365b.md) w centrum administracyjnym. Ponadto jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników w kreatorze

Wszyscy użytkownicy dodawani w kreatorze otrzymują automatycznie przypisaną licencję microsoft 365 Business.

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w kreatorze](media/addnewuserspage.png)

1. Jeśli subskrypcja usługi Microsoft 365 Business ma istniejących użytkowników (na przykład, jeśli użyto usługi Azure AD Connect), masz teraz opcję przypisywania do nich licencji. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników pojawi się również opcja udostępniania poświadczeń nowym dodanym użytkownikom. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli wybrano użycie domeny .onmicrosoft lub używane usługi Azure AD Connect do konfigurowania użytkowników, nie będzie widać tego kroku.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak się nie stanie, [zmień serwery nazw, aby skonfigurować usługę Office 365 z dowolnym rejestratorem domen](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale host DNS jest włączony do [łączenia domen,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)wybierz pozycję **Dodaj dla mnie rekordy**. Na stronie **Wybierz usługi online** zaakceptuj wszystkie ustawienia domyślne i wybierz pozycję **Dalej**i wybierz pozycję **Autoryzowania** na stronie hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie włączone dla połączenia domeny), musisz zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostają w kontakcie. Zobacz [podstawy domeny,](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) aby uzyskać więcej informacji.

        ![Strona Aktywuj rekordy.](media/activaterecords.png)

2. Wykonaj czynności kreatora i wiadomości e-mail i inne usługi zostaną skonfigurowane dla Ciebie.

### <a name="protect-your-organization"></a>Chroń swoją organizację 

Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*. Można również utworzyć dodatkowe grupy, do których można przypisać zasady w centrum administracyjnym.

1. W przypadku **aplikacji Zwiększ ochronę przed zaawansowanymi zagrożeniami cybernetycznymi**zaleca się zaakceptowanie wartości domyślnych, aby umożliwić usługi Office [365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanowanie plików i łączy w aplikacjach pakietu Office.

    ![Zrzut ekranu przedstawiający stronę Zwiększ ochronę.](media/increasetreatprotection.png)


2. Na stronie **Zapobiegaj wyciekom poufnych danych** zaakceptuj wartości domyślne, aby włączyć profilaktykę utraty danych usługi Office 365 (DLP), aby śledzić poufne dane w aplikacjach pakietu Office i zapobiec przypadkowemu udostępnieniu ich poza organizacją.

3. Na stronie **Chroń dane w pakiecie Office dla urządzeń przenośnych** pozostaw zarządzanie aplikacjami mobilnymi, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję **Utwórz zasady zarządzania aplikacjami mobilnymi**.

    ![Zrzut ekranu przedstawiający chroń dane na stronie pakietu Office dla urządzeń przenośnych.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Bezpieczne komputery z systemem Windows 10

Po lewej stronie urządzenia nawigacyjnego wybierz **pozycję Instalator,** a następnie w obszarze **Sing-in i zabezpieczeń**wybierz pozycję Zabezpiecz komputery z systemem Windows **10**. Wybierz **pozycję Widok,** aby rozpocząć. Aby uzyskać pełne instrukcje, zobacz [zabezpieczanie komputerów z systemem Windows 10.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich usługi Office 365

Jeśli w ybrano automatyczne instalowanie aplikacji pakietu Office podczas instalacji, aplikacje zostaną zainstalowane na urządzeniach z systemem Windows 10 po zalogowaniu się użytkowników do usługi Azure AD z urządzeń z systemem Windows przy użyciu poświadczeń służbowych.

Aby zainstalować pakiet Office na urządzeniach z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business](set-up-mobile-devices.md).

Pakiet Office można również zainstalować indywidualnie. Instrukcje można [znaleźć w pakiecie Office na komputerze PC lub Mac.](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Zobacz też

[Szkoleniowe klipy wideo dotyczące rozwiązania Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
