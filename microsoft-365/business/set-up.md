---
title: Konfigurowanie usługi Microsoft 365 Business przy użyciu kreatora konfiguracji
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
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować Microsoft 365 Business, wykonując cztery kroki.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982197"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>Konfigurowanie usługi Microsoft 365 Business przy użyciu kreatora konfiguracji

Wykonaj kroki 1-4 poniżej.
  
### <a name="set-up-microsoft-365-business"></a>Konfigurowanie usługi Microsoft 365 Business

Obejrzyj film o tym, jak skonfigurować Microsoft 365 Business, gdy nie masz usługi Active Directory na lokalnym:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
Kroki konfiguracji zawiera informacje dotyczące ustawień, które zawierają lokalną usługę Active Directory. Jeśli chcesz w dalszym ciągu dostęp do urządzeń przyłączonych do domeny, przeczytanie następujących artykułów dla dwóch różnych rozwiązanie pozwalające który i wykonaj kroki przed uruchomieniem Kreatora instalacji:
  
- [Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10](manage-windows-devices.md)
    
    -Jest to zalecany sposób.
    
- [Dostęp do zasobów lokalnych z Azure urządzenia przyłączonych do AD w Microsoft 365 Business](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>Krok 1: Spersonalizować logowanie

1. Zaloguj się do usługi [Microsoft 365 Business](https://portal.microsoft.com) za pomocą poświadczeń administratora globalnego. Wybierz kafelek **Administrator**, aby przejść do centrum administracyjnego. 
    
2. W centrum administracyjnym wybierz pozycję **Rozpocznij konfigurowanie** (lub pozycję **Kontynuuj konfigurowanie** w zależności od swojego stanu), aby uruchomić kreatora. 
    
3. Wprowadź żądaną nazwę domeny (np. contoso.com).
    
    Przejdź dalej i wprowadź swoją domenę, nawet jeśli po sprawdzeniu podczas używania Azure AD Connect, np. Następujące dwa kroki można pominąć Jeśli Azure AD Connect używane do zweryfikowania domeny.
    
4. Postępuj zgodnie z instrukcjami w kreatorze [Tworzenie rekordów DNS u dowolnego dostawcy usług hosta DNS dla usługi Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) sprawdza, czy użytkownik jest właścicielem domeny. 
    
    Można wyświetlić przykład wideo [wideo: Instalatora Office 365 w nowym Centrum Admin](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Należy zauważyć, że ten film nie obejmuje czynności ochrony danych systemu Microsoft 365 Business.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>Krok 2: Dodawanie użytkowników i przypisywanie licencji

1. Użytkowników możesz dodać od razu tutaj albo [później](add-users-m365b.md) w centrum administracyjnym. 
    
    Każdy dodany użytkownik automatycznie otrzymuje licencję na usługę Microsoft 365 Business.
    
2. Jeśli Twoja subskrypcja usługi Microsoft 365 Business zawiera już użytkowników (na przykład użyto narzędzia Azure AD Connect), zobaczysz opcję przypisania im licencji. Możesz dodać licencje dla tych użytkowników.
    
3. Zobaczysz też opcję udostępnienia poświadczeń nowym użytkownikom. Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.
    
4. Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**. 
    
    Jeśli jest przesuwana od innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [migracji wiadomości e-mail i kontaktów do usługi Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>Krok 3: Łączenie domeny

> [!NOTE]
> Jeśli wybrany do korzystania z domeny .onmicrosoft lub używane Azure Połącz AD, nie zobaczysz ten krok. 
  
Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.
  
1. Kreator instalacji zazwyczaj wykrywa rejestratorem i zapewnia łącza do instrukcji krok po kroku aktualizować rekordy NS w witrynie sieci Web rejestratora. Jeśli tak nie jest, [Zmień serwery nazw do skonfigurowania usługi Office 365 z dowolnym domen](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. Umożliwia to skonfigurowanie poczty e-mail i innych usług.
    
### <a name="step-4-manage-devices-and-work-files"></a>Krok 4: Zarządzanie urządzeniami i pliki robocze

1. **Chroń pliki robocze na urządzeniach przenośnych** strony ustawić **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** i ustawienia **zarządzania dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** na **na**. Można także przejść każda podrzędna ustawienie klikając cudzysłów ostrokątny obok każdego ustawienia.
  
  Wszystkie pliki prac użytkowników licencjonowanych obecnie są chronione na iOS lub androidem, tak szybko jak [zainstalować aplikacje pakietu Office](set-up-mobile-devices.md) (i uwierzytelnianie przy użyciu poświadczeń Microsoft 365 Business). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. Na stronie **Konfiguracja urządzenia zestaw Windows 10** ustawieniu **Bezpiecznego urządzenia z systemem Windows 10** **na**.
  
   Można także przejść każda podrzędna ustawienie klikając podwójną strzałkę obok niej.
  
3. W ustawieniu **Zainstaluj pakiet Office na urządzeniach 10 systemu Windows** **Tak,** Jeśli wszyscy użytkownicy mają komputery Windows 10 i instaluje nie istniejących Office lub -Szybka instalacja pakietu Office. Jeśli nie jest to możliwe, należy ustawić tę opcję na **nie**. Można [automatycznie zainstalować pakiet Office](auto-install-or-uninstall-office.md) później z Centrum administracyjnego, po przygotowaniu komputerów użytkowników. Aby uzyskać instrukcje zobacz [Przygotowanie do instalacji klienta pakietu Office](prepare-for-office-client-deployment.md).
  
    Pliki robocze licencjonowani użytkownicy na urządzeniach Windows 10 będą rzutowane tak szybko jak [dołączyć do swoich urządzeń Windows 10](set-up-windows-devices.md) do domeny firmy Microsoft 365 Azure AD lub [zainstalować system Windows 10 na nowym komputerze](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) podczas przyłączania się jednocześnie Microsoft 365 Domeny Azure AD firmy. 
  
4. Kliknij przycisk **Dalej** i po zakończeniu instalacji. 
  
    Proszę zostawić opinię o ten krok, aby pomóc w ulepszeniu doświadczenia.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>Dodatkowych ustawień zabezpieczeń

Oprócz zabezpieczeń i ustawienie zgodności w Kreatorze instalacji można skonfigurować następujące dodatkowe ustawienia:
  
- Konfigurowanie ochrony przed niebezpiecznymi załącznikami. **Zaawansowana ochrona przed zagrożeniami** (ATP) identyfikuje niebezpieczną zawartość, a następnie blokuje dostawy niebezpiecznych załączników, ochrona przed wyłudzeniami i infekcjami szkodnika. Aby włączyć ochronę załączników, zobacz [Ustawianie zasad Office 365 ATP bezpieczne załączniki](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- Chronić środowisko, gdy użytkownik kliknie niebezpiecznego łącza. ATP sprawdza łącza w wiadomości e-mail w momencie użytkownik kliknie je. Jeżeli łącze jest niebezpieczny, użytkownik jest ostrzegany, nie do odwiedzenia tej witryny lub poinformowane, że witryna została zablokowana. Ułatwia to ochronę przed schematami wyłudzania informacji. [Ustawianie zasad bezpiecznego łącza Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) lub [ustawienie zasady bezpiecznego łącza Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Można zachować całą zawartość skrzynki pocztowej, w tym elementów usuniętych przez umieszczenie całej skrzynki pocztowej użytkownika na **spory sądowe przytrzymaj**. Aby uzyskać instrukcje zobacz 
- [Konfigurowanie przechowywanie wiadomości e-mail z programu Exchange Online archiwizacji](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Na przykład, skonfigurować niestandardowych **zasad przechowywania**do zachowania przez określoną ilość czasu lub trwale usunąć zawartość z końcem okresu przetrzymania. Można włączyć zasady przechowywania dostosowanych w Centrum zgodności, przejdź do **zarządzania danymi** i papierów wartościowych \> **zatrzymania**, a następnie wykonaj kroki w kreatorze. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
    
## <a name="next-steps"></a>Dalsze kroki

Dla użytkowników, którzy mają licencje, następnym krokiem jest skonfigurowanie urządzeń.<br/> Zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md) i [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business](set-up-mobile-devices.md). <br/>Zobacz [Zarządzanie usługą Microsoft 365 Business](manage.md), aby uzyskać linki do tematów dotyczących konfigurowania zasad ochrony urządzeń i aplikacji oraz usuwania danych z urządzeń użytkowników. 
  


