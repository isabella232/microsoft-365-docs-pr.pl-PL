---
title: Konfigurowanie usługi Microsoft 365 Business Premium
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z czynnościami konfiguracyjną usługi Microsoft 365 Business Premium, w tym dodawaniem domeny i użytkowników, konfigurowaniem zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: a06fb48ef5e1386a5c7b4df08500125f37943df6
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198447"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurowanie usługi Microsoft 365 Business Premium w kreatorze konfiguracji

Obejrzyj ten klip wideo, aby uzyskać omówienie konfiguracji usługi Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i konfigurowanie zasad

Przy zakupie usługi Microsoft 365 Business Premium masz możliwość użycia domeny, która należy do Ciebie, lub zakupu domeny podczas [jej rejestracji.](sign-up.md)

- Jeśli podczas rejestracji w domenie kupiono nową domenę, to jest ona w ogóle ustawiona. Możesz przejść do dodawania użytkowników [i przypisywania licencji.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu spersonalizowania logowania

1. Zaloguj się do [centrum administracyjnego platformy Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz **pozycję Przejdź do konfiguracji,** aby uruchomić kreatora.

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. Na stronie **Instalowanie aplikacji pakietu Office** możesz opcjonalnie zainstalować aplikacje na własnym komputerze.
    
4. W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).

    > [!IMPORTANT]
    > Jeśli podczas rejestracji zakupiono domenę, nie zobaczysz tutaj kroku **Dodaj** domenę. Zamiast tego [przejdź do przycisku Dodaj](#add-users-and-assign-licenses) użytkowników.

    ![Zrzut ekranu przedstawiający stronę Personalizowanie logowania.](../media/adddomain.png)

    
4. Postępuj zgodnie z instrukcjami kreatora, aby utworzyć rekordy DNS dla platformy [Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) u dowolnego dostawcy hostingu DNS, który weryfikuje, że jesteś właścicielem domeny. Jeśli znasz hosta domeny, zobacz też szczegółowe [instrukcje dla danego hosta.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Jeśli Twój dostawca hostingu to Firma [](/office365/admin/get-help-with-domains/domain-connect)GoDaddy lub inny host z włączonym nawiązywaniem połączenia z domeną, ten proces jest łatwy i zostanie automatycznie poproszony o zalogowanie się i uwierzytelnienie przez firmę Microsoft w Twoim imieniu.

    ![Na stronie Potwierdzanie dostępu w daddy wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

Użytkowników można dodać w kreatorze, ale można też [dodać](../admin/add-users/add-users.md) ich później w centrum administracyjnym. Ponadto, jeśli masz lokalny kontroler domeny, możesz dodawać użytkowników za pomocą [programu Azure AD Connect.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników w kreatorze

Każdy użytkownik, który dodasz w kreatorze, automatycznie otrzyma licencję na usługę Microsoft 365 Business Premium.

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w kreatorze](../media/addnewuserspage.png)

1. Jeśli Twoja subskrypcja usługi Microsoft 365 Business Premium ma już użytkowników (na przykład jeśli używasz programu Azure AD Connect), możesz teraz przypisać im licencje. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników zostanie również dodana opcja udostępnienia poświadczeń nowym użytkownikom. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli do skonfigurowania użytkowników wybrano domenę .onmicrosoft lub do skonfigurowania użytkowników był używany program Azure AD Connect, ten krok nie zostanie wyświetlony.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak się nie stanie, zmień serwery nazw, aby skonfigurować [usługę Microsoft 365 u dowolnego rejestratora domen.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę internetową, ale dla Twojego hosta DNS włączono łączenie [domen,](/office365/admin/get-help-with-domains/domain-connect)wybierz pozycję **Dodaj rekordy.** Na stronie **Wybierz usługi online** zaakceptuj wszystkie ustawienia domyślne, wybierz pozycję **Dalej,** a następnie wybierz pozycję **Autoryzuj** na stronie swojego hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (bez włączonego łączenia domen), musisz zarządzać swoimi rekordami DNS, aby upewnić się, że istniejące usługi pozostają połączone. Aby [uzyskać więcej informacji, zobacz](/office365/admin/get-help-with-domains/dns-basics) Podstawowe informacje o domenie.

        ![Aktywowanie strony rekordów.](../media/activaterecords.png)

2. Postępuj zgodnie z instrukcjami kreatora, aby skonfigurować pocztę e-mail i inne usługi.

### <a name="protect-your-organization"></a>Ochrona organizacji 

Zasady ustawione w kreatorze są automatycznie stosowane do [grupy](/office365/admin/create-groups/compare-groups#security-groups) zabezpieczeń o nazwie *Wszyscy użytkownicy.* Możesz również utworzyć dodatkowe grupy, do których będą przypisywane zasady w centrum administracyjnym.

1. Na stronie Zwiększanie ochrony przed **zaawansowanymi zagrożeniami** cyberzagrożeniami zalecane jest zaakceptowanie ustawień domyślnych, aby pliki i linki w aplikacjach pakietu Office można było skanować za pomocą funkcji Zaawansowana ochrona przed zagrożeniami w usłudze [Office 365.](../security/office-365-security/defender-for-office-365.md)

    ![Zrzut ekranu przedstawiający stronę Zwiększanie ochrony.](../media/increasetreatprotection.png)


2. Na stronie **Zapobiegaj wyciekom poufnych** danych zaakceptuj wartości domyślne, aby włączyć zapobieganie utracie danych (DLP, Data Loss Prevention) usługi Office 365 w celu śledzenia poufnych danych w aplikacjach pakietu Office i zapobiegania przypadkowemu udostępnianiu ich poza Twoją organizacją.

3. Na stronie **Ochrona danych w psłudze Office** dla urządzeń przenośnych pozostaw wł. pozycję Zarządzanie aplikacją mobilną, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję Utwórz zasady zarządzania **aplikacją mobilną.**

    ![Zrzut ekranu przedstawiający stronę Ochrona danych w psłudze Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpieczanie komputerów z systemem Windows 10

W okienku po lewej stronie wybierz pozycję **Konfiguracja,** a następnie w obszarze Logowanie i zabezpieczenia wybierz pozycję Zabezpiecz swoje komputery z **systemem Windows 10.** Wybierz **pozycję Widok,** aby rozpocząć. Zobacz Zabezpieczanie komputerów z systemem [Windows 10,](secure-win-10-pcs.md) aby uzyskać pełne instrukcje.

## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich usługi Office 365

Jeśli wybierzesz automatyczne instalowanie aplikacji pakietu Office podczas instalacji, zostaną one zainstalowane na urządzeniach z systemem Windows 10 po zalogowaniu się użytkowników do usługi Azure AD na swoich urządzeniach z systemem Windows przy użyciu poświadczeń służbowych.

Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz Konfigurowanie urządzeń przenośnych dla użytkowników usługi [Microsoft 365 Business Premium.](set-up-mobile-devices.md)

Możesz również zainstalować pakiet Office pojedynczo. Aby [uzyskać instrukcje, zobacz](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) Instalowanie pakietu Office na komputerze PC lub Mac.

## <a name="see-also"></a>Zobacz też

[Szkoleniowe klipy wideo dotyczące platformy Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
