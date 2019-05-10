---
title: Konfigurowanie usługi Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660864"
---
# <a name="set-up-microsoft-365-business"></a>Konfigurowanie usługi Microsoft 365 Business

Przed rozpoczęciem pracy, zobacz [Uzyskiwanie Microsoft Business 365](get-microsoft-365-business.md) szczegółowe zapisywania się.

Obejrzyj [krótki klip wideo o tym, jak skonfigurować Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) przy użyciu zestawu kreatora, a gdy nie ma usługi Active Directory na lokalnym
  

## <a name="overview"></a>Omówienie

Większość ustawień czynności może odbywać się w Kreatorze instalacji, ale inne opcje są również wyświetlane.

1. [Dodawanie domeny](#add-your-domain-to-personalize-sign-in) (jeśli kupiłeś domeny podczas [zarejestrować się](sign-up.md), ten krok jest już zrobione.)
2. Dodaj użytkowników. Możesz to zrobić na jeden z trzech sposobów:
    - W oknie [Kreatora instalacji](#add-users-in-the-wizard).
    - Użyj synchronizacji katalogów, aby [dodać użytkowników za pomocą Azure AD Connect](#add-users-by-using-azure-ad-connect) , jeśli masz lokalnej usługi Active directory.
    - Można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym.
3. Konfigurowanie zasad zabezpieczeń i skonfigurować urządzenia. Możesz to zrobić na jeden z trzech sposobów:
    - W oknie [Kreatora instalacji](#set-up-policies-in-the-wizard).  
    - W [Centrum administracyjnego](#modify-or-add-policies-in-the-admin-center).
    - W [Centrum administracyjnego usługi Intune](https://docs.microsoft.com/intune/what-is-device-management).
4. Konfigurowanie i zarządzanie urządzeniami Windows 10.

    Po dołączeniu urządzenia WIndows 10 do Azure AD wszystkich zasad będzie stosowane do niego.
    - Ustawianie konfiguracji urządzeń systemu Windows 10 w oknie [Kreatora instalacji](#set-up-policies-in-the-wizard).
    - Dołącz [nowe urządzenie Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) do Azure AD.
    - Dołącz do [istniejącego urządzenia Windows 10](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) do Azure AD.
1. Zainstaluj pakiet Office 365 Business.
    - Można automatycznie zainstalować pakiet Office w urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](#set-up-policies-in-the-wizard).
    - Automatycznie [zainstalować pakiet Office](auto-install-or-uninstall-office.md) z Centrum administracyjnego.
    - Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
1. Konfigurowanie dodatkowych zabezpieczeń.
    - Kreator instalacji dodaje zasad, aby zabezpieczyć swoje urządzenia, ale można również Państwo skorzystać z funkcji [dodatkowych zabezpieczeń](#additional-security-settings) pomaga chronić dane, kont i wiadomości e-mail. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i ustawianie zasad

![Transparent odsyłających do https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Kupując Microsoft 365 Business, istnieje możliwość korzystania z własnej domeny lub kupić jeden podczas [zapisywania się](sign-up.md).

- Jeśli zakupiono nową domenę podczas rejestracji, domeny jest ustawiona w górę i można przenieść do [dodawania użytkowników i przypisywanie licencji](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny do spersonalizowania logowanie

1. Zaloguj się do [Centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz przycisk **Dodaj domenę** , aby uruchomić kreatora.

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
Jeśli jest używany kontroler domeny lokalnej, a jest używana usługa Active Directory, zobacz [jak ddd użytkowników za pomocą Azure AD Connect](#add-users-by-using-azure-ad-connect).

![Zrzut ekranu strony Dodaj nowych użytkowników w Kreatorze](media/addnewuserspage.png)

1. Jeśli Twoja subskrypcja usługi Microsoft 365 Business zawiera już użytkowników (na przykład użyto narzędzia Azure AD Connect), zobaczysz opcję przypisania im licencji. Możesz dodać licencje dla tych użytkowników.

3. Po dodaniu użytkowników otrzymają również opcję udostępniania poświadczeń z nowych użytkowników, które zostały dodane. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

4. Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**. 

    Jeśli jest przesuwana od innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [migracji wiadomości e-mail i kontaktów do usługi Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>Dodawanie użytkowników za pomocą Azure AD Connect

 Jeśli masz kontroler domeny lokalnej z usługą Active Directory, synchronizowania użytkowników Microsoft 365 Business przy użyciu [Azure Połącz AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express). Zakończ to przed uruchomieniem Kreatora instalacji. Można go pobrać w Centrum administracyjnym:

- Przejdź do **użytkowników** \> **aktywnych użytkowników**, wybierz Wielokropek na górze strony, a następnie wybierz **synchronizacji katalogów** do pobrania Azure Połącz AD.

    ![Na stronie aktywnych użytkowników wybierz elipsy > katalog snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Jeśli tworzenie użytkowników w ten sposób będzie jeszcze do przypisywania licencji do nich w Centrum administracyjnym.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Dostęp do domeny aplikacji i urządzeń w dalszym ciągu

Jeśli chcesz w dalszym ciągu dostęp do domeny aplikacji i urządzeń, przeczytanie następujących artykułów dla dwóch różnych rozwiązanie pozwalające który:
  
- [Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10](manage-windows-devices.md)
    - Jest to zalecany sposób.

- [Dostęp do zasobów lokalnych z Azure urządzenia przyłączonych do AD w Microsoft 365 Business](access-resources.md)

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli wybrany do korzystania z domeny .onmicrosoft lub Azure AD Connect umożliwia konfigurowanie użytkowników, nie zobaczysz ten krok.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak nie jest, [Zmień serwery nazw do skonfigurowania usługi Office 365 z dowolnym domen](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącej witryny sieci web, można zarządzać własne rekordy DNS, aby upewnić się, że łączność istniejących usług. Zobacz [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) , aby uzyskać więcej informacji.

        ![Domeny połączyć stronę z I zarządzać własną rekordów DNS.](media/connectyourdomainpage.png)

2. Postępuj zgodnie z instrukcjami w kreatorze i poczty e-mail i innych usług ustala się dla Ciebie.

### <a name="set-up-security-policies-and-device-configurations"></a>Konfigurowanie zasad zabezpieczeń i konfiguracji urządzeń 

Te zasady są stosowane do każdego użytkownika, jeśli użytkownik chce przypisać różne zasady do zestawu użytkowników dać licencji, lub grupie użytkowników.

#### <a name="set-up-policies-in-the-wizard"></a>Ustawianie zasad w Kreatorze

Zasady, które można skonfigurować w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*.

1. Na **chronić pliki praca na urządzeniach przenośnych** opcję **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** jest zaznaczone domyślnie. Masz możliwość włączyć **Zarządzanie dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych**i jest to zalecane.

    ![Zrzut ekranu chronić pliki pracy na stronie dla urządzeń przenośnych.](media/protectworkfilesondevices.png)

     - Jeżeli rozwiniesz **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione**, [wartości domyślne](protect-work-files-on-lost-or-stolen-device.md) są wstępnie wybrane:

        ![Zrzut ekranu z wartości domyślne dla ochrony plików na urządzeniach utracone.](media/protectworkfilesondevicesdefault.png)

    - Wybierz polecenie **Zarządzaj dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** i rozwiń ją, wyświetlone zostaną [wartości domyślne](manage-user-access-on-mobile-devices.md) . Zalecane jest zaakceptowanie domyślnych wartości podczas instalacji w celu utworzenia zasad aplikacji dla systemów Android, iOS i Windows 10 dotyczących wszystkich użytkowników. Po zakończeniu instalacji możesz utworzyć więcej zasad.

        ![Zrzut ekranu ustawienia ochrony dla plików pakietu Office na telefon komórkowy.](media/useraccessonmobile.png)

2. Ostatni krok na ochronę danych i urządzeń umożliwia konfigurowanie zasad w celu zabezpieczenia systemu Windows 10 urządzeń. Te ustawienia są stosowane automatycznie, gdy użytkownik systemu Windows 10 łączy się z organizacji. Po rozwinięciu **Secure Windows 10 urządzenia** , aby wyświetlić i zmodyfikować [wartości domyślne](secure-windows-10-devices.md).
3. Można także [automatycznie zainstalować pakiet Office](install-office-on-windows-10-during-setup.md) na urządzeniach Windows 10.

    ![Zrzut ekranu przedstawiający Ustaw stronę konfiguracji urządzenia Windows 10.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Modyfikowanie lub Dodawanie zasady w Centrum administracyjnym

Zobacz [Zarządzanie Microsoft 365 Business](manage.md) dla zasady łącza do tematów dotyczących sposobu wyświetlania i modyfikowania ochrony urządzeń i aplikacji i jak usunąć dane z lub resetowania urządzenia użytkownika.

## <a name="deploy-and-manage-windows-10"></a>Wdrażanie i zarządzanie systemem Windows 10
Zobacz [Konfigurowanie urządzeń systemu Windows dla użytkowników biznesowych 365 firmy Microsoft,](set-up-windows-devices.md) Aby ręcznie połączyć Azure AD, albo w trakcie instalacji dla nowych komputerów lub zmieniając profilu rejestrowania dla istniejących komputerów. 

### <a name="use-autopilot-to-set-up-new-devices"></a>Służy do definiowania nowych urządzeń autopilota

Można użyć [Windows Autopilot](add-autopilot-devices-and-profile.md) automatycznie wstępnie skonfigurować **Nowe** urządzenia Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może zrobić to dla Ciebie. Można także przejść do [Magazyn Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) i zapytać specjalisty w zakresie technologii cloud Ustawianie nowych urządzeń, które kupić dla Ciebie.

### <a name="access-on-premises-resources"></a>Dostęp do zasobów lokalnych

Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych. Postępuj zgodnie z instrukcjami [włączyć przyłączonych do domeny Windows 10 urządzenia mają być zarządzane przez Microsoft 365 Business](manage-windows-devices.md) można wybrać tę opcję. Jest to preferowana metoda i urządzeń, w tym stanie są nazywane hybrydowy Azure AD dołączył do urządzenia.

Jeśli Twoja firma ma lokalnej usługi Active Directory, który zawiera niektóre zasobów lokalnych (takich jak udziały plików i drukarek), może dać Azure AD przyłączony urządzeniom dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostępu do zasobów lokalnych z Azure AD dołączył do urządzenia w Microsoft 365 Business](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich pakietu Office 365

Jeśli wybrano opcję automatycznie zainstalować aplikacje pakietu Office w trakcie zestaw się, aplikacje zainstaluje na urządzeniach Windows 10 po użytkowników jest zarejestrowany w programie Azure AD z ich urządzeń systemu Windows przy użyciu poświadczeń pracy.
Aby zainstalować pakiet Office na przenośnym lub tabletu, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników biznesowych 365 firmy Microsoft](set-up-mobile-devices.md).

Można także zainstalować Office indywidualnie. Zobacz [instalacji pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) , aby uzyskać instrukcje.

## <a name="additional-security-settings"></a>Dodatkowych ustawień zabezpieczeń

Oprócz zabezpieczeń i ustawienie zgodności w Kreatorze instalacji można skonfigurować następujące dodatkowe ustawienia:
  
- **E-mail, ochrona przed złośliwym oprogramowaniem**
- **Zaawansowane zagrożenia ochrony (ATP) bezpieczne załączniki**
- **Łącza bezpieczny ATP**
- **ZDOLNY anti-phishing**
- **Exchange Online  archiwum**
- **Zapobieganie utracie danych (DLP)**
- **Ochrona informacji Azure** (Plan 1)
- **Dostępność portalu Windows Intune**

Aby rozpocząć, zobacz [Konfigurowanie zasad zabezpieczeń zaawansowanych](set-up-advanced-security.md).

Zobacz też [top 10 sposobów zabezpieczenia firmy Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) do utworzenia planu działań najważniejsze wskazówki dotyczące zabezpieczeń.