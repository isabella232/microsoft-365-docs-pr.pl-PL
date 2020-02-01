---
title: Zwiększ ochronę przed zagrożeniami dla firmy Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami w usłudze Office 365 i zabezpiecz poufne dane.
ms.openlocfilehash: 191e1ad301e12ae45fe3a5d6d990d2357c5d0bab
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593886"
---
# <a name="increase-threat-protection"></a>Zwiększenie ochrony przed zagrożeniami

Ten artykuł pomaga zwiększyć ochronę subskrypcji usługi Microsoft 365 w celu ochrony przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami. Zalecenia te są odpowiednie dla organizacji o zwiększonym zapotrzebowania na bezpieczeństwo, takich jak kancelarie prawne i kliniki opieki zdrowotnej.

Przed rozpoczęciem sprawdź bezpieczny wynik usługi Office 365. Usługa Office 365 Secure Score analizuje zabezpieczenia organizacji usługi Office 365 na podstawie regularnych działań i ustawień zabezpieczeń oraz przypisuje wynik. Zacznij od uwzględnienia aktualnego wyniku. Aby zwiększyć wynik, wykonaj czynności zalecane w tym artykule. Celem nie jest osiągnięcie maksymalnego wyniku, ale świadomość możliwości ochrony środowiska, które nie wpływają negatywnie na produktywność użytkowników. 

Aby uzyskać więcej informacji, zobacz [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podniesienie poziomu ochrony przed złośliwym oprogramowaniem w poczcie

Środowisko usługi Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem. Możesz zwiększyć tę ochronę, blokując załączniki z typami plików, które są powszechnie używane w przypadku złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomościach e-mail:
  
1. Przejdź [https://protection.office.com](https://protection.office.com) do poświadczeń konta administratora i zaloguj się. 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady** \> **chroniące przed złośliwym oprogramowaniem**.
    
3. Kliknij dwukrotnie domyślne zasady, aby edytować tę zasadę dla całej firmy.
    
4. Wybierz **pozycję Ustawienia**.
    
5. W obszarze **Filtr typowych typów załączników**wybierz **pozycję Wł.** Zablokowane typy plików są wyświetlane w oknie bezpośrednio pod tym formantem. Upewnij się, że dodajesz następujące typy plików:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   W razie potrzeby można później dodać lub usunąć typy plików.
    
6. Wybierz **pozycję Zapisz.**
    
Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrona przed oprogramowaniem ransomware

Ransomware ogranicza dostęp do danych, szyfrując pliki lub blokując ekrany komputerów. Następnie próbuje wyłudzić pieniądze od ofiar, prosząc o "okup", zwykle w postaci kryptowalut, takich jak Bitcoin, w zamian za dostęp do danych. 
  
Aby chronić przed oprogramowaniem wymuszającym okup, utwórz co lub więcej reguł przepływu poczty, aby zablokować rozszerzenia plików, które są powszechnie używane w oprogramowaniu ransomware. (Te reguły zostały dodane w [celu podniesienia poziomu ochrony przed złośliwym oprogramowaniem w](#raise-the-level-of-protection-against-malware-in-mail) kroku poczty). Możesz również ostrzec użytkowników, którzy otrzymują te załączniki w wiadomości e-mail.

Oprócz plików zablokowanych w poprzednim kroku, dobrą praktyką jest utworzenie reguły ostrzegającej użytkowników przed otwarciem załączników plików pakietu Office, które zawierają makra. Ransomware może być ukryty w makrach, więc ostrzegaj użytkowników, aby nie otwierali tych plików od osób, których nie znają.

Aby utworzyć regułę transportu poczty:
  
1. Przejdź do centrum <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administracyjnego w programie , a nie wybieraj **pozycję Centra** \> administracyjne **Exchange**.
    
2. W kategorii **przepływ poczty** wybierz **reguły**.
    
3. Zaznacz **+**, a następnie wybierz pozycję **Utwórz nową regułę**.
    
4. Wybierz **pozycję Więcej opcji** u dołu okna dialogowego, aby wyświetlić pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli reguły. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.
    
6. Wybierz pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzeganie użytkowników przed otwarciem załączników plików pakietu Office**||
|:-----|:-----|:-----|
|Name (Nazwa)  <br/> |Reguła anty-ransomware: ostrzegaj użytkowników  <br/>  |
|Zastosuj tę regułę, jeśli . . .  <br/> |Dowolny załącznik . . . rozszerzenie pliku pasuje do pliku . . .  <br/> |
|Określanie wyrazów lub fraz  <br/> |Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Wykonaj następujące czynności . . .  <br/> |Powiadamianie adresata o wiadomości  <br/> |
|Podaj tekst wiadomości  <br/> |Nie otwieraj plików tego typu od osób, których nie znasz, ponieważ mogą one zawierać makra ze złośliwym kodem.  <br/> |
   
Aby uzyskać więcej informacji, zobacz:
  
- [Jak radzić sobie z oprogramowaniem ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Przywracanie usługi OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zatrzymywanie automatycznego przekazywania wiadomości e-mail

Hakerzy, którzy uzyskują dostęp do skrzynki pocztowej użytkownika, mogą wykraść pocztę, ustawiając skrzynkę pocztową tak, aby automatycznie przesyłała wiadomości e-mail. Może się to zdarzyć nawet bez świadomości użytkownika. Aby temu zapobiec, skonfiguruj regułę przepływu poczty. 
  
Aby utworzyć regułę transportu poczty, obejrzyj [ten krótki film](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) lub wykonaj następujące czynności:
  
1. W centrum administracyjnym programu Microsoft 365 wybierz pozycję **Centra** \> administracyjne **programu Exchange**.
    
2. W kategorii **przepływ poczty** wybierz **reguły**.
    
3. Zaznacz **+**, a następnie wybierz pozycję **Utwórz nową regułę**.
    
4. Aby wyświetlić wszystkie opcje, wybierz **pozycję Więcej opcji** u dołu okna dialogowego. 
    
5. Zastosuj ustawienia w poniższej tabeli. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.
    
6. Wybierz pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzeganie użytkowników przed otwarciem załączników plików pakietu Office**|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zapobieganie automatycznemu przekazywaniu wiadomości e-mail do domen zewnętrznych  <br/> |
|Zastosuj tę regułę, jeśli ...  <br/> |Nadawca . . . jest zewnętrzna/wewnętrzna. . . Wewnątrz organizacji  <br/> |
|Dodaj warunek  <br/> |Właściwości wiadomości . . . dołącz typ wiadomości . . . Automatyczne przesyłanie do przodu  <br/> |
|Wykonaj następujące czynności ...  <br/> |Zablokuj wiadomość . . . odrzucić wiadomość i dołączyć wyjaśnienie.  <br/> |
|Podaj tekst wiadomości  <br/> |Automatyczne przekazywanie wiadomości e-mail poza tą organizacją jest uniemożliwione ze względów bezpieczeństwa.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Chroń swój adres e-mail przed atakami phishingowymi

Jeśli skonfigurowano co lub więcej domen niestandardowych dla środowiska usługi Office 365 lub Microsoft 365, możesz skonfigurować ukierunkowaną ochronę przed wyłudzaniem informacji. Ochrona przed wyłudzaniem informacji w usłudze ATP, część zaawansowanej ochrony przed zagrożeniami w usłudze Office 365, może pomóc chronić organizację przed złośliwymi atakami phishingowymi opartymi na personifikacji i innymi atakami phishingowymi. Jeśli domena nie została skonfigurowana, nie musisz tego robić.
  
Zaleca się rozpoczęcie pracy z tą ochroną, tworząc zasady chroniące najważniejszych użytkowników i domenę niestandardową. 

Aby utworzyć zasady przeciwdziałania wyłudzaniu informacji w atp, obejrzyj [ten krótki film szkoleniowy](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)lub wykonaj następujące czynności:
  
1. Przejdź do witryny [https://protection.office.com](https://protection.office.com). 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie **Zasady** wybierz pozycję **ATP anti-phishing**.
    
4. Na stronie **Anti-phishing (Ochrona przed wyłudzaniem informacji)** wybierz **pozycję + Utwórz**. Uruchamia kreatora, który przeprowadzi Cię przez zdefiniowanie zasad antyphishingowych.
    
5. Określ nazwę, opis i ustawienia zasad zgodnie z zaleceniami w poniższej tabeli. Aby uzyskać więcej informacji, [zobacz Dowiedz się więcej o opcjach zasad antyphishingowych ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) 
    
6. Po przejrzeniu ustawień wybierz pozycję **Utwórz tę zasadę** lub **Zapisz**, stosownie do potrzeb.
    

|**Ustawianie lub opcja**<br/>|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Domena i najcenniejszych pracowników kampanii  <br/> |
|Opis  <br/> |Upewnij się, że najważniejszy personel i nasza domena nie są podszywane.  <br/> |
|Dodawanie użytkowników do ochrony  <br/> |Wybierz **+ Dodaj warunek, odbiorcą jest**. Wpisz nazwy użytkowników lub wprowadź adres e-mail kandydata, menedżera kampanii i innych ważnych pracowników. Można dodać maksymalnie 20 adresów wewnętrznych i zewnętrznych, które mają być chronione przed personifikacją.  <br/> |
|Dodawanie domen do ochrony  <br/> |Wybierz **+ Dodaj warunek, domena adresata jest**. Jeśli zdefiniowano domenę niestandardową skojarzoną z subskrypcją usługi Microsoft 365, wprowadź domenę niestandardową skojarzoną z subskrypcją usługi Microsoft 365. Możesz wprowadzić więcej niż jedną domenę.  <br/> |
|Wybierz akcje  <br/> |Jeśli osoba jest wysyłana przez osobę podszywającą się pod osobę, wybierz **opcję Przekieruj wiadomość na inny adres e-mail,** a następnie wpisz adres e-mail administratora zabezpieczeń; na przykład *<span><span>Alicja @contoso.com*. Jeśli wiadomość e-mail jest wysyłana przez domenę podszywającą się pod osoby: wybierz **wiadomość kwarantanny**.  <br/> |
|Inteligencja skrzynki pocztowej  <br/> |Domyślnie podczas tworzenia nowych zasad zapobiegających wyłudzaniu informacji jest wybierana inteligencja skrzynek pocztowych. Pozostaw to ustawienie **włączone,** aby uzyskać najlepsze wyniki.  <br/> |
|Dodawanie zaufanych nadawców i domen  <br/> |W tym miejscu możesz dodać własną domenę lub inne zaufane domeny.  <br/> |
|Stosowane do  <br/> |Wybierz **pozycję Domena adresata to**. W **obszarze Dowolne z nich**wybierz pozycję **Wybierz**. Wybierz **+ Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso.<span> com <span>*, na liście, a następnie wybierz pozycję **Dodaj**. Wybierz **gotowe**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrona przed złośliwymi załącznikami i plikami za pomocą bezpiecznych załączników ATP

Użytkownicy regularnie wysyłają, odbierają i udostępniają załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Nie zawsze jest łatwo stwierdzić, czy załącznik jest bezpieczny, czy złośliwy, patrząc na wiadomość e-mail. Zaawansowana ochrona przed zagrożeniami usługi Office 365 obejmuje ochronę bezpiecznego załącznika usługi ATP, ale ta ochrona nie jest domyślnie włączona. Zaleca się utworzenie nowej reguły, aby rozpocząć korzystanie z tej ochrony. Ta ochrona obejmuje pliki w programach SharePoint, OneDrive i Microsoft Teams.
  
Aby utworzyć zasady bezpiecznego załącznika ATP, obejrzyj [ten krótki klip wideo](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)lub wykonaj następujące kroki:
  
1. Przejdź [https://protection.office.com](https://protection.office.com)do i zaloguj się przy swoim koncie administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie Zasady wybierz **pozycję Bezpieczne załączniki ATP**.
    
4. Na stronie Bezpieczne załączniki zastosuj tę ochronę szeroko, zaznaczając pole wyboru **Włącz przystawkę ATP dla programu SharePoint, OneDrive i Microsoft Teams.** 
    
5. Wybierz, **+** aby utworzyć nową zasadę. 
    
6. Zastosuj ustawienia w poniższej tabeli. 
    
7. Po przejrzeniu ustawień wybierz pozycję **Utwórz tę zasadę** lub **Zapisz**, stosownie do potrzeb.
    

|**Ustawianie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Blokuj bieżące i przyszłe wiadomości e-mail z wykrytym złośliwym oprogramowaniem.  <br/> |
|Opis  <br/> |Blokuj bieżące i przyszłe wiadomości e-mail i załączniki za pomocą wykrytego złośliwego oprogramowania.  <br/> |
|Zapisywanie załączników nieznanych odpowiedzi na złośliwe oprogramowanie  <br/> |Wybierz **pozycję Blokuj — blokuj bieżące i przyszłe wiadomości e-mail i załączniki za pomocą wykrytego złośliwego oprogramowania.**  <br/> |
|Przekieruj załącznik przy wykrywaniu  <br/> |Włącz przekierowanie (zaznacz to pole) Wprowadź konto administratora lub konfigurację skrzynki pocztowej w celu kwarantanny.          Zastosuj powyższe zaznaczenie, jeśli wystąpi skanowanie złośliwego oprogramowania w poszukiwaniu czasu lub wystąpił błąd (zaznacz to pole).  <br/> |
|Stosowane do  <br/> |Domeną adresata jest . . . wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Konfigurowanie zasad ochrony przed wyłudzaniem informacji usługi Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrona przed atakami phishingowymi dzięki bezpiecznym linkom ATP

Hakerzy czasami ukrywają złośliwe witryny w linkach w wiadomościach e-mail lub innych plikach. Bezpieczne łącza usługi Office 365 ATP (bezpieczne łącza atp), część zaawansowanej ochrony przed zagrożeniami usługi Office 365, mogą pomóc w ochronie organizacji, zapewniając weryfikację adresów internetowych (URL) w wiadomościach e-mail i dokumentach pakietu Office. Ochrona jest definiowana za pomocą zasad bezpiecznych łączy ATP.
  
Zaleca się wykonanie następujących czynności:
  
- Zmodyfikuj zasady domyślne, aby zwiększyć ochronę.
    
- Dodaj nowe zasady skierowane do wszystkich adresatów w domenie.
    
Aby skonfigurować bezpieczne łącza atp, obejrzyj [ten krótki film treningowy](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)lub wykonaj następujące czynności:
  
1. Przejdź [https://protection.office.com](https://protection.office.com)do i zaloguj się przy swoim koncie administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie Zasady wybierz pozycję **Bezpieczne łącza ATP**.
    
Aby zmodyfikować zasady domyślne:
  
1. Na stronie Bezpieczne łącza w obszarze **Zasady, które mają zastosowanie do całej organizacji,** wybierz zasady **domyślne.** 
    
2. W obszarze **Ustawienia, które mają zastosowanie do zawartości z wyjątkiem poczty e-mail,** wybierz **pozycję Office 365 ProPlus, Office dla systemów iOS i Android**.
    
3. Wybierz pozycję **Zapisz**. 
    
Aby utworzyć nowe zasady skierowane do wszystkich adresatów w domenie:
  
1. Na stronie Bezpieczne łącza w obszarze **Zasady, które mają zastosowanie do całej organizacji,** wybierz, **+** aby utworzyć nowe zasady. 
    
2. Zastosuj ustawienia wymienione w poniższej tabeli.
    
3. Wybierz pozycję **Zapisz**. 

|**Ustawianie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zasady dotyczące bezpiecznych łączy dla wszystkich adresatów w domenie  <br/> |
|Wybierz akcję dla nieznanych potencjalnie szkodliwych adresów URL w wiadomościach  <br/> |Wybierz **wł. - adresy URL zostaną przepisane i sprawdzone na liście znanych złośliwych linków, gdy użytkownik kliknie łącze**.  <br/> |
|Skanowanie zawartości do pobrania za pomocą bezpiecznych załączników  <br/> |Zaznacz to pole.  <br/> |
|Stosowane do  <br/> |Domeną adresata jest . . . wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [łącza bezpieczne usługi Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do [witryny Azure portal](https://portal.azure.com/).

2. Wybierz **pozycję Wszystkie usługi** i wpisz usługę *Intune* w **polu wyszukiwania**.

3. Gdy pojawią się wyniki, wybierz początek obok **usługi Microsoft Intune,** aby uczynić go ulubionym i łatwym do znalezienia później.

Oprócz centrum administracyjnego można używać usługi Intune do rejestrowania urządzeń w organizacji i zarządzania nimi. Aby uzyskać więcej informacji, zobacz [Możliwości według metody rejestracji dla urządzeń z systemem Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) i opcje rejestracji dla urządzeń [zarządzanych przez usługę Intune](https://docs.microsoft.com/intune/enrollment-options).
