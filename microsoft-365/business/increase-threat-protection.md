---
title: Zwiększenie ochrony przed zagrożeniami dla usługi Microsoft 365 Business
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami usługi Office 365 i zabezpiecz poufne dane przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami.
ms.openlocfilehash: 9d7bae60091c87fa0246a697f2a49e1cbc6e2f06
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550362"
---
# <a name="increase-threat-protection"></a>Zwiększenie ochrony przed zagrożeniami

Ten artykuł pomaga zwiększyć ochronę w subskrypcji usługi Microsoft 365 w celu ochrony przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami. Zalecenia te są odpowiednie dla organizacji o zwiększonym zapotrzebowania na bezpieczeństwo, takich jak kancelarie prawne i kliniki opieki zdrowotnej.

Przed rozpoczęciem sprawdź bezpieczny wynik usługi Office 365. Bezpieczny wynik usługi Office 365 analizuje zabezpieczenia organizacji usługi Office 365 na podstawie regularnych działań i ustawień zabezpieczeń oraz przypisuje wynik. Zacznij od uwzględnienia aktualnego wyniku. Aby zwiększyć swój wynik, wykonaj czynności zalecane w tym artykule. Celem nie jest osiągnięcie maksymalnego wyniku, ale zdawanie możliwości ochrony środowiska, które nie mają negatywnego wpływu na produktywność użytkowników. 

Aby uzyskać więcej informacji, zobacz [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podniesienie poziomu ochrony przed złośliwym oprogramowaniem w poczcie

Środowisko usługi Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem. Możesz zwiększyć tę ochronę, blokując załączniki z typami plików, które są powszechnie używane w przypadku złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomościach e-mail:
  
1. Przejdź [https://protection.office.com](https://protection.office.com) do i zaloguj się przy użyciu poświadczeń konta administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Ochrona** \> **przed złośliwym oprogramowaniem**.
    
3. Kliknij dwukrotnie domyślne zasady, aby edytować te zasady dotyczące całej firmy.
    
4. Wybierz **pozycję Ustawienia**.
    
5. W obszarze **Filtr Typowe typy załączników**wybierz pozycję **Wł.** Typy plików, które są blokowane są wymienione w oknie bezpośrednio pod tym formantem. Upewnij się, że dodajesz następujące typy plików:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif, pif, pif  <br/> 
   
   W razie potrzeby można później dodać lub usunąć typy plików.
    
6. Wybierz **pozycję Zapisz.**
    
Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrona przed oprogramowaniem ransomware

Ransomware ogranicza dostęp do danych poprzez szyfrowanie plików lub blokowanie ekranów komputerów. Następnie próbuje wyłudzić pieniądze od ofiar, prosząc o "okup", zwykle w postaci kryptowalut, takich jak Bitcoin, w zamian za dostęp do danych. 
  
Aby chronić się przed oprogramowaniem wymuszającym okup, utwórz co najmniej jedną regułę przepływu poczty, aby zablokować rozszerzenia plików, które są powszechnie używane do ransomware. (Dodano te reguły w [podnoszeniu poziomu ochrony przed złośliwym oprogramowaniem w](#raise-the-level-of-protection-against-malware-in-mail) kroku poczty). Możesz również ostrzec użytkowników, którzy otrzymują te załączniki w wiadomoście e-mail.

Oprócz plików zablokowanych w poprzednim kroku dobrą praktyką jest utworzenie reguły ostrzegającej użytkowników przed otwarciem załączników plików pakietu Office, które zawierają makra. Ransomware może być ukryty wewnątrz makr, więc ostrzegaj użytkowników, aby nie otwierali tych plików od osób, których nie znają.

Aby utworzyć regułę transportu poczty:
  
1. Przejdź do centrum <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administracyjnego w programie , a **polecenie Centrum administracyjne** \> **Exchange**.
    
2. W kategorii **przepływu poczty** wybierz **reguły**.
    
3. Wybierz **+** pozycję , a następnie wybierz **pozycję Utwórz nową regułę**.
    
4. Wybierz **pozycję Więcej opcji** u dołu okna dialogowego, aby wyświetlić pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli dla reguły. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.
    
6. Wybierz pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office**||
|:-----|:-----|:-----|
|Name (Nazwa)  <br/> |Reguła anty-ransomware: ostrzegaj użytkowników  <br/>  |
|Zastosuj tę regułę, jeśli . . .  <br/> |Dowolny załącznik . . . rozszerzenia pliku pasuje . . .  <br/> |
|Określanie wyrazów lub fraz  <br/> |Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Wykonaj następujące czynności . . .  <br/> |Powiadom adresata za pomocą wiadomości  <br/> |
|Podaj tekst wiadomości  <br/> |Nie należy otwierać tego typu plików od osób, których nie znasz, ponieważ mogą one zawierać makra ze złośliwym kodem.  <br/> |
   
Aby uzyskać więcej informacji, zobacz:
  
- [Jak radzić sobie z oprogramowaniem ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Przywracanie usługi OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zatrzymywanie automatycznego przekazywania wiadomości e-mail

Hakerzy, którzy uzyskują dostęp do skrzynki pocztowej użytkownika, mogą ukraść pocztę, ustawiając skrzynkę pocztową tak, aby automatycznie przesyłała dalej wiadomości e-mail. Może się to zdarzyć nawet bez świadomości użytkownika. Aby temu zapobiec, należy skonfigurować regułę przepływu poczty. 
  
Aby utworzyć regułę transportu poczty, obejrzyj [ten krótki film lub](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) wykonaj następujące kroki:
  
1. W centrum administracyjnym usługi Microsoft 365 wybierz pozycję **Centra** \> administracyjne **programu Exchange**.
    
2. W kategorii **przepływu poczty** wybierz **reguły**.
    
3. Wybierz **+** pozycję , a następnie wybierz **pozycję Utwórz nową regułę**.
    
4. Aby wyświetlić wszystkie opcje, wybierz **pozycję Więcej opcji** u dołu okna dialogowego. 
    
5. Zastosuj ustawienia w poniższej tabeli. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.
    
6. Wybierz pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office**|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zapobieganie automatycznemu przesyłaniu wiadomości e-mail do domen zewnętrznych  <br/> |
|Zastosuj tę regułę, jeśli ...  <br/> |Nadawca . . . jest zewnętrzna/wewnętrzna . . . Wewnątrz organizacji  <br/> |
|Dodaj warunek  <br/> |Właściwości wiadomości . . . dołącz typ wiadomości . . . Automatyczne przesyłanie do przodu  <br/> |
|Wykonaj następujące ...  <br/> |Zablokuj wiadomość . . . odrzucić wiadomość i dołączyć wyjaśnienie.  <br/> |
|Podaj tekst wiadomości  <br/> |Automatyczne przekazywanie wiadomości e-mail poza tą organizacją jest uniemożliwione ze względów bezpieczeństwa.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrona poczty e-mail przed atakami phishingowymi

Jeśli skonfigurowano co najmniej jedną domenę niestandardową dla środowiska usługi Office 365 lub Microsoft 365, możesz skonfigurować ukierunkowaną ochronę przed wyłudzaniem informacji. Ochrona przed wyłudzaniem informacji przez usługę ATP, która jest częścią zaawansowanej ochrony przed zagrożeniami usługi Office 365, może pomóc w ochronie organizacji przed złośliwymi atakami phishingowymi opartymi na personifikacji i innymi atakami phishingowymi. Jeśli domena niezostała skonfigurowana, nie musisz tego robić.
  
Zalecamy rozpoczęcie pracy z tą ochroną, tworząc zasady chroniące najważniejszych użytkowników i domenę niestandardową. 

Aby utworzyć zasady ochrony przed wyłudzaniem informacji przez atp, obejrzyj [ten krótki film szkoleniowy](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)lub wykonaj następujące czynności:
  
1. Przejdź do witryny [https://protection.office.com](https://protection.office.com). 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie **Zasady** wybierz pozycję **ATP anti-phishing**.
    
4. Na stronie **Ochrona przed wyłudzaniem informacji** wybierz pozycję + **Utwórz**. Zostanie uruchomiony kreator, który przeprowadzi Cię przez zdefiniowanie zasad ochrony przed wyłudzaniem informacji.
    
5. Określ nazwę, opis i ustawienia zasad zgodnie z zaleceniami w poniższej tabeli. Aby uzyskać więcej informacji, zobacz [Dowiedz się więcej o opcjach zasad ochrony przed wyłudzaniem informacji przez atp](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Po przejrzeniu ustawień wybierz pozycję **Utwórz tę zasadę** lub **Zapisz**, odpowiednio.
    

|**Ustawienie lub opcja**<br/>|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Domena i najcenniejszy personel kampanii  <br/> |
|Opis  <br/> |Upewnij się, że najważniejszy personel i nasza domena nie są podszywani.  <br/> |
|Dodawanie użytkowników do ochrony  <br/> |Wybierz **+ Dodaj warunek, adresatjest**. Wpisz nazwy użytkowników lub wprowadź adres e-mail kandydata, menedżera kampanii i innych ważnych pracowników. Można dodać maksymalnie 20 adresów wewnętrznych i zewnętrznych, które mają być chronione przed personifikacją.  <br/> |
|Dodawanie domen do ochrony  <br/> |Wybierz **+ Dodaj warunek, Domena adresata jest**. Wprowadź domenę niestandardową skojarzoną z subskrypcją usługi Microsoft 365, jeśli została zdefiniowana. Można wprowadzić więcej niż jedną domenę.  <br/> |
|Wybieranie akcji  <br/> |Jeśli wiadomość e-mail jest wysyłana przez personifikatowanego użytkownika: wybierz **pozycję Przekieruj wiadomość na inny adres e-mail,** a następnie wpisz adres e-mail administratora zabezpieczeń; na przykład *<span><span>Alicja @contoso.com*. Jeśli wiadomość e-mail jest wysyłana przez domenę podszywającą się pod osobę: wybierz **pozycję Podsyć wiadomość**.  <br/> |
|Inteligencja skrzynki pocztowej  <br/> |Domyślnie podczas tworzenia nowych zasad ochrony przed wyłudzaniem informacji wybierasię inteligencję skrzynki pocztowej. Pozostaw to ustawienie **Włączone, aby** uzyskać najlepsze wyniki.  <br/> |
|Dodawanie zaufanych nadawców i domen  <br/> |W tym miejscu możesz dodać własną domenę lub inne zaufane domeny.  <br/> |
|Zastosowana do  <br/> |Wybierz **pozycję Domena adresata to**. W obszarze **Dowolna z tych**opcji wybierz **pozycję Wybierz**. Wybierz **pozycję + Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso.<span> com <span>*, na liście, a następnie wybierz **pozycję Dodaj**. Wybierz **pozycję Gotowe**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrona przed złośliwymi załącznikami i plikami za pomocą bezpiecznych załączników ATP

Użytkownicy regularnie wysyłają, odbierają i udostępniają załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Nie zawsze jest łatwo stwierdzić, czy załącznik jest bezpieczny czy złośliwy, po prostu patrząc na wiadomość e-mail. Zaawansowana ochrona przed zagrożeniami usługi Office 365 obejmuje ochronę przed bezpiecznym przywiązaniem atp, ale ta ochrona nie jest domyślnie włączona. Zaleca się utworzenie nowej reguły, aby rozpocząć korzystanie z tej ochrony. Ta ochrona obejmuje pliki w programach SharePoint, OneDrive i Microsoft Teams.
  
Aby utworzyć zasady bezpiecznego załącznika ATP, obejrzyj [ten krótki film lub](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)wykonaj następujące czynności:
  
1. Przejdź [https://protection.office.com](https://protection.office.com)do strony i zaloguj się przy konto administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie Zasady wybierz pozycję **Załączniki bezpieczne atp**.
    
4. Na stronie Bezpieczne załączniki zastosuj tę ochronę szeroko, zaznaczając pole wyboru **Włącz atp dla programów SharePoint, OneDrive i Microsoft Teams.** 
    
5. Wybierz, **+** aby utworzyć nową zasadę. 
    
6. Zastosuj ustawienia w poniższej tabeli. 
    
7. Po przejrzeniu ustawień wybierz pozycję **Utwórz tę zasadę** lub **Zapisz**, odpowiednio.
    

|**Ustawienie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Blokuj bieżące i przyszłe wiadomości e-mail z wykrytym złośliwym oprogramowaniem.  <br/> |
|Opis  <br/> |Blokuj bieżące i przyszłe wiadomości e-mail i załączniki z wykrytym złośliwym oprogramowaniem.  <br/> |
|Zapisywanie załączników nieznanej odpowiedzi złośliwego oprogramowania  <br/> |Wybierz **Blokuj - Zablokuj bieżące i przyszłe wiadomości e-mail i załączniki z wykrytym złośliwym oprogramowaniem.**  <br/> |
|Przekieruj załącznik podczas wykrywania  <br/> |Włącz przekierowanie (zaznacz to pole) Wprowadź konto administratora lub konfigurację skrzynki pocztowej do kwarantanny.          Zastosuj powyższy wybór, jeśli pojawi się skanowanie złośliwego oprogramowania w poszukiwaniu przekroczenia czasu załączników lub wystąpienia błędu (zaznacz to pole).  <br/> |
|Zastosowana do  <br/> |Domeną adresata jest . . . wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Konfigurowanie zasad ochrony przed wyłudzaniem informacji usługi Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrona przed atakami phishingowymi za pomocą bezpiecznych łączy ATP

Hakerzy czasami ukrywają złośliwe witryny w linkach w wiadomościach e-mail lub innych plikach. Bezpieczne łącza usługi Office 365 ATP (bezpieczne łącza ATP), część zaawansowanej ochrony przed zagrożeniami usługi Office 365, mogą pomóc w ochronie organizacji, zapewniając weryfikację adresów internetowych (URL) w wiadomościach e-mail i dokumentach pakietu Office, zapewniając weryfikację adresów internetowych (URL) w wiadomościach e-mail i dokumentach pakietu Office. Ochrona jest definiowana za pomocą zasad bezpiecznych łączy ATP.
  
Zalecamy wykonanie następujących czynności:
  
- Zmodyfikuj domyślne zasady, aby zwiększyć ochronę.
    
- Dodaj nowe zasady skierowane do wszystkich adresatów w domenie.
    
Aby skonfigurować bezpieczne łącza ATP, obejrzyj [ten krótki film szkoleniowy](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)lub wykonaj następujące czynności:
  
1. Przejdź [https://protection.office.com](https://protection.office.com)do strony i zaloguj się przy konto administratora. 
    
2. W Centrum zgodności zabezpieczeń &amp; usługi Office 365 w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Zasady**.
    
3. Na stronie Zasady wybierz pozycję **Bezpieczne łącza ATP**.
    
Aby zmodyfikować zasady domyślne:
  
1. Na stronie Bezpieczne łącza w obszarze **Zasady dotyczące całej organizacji**wybierz zasady **domyślne.** 
    
2. W obszarze **Ustawienia dotyczące zawartości z wyjątkiem poczty e-mail**wybierz pozycję Office **365 ProPlus, Office for iOS i Android**.
    
3. Wybierz pozycję **Zapisz**. 
    
Aby utworzyć nową zasadę skierowaną do wszystkich adresatów w domenie:
  
1. Na stronie Bezpieczne łącza w obszarze **Zasady, które mają zastosowanie do całej organizacji,** wybierz, **+** aby utworzyć nową zasadę. 
    
2. Zastosuj ustawienia wymienione w poniższej tabeli.
    
3. Wybierz pozycję **Zapisz**. 

|**Ustawienie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zasady dotyczące bezpiecznych łączy dla wszystkich adresatów w domenie  <br/> |
|Wybieranie akcji dla nieznanych potencjalnie złośliwych adresów URL w wiadomościach  <br/> |Wybierz **Pozycję Włącz - adresy URL zostaną przepisane i sprawdzone na liście znanych złośliwych linków po kliknięciu przez użytkownika linku.**  <br/> |
|Skanowanie zawartości do pobrania za pomocą bezpiecznych załączników  <br/> |Zaznacz to pole.  <br/> |
|Zastosowana do  <br/> |Domeną adresata jest . . . wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Łącza bezpieczne usługi Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do [portalu Azure](https://portal.azure.com/).

2. Wybierz **pozycję Wszystkie usługi** i wpisz w *usłudze Intune* w polu **wyszukiwania**.

3. Po wyświetleniu wyników wybierz start obok usługi **Microsoft Intune,** aby uczynić ją ulubioną i łatwą do znalezienia później.

Oprócz centrum administracyjnego można używać usługi Intune do rejestrowania urządzeń organizacji i zarządzania nimi. Aby uzyskać więcej informacji, zobacz [Możliwości według metody rejestracji dla urządzeń z systemem Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) i opcje rejestracji dla urządzeń [zarządzanych przez usługę Intune](https://docs.microsoft.com/intune/enrollment-options).
