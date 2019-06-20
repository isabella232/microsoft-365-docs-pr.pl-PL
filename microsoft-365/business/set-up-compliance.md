---
title: Zwiększ ochronę przed zagrożeniami dla Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
description: Konfigurowanie pakietu Office 365 Zaawansowana ochrona przed zagrożeniami i ochrony poufnych danych.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086370"
---
# <a name="set-up-compliance-features"></a>Konfigurowanie funkcji zgodności

365 firmy Microsoft zawiera funkcje do ochrony Twoich danych i urządzeń i pomagają zabezpieczyć Twoje i poufne informacje klientów.

## <a name="set-up-dlp-features"></a>Konfigurowanie funkcji DLP

Zobacz [Tworzenie zasad DLP z szablonu](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) , na przykład dotyczące sposobu definiowania zasad ochrony przed identyfikowalne dane osobowe. 
  
DLP zawiera wiele szablonów zasad gotowe do użycia dla wielu różnych ustawień regionalnych. Na przykład, danych finansowych Australia, Kanada ustawy informacji osobowych, danych finansowych USA, itp. Aby uzyskać pełną listę, zobacz [Szablony zasad DLP co zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Wszystkie te szablony można włączyć podobne do przykładu PII szablonu. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurowanie przechowywanie wiadomości e-mail z programu Exchange Online — archiwum

 Funkcje licencji **Exchange Online — archiwum** pomóc w zachowaniu zgodności i normami zachowując e-mail zawartości dla zbierania elektronicznych materiałów dowodowych. Również pomaga zmniejszyć ryzyko w przypadku pozwu i daje możliwość odzyskania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy. Możesz użyć sądowym, aby zachować całą zawartość użytkownika lub umożliwia dostosowywanie, mają być zachowane zasady przechowywania.
  
**Sądowym:** Można zachować całą zawartość skrzynki pocztowej przytrzymaj tym elementów usuniętych przez umieszczenie całej skrzynki pocztowej użytkownika na postępowania sądowego. 
    
Aby umieścić skrzynkę pocztową z postępowaniem sądowym, w Centrum administracyjnym:
    
1. W nawigacji z lewej strony, przejdź do **użytkowników** \> **aktywnych użytkowników**.
    
2. Wybierz użytkownika, której skrzynkę pocztową chcesz umieścić na spory sądowe przytrzymaj i w okienku użytkownika rozwiń **Ustawienia poczty** i obok **Więcej ustawień** , wybierz polecenie **Właściwości, edytowanie programu Exchange**.
    
3. Na stronie skrzynki pocztowej użytkownika, wybierz opcję ** Funkcje skrzynki pocztowej ** na nawigacji z lewej strony, a następnie wybierz **Włącz** łącze w obszarze **sądowym**.
    
4. W **sądowym** okno dialogowe można określić postępowania sądowego przytrzymaj czasu trwania w polu **czas trwania sądowym** , pozostaw pole puste, jeśli chcesz umieścić nieskończone blokady. Można również dodawać notatki i bezpośrednie właściciela pola korespondencji do witryny, może zajść potrzeba wyjaśnienia, więcej informacji na temat postępowania sądowego przytrzymaj \> **zapisać**.
    
**Retencji:** Zasady przechowywania niestandardowe, na przykład, można włączyć w celu zachowania przez określoną ilość czasu lub trwale usunąć zawartość z końcem okresu przetrzymania. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Konfigurowanie funkcji ochrony informacji Azure

Ochrona informacji Azure (AIP) pomaga klasyfikowania i opcjonalnie chronić Twoje dokumenty i wiadomości e-mail, stosując etykiety. Etykiety można automatycznie zastosowane przez administratorów, którzy definiują zasady i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, gdzie użytkownicy są podane zalecenia.

W programie Outlook w sieci web do wiadomości e-mail można zastosować następujące etykiety wbudowanych i ograniczenia:
  
- **Nie przesyłaj dalej**: Adresaci mogą czytać wiadomości, ale one nie można przesłać dalej, wydrukować ani skopiować zawartości
    
- **Szyfruj**: całą wiadomość jest zaszyfrowana. Adresaci muszą potwierdzić swoją tożsamość przed uzyskaniem dostępu do zaszyfrowanej zawartości i nie można usunąć szyfrowania.
    
- **Poufne**: daje pracowników w firmie pełne uprawnienia w odniesieniu do treści wiadomości e-mail i załączniki, ale nie do osób spoza organizacji. Właścicieli danych można śledzić i odwołać zawartości w dowolnym momencie.
    
- **Ściśle tajne**: tego ograniczenia mogą być stosowane do ściśle poufne dane, dzięki czemu pracownicy wyświetlić, edytować i odpowiedzieć, ale nie do przodu, drukowania lub kopiowania danych. Właścicieli danych można śledzić i odwołać zawartości w dowolnym momencie.

### <a name="make-sure-azure-information-protection-is-activated"></a>Upewnij się, że włączono ochronę informacji Azure

Aby zweryfikować, że AIP jest włączona:

1. Zalogować się do [portalu Azure](https://portal.azure.com/).

2. Wybierz **wszystkie usługi** i typ w *Ochronie informacji Azure* w **Pole wyszukiwania**.

3. Gdy wyniki są wyświetlane, kliknij przycisk start, dalej do **Ochrony informacji Azure** , aby dodać ją do ulubionych i łatwo później odnaleźć.

4. Wybierz opcję **Ochrony informacji Azure** \> **aktywacji ochrony** i upewnij się, że stan jest ustawiony do aktywowany. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Wyświetlanie etykiety zasad i domyślną ochronę informacji Azure 

Aby przeglądać i modyfikować, istniejące etykiety:

1. Na pulpicie nawigacyjnym Azure ochrony informacji, wybierz **Klasyfikacje** \> **etykiety**. <br/>![Standardowe etykiety dla ochrony informacji Azure.](media/AIPLabels.png)

2. Wszelkie etykiety, aby wyświetlić opcje można wybrać, można zmienić nazwę wyświetlaną, kolory itd.
 
3. Zobacz [Modyfikuj i Utwórz nowe etykiety](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Jeśli chcesz tworzyć swoje własne. 

### <a name="install-the-azure-information-protection-client-manually"></a>Ręcznie zainstaluj klienta ochrony informacji Azure

Aby ręcznie zainstalować klienta AIP:

1. **AzInfoProtection.exe** pobrać z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Można sprawdzić, czy instalacja zadziałała wyświetlając dokument programu Word i upewniając się, że opcja **Ochrona** jest dostępna na karcie **Narzędzia główne** . <br/>![Kartę Ochrona listy rozwijanej w dokumencie programu Word.](media/Word_Protect.png)

Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
