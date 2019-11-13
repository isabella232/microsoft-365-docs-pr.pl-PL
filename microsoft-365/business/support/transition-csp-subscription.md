---
title: Przejście do subskrypcji Microsoft 365 Business CSP 
description: Dowiedz się, jak można przejść subskrypcję Microsoft 365 Business CSP od wersji zapoznawczej do GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, przejściowa subskrypcja CSP
ms.date: 11/01/2017
ms.openlocfilehash: b907c3a3bccc4179369890b7769dcb14ba2acbb7
ms.sourcegitcommit: e4f2f06daa264b8b476813a2dfe80cffb59f968f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/13/2019
ms.locfileid: "38311099"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Przejście do subskrypcji Microsoft 365 Business CSP

Jeśli masz subskrypcję Microsoft 365 Business Preview CSP, wykonaj ten przewodnik, aby dowiedzieć się, jak można przejść istniejącej subskrypcji podglądu do Microsoft 365 Business GA (ogólna dostępność).

**Jak przejść do wersji zapoznawczej subskrypcji do GA**

1. Zaloguj się do <a href="https://partnercenter.microsoft.com" target="_blank">Centrum partnerskiego</a>.
2. Z poziomu pulpitu nawigacyjnego wybierz pozycję **klienci**, a następnie Znajdź i wybierz nazwę firmy.

    Zostaną wyświetlone subskrypcje dla firmy.

    ![Subskrypcje klienta w centrum partnerskim](images/pc_customer_subscriptions_1.png)
    
3. Na stronie **subskrypcje** firmy wybierz pozycję **Dodaj subskrypcję**.
4. Na stronie **Nowa subskrypcja** wybierz pozycję **mała firma** , a następnie z listy wybierz pozycję **Microsoft 365 Business** .
5. Dodaj liczbę licencji, a następnie wybierz pozycję **Dalej: Przejrzyj** , aby przejrzeć subskrypcję, a następnie wybierz pozycję **Prześlij**.

    ![Przejrzyj nową subskrypcję Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Subskrypcje oparte na licencji** będą pokazywać **Microsoft 365 Business Preview** i **Microsoft 365 Business**. Następnie wstrzymasz subskrypcję Preview.

6. Wybierz pozycję **Microsoft 365 Business Preview**.
7. Na stronie **Microsoft 365 Business Preview** wybierz **zawieszone** do zawieszenia subskrypcji Preview.

    ![Zawieszanie subskrypcji Microsoft 365 Business Preview](images/pc_customer_m365bpreview_suspend.png)

8. Wybierz **Prześlij** , aby potwierdzić.

    Na stronie **subskrypcje** Potwierdź, że stan **Microsoft 365 Business Preview** pokazuje **zawieszone**.

    ![Potwierdź, że stan subskrypcji Preview jest zawieszony](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcjonalnie można również zweryfikować umowę licencyjną. W tym celu wykonaj następujące czynności:
    1. Wybierz **użytkowników i licencje** na stronie **subskrypcji** firmy.
    2. Na stronie **Użytkownicy i licencje** wybierz użytkownika.
    3. Na stronie użytkownika sprawdź sekcję **Przypisywanie licencji** i Potwierdź, że pokazuje ona **Microsoft 365 Business**.

        ![Potwierdź, że licencja Microsoft 365 Business jest przypisana do użytkownika](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Wpływ na klientów i użytkowników w trakcie i po przejściu

Nie ma wpływu na klientów i użytkowników podczas przejścia i po przejściu.

## <a name="impact-to-customers-who-dont-transition"></a>Wpływ na klientów, którzy nie przejścia

Poniższa tabela podsumowuje wpływ na klientów, którzy nie przejścia z subskrypcji Microsoft 365 Business Preview do subskrypcji Microsoft 365 Business.

|       | Od t-0 do T + 30     | T + 30 do T + 60 | T + 60 do T + 120 | Poza T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stan** | W okresie prolongaty | Wygasłe      | Wyłączone      | Deprovisioned |
| **Wpływ na usługi**                                                        |
| **Portal administracyjny firmy Microsoft 365** | Brak wpływu na funkcjonalność | Brak wpływu na funkcjonalność | Można dodawać/usuwać użytkowników, kupować subskrypcje.</br> Nie można przypisać/odwołać licencji. | Subskrypcja klienta i wszystkie dane są usuwane. Administrator może zarządzać innymi płatną subskrypcją. |
| **Aplikacje pakietu Office**                         | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Pakiet Office wchodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. | Pakiet Office wchodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. |
| **Usługi w chmurze (SharePoint Online, Exchange Online, Skype, zespoły i inne)** | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Użytkownicy końcowi i Administratorzy nie mają dostępu do danych w chmurze. | Subskrypcja klienta i wszystkie dane są usuwane. |
| **Komponenty EM + S** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Funkcja nie jest już wymuszana.</br> Zobacz [wpływ na urządzenia mobilne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [WPŁYWIE na komputer z systemem Windows 10 po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) , aby uzyskać więcej informacji. | Funkcja nie jest już wymuszana.</br> Zobacz [wpływ na urządzenia mobilne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [WPŁYWIE na komputer z systemem Windows 10 po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) , aby uzyskać więcej informacji. |
| **Windows 10 dla firm** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Funkcja nie jest już wymuszana.</br> Zobacz [wpływ na urządzenia mobilne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [WPŁYWIE na komputer z systemem Windows 10 po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) , aby uzyskać więcej informacji. | Funkcja nie jest już wymuszana.</br> Zobacz [wpływ na urządzenia mobilne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [WPŁYWIE na komputer z systemem Windows 10 po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) , aby uzyskać więcej informacji. |
| **Logowanie do usługi Azure AD na komputerze z systemem Windows 10** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Po usunięciu dzierżawy użytkownik może logować się tylko przy użyciu poświadczeń lokalnych. Ponownie obraz urządzenia, jeśli nie ma żadnych poświadczeń lokalnych. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Wpływ urządzenia mobilnego na wygaśnięcie subskrypcji

Poniższa tabela podsumowuje wpływ na zasady zarządzania aplikacjami na urządzeniach przenośnych.

|                            | Doświadczenie w pełni licencjonowane                      | T + 60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Usuwanie plików roboczych z nieaktywnego urządzenia** | Pliki robocze są usuwane po wybranych dniach | Pliki robocze pozostają na osobistych urządzeniach użytkownika |
| **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** | Pliki służbowe można zapisywać tylko w usłudze OneDrive dla firm | Pliki robocze można zapisywać w dowolnym miejscu |
| **Szyfruj pliki służbowe** | Pliki robocze są szyfrowane | Pliki robocze nie są już szyfrowane.</br> Zasady zabezpieczeń są usuwane, a dane pakietu Office w aplikacjach są usuwane. |
| **Wymaganie kodu PIN lub odcisku palca w celu uzyskiwania dostępu do aplikacji pakietu Office** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Resetuj kod PIN, gdy logowanie nie powiedzie się** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Wymagaj od użytkowników logowania się ponownie po bezczynności aplikacji pakietu Office** | Wymagane logowanie | Nie jest wymagane logowanie |
| **Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta** | Nie można uzyskać dostępu do plików roboczych na urządzeniach jailbroken/zakorzenione | Pliki pracy mogą być dostępne na jailbroken/zakorzenione urządzeń |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Kopiuj/Wklej ograniczone do aplikacji dostępnych w ramach subskrypcji Microsoft 365 Business | Kopiuj/Wklej dostępne dla wszystkich aplikacji |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Wpływ komputera z systemem Windows 10 na wygaśnięcie subskrypcji

Poniższa tabela podsumowuje wpływ na zasady konfiguracji urządzeń systemu Windows 10.

|                            | Doświadczenie w pełni licencjonowane                      | T + 60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Pomóż chronić komputery przed zagrożeniami za pomocą Windows Defender** | Włączanie/wyłączanie jest poza kontrolą użytkownika | Użytkownik puszka metalowa włączyć/wyłączyć Windows Obrońca u ten Windows 10 PC |
| **Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge** | Ochrona komputera w programie Microsoft Edge | Użytkownik może włączyć/wyłączyć ochronę komputera w Microsoft Edge |
| **Wyłączanie ekranu urządzenia w trybie bezczynności** | Admin definiuje zasady limitu czasu ekranu | Limit czasu ekranu może być skonfigurowany przez użytkownika końcowego |
| **Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store** | Administrator definiuje, czy użytkownik może pobierać aplikacje ze sklepu Microsoft Store | Użytkownik może pobierać aplikacje z Microsoft Store w dowolnym czasie |
| **Zezwalaj użytkownikom na korzystanie z Cortany** | Administrator definiuje zasady dostępu użytkownika do Cortany | Urządzenia użytkownika, aby włączyć/wyłączyć Cortana |
| **Zezwalaj użytkownikom na otrzymywanie porad i reklam od firmy Microsoft** | Administrator definiuje zasady dotyczące otrzymywania porad i reklam od firmy Microsoft | Użytkownik może włączyć/wyłączyć porady i reklamy firmy Microsoft |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Administrator definiuje zasady, aby urządzenia z systemem Windows 10 były aktualne | Użytkownicy mogą zdecydować, kiedy aktualizować system Windows |
