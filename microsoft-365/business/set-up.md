---
title: Konfigurowanie usługi Microsoft 365 Business
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
description: Dowiedz się, jak skonfigurować firmę Microsoft 365 Business.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831308"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurowanie Microsoft 365 Business w Kreatorze instalacji

Obejrzyj ten film, aby uzyskać omówienie konfiguracji firmy Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli znalazłeś ten film pomocne, sprawdź [kompletny cykl szkoleń dla małych firm i tych nowych Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i Konfigurowanie zasad

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Podczas zakupu Microsoft 365 Business, masz możliwość korzystania z domeny, którą posiadasz, lub kupując go podczas [rejestracji](sign-up.md).

- Jeśli po zalogowaniu się zarejestrowano nową domenę, domena jest ustawiona i można ją przenieść, aby [dodać użytkowników i przypisać licencje](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu personalizacji logowania

1. Zaloguj się do [Centrum administracyjnego Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz **Przejdź do konfiguracji** , aby uruchomić kreatora.

    ![Wybierz pozycję Przejdź do konfiguracji.](media/gotosetupinadmincenter.png)

3. Na stronie **Instalowanie aplikacji pakietu Office** można opcjonalnie instalować aplikacje na własnym komputerze.
    
4. W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (np. contoso.com).

    > [!IMPORTANT]
    > Jeśli domena została kupiona podczas rejestracji, nie zobaczysz tutaj kroku **Dodaj domenę** . Idź do [Dodaj użytkowników](#add-users-and-assign-licenses) zamiast.

    ![Zrzut ekranu Personalizuj swoją stronę logowania.](media/adddomain.png)

    
4. Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS w dowolnym dostawcy hostingu DNS dla pakietu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , który weryfikuje właścicielem domeny. Jeśli znasz swojego hosta domeny, zobacz także instrukcje dotyczące [hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jeśli dostawcą hostingu jest firma GoDaddy lub inny host z włączoną funkcją [Połącz z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces jest łatwy i automatycznie zostanie wyświetlony monit o zalogowanie się i pozwolić firmie Microsoft na uwierzytelnienie w Twoim imieniu.

    ![Na stronie Potwierdzanie dostępu GoDaddy wybierz Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

Można dodać użytkowników w kreatorze, ale można również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym. Ponadto jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników w Kreatorze

Wszyscy użytkownicy dodawani w Kreatorze otrzymują automatycznie przypisaną licencję Microsoft 365 Business.

![Zrzut ekranu Dodaj nowych użytkowników strony w Kreatorze](media/addnewuserspage.png)

1. Jeśli Twoja subskrypcja Microsoft 365 Business ma istniejących użytkowników (na przykład, jeśli używasz programu Azure AD Connect), masz możliwość przypisania licencji do nich teraz. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników otrzymasz również opcję udostępnienia poświadczeń nowym użytkownikom, które dodałeś. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli zdecydujesz się użyć domeny. onmicrosoft lub użyć usługi Azure AD Connect do konfigurowania użytkowników, nie zobaczysz tego kroku.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak się nie [stanie, Zmień serwery nazw, aby skonfigurować pakiet Office 365 z dowolnym rejestratorem domeny](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale Twój host DNS jest włączony dla [połączenia z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), wybierz opcję **Dodaj rekordy dla mnie**. Na stronie **Wybieranie usług online** Zaakceptuj wszystkie ustawienia domyślne i wybierz pozycję **dalej**, a następnie wybierz pozycję **AUTORYZUJ** na stronie hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie jest włączona dla połączenia z domeną), będziesz chciał zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostać w kontakcie. Więcej informacji znajdziesz w artykule [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Aktywuj rekordy strony.](media/activaterecords.png)

2. Postępuj zgodnie z instrukcjami kreatora, a poczta e-mail i inne usługi zostaną skonfigurowane.

### <a name="protect-your-organization"></a>Chroń swoją organizację 

Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*. Można również utworzyć dodatkowe grupy, aby przypisać zasady w centrum administracyjnym.

1. W sprawie **zwiększenia ochrony przed zaawansowanymi zagrożeniami cybernetycznymi**zaleca się zaakceptowanie wartości domyślnych, aby pozwolić, aby pliki skanowania [pakietu Office 365 z wyprzedzeniem ochrony przed zagrożeniami](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) i łącza w aplikacjach pakietu Office.

    ![Zrzut ekranu strony Zwiększ ochronę.](media/increasetreatprotection.png)


2. Na **zapobieganie przeciekom poufnych danych** strony, zaakceptuj ustawienia domyślne, aby włączyć Office 365 ochrony przed utratą danych (DLP) do śledzenia poufnych danych w aplikacjach pakietu Office i zapobiec przypadkowemu udostępnieniu tych poza organizacją.

3. Na stronie **Chroń dane w pakiecie Office dla urządzeń przenośnych** pozostaw Zarządzanie aplikacjami mobilnymi, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję **Utwórz zasady zarządzania aplikacjami mobilnymi**.

    ![Zrzut ekranu z Chroń dane w pakiecie Office dla urządzeń przenośnych strony.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Bezpieczne komputery z systemem Windows 10

Na lewej NAV wybierz **Ustawienia** , a następnie w obszarze **Sing-in i zabezpieczeń**, wybierz opcję **Zabezpiecz komputery z systemem Windows 10**. Wybierz **Widok** aby rozpocząć. Aby uzyskać pełne instrukcje, zobacz [Zabezpieczanie komputerów z systemem Windows 10](secure-win-10-pcs.md) .

## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich pakietu Office 365

Jeśli wybrano opcję automatycznego instalowania aplikacji pakietu Office podczas instalacji, aplikacje zostaną zainstalowane na urządzeniach z systemem Windows 10, gdy użytkownicy zalogują się do usługi Azure AD z ich urządzeń z systemem Windows przy użyciu poświadczeń pracy.

Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business](set-up-mobile-devices.md).

Pakiet Office można również zainstalować osobno. Instrukcje znajdziesz [w artykule Instalowanie pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>See also

[Filmy szkoleniowe Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
