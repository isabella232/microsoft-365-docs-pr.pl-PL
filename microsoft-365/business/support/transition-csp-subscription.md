---
title: Przechodzenie subskrypcji dostawcy usług Kryptograficznych firmy Microsoft 365 
description: Dowiedz się, jak można przejść subskrypcję dostawcy usług kryptograficznych dla firm firmy Microsoft 365 z wersji zapoznawczej do ogólnej dostępności (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, subskrypcja transition CSP
ms.date: 11/01/2017
ms.openlocfilehash: 77b7b474a5ad17db58e283ea61b074c959905d1b
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560785"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Przechodzenie subskrypcji dostawcy usług Kryptograficznych firmy Microsoft 365

Jeśli masz subskrypcję programu CSP usługi Microsoft 365 Business Preview, wykonaj ten przewodnik, aby dowiedzieć się, jak można przejść do istniejącej subskrypcji w wersji zapoznawczej na usługę Microsoft 365 Business GA (ogólna dostępność).

**Jak przejść subskrypcję w wersji zapoznawczej do ga**

1. Zaloguj się w <a href="https://partnercenter.microsoft.com" target="_blank">Centrum partnerskim</a>.
2. Na pulpicie nawigacyjnym wybierz pozycję **Klienci**, a następnie znajdź i wybierz nazwę firmy.

    Subskrypcje dla firmy zostaną wymienione.

    ![Subskrypcje klientów w Centrum partnerskim](../../media/pc_customer_subscriptions_1.png)
    
3. Na stronie **Subskrypcje** firmy wybierz pozycję **Dodaj subskrypcję**.
4. Na stronie **Nowa subskrypcja** wybierz pozycję **Małe firmy,** a następnie wybierz pozycję **Microsoft 365 Business** z listy.
5. Dodaj liczbę licencji, a następnie wybierz pozycję **Dalej: Przejrzyj,** aby przejrzeć subskrypcję, a następnie wybierz pozycję **Prześlij**.

    ![Przeglądanie nowej subskrypcji usługi Microsoft 365 Business](../../media/pc_customer_reviewnewsubscription.png)

    **Subskrypcje oparte na licencji pokażą** **microsoft 365 Business Preview** i Microsoft **365 Business**. Następnie zawiesisz subskrypcję wersji zapoznawczej.

6. Wybierz **pozycję Microsoft 365 Business Preview**.
7. Na stronie **Microsoft 365 Business Preview** wybierz pozycję **Zawieszone,** aby zawiesić subskrypcję wersji zapoznawczej.

    ![Zawieszanie subskrypcji usługi Microsoft 365 Business Preview](../../media/pc_customer_m365bpreview_suspend.png)

8. Wybierz **pozycję Prześlij,** aby potwierdzić.

    Na stronie **Subskrypcje** upewnij się, że stan **Microsoft 365 Business Preview** jest wyświetlany jako **Zawieszone**.

    ![Potwierdzanie stanu subskrypcji w wersji Preview jest zawieszone](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcjonalnie można również sprawdzić poprawność umowy licencyjnej. W tym celu wykonaj następujące czynności:
    1. Wybierz **pozycję Użytkownicy i licencje** na stronie **Subskrypcje** firmy.
    2. Na stronie **Użytkownicy i licencje** wybierz użytkownika.
    3. Na stronie użytkownika sprawdź sekcję **Przypisywanie licencji** i upewnij się, że jest ona wyświetlana pod **numerem Microsoft 365 Business**.

        ![Potwierdzanie, że licencja microsoft 365 Business jest przypisana do użytkownika](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Wpływ na klientów i użytkowników w trakcie i po okresie przejściowym

Nie ma to wpływu na klientów i użytkowników podczas przejścia i przejścia post.

## <a name="impact-to-customers-who-dont-transition"></a>Wpływ na klientów, którzy nie przechodzą

W poniższej tabeli podsumowano wpływ na klientów, którzy nie przechodzą z subskrypcji usługi Microsoft 365 Business Preview do subskrypcji usługi Microsoft 365 Business.

|       | T-0 do T+30     | T+30 do T+60 | T+60 do T+120 | Poza T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stan** | W okresie karencji | Wygasłe      | Wyłączone      | Cofnięte aprowizac |
| **Wpływ na usługi**                                                        |
| **Portal administracyjny usługi Microsoft 365 Business** | Brak wpływu na funkcjonalność | Brak wpływu na funkcjonalność | Można dodawać/usuwać użytkowników, kupować subskrypcje.</br> Nie można przypisać/odwołać licencji. | Subskrypcja klienta i wszystkie dane są usuwane. Administrator może zarządzać innymi płatnymi subskrypcjami. |
| **Aplikacje pakietu Office**                         | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Pakiet Office przechodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. | Pakiet Office przechodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. |
| **Usługi w chmurze (sharepoint online, exchange online, skype, zespoły i inne)** | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Użytkownicy końcowi i administratorzy nie mają dostępu do danych w chmurze. | Subskrypcja klienta i wszystkie dane są usuwane. |
| **Komponenty EM+S** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Możliwości nie są już wymuszane.</br> Aby uzyskać więcej informacji, zobacz [Wpływ na urządzenie przenośne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows [10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) | Możliwości nie są już wymuszane.</br> Aby uzyskać więcej informacji, zobacz [Wpływ na urządzenie przenośne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows [10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Windows 10 Business** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Możliwości nie są już wymuszane.</br> Aby uzyskać więcej informacji, zobacz [Wpływ na urządzenie przenośne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows [10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) | Możliwości nie są już wymuszane.</br> Aby uzyskać więcej informacji, zobacz [Wpływ na urządzenie przenośne po wygaśnięciu subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i wpływ na komputer z systemem Windows [10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Logowanie usługi Azure AD do komputera z systemem Windows 10** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Po usunięciu dzierżawy użytkownik może zalogować się tylko przy użyciu poświadczeń lokalnych. Ponowne zdjęcie urządzenia, jeśli nie ma żadnych poświadczeń lokalnych. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Wpływ urządzenia przenośnego po wygaśnięciu subskrypcji

W poniższej tabeli podsumowano wpływ zasad zarządzania aplikacjami na urządzenia przenośne.

|                            | W pełni licencjonowane doświadczenie                      | T+60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Usuwanie plików roboczych z nieaktywnego urządzenia** | Pliki robocze są usuwane po wybranych dniach | Pliki robocze pozostają na urządzeniach osobistych użytkownika |
| **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** | Pliki robocze można zapisywać tylko w usłudze OneDrive dla Firm | Pliki robocze można zapisywać w dowolnym miejscu |
| **Szyfruj pliki służbowe** | Pliki robocze są szyfrowane | Pliki robocze nie są już szyfrowane.</br> Zasady zabezpieczeń są usuwane, a dane pakietu Office w aplikacjach są usuwane. |
| **Wymaganie numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Resetowanie numeru PIN w przypadku niepowodzenia logowania** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Wymaganie od użytkowników ponownego logowania się po bezczynności aplikacji pakietu Office** | Wymagane logowanie | Nie jest wymagane logowanie |
| **Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta** | Pliki robocze nie są dostępne na jailbroken / zakorzenione urządzenia | Pliki robocze są dostępne na jailbroken / zakorzenione urządzenia |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Kopiowanie/wklejanie ograniczone do aplikacji dostępnych w ramach subskrypcji usługi Microsoft 365 Business | Kopiowanie/wklejanie dostępne dla wszystkich aplikacji |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Wpływ komputera z systemem Windows 10 na wygaśnięcie subskrypcji

W poniższej tabeli podsumowano wpływ zasad konfiguracji urządzeń z systemem Windows 10.

|                            | W pełni licencjonowane doświadczenie                      | T+60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ochrona komputerów przed zagrożeniami za pomocą usługi Windows Defender** | Włączanie/wyłączanie jest poza kontrolą użytkownika | Użytkownik może włączyć/wyłączyć usługę Windows Defender na komputerze z systemem Windows 10 |
| **Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge** | Ochrona komputera w programie Microsoft Edge | Użytkownik może włączyć/wyłączyć ochronę komputera w programie Microsoft Edge |
| **Wyłączanie ekranu urządzenia w trybie bezczynności** | Administrator definiuje zasady interwału czasu pracy ekranu | Timetime timetime można skonfigurować przez użytkownika końcowego |
| **Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store** | Administrator określa, czy użytkownik może pobierać aplikacje ze sklepu Microsoft Store | Użytkownik może pobierać aplikacje ze sklepu Microsoft Store w dowolnym momencie |
| **Zezwalaj użytkownikom na korzystanie z Cortany** | Administrator definiuje zasady dotyczące dostępu użytkowników do Cortany | Urządzenia użytkownika do wyłączeniu/wyłączenia Cortany |
| **Zezwalaj użytkownikom na otrzymywanie porad i reklam od firmy Microsoft** | Administrator definiuje zasady dotyczące otrzymywania przez użytkownika porad i reklam od firmy Microsoft | Użytkownik może włączać/wyłączać porady i reklamy firmy Microsoft |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Administrator definiuje zasady, aby aktualizować urządzenia z systemem Windows 10 | Użytkownicy mogą zdecydować, kiedy zaktualizować system Windows |
