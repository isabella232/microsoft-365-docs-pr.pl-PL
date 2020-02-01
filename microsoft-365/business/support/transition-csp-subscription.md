---
title: Przechodzenie na subskrypcję dostawcy usługi CSP dla firm firmy Microsoft 365 
description: Dowiedz się, jak przejść subskrypcję dostawcy csp dla firm Microsoft 365 Business z wersji zapoznawczej na ga. 
author: jasongroce
f1.keywords:
- NOCSH
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Subskrypcja dostawcy CSP usługi Microsoft 365 Business, Microsoft 365, SMB, przejście do systemu CSP
ms.date: 11/01/2017
ms.openlocfilehash: 4aadfa24bec8728c7e011ac6da48a8e30516e145
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41595050"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Przechodzenie na subskrypcję dostawcy usługi CSP dla firm firmy Microsoft 365

Jeśli masz subskrypcję dostawcy usług CSP w wersji Microsoft 365 Business Preview, postępuj zgodnie z tym przewodnikiem, aby dowiedzieć się, jak przejść istniejącą subskrypcję wersji zapoznawczej na usługę Microsoft 365 Business GA (ogólna dostępność).

**Jak przejść subskrypcję w wersji zapoznawczej na ga**

1. Zaloguj się do <a href="https://partnercenter.microsoft.com" target="_blank">Centrum partnerów</a>.
2. Na pulpicie nawigacyjnym wybierz **pozycję Klienci**, a następnie znajdź i wybierz nazwę firmy.

    Subskrypcje dla firmy zostaną wymienione.

    ![Subskrypcje klientów w Centrum partnerskim](images/pc_customer_subscriptions_1.png)
    
3. Na stronie **Subskrypcje** firmy wybierz pozycję **Dodaj subskrypcję**.
4. Na stronie **Nowa subskrypcja** wybierz **pozycję Małe firmy,** a następnie wybierz z listy pozycję Microsoft **365 Business.**
5. Dodaj liczbę licencji, a następnie wybierz **pozycję Dalej: Przejrzyj,** aby przejrzeć subskrypcję, a następnie wybierz pozycję **Prześlij**.

    ![Przeglądanie nowej subskrypcji usługi Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Subskrypcje oparte na licencji** będą wyświetlać **usługi Microsoft 365 Business Preview** i Microsoft **365 Business**. Następnie zawiesisz subskrypcję podglądu.

6. Wybierz **pozycję Microsoft 365 Business Preview**.
7. Na stronie **Microsoft 365 Business Preview** wybierz pozycję **Zawieszone,** aby zawiesić subskrypcję w wersji zapoznawczej.

    ![Zawieszanie subskrypcji usługi Microsoft 365 Business Preview](images/pc_customer_m365bpreview_suspend.png)

8. Wybierz **pozycję Prześlij,** aby potwierdzić.

    Na stronie **Subskrypcje** upewnij się, że stan **usługi Microsoft 365 Business Preview** jest wyświetlany w **zawieszeniu**.

    ![Potwierdzanie stanu subskrypcji podglądu jest zawieszone](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcjonalnie można również sprawdzić poprawność umowy licencyjnej. W tym celu wykonaj następujące czynności:
    1. Wybierz **pozycję Użytkownicy i licencje** ze strony **Subskrypcje** firmy.
    2. Na stronie **Użytkownicy i licencje** wybierz użytkownika.
    3. Na stronie użytkownika sprawdź sekcję **Przypisz licencje** i upewnij się, że zawiera ona program **Microsoft 365 Business**.

        ![Potwierdzanie, że licencja Microsoft 365 Business jest przypisana do użytkownika](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Wpływ na klientów i użytkowników w trakcie i po przejściu

Nie ma to wpływu na klientów i użytkowników podczas przejścia i przejścia posta.

## <a name="impact-to-customers-who-dont-transition"></a>Wpływ na klientów, którzy nie przechodzą

W poniższej tabeli podsumowano wpływ na klientów, którzy nie przechodzą z subskrypcji usługi Microsoft 365 Business Preview do subskrypcji usługi Microsoft 365 Business.

|       | T-0 do T+30     | T+30 do T+60 | T+60 do T+120 | Poza T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stan** | W okresie karencji | Wygasłe      | Wyłączone      | Cofnięte aprowizowane |
| **Wpływ na usługi**                                                        |
| **Portal administracyjny firmy Microsoft 365 Business** | Brak wpływu na funkcjonalność | Brak wpływu na funkcjonalność | Można dodawać/usuwać użytkowników, kupować subskrypcje.</br> Nie można przypisać/odwołać licencji. | subskrypcji klienta i wszystkie dane zostaną usunięte. Administrator może zarządzać innymi płatnymi subskrypcjami. |
| **Aplikacje pakietu Office**                         | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Pakiet Office przechodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. | Pakiet Office przechodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. |
| **Usługi w chmurze (SharePoint Online, Exchange Online, Skype, Teams i inne)** | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Użytkownicy końcowi i administratorzy nie mają dostępu do danych w chmurze. | subskrypcji klienta i wszystkie dane są usuwane. |
| **Komponenty EM+S** | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Możliwości nie są już wymuszane.</br> Zobacz, [że wpływ urządzenia przenośnego na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows 10 w momencie [wygaśnięcia subskrypcji,](#windows-10-pc-impacts-upon-subscription-expiration) aby uzyskać więcej informacji. | Możliwości nie są już wymuszane.</br> Zobacz, [że wpływ urządzenia przenośnego na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows 10 w momencie [wygaśnięcia subskrypcji,](#windows-10-pc-impacts-upon-subscription-expiration) aby uzyskać więcej informacji. |
| **Windows 10 Biznes** | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Możliwości nie są już wymuszane.</br> Zobacz, [że wpływ urządzenia przenośnego na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows 10 w momencie [wygaśnięcia subskrypcji,](#windows-10-pc-impacts-upon-subscription-expiration) aby uzyskać więcej informacji. | Możliwości nie są już wymuszane.</br> Zobacz, [że wpływ urządzenia przenośnego na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows 10 w momencie [wygaśnięcia subskrypcji,](#windows-10-pc-impacts-upon-subscription-expiration) aby uzyskać więcej informacji. |
| **Logowanie usługi Azure AD na komputerze z systemem Windows 10** | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu administratora</br> Brak wpływu na użytkownika końcowego | Po usunięciu dzierżawy użytkownik może zalogować się tylko przy użyciu poświadczeń lokalnych. Ponownie obraz urządzenia, jeśli nie ma żadnych poświadczeń lokalnych. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Wpływ urządzenia przenośnego na wygaśnięcie subskrypcji

W poniższej tabeli podsumowano wpływ na zasady zarządzania aplikacjami na urządzenia przenośne.

|                            | W pełni licencjonowane doświadczenie                      | T +60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Usuwanie plików roboczych z nieaktywnego urządzenia** | Pliki robocze są usuwane po wybranych dniach | Pliki robocze pozostają na urządzeniach osobistych użytkownika |
| **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** | Pliki służbowe można zapisywać tylko w usłudze OneDrive dla Firm | Pliki robocze można zapisywać w dowolnym miejscu |
| **Szyfruj pliki służbowe** | Pliki robocze są szyfrowane | Pliki robocze nie są już szyfrowane.</br> Zasady zabezpieczeń są usuwane, a dane pakietu Office w aplikacjach są usuwane. |
| **Wymaganie kodu PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Resetowanie numeru PIN po awarii logowania** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Wymaganie od użytkowników ponownego logowania się po bezczynności aplikacji pakietu Office** | Wymagane logowanie | Logowanie nie jest wymagane |
| **Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta** | Pliki robocze nie są dostępne na jailbroken / zakorzenione urządzenia | Pliki robocze są dostępne na jailbroken / zakorzenione urządzenia |
| **Zezwalanie użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Kopiowanie/wklejanie ograniczone do aplikacji dostępnych w ramach subskrypcji usługi Microsoft 365 Business | Kopiowanie/wklejanie dostępne dla wszystkich aplikacji |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>System Windows 10 PC wpływa na wygaśnięcie subskrypcji

W poniższej tabeli podsumowano wpływ na zasady konfiguracji urządzeń z systemem Windows 10.

|                            | W pełni licencjonowane doświadczenie                      | T +60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ochrona komputerów przed zagrożeniami przy użyciu usługi Windows Defender** | Włączanie/wyłączanie jest poza kontrolą użytkownika | Użytkownik może włączyć /wyłączyć usługę Windows Defender na komputerze z systemem Windows 10 |
| **Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge** | Ochrona komputera w programie Microsoft Edge | Użytkownik może włączyć/wyłączyć ochronę komputera w programie Microsoft Edge |
| **Wyłączanie ekranu urządzenia podczas biegu jałowego** | Administrator definiuje zasady interwału czasu ekranowego | Zrzut czasu ekranu może być skonfigurowany przez użytkownika końcowego |
| **Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store** | Administrator określa, czy użytkownik może pobierać aplikacje ze sklepu Microsoft Store | Użytkownik może pobierać aplikacje ze sklepu Microsoft Store w dowolnym momencie |
| **Zezwalaj użytkownikom na korzystanie z Cortany** | Administrator definiuje zasady dotyczące dostępu użytkowników do Cortany | Urządzenia użytkownika, aby włączyć /wyłączyć Cortana |
| **Zezwalaj użytkownikom na otrzymywanie porad i reklam od firmy Microsoft** | Administrator definiuje zasady dotyczące otrzymywania przez użytkowników porad i reklam od firmy Microsoft | Użytkownik może włączać/wyłączać porady i reklamy firmy Microsoft |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Administrator definiuje zasady, aby aktualizować urządzenia z systemem Windows 10 | Użytkownicy mogą zdecydować, kiedy zaktualizować system Windows |
