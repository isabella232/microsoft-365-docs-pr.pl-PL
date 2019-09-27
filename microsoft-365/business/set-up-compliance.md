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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami w pakiecie Office 365 i Chroń poufne dane.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288750"
---
# <a name="set-up-compliance-features"></a>Konfigurowanie funkcji zgodności

Twoja firma Microsoft 365 Business zawiera funkcje chroniące dane i urządzenia oraz pomagające w zabezpieczeniu poufnych informacji Twoich i Twoich klientów.

## <a name="set-up-dlp-features"></a>Konfigurowanie funkcji DLP

Zobacz [Tworzenie zasad DLP z szablonu](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) , aby zapoznać się z przykładem sposobu konfigurowania zasad w celu ochrony przed danymi osobowymi (PII). 
  
DLP zawiera wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych. Na przykład, Australia dane finansowe, Kanada informacje osobiste Act, dane finansowe USA, itp. Zobacz [, jakie szablony zasad DLP zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pełną listę. Wszystkie te szablony można włączyć podobne do przykładu szablonu PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurowanie przechowywania poczty e-mail przy użyciu usługi Exchange Online archiwizacji

 Funkcje **programu Exchange Online archiwizowanie** licencji ułatwiają zachowanie zgodności i standardów regulacyjnych przez zachowanie zawartości poczty elektronicznej na potrzeby zbierania elektronicznych materiałów dowodowych. Pomaga również zmniejszyć ryzyko w przypadku pozew i umożliwia odzyskanie danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy. Aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować, możesz użyć wstrzymania w postępowaniu sądowym.
  
**Sądowym:** Możesz zachować całą zawartość skrzynki pocztowej, w tym elementy usunięte, umieszczając całą skrzynkę pocztową użytkownika w postępowaniu sądowym. 
    
Aby umieścić skrzynkę pocztową w postępowaniu sądowym, w centrum administracyjnym:
    
1. W lewym NAV przejdź do **użytkowników** \> **aktywnych**użytkowników.
    
2. Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić na sądowym i w okienku użytkownika rozwiń **Ustawienia poczty** i obok **więcej ustawień** wybierz **Edytuj właściwości programu Exchange**.
    
3. Na stronie skrzynki pocztowej dla użytkownika wybierz * * funkcje skrzynki pocztowej * * na lewej NAV, a następnie wybierz **Włącz** łącze w związku z **postępowaniem sądowym**.
    
4. W oknie dialogowym wstrzymanie w postępowaniu **sądowym** można określić czas trwania wstrzymania w trakcie postępowania sądowego w polu **czas trwania wstrzymania** , pozostawić pole puste, jeśli chcesz umieścić nieskończoną wstrzymania. Można również dodawać notatki i kierować właścicielem skrzynki pocztowej do witryny sieci Web może być trzeba wyjaśnić więcej o sądowym wstrzymanie \> **zapisywania**.
    
**Zatrzymanie:** Można włączyć niestandardowe zasady przechowywania, na przykład, aby zachować określoną ilość czasu lub trwale usunąć zawartość na końcu okresu przechowywania. Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Konfigurowanie funkcji usługi Azure Information Protection

Usługa Azure Information Protection (AIP) pomaga klasyfikować i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety. Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub przy użyciu kombinacji, gdzie użytkownicy są podane zalecenia.

W programie Outlook w sieci Web można zastosować następujące wbudowane etykiety i ograniczenia do wiadomości e-mail:
  
- **Nie przesyłają dalej**: odbiorcy mogą odczytać wiadomość, ale nie mogą przekazywać, drukować ani kopiować zawartości
    
- **Encrypt**: cała wiadomość jest szyfrowana. Odbiorcy muszą potwierdzić swoją tożsamość przed uzyskaniem dostępu do zaszyfrowanej zawartości i nie mogą usunąć szyfrowania.
    
- **Poufne**: zapewnia pracownikom w organizacji pełne uprawnienia do zawartości wiadomości e-mail i załączników, ale nie do osób spoza organizacji. Właściciele danych mogą śledzić i odwoływać zawartość w dowolnym momencie.
    
- **Wysoce poufne**: to ograniczenie można zastosować do wysoce poufnych danych, umożliwiając pracownikom wyświetlanie, edytowanie i odpowiadanie, ale nie przekazywanie, drukowanie lub kopiowanie danych. Właściciele danych mogą śledzić i odwoływać zawartość w dowolnym momencie.

### <a name="make-sure-azure-information-protection-is-activated"></a>Upewnij się, że usługa Azure Information Protection jest aktywna

Aby sprawdzić, czy włączono AIP:

1. Zaloguj się do [witryny Azure Portal](https://portal.azure.com/).

2. Wybierz **wszystkie usługi** i wpisz w *usłudze Azure Information Protection* w **polu wyszukiwania**.

3. Po wyświetleniu wyników kliknij przycisk Start obok **usługi Azure Information Protection** , aby uczynić go ulubionym i łatwo znaleźć później.

4. Wybierz \> **aktywacji ochrony** **informacji Azure** i upewnij się, że stan jest ustawiony na aktywowany. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Wyświetlanie zasad usługi Azure Information Protection i etykiet domyślnych 

Aby wyświetlić i zmodyfikować istniejące etykiety:

1. Na pulpicie nawigacyjnym usługi Azure Information Protection wybierz pozycję **klasyfikacje** \> **etykiet**. <br/>![Standardowe etykiety dla usługi Azure Information Protection.](media/AIPLabels.png)

2. Można wybrać dowolną etykietę, aby wyświetlić opcje, można zmienić nazwę wyświetlaną, kolory, itp.
 
3. Zobacz [modyfikowanie i tworzenie nowych etykiet](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) , jeśli chcesz tworzyć własne. 

### <a name="install-the-azure-information-protection-client-manually"></a>Ręczne instalowanie klienta usługi Azure Information Protection

Aby ręcznie zainstalować klienta AIP:

1. Pobierz **Azinfoprotection. exe** z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Można sprawdzić, czy instalacja zadziałało, przeglądając dokument programu Word i upewniając się, że opcja **Chroń** jest dostępna na karcie **Narzędzia główne** . <br/>![Karta ochrona listy rozwijanej w dokumencie programu Word.](media/Word_Protect.png)

Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
