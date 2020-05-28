---
title: Zwiększenie ochrony przed zagrożeniami dla usługi Microsoft 365 dla firm
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami w usłudze Office 365 i zabezpiecz poufne dane przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami.
ms.openlocfilehash: 6fa4d1595c379aaccf3a0cbfca020fbd32376fb9
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400875"
---
# <a name="increase-threat-protection"></a>Zwiększenie ochrony przed zagrożeniami

Ten artykuł pomaga zwiększyć ochronę w subskrypcji usługi Microsoft 365 w celu ochrony przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami. Zalecenia te są odpowiednie dla organizacji o zwiększonym zapotrzebowaniu na bezpieczeństwo, takich jak kancelarie prawne i kliniki opieki zdrowotnej.

Przed rozpoczęciem sprawdź bezpieczny wynik usługi Office 365. Usługa Office 365 Secure Score analizuje zabezpieczenia organizacji na podstawie regularnych działań i ustawień zabezpieczeń oraz przypisuje wynik. Zacznij od uwzględnienia bieżącego wyniku. Aby zwiększyć swój wynik, wykonaj czynności zalecane w tym artykule. Celem nie jest osiągnięcie maksymalnego wyniku, ale uświadomienie sobie możliwości ochrony środowiska, które nie wpływają negatywnie na produktywność użytkowników. 

Aby uzyskać więcej informacji, zobacz [Microsoft Secure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podniesienie poziomu ochrony przed złośliwym oprogramowaniem w poczcie

Środowisko usługi Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem. Tę ochronę można zwiększyć, blokując załączniki z typami plików, które są powszechnie używane do złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomościach e-mail:
  
1. Przejdź do danych logowania do [https://protection.office.com](https://protection.office.com) konta administratora i zaloguj się. 
    
2. W Centrum zgodności zabezpieczeń &amp; w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Ochrona** \> **przed złośliwym oprogramowaniem**zasad .
    
3. Kliknij dwukrotnie domyślną zasadę, aby edytować te zasady dla całej firmy.
    
4. Wybierz **pozycję Ustawienia**.
    
5. W obszarze **Filtr Typowych typów załączników**wybierz pozycję **Włączone**. Typy plików, które są zablokowane są wyświetlane w oknie bezpośrednio poniżej tego formantu. Upewnij się, że dodano następujące typy plików:
   - ade, adp, ani, bas, nietoperz, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   W razie potrzeby można dodać lub usunąć typy plików później.
    
6. Wybierz **pozycję Zapisz.**
    
Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrona przed oprogramowaniem wymuszającym okup

Ransomware ogranicza dostęp do danych poprzez szyfrowanie plików lub blokowanie ekranów komputerów. Następnie próbuje wyłudzać pieniądze od ofiar, prosząc o "okup", zwykle w postaci kryptowalut, takich jak Bitcoin, w zamian za dostęp do danych. 
  
Aby chronić przed oprogramowaniem wymuszającym okup, utwórz jedną lub więcej reguł przepływu poczty, aby zablokować rozszerzenia plików, które są powszechnie używane w przypadku oprogramowania wymuszającego okup. (Te reguły zostały dodane w [celu podniesienia poziomu ochrony przed złośliwym oprogramowaniem w](#raise-the-level-of-protection-against-malware-in-mail) kroku poczty). Możesz też ostrzec użytkowników, którzy otrzymają te załączniki w wiadomości e-mail.

Oprócz plików zablokowanych w poprzednim kroku dobrą praktyką jest utworzenie reguły ostrzegającej użytkowników przed otwarciem załączników plików pakietu Office, które zawierają makra. Ransomware może być ukryty wewnątrz makr, więc ostrzegaj użytkowników, aby nie otwierali tych plików od osób, których nie znają.

Aby utworzyć regułę transportu poczty:
  
1. Przejdź do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> programie , i wybierz pozycję Centra **administracyjne** \> **Exchange**.
    
2. W kategorii **przepływ poczty** wybierz **pozycję reguły**.
    
3. Wybierz **+** , a następnie wybierz pozycję **Utwórz nową regułę**.
    
4. Wybierz **pozycję Więcej opcji** u dołu okna dialogowego, aby wyświetlić pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli dla reguły. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.
    
6. Wybierz pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office**||
|:-----|:-----|:-----|
|Name (Nazwa)  <br/> |Reguła ochrony przed oprogramowaniem wymuszającym okup: ostrzegaj użytkowników  <br/>  |
|Zastosuj tę regułę, jeśli . . .  <br/> |Dowolny załącznik . . . rozszerzenie pliku pasuje . . .  <br/> |
|Określanie słów lub fraz  <br/> |Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Wykonaj następujące czynności . . .  <br/> |Powiadamianie adresata wiadomością  <br/> |
|Podaj tekst wiadomości  <br/> |Nie należy otwierać tego typu plików od osób, których nie znasz, ponieważ mogą one zawierać makra ze złośliwym kodem.  <br/> |
   
Aby uzyskać więcej informacji, zobacz:
  
- [Jak radzić sobie z oprogramowaniem wymuszającym okup](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Przywracanie usługi OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zatrzymywanie automatycznego przekazywania wiadomości e-mail

Hakerzy uzyskujący dostęp do skrzynki pocztowej użytkownika mogą kraść pocztę, ustawiając skrzynkę pocztową na automatyczne przesyłanie dalej wiadomości e-mail. Może się to zdarzyć nawet bez świadomości użytkownika. Aby temu zapobiec, skonfiguruj regułę przepływu poczty. 
  
Aby utworzyć regułę transportu poczty, obejrzyj [ten krótki klip wideo](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) lub wykonaj następujące czynności:
  
1. W centrum administracyjnym usługi Microsoft 365 wybierz pozycję **Centra administracyjne** \> **programu Exchange**.
    
2. W kategorii **przepływ poczty** wybierz **pozycję reguły**.
    
3. Wybierz **+** , a następnie wybierz pozycję **Utwórz nową regułę**.
    
4. Aby wyświetlić wszystkie opcje, wybierz **pozycję Więcej opcji** u dołu okna dialogowego. 
    
5. Zastosuj ustawienia w poniższej tabeli. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.
    
6. Wybierz pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office**|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zapobieganie automatycznemu przekazywaniu wiadomości e-mail do domen zewnętrznych  <br/> |
|Zastosuj tę regułę, jeśli ...  <br/> |Nadawca . . . jest zewnętrzna/wewnętrzna . . . Wewnątrz organizacji  <br/> |
|Dodaj warunek  <br/> |Właściwości wiadomości . . . uwzględnić typ wiadomości . . . Automatyczne przekazywanie do przodu  <br/> |
|Wykonaj następujące czynności ...  <br/> |Zablokuj wiadomość . . . odrzucić wiadomość i dołączyć wyjaśnienie.  <br/> |
|Podaj tekst wiadomości  <br/> |Ze względów bezpieczeństwa uniemożliwiona jest automatyczne przekazywanie wiadomości e-mail poza tą organizacją.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrona poczty e-mail przed atakami phishingowymi

Jeśli skonfigurowano co najmniej jedną domenę niestandardową dla środowiska usługi Office 365 lub Microsoft 365, możesz skonfigurować ukierunkowaną ochronę przed wyłudzaniem informacji. Ochrona przed wyłudzaniem informacji przez narzędzie ATP, część zaawansowanej ochrony przed zagrożeniami usługi Office 365, może pomóc chronić twoją organizację przed złośliwymi atakami phishingowymi opartymi na personifikacjach i innymi atakami phishingowymi. Jeśli domena niestandardowa nie została skonfigurowana, nie musisz tego robić.
  
Zalecamy rozpoczęcie pracy z tą ochroną, tworząc zasady chroniące najważniejszych użytkowników i domenę niestandardową. 

Aby utworzyć zasady przeciwdziałania wyłudzaniem informacji przez narzędzie ATP, obejrzyj [ten krótki film szkoleniowy](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)lub wykonaj następujące czynności:
  
1. Przejdź do witryny [https://protection.office.com](https://protection.office.com). 
    
2. W Centrum zgodności zabezpieczeń &amp; w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie **Zasady** wybierz pozycję **ATP anti-phishing**.
    
4. Na stronie **Ochrona przed wyłudzaniem informacji** wybierz pozycję + **Utwórz**. Uruchamia się kreator, który przeprowadzi Cię przez definiowanie zasad ochrony przed wyłudzaniem informacji.
    
5. Określ nazwę, opis i ustawienia zasad zgodnie z zaleceniami w poniższej tabeli. Aby uzyskać więcej informacji, zobacz [Dowiedz się więcej o opcjach zasad przeciwdziałania wyłudzaniem informacji o atp](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Po przejrzeniu ustawień wybierz pozycję **Utwórz tę zasadę** lub **Zapisz**, stosownie do przypadku.
    

|**Ustawienie lub opcja**<br/>|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Domena i najcenniejszy personel kampanii  <br/> |
|Opis  <br/> |Upewnij się, że najważniejszy personel i nasza domena nie są personifikowane.  <br/> |
|Dodawanie użytkowników do ochrony  <br/> |Wybierz **+ Dodaj warunek, odbiorcą jest**. Wpisz nazwy użytkowników lub wpisz adres e-mail kandydata, menedżera kampanii i innych ważnych członków personelu. Można dodać maksymalnie 20 adresów wewnętrznych i zewnętrznych, które mają być chronione przed personifikacją.  <br/> |
|Dodawanie domen do ochrony  <br/> |Wybierz **+ Dodaj warunek, domena adresata to**. Wprowadź domenę niestandardową skojarzoną z subskrypcją usługi Microsoft 365, jeśli została zdefiniowana. Można wprowadzić więcej niż jedną domenę.  <br/> |
|Wybieranie akcji  <br/> |Jeśli wiadomość e-mail jest wysyłana przez użytkownika personifikowanego: wybierz **opcję Przekieruj wiadomość na inny adres e-mail,** a następnie wpisz adres e-mail administratora zabezpieczeń; na przykład *Alicja <span> <span> @contoso.com*. Jeśli wiadomość e-mail jest wysyłana przez domenę personifikacji: wybierz **komunikat Kwarantanna**.  <br/> |
|Inteligencja skrzynek pocztowych  <br/> |Domyślnie podczas tworzenia nowej zasady ochrony przed wyłudzaniem informacji jest wybierana jest inteligencja skrzynek pocztowych. Pozostaw to ustawienie **Włączone,** aby uzyskać najlepsze wyniki.  <br/> |
|Dodawanie zaufanych nadawców i domen  <br/> |W tym miejscu możesz dodać własną domenę lub inne zaufane domeny.  <br/> |
|Stosowane do  <br/> |**Wybierz domenę adresata**. W **obszarze Dowolna z tych**opcji wybierz pozycję **Wybierz**. Wybierz **+ Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso. <span> <span> com*, na liście, a następnie wybierz pozycję **Dodaj**. Wybierz **opcję Gotowe**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrona przed złośliwymi załącznikami i plikami za pomocą bezpiecznych załączników ATP

Użytkownicy regularnie wysyłają, odbierają i udostępniają załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Nie zawsze jest łatwo stwierdzić, czy załącznik jest bezpieczny czy złośliwy, patrząc na wiadomość e-mail. Zaawansowana ochrona przed zagrożeniami usługi Office 365 obejmuje ochronę bezpiecznego załącznika ATP, ale ta ochrona nie jest domyślnie włączona. Zaleca się utworzenie nowej reguły, aby rozpocząć korzystanie z tej ochrony. Ta ochrona obejmuje pliki w programie SharePoint, OneDrive i usłudze Microsoft Teams.
  
Aby utworzyć zasady bezpiecznego załącznika ATP, obejrzyj [ten krótki klip wideo](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)lub wykonaj następujące czynności:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) programu i zaloguj się za pomocą konta administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie Zasady wybierz pozycję **Bezpieczne załączniki ATP**.
    
4. Na stronie Bezpieczne załączniki zastosuj tę ochronę szeroko, zaznaczając pole wyboru **Włącz atp dla programu SharePoint, OneDrive i Microsoft Teams.** 
    
5. Wybierz, **+** aby utworzyć nową zasadę. 
    
6. Zastosuj ustawienia w poniższej tabeli. 
    
7. Po przejrzeniu ustawień wybierz pozycję **Utwórz tę zasadę** lub **Zapisz**, stosownie do przypadku.
    

|**Ustawienie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Blokowanie bieżących i przyszłych wiadomości e-mail z wykrytym złośliwym oprogramowaniem.  <br/> |
|Opis  <br/> |Blokowanie bieżących i przyszłych wiadomości e-mail i załączników za pomocą wykrytego złośliwego oprogramowania.  <br/> |
|Zapisywanie załączników nieznaną odpowiedzią na złośliwe oprogramowanie  <br/> |Wybierz **pozycję Blokuj — blokowanie bieżących i przyszłych wiadomości e-mail i załączników za pomocą wykrytego złośliwego oprogramowania**.  <br/> |
|Przekierowywanie załącznika po wykryciu  <br/> |Włącz przekierowanie (zaznacz to pole) Wprowadź konto administratora lub konfigurację skrzynki pocztowej do kwarantanny.          Zastosuj powyższy wybór, jeśli czas skanowania załączników lub wystąpienie błędu w przypadku złośliwego oprogramowania w poszukiwaniu załączników (zaznacz to pole).  <br/> |
|Stosowane do  <br/> |Domeną adresata jest domena . . . wybierz swoją domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Konfigurowanie zasad ochrony przed wyłudzaniem informacji przez usługi Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrona przed atakami phishingowymi dzięki bezpiecznych linkach ATP

Hakerzy czasami ukrywają złośliwe strony internetowe w linkach w wiadomościach e-mail lub innych plikach. Bezpieczne łącza usługi Office 365 ATP (ATP Safe Links), część zaawansowanej ochrony przed zagrożeniami usługi Office 365, mogą pomóc w ochronie organizacji, zapewniając weryfikację adresów sieci Web (URL) w wiadomościach e-mail i dokumentach pakietu Office. Ochrona jest definiowana za pomocą zasad bezpiecznych łączy ATP.
  
Zaleca się wykonanie następujących czynności:
  
- Zmodyfikuj domyślną zasadę, aby zwiększyć ochronę.
    
- Dodaj nową zasadę skierowaną do wszystkich adresatów w domenie.
    
Aby skonfigurować bezpieczne łącza ATP, obejrzyj [ten krótki film szkoleniowy](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)lub wykonaj następujące czynności:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) programu i zaloguj się za pomocą konta administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie Zasady wybierz pozycję **Bezpieczne łącza ATP**.
    
Aby zmodyfikować domyślną zasadę:
  
1. Na stronie Bezpieczne łącza w obszarze **Zasady dotyczące całej organizacji**wybierz pozycję **Domyślne** zasady. 
    
2. W **obszarze Ustawienia dotyczące zawartości z wyjątkiem poczty e-mail**wybierz pozycję Microsoft **365 Apps for enterprise, Office for iOS i Android**.
    
3. Wybierz pozycję **Zapisz**. 
    
Aby utworzyć nową zasadę skierowaną do wszystkich adresatów w domenie:
  
1. Na stronie Bezpieczne łącza w obszarze **Zasady dotyczące całej organizacji**wybierz pozycję **+** Utwórz nową zasadę. 
    
2. Zastosuj ustawienia wymienione w poniższej tabeli.
    
3. Wybierz pozycję **Zapisz**. 

|**Ustawienie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zasady dotyczące bezpiecznych łączy dla wszystkich adresatów w domenie  <br/> |
|Wybierz akcję dla nieznanych potencjalnie złośliwych adresów URL w wiadomościach  <br/> |Wybierz **on - adresy URL zostaną przepisane i sprawdzone względem listy znanych złośliwych linków, gdy użytkownik kliknie link**.  <br/> |
|Skanowanie zawartości do pobrania za pomocą bezpiecznych załączników  <br/> |Zaznacz to pole.  <br/> |
|Stosowane do  <br/> |Domeną adresata jest domena . . . wybierz swoją domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Bezpieczne łącza usługi Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do [witryny Azure portal](https://portal.azure.com/).

2. Wybierz **pozycję Wszystkie usługi** i wpisz w *usłudze Intune* w **polu wyszukiwania**.

3. Gdy wyniki pojawią się, wybierz start obok **usługi Microsoft Intune,** aby uczynić ją ulubioną i łatwą do znalezienia później.

Oprócz centrum administracyjnego można używać usługi Intune do rejestrowania urządzeń organizacji i zarządzania nimi. Aby uzyskać więcej informacji, zobacz [Możliwości według metody rejestracji dla urządzeń z systemem Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) i opcje rejestracji dla urządzeń [zarządzanych przez usługę Intune](https://docs.microsoft.com/intune/enrollment-options).
