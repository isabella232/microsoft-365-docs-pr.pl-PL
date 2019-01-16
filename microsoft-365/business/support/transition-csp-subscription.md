---
title: Przejście subskrypcji dostawcy usług Kryptograficznych firmy Microsoft 365 Business 
description: Dowiedz się jak może przejść subskrypcji dostawcy usług Kryptograficznych firmy Microsoft 365 biznesowych z podglądu GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft Business 365, Microsoft 365 SMB, przejście subskrypcji dostawcy usług Kryptograficznych
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982487"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Przejście subskrypcji dostawcy usług Kryptograficznych firmy Microsoft 365 Business

Jeśli masz subskrypcję Microsoft 365 Business podglądu dostawcy usług Kryptograficznych, należy wykonać tego przewodnika, aby dowiedzieć się, jak można przejścia istniejącej subskrypcji podglądu do Microsoft 365 Business GA (ogólnie dostępne).

**Jak przenieść subskrypcję Podgląd GA**

1. Zaloguj się do <a href="https://partnercenter.microsoft.com" target="_blank">Centrum partnera</a>.
2. Z pulpitu nawigacyjnego wybierz **odbiorców**, a następnie znajdź i zaznacz nazwę firmy.

    Subskrypcje dla firmy zostaną wyświetlone.

    ![Subskrypcje klienta w Centrum partnerów](images/pc_customer_subscriptions_1.png)
    
3. Na stronie **subskrypcji** firmy wybierz **Dodaj subskrypcję**.
4. Na stronie **nowej subskrypcji** wybierz **małych firm** , a następnie wybierz **Microsoft 365 Business** z listy.
5. Dodawanie liczby licencji, a następnie wybierz **Następny: Przejrzyj** do przeglądu subskrypcji i kliknij przycisk **Prześlij**.

    ![Przegląd nowej subskrypcji, aby Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Subskrypcje na podstawie licencji** pokaże **Podgląd Business 365 firmy Microsoft** i **Microsoft 365 Business**. Trzeba będzie dalej zawiesić subskrypcji podglądu.

6. Zaznacz opcję **Podgląd 365 firmy Microsoft**.
7. Na stronie **Microsoft 365 Business podglądu** wybierz **zawieszone** do zawieszenia subskrypcji podglądu.

    ![Zawiesić subskrypcji Microsoft 365 Business podglądu](images/pc_customer_m365bpreview_suspend.png)

8. Wybierz opcję **Prześlij** , aby potwierdzić.

    Na stronie **subskrypcji** upewnij się, że stan **Microsoft 365 Business Podgląd** pokazuje **zawieszone**.

    ![Potwierdzić, że stan subskrypcji podglądu jest zawieszone](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcjonalnie można zweryfikować umowę licencyjną. Aby to zrobić, wykonaj następujące kroki:
    1. Wybierz **użytkowników i licencje** ze strony **subskrypcji** firmy.
    2. Ze strony **użytkowników i licencje** wybierz użytkownika.
    3. Na stronie użytkownika w sekcji **Przypisywanie licencji** i potwierdzić, że wynika z niego **Microsoft 365 Business**.

        ![Potwierdź, że licencja Microsoft 365 Business jest przypisany do użytkownika](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Wpływ na klientów i użytkowników podczas i po przejściu

Nie ma wpływu na klientów i użytkowników podczas przejścia i przejścia post.

## <a name="impact-to-customers-who-dont-transition"></a>Wpływ na klientów, którzy nie przejścia

W następującej tabeli podsumowano wpływ zagrożenia na klientów, którzy nie przejście z subskrypcji Microsoft 365 Business podglądu do subskrypcji Microsoft 365 Business.

|       | T-0-T + 30     | T + 30-T + 60 | T + 60 do T + 120 | Poza T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stan** | W okresie prolongaty | Wygasła      | Wyłączone      | Wstrzymano jej obsługi administracyjnej |
| **Wpływa na usługę**                                                        |
| **Microsoft 365 Business administracji portalu** | Bez wpływu na funkcjonalność | Bez wpływu na funkcjonalność | Można dodawać/usuwać użytkowników, zakupu subskrypcji.</br> Nie można przypisać revoke licencje. | Skreśla się subskrypcji klienta i wszystkie dane. Administrator może zarządzać innych płatnych subskrypcji. |
| **Aplikacje pakietu Office**                         | Bez wpływu na użytkownika końcowego | Bez wpływu na użytkownika końcowego | Office przejdzie w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. | Office przejdzie w tryb zmniejszonej funkcjonalności.</br> Użytkownicy mogą wyświetlać tylko pliki. |
| **Usługi w chmurze (SharePoint Online, Exchange Online, Skype, zespołów i więcej)** | Bez wpływu na użytkownika końcowego | Bez wpływu na użytkownika końcowego | Użytkownicy końcowi i administratorzy nie mają dostępu do danych w chmurze. | Subskrypcji klienta i wszystkie dane są usuwane. |
| **Składniki EM + S** | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Możliwości przestaną być wymuszane.</br> Aby uzyskać więcej informacji, zobacz [urządzenia przenośnego wpływa na wygaśnięcia subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływu na środowisko Windows 10 PC, po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) . | Możliwości przestaną być wymuszane.</br> Aby uzyskać więcej informacji, zobacz [urządzenia przenośnego wpływa na wygaśnięcia subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływu na środowisko Windows 10 PC, po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **System Windows 10 Business** | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Możliwości przestaną być wymuszane.</br> Aby uzyskać więcej informacji, zobacz [urządzenia przenośnego wpływa na wygaśnięcia subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływu na środowisko Windows 10 PC, po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) . | Możliwości przestaną być wymuszane.</br> Aby uzyskać więcej informacji, zobacz [urządzenia przenośnego wpływa na wygaśnięcia subskrypcji](#mobile-device-impacts-upon-subscription-expiration) i [wpływu na środowisko Windows 10 PC, po wygaśnięciu subskrypcji](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **AD logowanie do komputera z systemem Windows 10** | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Brak wpływu admin</br> Bez wpływu na użytkownika końcowego | Po usunięciu dzierżawy, użytkownik może zalogować się tylko lokalnych poświadczeń. Jeśli żadne poświadczenia lokalnego ponownie utworzyć obraz urządzenia. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Urządzenie przenośne wpływa na wygaśnięcia subskrypcji

Tabela followint zawiera podsumowanie wpływu na zasady zarządzania aplikacjami na urządzeniach przenośnych.

|                            | Doświadczenie w pełni licencjonowanych                      | T + 60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Usuń pliki pracy z urządzenia nieaktywne** | Pliki robocze są usuwane po wybranych dni | Praca pliki pozostają na urządzeniach osobistych użytkownika |
| **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** | Pliki robocze można zapisywać tylko na OneDrive dla firmy | Pliki robocze można zapisać w dowolnym miejscu |
| **Szyfruj pliki służbowe** | Pliki robocze są szyfrowane. | Pliki robocze nie będą zaszyfrowane.</br> Zasady zabezpieczeń są usuwane i usunięciu danych pakietu Office w aplikacjach. |
| **Wymagaj numeru PIN lub czytnik linii papilarnych dostęp do aplikacji pakietu Office** | Ograniczony dostęp do aplikacji | Żadne ograniczenie dostępu na poziomie aplikacji |
| **Resetuj numer PIN podczas logowania nie powiedzie się.** | Ograniczony dostęp do aplikacji | Żadne ograniczenie dostępu na poziomie aplikacji |
| **Użytkownicy muszą zalogować się ponownie po bezczynności aplikacje pakietu Office** | Wymagana rejestracja w | Nie wymagana rejestracja w dostęp do aplikacji |
| **Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta** | Pliki robocze nie jest dostępny na urządzeniach ukorzenionych/jailbroken | Pliki robocze mogą być dostępne na jailbroken/ukorzenionych urządzeń |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do osobistych aplikacji** | Kopiuj/wklej ograniczone do aplikacji dostępnych w ramach subskrypcji programu Microsoft Business 365 | Kopiuj/wklej dostępne dla wszystkich aplikacji |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Komputer Windows 10 wpływa na wygaśnięcia subskrypcji

W następującej tabeli podsumowano wpływu na zasady konfiguracji urządzeń Windows 10.

|                            | Doświadczenie w pełni licencjonowanych                      | T + 60 dni po wygaśnięciu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Chronić komputery przed zagrożeniami za pomocą Windows Defender** | Włączanie/wyłączanie jest poza kontrolą użytkownika | Użytkownik może włączyć/wyłączyć programu Windows Defender na komputerze z programem Windows 10 |
| **Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge** | Ochrona komputera w programie Microsoft Edge | Użytkownik może włączyć/wyłączyć ochronę komputera w programie Microsoft Edge |
| **Wyłącz ekran device podczas bezczynności** | Administrator definiuje zasady interwał limitu czasu ekranu | Limit czasu ekranu mogą być konfigurowane przez użytkownika końcowego |
| **Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store** | Administrator określa, czy użytkownik może pobrać aplikacje Microsoft Store | Użytkownik może pobrać aplikacje Microsoft Store anytime |
| **Zezwalaj użytkownikom na korzystanie z Cortany** | Administrator definiuje zasady dostępu użytkownika do Cortana | Urządzenia użytkownika, aby włączyć/wyłączyć Cortana |
| **Zezwalaj użytkownikom na otrzymywanie i reklamy od firmy Microsoft** | Administrator definiuje zasady dla użytkownika otrzymywać porady i reklamy od firmy Microsoft | Użytkownik może włączyć/wyłączyć porady i reklamy od firmy Microsoft |
| **Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych** | Administrator definiuje zasady, aby zapewnić aktualność systemu Windows 10 urządzeń | Użytkownicy mogą decydować o terminie aktualizacji systemu Windows |




