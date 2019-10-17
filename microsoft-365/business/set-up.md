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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować firmę Microsoft 365 Business.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575553"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurowanie Microsoft 365 Business w Kreatorze instalacji

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i Konfigurowanie zasad

[![Etykieta, aby poinformować, że centrum admin zmienia się i można znaleźć więcej szczegółów na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Podczas zakupu Microsoft 365 Business, masz możliwość korzystania z domeny, którą posiadasz, lub kupując go podczas [rejestracji](sign-up.md).

- Jeśli po zalogowaniu się zarejestrowano nową domenę, domena jest ustawiona i można ją przenieść, aby [dodać użytkowników i przypisać licencje](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu personalizacji logowania

1. Zaloguj się do [Centrum administracyjnego Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz pozycję **Dodaj domenę** lub **Dodaj użytkowników** , aby uruchomić kreatora.
    > [!IMPORTANT]
    > Jeśli domena została kupiona podczas rejestracji, nie zobaczysz tutaj kroku **Dodaj domenę** . Idź do [Dodaj użytkowników](#add-users-and-assign-licenses) zamiast.

    ![Wybierz pozycję Przejdź do konfiguracji.](media/gotosetupinadmincenter.png)
    
3. W Kreatorze wprowadź nazwę domeny, której chcesz użyć (np. contoso.com).


    ![Zrzut ekranu Personalizuj swoją stronę logowania.](media/personalizesignin.png)

    
4. Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS w dowolnym dostawcy hostingu DNS dla pakietu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , który weryfikuje właścicielem domeny. Jeśli znasz swojego hosta domeny, zobacz także instrukcje dotyczące [hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jeśli dostawcą hostingu jest firma GoDaddy lub inny host z włączoną funkcją [Domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces jest łatwy, a użytkownik zostanie automatycznie poproszony o zalogowanie się i niech Microsoft uwierzytelni się w Twoim imieniu:

    ![Na stronie Potwierdzanie dostępu GoDaddy wybierz Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

Można dodać użytkowników w kreatorze, ale można również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym. Ponadto jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników w Kreatorze

Wszyscy użytkownicy dodawani w Kreatorze otrzymują automatycznie przypisaną licencję Microsoft 365 Business.

![Zrzut ekranu Dodaj nowych użytkowników strony w Kreatorze](media/addnewuserspage.png)

1. Jeśli Twoja subskrypcja Microsoft 365 Business ma istniejących użytkowników (na przykład, jeśli używasz programu Azure AD Connect), masz możliwość przypisania licencji do nich teraz. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników otrzymasz również opcję udostępnienia poświadczeń nowym użytkownikom, które dodałeś. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

3. Na stronie Tworzenie zespołów w organizacji można wybrać opcję dodawania zespołów i dodawania do nich użytkowników. Można również to zrobić później. Aby uzyskać więcej informacji, zobacz [Tworzenie zespołu w całej firmie](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).

4. Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**. 

    Jeśli przenoś się z innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [przenieść pocztę e-mail i kontakty do pakietu Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli zdecydujesz się użyć domeny. onmicrosoft lub użyć usługi Azure AD Connect do konfigurowania użytkowników, nie zobaczysz tego kroku.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak się nie [stanie, Zmień serwery nazw, aby skonfigurować pakiet Office 365 z dowolnym rejestratorem domeny](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale Twój host DNS jest włączony dla [połączenia z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), wybierz opcję **Dodaj rekordy dla mnie**. Na stronie **Wybieranie usług online** Zaakceptuj wszystkie ustawienia domyślne i wybierz pozycję **dalej**, a następnie wybierz pozycję **AUTORYZUJ** na stronie hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie jest włączona dla połączenia z domeną), będziesz chciał zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostać w kontakcie. Więcej informacji znajdziesz w artykule [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Połącz stronę domeny z zarządzam własnymi rekordami DNS.](media/connectyourdomainpage.png)

2. Postępuj zgodnie z instrukcjami kreatora, a poczta e-mail i inne usługi zostaną skonfigurowane.

### <a name="protect-data-and-devices"></a>Chroń dane i urządzenia 

Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*. Można również utworzyć dodatkowe grupy, aby przypisać zasady w centrum administracyjnym.

1. Na stronie **Chroń pliki robocze na urządzeniach przenośnych** opcja **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** , jest domyślnie zaznaczona. Masz opcję, aby włączyć zarządzanie, **jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych**, a to jest zalecane.

    ![Zrzut ekranu z Chroń pliki robocze na urządzeniach przenośnych strony.](media/protectworkfilesondevices.png)

     - Rozwiń pozycję **Chroń pliki robocze, gdy urządzenia zostaną zgubione lub skradzione** , aby wyświetlić [wartości domyślne](protect-work-files-on-lost-or-stolen-device.md):

        ![Zrzut ekranu z wartościami domyślnymi chroniącymi pliki na utraconych urządzeniach.](media/protectworkfilesondevicesdefault.png)

    - Wybierz **Zarządzaj, jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych** i rozwiń go, aby wyświetlić [wartości domyślne](manage-user-access-on-mobile-devices.md). Zaleca się zaakceptowanie wartości domyślnych podczas instalacji, aby utworzyć zasady aplikacji dla systemu Android, iOS i Windows 10, które mają zastosowanie do wszystkich użytkowników. Po zakończeniu instalacji możesz utworzyć więcej zasad.

        ![Zrzut ekranu ustawień ochrony dla plików pakietu Office na urządzeniach przenośnych.](media/useraccessonmobile.png)

2. Ostatni krok na temat ochrony danych i urządzeń umożliwia konfigurowanie zasad zabezpieczania urządzeń z systemem Windows 10. Te ustawienia są stosowane automatycznie, gdy użytkownik Windows 10 łączy się z organizacją. Można rozwinąć **bezpieczne urządzenia z systemem Windows 10** , aby zobaczyć i zmodyfikować [wartości domyślne](secure-windows-10-devices.md).
3. Można również wybrać opcję [automatycznej instalacji pakietu Office](install-office-on-windows-10-during-setup.md) na urządzeniach z systemem Windows 10.

    ![Zrzut ekranu zestawu Windows 10 konfiguracji urządzenia strony.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich pakietu Office 365

Jeśli wybrano automatyczne instalowanie aplikacji pakietu Office w trakcie konfigurowania, aplikacje zostaną zainstalowane na urządzeniach z systemem Windows 10, gdy użytkownicy zalogują się do usługi Azure AD z ich urządzeń z systemem Windows przy użyciu poświadczeń pracy.
Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business](set-up-mobile-devices.md).

Pakiet Office można również zainstalować osobno. Instrukcje znajdziesz [w artykule Instalowanie pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .
