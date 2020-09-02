---
title: Konfigurowanie programu Microsoft 365 Business Premium
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
description: Odkryj kroki konfiguracji programu Microsoft 365 Business Premium, w tym dodawanie domeny i użytkowników, Konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324501"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurowanie usługi Microsoft 365 Business Premium w Kreatorze konfiguracji

Obejrzyj ten klip wideo, aby zapoznać się z omówieniem konfiguracji programu Microsoft 365 Business Premium.<br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a>Dodawanie domeny, użytkowników i Konfigurowanie zasad

Po zakupie produktu Microsoft 365 Business Premium możesz korzystać z domeny, którą posiadasz, lub kupić ją podczas [tworzenia konta](sign-up.md).

- Jeśli nowa domena została zakupiona podczas tworzenia konta, Twoja domena jest skonfigurowana i możesz ją przenieść, aby [dodać użytkowników i przypisać licencje](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Dodawanie domeny w celu personalizacji logowania

1. Zaloguj się do [Centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego. 

2. Wybierz pozycję **Przejdź do konfiguracji** , aby uruchomić kreatora.

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. Na stronie **Instalowanie aplikacji pakietu Office** możesz opcjonalnie zainstalować aplikacje na własnym komputerze.
    
4. W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).

    > [!IMPORTANT]
    > Jeśli w trakcie tworzenia konta została kupiona domena, w tym miejscu nie będzie widoczny krok **Dodaj domenę** . Zamiast tego przejdź do obszaru [Dodaj użytkowników](#add-users-and-assign-licenses) .

    ![Zrzut ekranu przedstawiający stronę logowania.](../media/adddomain.png)

    
4. Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS u dowolnego dostawcy hostingu DNS dla systemu Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , który weryfikuje, że jesteś właścicielem domeny. Jeśli znasz hosta domeny, zobacz też [instrukcje dotyczące hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jeśli Twój dostawca hostingu jest GoDaddy lub inny host jest włączony z funkcją [łączenia się z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces jest prosty i automatycznie zostanie wyświetlony monit o zalogowanie się i umożliwienie firmie Microsoft uwierzytelniania w Twoim imieniu.

    ![Na stronie GoDaddy Potwierdź dostęp wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Dodawanie użytkowników i przypisywanie licencji

Możesz dodać użytkowników w kreatorze, ale możesz również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym. Ponadto, jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą funkcji [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Dodawanie użytkowników w Kreatorze

Wszyscy użytkownicy dodaniu w Kreatorze uzyskają automatycznie przypisaną licencję Microsoft 365 Business Premium.

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w Kreatorze](../media/addnewuserspage.png)

1. Jeśli Twoja subskrypcja programu Microsoft 365 Business Premium ma istniejących użytkowników (na przykład w przypadku korzystania z usługi Azure AD Connect), uzyskasz możliwość przydzielenia im licencji. Możesz dodać licencje dla tych użytkowników.

2. Po dodaniu użytkowników możesz także skorzystać z opcji udostępniania poświadczeń nowym użytkownikom, które dodali. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.

### <a name="connect-your-domain"></a>Łączenie domeny

> [!NOTE]
> Jeśli w celu skonfigurowania użytkowników użyto domeny. onmicrosoft lub usługi Azure AD Connect, ten krok nie będzie widoczny.
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora. Jeśli nie, [Zmień serwery nazw, aby skonfigurować aplikację Microsoft 365 z dowolnym rejestratorem domen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale Twój host DNS jest włączony dla [połączenia z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), wybierz pozycję **Dodaj rekordy dla mnie**. Na stronie **Wybieranie usług online** Zaakceptuj wszystkie ustawienia domyślne i wybierz pozycję **dalej**, a następnie wybierz pozycję **AUTORYZUJ** na stronie swojego hosta DNS.
    - Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie włączono dla połączenia z domeną), możesz zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostają połączone. Aby uzyskać więcej informacji, zobacz podstawowe informacje o [domenie](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Strona aktywowania rekordów.](../media/activaterecords.png)

2. Postępuj zgodnie z instrukcjami w kreatorze, a poczta e-mail i inne usługi zostaną skonfigurowane.

### <a name="protect-your-organization"></a>Ochrona organizacji 

Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grup zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*. Możesz również utworzyć dodatkowe grupy, aby przypisać zasady w centrum administracyjnym.

1. W przypadku **zaawansowanych zagrożeń cyber**zaleca się zaakceptowanie ustawień domyślnych, aby umożliwić [ochronę przed zagrożeniami pakietu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanowanie plików i linków w aplikacjach pakietu Office.

    ![Zrzut ekranu przedstawiający stronę zwiększania ochrony.](../media/increasetreatprotection.png)


2. Na stronie **zapobieganie przeciekom wrażliwych danych** zaakceptuj ustawienia domyślne, aby włączyć ochronę przed utratą danych pakietu Office 365 (DLP) w celu śledzenia wrażliwych danych w aplikacjach pakietu Office i zapobiegania przypadkowemu udostępnianiu tych informacji poza organizacją.

3. Na stronie **Ochrona danych w pakiecie Office dla urządzeń przenośnych** pozostaw pozycję Zarządzanie aplikacjami mobilnymi, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję **Utwórz zasady zarządzania aplikacjami mobilnymi**.

    ![Zrzut ekranu przedstawiający ochronę danych w pakiecie Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Bezpieczne komputery z systemem Windows 10

W lewym okienku nawigacji wybierz pozycję **Konfiguracja** , a następnie w obszarze **Logowanie i zabezpieczenia**wybierz pozycję **Zabezpiecz komputery z systemem Windows 10**. Wybierz pozycję **Wyświetl** , aby rozpocząć. Zobacz [Zabezpieczanie komputerów z systemem Windows 10](secure-win-10-pcs.md) , aby uzyskać pełne instrukcje.

## <a name="deploy-office-365-client-apps"></a>Wdrażanie aplikacji klienckich pakietu Office 365

Jeśli podczas instalacji wybrano opcję automatycznego instalowania aplikacji pakietu Office, aplikacje te zostaną zainstalowane na urządzeniach z systemem Windows 10, gdy użytkownicy zalogują się do usługi Azure AD z urządzeń z systemem Windows za pomocą poświadczeń służbowych.

Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business Premium](set-up-mobile-devices.md).

Możesz również zainstalować pakiet Office osobno. Aby uzyskać instrukcje, zobacz [Instalowanie pakietu Office na komputerze PC lub Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>Zobacz też

[Szkolenia wideo dotyczące programu Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
