---
title: Konfigurowanie Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Zapoznaj się z krokami konfiguracji Microsoft 365 Business Premium, w tym dodawanie domeny i użytkowników, konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 74a98e915577cf86ec32a706bd3b8f558f49db95
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227644"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurowanie Microsoft 365 Business Premium kreatora konfiguracji

## <a name="watch-overview-of-microsoft-365-setup"></a>Obejrzyj: Omówienie konfigurowania Microsoft 365 projektu

Obejrzyj ten klip wideo, aby uzyskać omówienie Microsoft 365 Business Premium konfiguracji.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i konfigurowanie zasad

Podczas zakupu Microsoft 365 Business Premium masz możliwość używania domeny, która należy do Ciebie, lub kupowania jej podczas [rejestracji](sign-up.md).

- Jeśli podczas rejestracji w domenie kupiono nową domenę, to jest ona w ogóle ustawiona. Możesz przejść do dodawania użytkowników [i przypisywania licencji.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu spersonalizowania logowania

1. Zaloguj się [centrum administracyjne platformy Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz **pozycję Przejdź do konfiguracji,** aby uruchomić kreatora.

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. Na **stronie Instalowanie Office aplikacji** możesz opcjonalnie zainstalować te aplikacje na swoim komputerze.
    
4. W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).

    > [!IMPORTANT]
    > Jeśli podczas rejestracji zakupiono domenę, nie zobaczysz tutaj kroku **Dodaj** domenę. Zamiast tego [przejdź do przycisku Dodaj](#add-users-and-assign-licenses) użytkowników.

    ![Zrzut ekranu przedstawiający stronę Personalizowanie logowania.](../media/adddomain.png)

    
4. Postępuj zgodnie z instrukcjami kreatora, aby utworzyć rekordy DNS u dowolnego dostawcy [hostingu DNS](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) dla Microsoft 365 weryfikację prawa do domeny. Jeśli znasz hosta domeny, zobacz też [Dodawanie domeny do](/microsoft-365/admin/setup/add-domain)Microsoft 365.

    Jeśli Twój dostawca hostingu to Firma [](/office365/admin/get-help-with-domains/domain-connect)GoDaddy lub inny host z włączonym nawiązywaniem połączenia z domeną, ten proces jest łatwy i zostanie automatycznie poproszony o zalogowanie się i uwierzytelnienie przez firmę Microsoft w Twoim imieniu.

    ![Na stronie Potwierdzanie dostępu w daddy wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

Użytkowników można dodać w kreatorze, ale można też [dodać](../admin/add-users/add-users.md) ich później w centrum administracyjnym. Ponadto, jeśli masz lokalny kontroler domeny, możesz dodawać użytkowników z [usługą Azure AD Połączenie.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników w kreatorze

Użytkownicy, których dodasz w kreatorze, zostaną automatycznie przypisani do Microsoft 365 Business Premium licencji.

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w kreatorze](../media/addnewuserspage.png)

1. Jeśli Twoja Microsoft 365 Business Premium ma już użytkowników (na przykład jeśli używasz usługi Azure AD Połączenie), możesz teraz przypisać im licencje. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników zostanie również dodana opcja udostępnienia poświadczeń nowym użytkownikom. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli do skonfigurowania użytkowników wybrano domenę .onmicrosoft lub do skonfigurowania użytkowników była używana usługa Azure AD Połączenie, ten krok nie zostanie wyświetlony.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak się nie stanie, zmień serwery nazw, aby Microsoft 365 [u dowolnego rejestratora domen.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę internetową, ale dla Twojego hosta DNS włączono łączenie [domen,](/office365/admin/get-help-with-domains/domain-connect)wybierz pozycję **Dodaj rekordy.** Na stronie **Wybierz usługi online** zaakceptuj wszystkie ustawienia domyślne, wybierz pozycję **Dalej,** a następnie wybierz pozycję **Autoryzuj** na stronie swojego hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (bez włączonego łączenia domen), musisz zarządzać swoimi rekordami DNS, aby upewnić się, że istniejące usługi pozostają połączone. Aby [uzyskać więcej informacji, zobacz](/office365/admin/get-help-with-domains/dns-basics) Podstawowe informacje o domenie.

        ![Aktywowanie strony rekordów.](../media/activaterecords.png)

2. Postępuj zgodnie z instrukcjami kreatora, aby skonfigurować pocztę e-mail i inne usługi.

### <a name="protect-your-organization"></a>Ochrona organizacji 

Zasady ustawione w kreatorze są automatycznie stosowane do [grupy](/office365/admin/create-groups/compare-groups#security-groups) zabezpieczeń o nazwie *Wszyscy użytkownicy.* Możesz również utworzyć dodatkowe grupy, do których będą przypisywane zasady w centrum administracyjnym.

1. Na stronie Zwiększanie ochrony przed **zaawansowanymi zagrożeniami** cyberzagrożeniami zalecane jest zaakceptowanie ustawień domyślnych w celu Office 365 zaawansowanej ochrony przed zagrożeniami w plikach i linkach w Office aplikacjach. [](../security/office-365-security/defender-for-office-365.md)

    ![Zrzut ekranu przedstawiający stronę Zwiększanie ochrony.](../media/increasetreatprotection.png)


2. Na stronie **Zapobiegaj wyciekom poufnych** danych zaakceptuj wartości domyślne Office 365, aby włączyć zapobieganie utracie danych (DLP, Data Loss Prevention) w celu śledzenia poufnych danych w aplikacjach Office i zapobiegania przypadkowemu udostępnianiu tych danych poza Twoją organizacją.

3. Na stronie **Ochrona danych w aplikacji Office** dla urządzeń przenośnych pozostaw opcję zarządzanie aplikacją mobilną wł., rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję Utwórz zasady zarządzania aplikacją **mobilną.**

    ![Zrzut ekranu przedstawiający stronę Ochrona danych Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpieczanie Windows 10 komputerach

W okienku po lewej stronie wybierz pozycję **Konfiguracja,** a następnie w obszarze Logowanie się i zabezpieczenia wybierz pozycję Zabezpiecz swoje **Windows 10 komputerach**. Wybierz **pozycję Widok,** aby rozpocząć. Zobacz [Zabezpieczanie komputera Windows 10, aby](secure-win-10-pcs.md) uzyskać pełne instrukcje.

## <a name="deploy-office-365-client-apps"></a>Wdrażanie Office 365 klienckich

Jeśli podczas instalacji wybierzesz automatyczne instalowanie aplikacji Office, zostaną one zainstalowane na urządzeniach z systemem Windows 10 po zalogowaniu się użytkowników do usługi Azure AD na ich urządzeniach z systemem Windows przy użyciu poświadczeń służbowych.

Aby zainstalować Office urządzeniach przenośnych z systemem iOS lub Android, zobacz Konfigurowanie urządzeń przenośnych [Microsoft 365 Business Premium użytkowników.](set-up-mobile-devices.md)

Możesz również zainstalować pakiet Office instalacji pojedynczo. Aby [uzyskać instrukcje,](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) Office zainstalować pakiet na komputerze PC lub Mac.

## <a name="related-content"></a>Zawartość pokrewna

[Microsoft 365 szkoleniowe klipy wideo dla firm](../business-video/index.yml) (strona linku)
