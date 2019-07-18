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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować Microsoft 365 Business.
ms.openlocfilehash: ac9c8b828ff131a15bf057fa8bdc0bf56dd00987
ms.sourcegitcommit: 75b97d1ff617bc4b1b0ef9135dfe6a8842ea1b52
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/18/2019
ms.locfileid: "35772572"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurowanie Microsoft 365 Business w Kreatorze instalacji

## <a name="add-your-domain-users-and-set-up-policies"></a>Domeny, użytkownicy, dodawanie i konfigurowanie zasad

![Transparent odsyłających do https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Kupując Microsoft 365 Business, istnieje możliwość korzystania z własnej domeny lub kupić jeden podczas [zapisywania się](sign-up.md).

- Jeśli zakupiono nową domenę podczas rejestracji, domeny jest ustawiona w górę i można przenieść do [dodawania użytkowników i przypisywanie licencji](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny do spersonalizowania logowanie

1. Zaloguj się do [Centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz polecenie **Dodaj domenę** lub **Dodawanie użytkowników** , aby uruchomić kreatora.
    > [!IMPORTANT]
    > Jeśli zakupiono domeny podczas rejestracji, będzie nie się **dodać domenę** krok tutaj. Przejdź do [Dodawanie użytkowników](#add-users-and-assign-licenses) .

    ![Wybierz Dodaj domenę.](media/addadomainadmincenter.png)
    
3. W Kreatorze wprowadź nazwę domeny, którą chcesz użyć (np. contoso.com).


    ![Zrzut ekranu Personalizuj stronę logowania.](media/personalizesignin.png)

    
4. Postępuj zgodnie z instrukcjami w kreatorze [Tworzenie rekordów DNS u dowolnego dostawcy usług hosta DNS dla usługi Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sprawdza, czy użytkownik jest właścicielem domeny. Jeśli znasz hostem domeny, zobacz też [host konkretne instrukcje](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jeśli dostawcą hostingu jest GoDaddy, proces jest łatwe i automatycznie uzyskasz zalogować się i powiadomić firmę Microsoft uwierzytelniania w Twoim imieniu:

    ![Na stronie Potwierdzenie dostępu GoDaddy wybierz opcję Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

W kreatorze można dodawać użytkowników, ale można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym. Dodatkowo Jeśli w komputerze znajduje się kontroler domeny lokalnej, można dodać użytkowników z [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Dodaj użytkowników w Kreatorze

Wszyscy użytkownicy, które można dodać w Kreatorze uzyskać automatycznie przypisywany licencji Microsoft 365 Business.

![Zrzut ekranu strony Dodaj nowych użytkowników w Kreatorze](media/addnewuserspage.png)

1. Jeśli subskrypcja Microsoft 365 Business istniejących użytkowników (na przykład, jeśli użyto Azure Połącz AD), masz możliwość przypisania licencji do nich teraz. Możesz dodać licencje dla tych użytkowników.

3. Po dodaniu użytkowników otrzymają również opcję udostępniania poświadczeń z nowych użytkowników, które zostały dodane. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

4. Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**. 

    Jeśli jest przesuwana od innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [migracji wiadomości e-mail i kontaktów do usługi Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli wybrany do korzystania z domeny .onmicrosoft lub Azure AD Connect umożliwia konfigurowanie użytkowników, nie zobaczysz ten krok.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak nie jest, [Zmień serwery nazw do skonfigurowania usługi Office 365 z dowolnym domen](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącej witryny sieci web, można zarządzać własne rekordy DNS, aby upewnić się, że łączność istniejących usług. Zobacz [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) , aby uzyskać więcej informacji.

        ![Domeny połączyć stronę z I zarządzać własną rekordów DNS.](media/connectyourdomainpage.png)

2. Postępuj zgodnie z instrukcjami w kreatorze i poczty e-mail i innych usług ustala się dla Ciebie.

### <a name="set-up-security-policies-and-device-configurations"></a>Konfigurowanie zasad zabezpieczeń i konfiguracji urządzeń 

Zasady, które można skonfigurować w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*. Można również utworzyć dodatkowe grupy do przypisywania zasad do w Centrum administracyjnym.

1. Na **chronić pliki praca na urządzeniach przenośnych** opcję **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** jest zaznaczone domyślnie. Masz możliwość włączyć **Zarządzanie dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych**i jest to zalecane.

    ![Zrzut ekranu chronić pliki pracy na stronie dla urządzeń przenośnych.](media/protectworkfilesondevices.png)

     - Rozwiń **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** , aby wyświetlić [wartości domyślnych](protect-work-files-on-lost-or-stolen-device.md):

        ![Zrzut ekranu z wartości domyślne dla ochrony plików na urządzeniach utracone.](media/protectworkfilesondevicesdefault.png)

    - Wybierz polecenie **Zarządzaj dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** i rozwinąć, aby wyświetlić [wartości domyślne](manage-user-access-on-mobile-devices.md). Firma Microsoft zaleca, aby zaakceptować wartości domyślne podczas instalacji do tworzenia zasad aplikacji dla Androida, iOS i 10 systemu Windows, które dotyczą wszystkich użytkowników. Po zakończeniu instalacji możesz utworzyć więcej zasad.

        ![Zrzut ekranu ustawienia ochrony dla plików pakietu Office na telefon komórkowy.](media/useraccessonmobile.png)

2. Ostatni krok na ochronę danych i urządzeń umożliwia konfigurowanie zasad w celu zabezpieczenia systemu Windows 10 urządzeń. Te ustawienia są stosowane automatycznie, gdy użytkownik systemu Windows 10 łączy się z organizacji. Po rozwinięciu **Secure Windows 10 urządzenia** , aby wyświetlić i zmodyfikować [wartości domyślne](secure-windows-10-devices.md).
3. Można także [automatycznie zainstalować pakiet Office](install-office-on-windows-10-during-setup.md) na urządzeniach Windows 10.

    ![Zrzut ekranu przedstawiający Ustaw stronę konfiguracji urządzenia Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich pakietu Office 365

Jeśli wybrano opcję automatycznie zainstalować aplikacje pakietu Office w trakcie zestaw się, aplikacje zainstaluje na urządzeniach Windows 10 po użytkowników jest zarejestrowany w programie Azure AD z ich urządzeń systemu Windows przy użyciu poświadczeń pracy.
Aby zainstalować pakiet Office na przenośnym lub tabletu, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników biznesowych 365 firmy Microsoft](set-up-mobile-devices.md).

Można także zainstalować Office indywidualnie. Zobacz [instalacji pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) , aby uzyskać instrukcje.
