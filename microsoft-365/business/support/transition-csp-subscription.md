---
title: Przejście subskrypcji usługi Microsoft 365 Business CSP
description: Dowiedz się, jak można przejść subskrypcję usługi Microsoft 365 Business CSP z wersji zapoznawczej do ogólnej dostępności (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Subskrypcja usługi Microsoft 365 Business, Microsoft 365, SMB, subskrypcja przejścia CSP
ms.date: 11/01/2017
ms.openlocfilehash: 5fc532b4a59d8e94068e7e1bae99bf8edac75abb
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403435"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Przejście subskrypcji usługi Microsoft 365 Business CSP

Jeśli masz subskrypcję CSP usługi Microsoft 365 Business Preview, postępuj zgodnie z tym przewodnikiem, aby dowiedzieć się, jak możesz przejść istniejącą subskrypcję w wersji zapoznawczej do usługi Microsoft 365 Business GA (ogólna dostępność).

**Jak przejść subskrypcję w wersji zapoznawczej do ga**

1. Zaloguj się do <a href="https://partnercenter.microsoft.com" target="_blank">Centrum partnerów</a>.
2. Na pulpicie nawigacyjnym wybierz pozycję **Klienci**, a następnie znajdź i wybierz nazwę firmy.

    Zostaną wyświetlone subskrypcje dla firmy.

    ![Subskrypcje klienta w Centrum partnerskim](../../media/pc_customer_subscriptions_1.png)
    
3. Na stronie **Subskrypcje** firmy wybierz pozycję **Dodaj subskrypcję**.
4. Na stronie **Nowa subskrypcja** wybierz pozycję **Mała firma,** a następnie wybierz pozycję **Microsoft 365 Business** z listy.
5. Dodaj liczbę licencji, a następnie wybierz pozycję **Dalej: Przejrzyj,** aby przejrzeć subskrypcję, a następnie wybierz pozycję **Prześlij**.

    ![Przejrzyj nową subskrypcję usługi Microsoft 365 Business](../../media/pc_customer_reviewnewsubscription.png)

    Subskrypcje **oparte na licencji** pokażą microsoft **365 Business Preview** i Microsoft **365 Business**. Następnie zawiesisz subskrypcję w wersji zapoznawczej.

6. Wybierz **pozycję Microsoft 365 Business Preview**.
7. Na stronie **Microsoft 365 Business Preview** wybierz pozycję **Zawieszone,** aby zawiesić subskrypcję w wersji zapoznawczej.

    ![Zawieszanie subskrypcji usługi Microsoft 365 Business Preview](../../media/pc_customer_m365bpreview_suspend.png)

8. Wybierz **opcję Prześlij,** aby potwierdzić.

    Na stronie **Subskrypcje** upewnij się, że stan **usługi Microsoft 365 Business Preview** jest wyświetlany w **zawieszeniu**.

    ![Potwierdzanie zawieszenia stanu subskrypcji w wersji zapoznawczej](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcjonalnie można również sprawdzić poprawność umowy licencyjnej. W tym celu wykonaj następujące czynności:
    1. Wybierz **pozycję Użytkownicy i licencje** ze strony **Subskrypcje** firmy.
    2. Na stronie **Użytkownicy i licencje** wybierz użytkownika.
    3. Na stronie użytkownika sprawdź sekcję **Przypisywanie licencji** i upewnij się, że jest ona wyświetlana w **usłudze Microsoft 365 Business**.

        ![Potwierdzanie, że licencja usługi Microsoft 365 Business jest przypisana do użytkownika](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Wpływ na klientów i użytkowników w okresie przejściowym i po jej zakończeniu

Nie ma to wpływu na klientów i użytkowników podczas przejścia i post transition.

## <a name="impact-to-customers-who-dont-transition"></a>Wpływ na klientów, którzy nie przechodzą na zmiany

W poniższej tabeli podsumowano wpływ na klientów, którzy nie przechodzą z subskrypcji usługi Microsoft 365 Business Preview na subskrypcję usługi Microsoft 365 Business.

|       | T-0 do T+30     | Od T+30 do T+60 | Od T+60 do T+120 | Poza T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stan** | W okresie karencji | Wygasłe      | Wyłączone      | Anulowanie obsługi administracyjnej |
| **Wpływ na usługi**                                                        |
| **Portal administracyjny usługi Microsoft 365 Business** | Brak wpływu na funkcjonalność | Brak wpływu na funkcjonalność | Można dodawać/usuwać użytkowników, kupować subskrypcje.</br> Nie można przypisać/odwołać licencji. | Subskrypcja klienta i wszystkie dane zostaną usunięte. Administrator może zarządzać innymi płatnymi subskrypcjami. |
| **Aplikacje pakietu Office**                         | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Pakiet Office wchodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. | Pakiet Office wchodzi w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. |
| **Usługi w chmurze (SharePoint Online, Exchange Online, Skype, Teams i inne)** | Brak wpływu na użytkownika końcowego | Brak wpływu na użytkownika końcowego | Użytkownicy końcowi i administratorzy nie mają dostępu do danych w chmurze. | Subskrypcja klienta i wszystkie dane są usuwane. |
| **Komponenty EM+S** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Możliwość nie jest już wymuszana.</br> Aby uzyskać więcej [informacji, zobacz Wpływ urządzeń przenośnych na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływ na komputer z systemem Windows 10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) | Możliwość nie jest już wymuszana.</br> Aby uzyskać więcej [informacji, zobacz Wpływ urządzeń przenośnych na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływ na komputer z systemem Windows 10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Windows 10 Biznes** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Możliwość nie jest już wymuszana.</br> Aby uzyskać więcej [informacji, zobacz Wpływ urządzeń przenośnych na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływ na komputer z systemem Windows 10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) | Możliwość nie jest już wymuszana.</br> Aby uzyskać więcej [informacji, zobacz Wpływ urządzeń przenośnych na wygaśnięcie subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływ na komputer z systemem Windows 10 po wygaśnięciu subskrypcji.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Logowanie usługi Azure AD do komputera z systemem Windows 10** | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Brak wpływu na administratora</br> Brak wpływu na użytkownika końcowego | Po usunięciu dzierżawy użytkownik może zalogować się tylko przy użyciu poświadczeń lokalnych. Ponownie obraz urządzenia, jeśli nie ma żadnych poświadczeń lokalnych. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Wpływ na urządzenie mobilne po wygaśnięciu subskrypcji

W poniższej tabeli podsumowano wpływ zasad zarządzania aplikacjami na urządzeniach przenośnych.

|                            | W pełni licencjonowane doświadczenie                      | T + 60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Usuwanie plików roboczych z nieaktywnego urządzenia** | Pliki robocze są usuwane po wybranych dniach | Pliki robocze pozostają na urządzeniach osobistych użytkownika |
| **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** | Pliki robocze można zapisywać tylko w usłudze OneDrive dla Firm | Pliki robocze można zapisywać w dowolnym miejscu |
| **Szyfruj pliki służbowe** | Pliki robocze są szyfrowane | Pliki robocze nie są już szyfrowane.</br> Zasady zabezpieczeń są usuwane, a dane pakietu Office w aplikacjach są usuwane. |
| **Wymagaj numeru PIN lub odcisku palca, aby uzyskać dostęp do aplikacji pakietu Office** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Resetowanie kodu PIN po awarii logowania** | Ograniczony dostęp do aplikacji | Brak ograniczeń dostępu na poziomie aplikacji |
| **Wymaganie od użytkowników ponownego zalogowania się po bezczynniu aplikacji pakietu Office** | Wymagane logowanie | Nie jest wymagane logowanie |
| **Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta** | Pliki robocze nie mogą być dostępne na jailbroken / zakorzenione urządzenia | Pliki robocze mogą być dostępne na jailbroken / zakorzenione urządzenia |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Kopiowanie/wklejanie ograniczone do aplikacji dostępnych w ramach subskrypcji usługi Microsoft 365 | Kopiowanie/wklejanie dostępne dla wszystkich aplikacji |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC wpływa na wygaśnięcie subskrypcji

W poniższej tabeli podsumowano wpływ na zasady konfiguracji urządzeń z systemem Windows 10.

|                            | W pełni licencjonowane doświadczenie                      | T + 60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ochrona komputerów przed zagrożeniami za pomocą usługi Windows Defender** | Włączanie/wyłączanie jest poza kontrolą użytkownika | Użytkownik może włączyć/ wyłączyć usługę Windows Defender na komputerze z systemem Windows 10 |
| **Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge** | Ochrona komputera w przeglądarce Microsoft Edge | Użytkownik może włączyć / wyłączyć ochronę komputera w przeglądarce Microsoft Edge |
| **Wyłączanie ekranu urządzenia, gdy jest bezczynny** | Administrator definiuje zasady interwału limitu czasu ekranu | Limit czasu ekranu może być skonfigurowany przez użytkownika końcowego |
| **Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store** | Administrator określa, czy użytkownik może pobierać aplikacje ze Sklepu Microsoft | Użytkownik może pobierać aplikacje ze sklepu Microsoft Store w dowolnym momencie |
| **Zezwalaj użytkownikom na korzystanie z Cortany** | Administrator definiuje zasady dotyczące dostępu użytkownika do Cortany | Urządzenia użytkownika do włączania/wyłączania Cortany |
| **Zezwalaj użytkownikom na otrzymywanie porad i reklam od firmy Microsoft** | Administrator definiuje zasady dotyczące otrzymywania przez użytkownika porad i reklam od firmy Microsoft | Użytkownik może włączać/ wyłączać porady i reklamy firmy Microsoft |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Administrator definiuje zasady, aby aktualizować urządzenia z systemem Windows 10 | Użytkownicy mogą zdecydować, kiedy zaktualizować system Windows |
