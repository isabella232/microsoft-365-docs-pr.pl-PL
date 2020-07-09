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
description: Zapoznaj się z instrukcjami dotyczącymi konfiguracji usługi Microsoft 365 Business Premium, w tym dodawaniem domeny i użytkowników, konfigurowaniem zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081900"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurowanie usługi Microsoft 365 Business Premium w kreatorze instalacji

W tym klipie wideo przedstawiono omówienie konfiguracji usługi Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i konfigurowanie zasad

Kupując usługę Microsoft 365 Business Premium, możesz korzystać z domeny, której jesteś właścicielem, lub kupować ją podczas [rejestracji.](sign-up.md)

- Jeśli podczas zarejestrowania się zakupiono nową domenę, domena jest skonfigurowana i można przejść do [dodaj użytkowników i przypisać licencje](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu personalizacji logowania

1. Zaloguj się do [centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz **pozycję Przejdź do konfiguracji,** aby uruchomić kreatora.

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. Na stronie **Instalowanie aplikacji pakietu Office** możesz opcjonalnie zainstalować aplikacje na własnym komputerze.
    
4. W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).

    > [!IMPORTANT]
    > Jeśli domena została kupiona podczas rejestracji, nie zobaczysz tutaj kroku **Dodaj domenę.** Zamiast tego przejdź do [dodaj użytkowników.](#add-users-and-assign-licenses)

    ![Zrzut ekranu przedstawiający stronę Personalizowanie logowania.](../media/adddomain.png)

    
4. Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS u dowolnego dostawcy hostingu DNS dla usługi Microsoft 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) który weryfikuje, że jesteś właścicielem domeny. Jeśli znasz swojego hosta domeny, zapoznaj się również z [instrukcjami dotyczącymi hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jeśli twoim dostawcą hostingu jest GoDaddy lub inny host włączony z [domeną connect,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)proces jest łatwy i zostaniesz automatycznie poproszony o zalogowanie się i umożliwienie firmie Microsoft uwierzytelnienia w Twoim imieniu.

    ![Na stronie Potwierdzenie dostępu GoDaddy wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

W kreatorze można dodawać użytkowników, ale można również [dodawać użytkowników później](add-users-m365b.md) w centrum administracyjnym. Ponadto jeśli masz lokalny kontroler domeny, możesz dodawać użytkowników za pomocą [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników do kreatora

Każdy użytkownik dodany w kreatorze automatycznie otrzymuje licencję microsoft 365 Business Premium.

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w kreatorze](../media/addnewuserspage.png)

1. Jeśli subskrypcja usługi Microsoft 365 Business Premium ma istniejących użytkowników (na przykład jeśli używano usługi Azure AD Connect), otrzymasz opcję przypisania do nich licencji teraz. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników otrzymasz również opcję udostępniania poświadczeń nowym użytkownikom, których dodasz. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli wybrano użycie domeny .onmicrosoft lub użyto usługi Azure AD Connect do skonfigurowania użytkowników, ten krok nie zostanie wyświetlony.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli tak nie jest, [zmień serwery nazw, aby skonfigurować usługę Microsoft 365 z dowolnym rejestratorem domen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale host DNS jest włączony dla [połączenia z domeną,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)wybierz pozycję **Dodaj rekordy dla mnie**. Na stronie **Wybierz usługi online** zaakceptuj wszystkie wartości domyślne, a następnie wybierz pozycję **Dalej**, a następnie wybierz pozycję **Autoryzuj** na stronie hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (niewłączone dla łączenia domen), należy zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostają w kontakcie. Aby uzyskać więcej informacji, zobacz [podstawy domeny.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Aktywuj stronę rekordów.](../media/activaterecords.png)

2. Wykonaj kroki opisane w kreatorze, a poczta e-mail i inne usługi zostaną skonfigurowane dla Ciebie.

### <a name="protect-your-organization"></a>Ochrona organizacji 

Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*. Można również utworzyć dodatkowe grupy, do których można przypisać zasady w centrum administracyjnym.

1. W obszarze **Zwiększ ochronę przed zaawansowanymi zagrożeniami cybernetycznymi**zaleca się zaakceptowanie ustawień domyślnych, aby [usługa Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanować pliki i łącza w aplikacjach pakietu Office.

    ![Zrzut ekranu przedstawiający stronę Zwiększ ochronę.](../media/increasetreatprotection.png)


2. Na stronie **Zapobiegaj wyciekom poufnych danych** zaakceptuj domyślne włączanie usługi Office 365 Data Loss Prevention (DLP) w celu śledzenia poufnych danych w aplikacjach pakietu Office i zapobiegania przypadkowemu udostępnianiu tych danych poza organizacją.

3. Na stronie **Ochrona danych w pakiecie Office dla urządzeń przenośnych** pozostaw zarządzanie aplikacjami mobilnymi, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję **Utwórz zasady zarządzania aplikacjami mobilnymi**.

    ![Zrzut ekranu przedstawiający ochronę danych na stronie pakietu Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Bezpieczne komputery z systemem Windows 10

Po lewej stronie wybierz **pozycję Instalator,** a następnie w obszarze **Logowanie i zabezpieczenia**wybierz pozycję Zabezpiecz komputery z systemem Windows **10**. Wybierz **pozycję Widok,** aby rozpocząć. Aby uzyskać pełne [instrukcje, zobacz zabezpieczanie komputerów z systemem Windows 10.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich usługi Office 365

Jeśli podczas instalacji zostanie wybrana opcja automatycznego instalowania aplikacji pakietu Office, aplikacje zostaną zainstalowane na urządzeniach z systemem Windows 10 po zalogowaniu się użytkowników do usługi Azure AD z urządzeń z systemem Windows przy użyciu poświadczeń służbowych.

Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business Premium](set-up-mobile-devices.md).

Pakiet Office można również zainstalować indywidualnie. Aby uzyskać instrukcje, zobacz [instalowanie pakietu Office na komputerze PC lub Mac.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Zobacz też

[Wideo dotyczące szkoleń dotyczących usługi Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
