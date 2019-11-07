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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami w pakiecie Office 365 i Chroń poufne dane.
ms.openlocfilehash: 1827b70f1e4d78a072753390c1a99d7cb4bd5cfd
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030769"
---
# <a name="increase-threat-protection"></a>Zwiększ ochronę przed zagrożeniami

Ten artykuł pomaga zwiększyć ochronę w subskrypcji Microsoft 365 w celu ochrony przed phishingiem, złośliwym oprogramowaniem i innymi zagrożeniami. Zalecenia te są odpowiednie dla organizacji z zwiększone zapotrzebowanie na bezpieczeństwo, jak kancelarie prawne, i kliniki opieki zdrowotnej.

Zanim zaczniesz, Sprawdź swój pakiet Office 365 bezpieczny wynik. Pakiet Office 365 bezpieczny wynik analizuje zabezpieczenia organizacji pakietu Office 365 w oparciu o zwykłe działania i ustawienia zabezpieczeń oraz przypisuje wynik. Zacznij od Odnotuj swój aktualny wynik. Podjęcie działań zalecanych w tym artykule zwiększa swój wynik. Celem nie jest osiągnięcie maksymalnego wyniku, ale zdawać sobie sprawę z możliwości ochrony środowiska, które nie wpływają negatywnie na produktywność użytkowników. 

Aby uzyskać więcej informacji, zobacz [bezpieczny wynik firmy Microsoft](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podniesienie poziomu ochrony przed złośliwym oprogramowaniem w poczcie

Środowisko Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem, ale można zwiększyć tę ochronę, blokując załączniki z typami plików, które są powszechnie używane w przypadku złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomościach e-mail:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu poświadczeń konta administratora. 
    
2. W Office 365 &amp; Security Compliance Center, w okienku nawigacyjnym po lewej stronie, w obszarze **zarządzania zagrożeniem**, wybierz polecenie **zasady** \> **ochrony przed złośliwym oprogramowaniem**.
    
3. Kliknij dwukrotnie zasadę domyślną, aby edytować tę zasadę dla całej firmy.
    
4. Kliknij przycisk **Ustawienia**.
    
5. W obszarze **typowe typy załączników filtru**, wybierz opcję **wł**. Typy plików, które są blokowane są wyświetlane w oknie bezpośrednio pod tym formantem.  Upewnij się, że dodajesz następujące typy plików:
   - ADE, ADP, ani, bas, nietoperz, chm, cmd, com, cpl, CRT, HLP, HT, HTA, inf, ins, ISP, praca, js, JSE, lnk, MDA, MDB, MDE, MDZ, msc, MSI, msp, MST, PCD, reg, SCR, SCT, SHS, URL, VB, VBE, vbs, WSC, wsf, WSH, exe, PIF  <br/> W razie potrzeby można później dodać lub usunąć typy plików.
    
6. Kliknij przycisk **Zapisz.**
    
Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrona przed oprogramowaniem typu ransomware

Oprogramowanie ransomware ogranicza dostęp do danych przez szyfrowanie plików lub blokowanie ekranów komputera. Następnie próbuje wyłudzić pieniądze od ofiar, prosząc o "okupu", zwykle w formie kryptowalut, takich jak Bitcoin, w zamian za dostęp do danych. 
  
Możesz zabezpieczyć się przed ransomware, tworząc jedną lub więcej reguł przepływu poczty do blokowania rozszerzeń plików, które są powszechnie używane do ransomware (te zostały dodane w [podnieść poziom ochrony przed złośliwym oprogramowaniem w kroku mail](#raise-the-level-of-protection-against-malware-in-mail) ), lub aby ostrzec użytkowników, którzy otrzymali te załączników w wiadomości e-mail.

Oprócz plików zablokowanych w poprzednim kroku dobrym rozwiązaniem jest również utworzenie reguły ostrzegających użytkowników przed otwarciem załączników plików pakietu Office, które zawierają makra. Ransomware mogą być ukryte wewnątrz makra, więc będziemy ostrzegać użytkowników, aby nie otwierać tych plików od ludzi, których nie znają.

Aby utworzyć regułę transportu poczty:
  
1. <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> Przejdź do centrum administracyjnego i wybierz **Exchange** **centra** \> administracyjne.
    
2. W kategorii **przepływ poczty** kliknij przycisk **reguły**.
    
3. Kliknij **+**, a następnie kliknij przycisk **Utwórz nową regułę**.
    
4. Kliknij przycisk **więcej opcji** w dolnej części okna dialogowego, aby wyświetlić pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli dla reguły. Pozostaw pozostałe ustawienia domyślne, chyba że chcesz je zmienić.
    
6. Kliknij pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office**||
|:-----|:-----|:-----|
|Name (Nazwa)  <br/> |Reguła anty-ransomware: Ostrzegaj użytkowników  <br/>  |
|Zastosuj tę regułę, jeśli. . .  <br/> |Dowolny załącznik. . . dopasowania pliku. . .  <br/> |
|Określanie wyrazów lub wyrażeń  <br/> |Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, XLA, XLAM, XLL, pptm, potm, PPAM, PPSM, SLDM  <br/>|
|Wykonaj następujące czynności. . .  <br/> |Powiadamianie adresata o wiadomości  <br/> |
|Podaj tekst komunikatu  <br/> |Nie otwieraj plików tego typu od osób, których nie znasz, ponieważ mogą one zawierać makra ze złośliwym kodem.  <br/> |
   
Aby uzyskać więcej informacji, zobacz:
  
- [Jak radzić sobie z ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Przywracanie usługi OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Zatrzymaj automatyczne przekazywanie wiadomości e-mail

Hakerzy, którzy uzyskują dostęp do skrzynki pocztowej użytkownika, mogą ukraść pocztę przez ustawienie skrzynki pocztowej na automatyczne przekazywanie wiadomości e-mail. Może się to zdarzyć nawet bez świadomości użytkownika. Można temu zapobiec, konfigurując regułę przepływu poczty. 
  
Aby utworzyć regułę transportu poczty, Obejrzyj [ten krótki film](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) lub wykonaj następujące czynności:
  
1. W centrum administracyjnym Microsoft 365 kliknij pozycję **centra** \> administracyjne **Exchange**.
    
2. W kategorii **przepływ poczty** kliknij przycisk **reguły**.
    
3. Kliknij **+**, a następnie kliknij przycisk **Utwórz nową regułę**.
    
4. Kliknij przycisk **więcej opcji** w dolnej części okna dialogowego, aby wyświetlić pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli. Pozostaw pozostałe ustawienia domyślne, chyba że chcesz je zmienić.
    
6. Kliknij pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office**|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zapobieganie automatycznemu przekazywaniu wiadomości e-mail do domen zewnętrznych  <br/> |
|Zastosuj tę regułę, jeśli...  <br/> |Nadawca. . . jest zewnętrzny/wewnętrzny. . . Wewnątrz organizacji  <br/> |
|Dodaj warunek  <br/> |Właściwości wiadomości. . . zawierać typ komunikatu. . . Automatyczne przewijanie do przodu  <br/> |
|Wykonaj następujące czynności...  <br/> |Zablokuj wiadomość. . . odrzucić wiadomość i dołączyć wyjaśnienie.  <br/> |
|Podaj tekst komunikatu  <br/> |Automatyczne przekazywanie wiadomości e-mail spoza tej organizacji jest uniemożliwione ze względów bezpieczeństwa.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Chroń swój adres e-mail przed atakami phishingowymi

Jeśli skonfigurowano jedną lub więcej domen niestandardowych dla pakietu Office 365 lub środowiska Microsoft 365, można skonfigurować ukierunkowaną ochronę przed phishingiem. Ochrona przed phishingiem ATP, będąca częścią pakietu Office 365 Zaawansowana ochrona przed zagrożeniami, może pomóc w ochronie organizacji przed złośliwymi atakami typu phishing opartymi na personifikacji i innymi atakami typu phishing. Jeśli nie skonfigurowano domeny niestandardowej, nie trzeba tego robić.
  
Zaleca się rozpoczęcie tej ochrony, tworząc zasadę chroniąc najważniejszych użytkowników i domenę niestandardową. 

  
Aby utworzyć politykę ochrony przed phishingiem ATP, Obejrzyj [ten krótki film treningowy](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)lub wykonaj następujące czynności:
  
1. Przejdź do witryny [https://protection.office.com](https://protection.office.com). 
    
2. W Office 365 Security &amp; Compliance Center, w okienku nawigacyjnym po lewej stronie, w obszarze **zarządzania zagrożeniem**, wybierz polecenie **zasad**.
    
3. Na stronie **zasady** wybierz opcję **anty-phishing ATP**.
    
4. Na stronie **Anti-phishing** wybierz pozycję **+ Utwórz**. Zostanie uruchomiony Kreator, który umożliwia zdefiniowanie zasad anty-phishingowych.
    
5. Określ nazwę, opis i ustawienia zasad zgodnie z zaleceniami na poniższej tabeli. Aby uzyskać więcej informacji, zobacz informacje [o opcjach zasad ochrony przed phishingiem ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) . 
    
6. Po dokonaniu przeglądu ustawień wybierz opcję **Utwórz tę zasadę** lub **Zapisz**, stosownie do potrzeb.
    

|**Ustawienie lub opcja**<br/>|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Domena i najcenniejszy personel kampanii  <br/> |
|Opis  <br/> |Upewnij się, że najważniejszy personel i nasza domena nie są personisperowani.  <br/> |
|Dodawanie użytkowników do ochrony  <br/> |Wybierz **+ Dodaj warunek, odbiorca jest**. Wpisz nazwy użytkowników lub wprowadź adres e-mail kandydata, menedżera kampanii i innych ważnych członków personelu. Można dodać maksymalnie 20 adresów wewnętrznych i zewnętrznych, które mają być chronione przed personifikacją.  <br/> |
|Dodawanie domen do ochrony  <br/> |Wybierz **+ Dodaj warunek, domena adresata**. Wprowadź niestandardową domenę skojarzoną z subskrypcją Microsoft 365, jeśli została zdefiniowana. Można wprowadzić więcej niż jedną domenę.  <br/> |
|Wybierz akcje  <br/> |Jeśli wiadomość e-mail jest wysyłana przez personisperowanego użytkownika: Wybierz **Przekierowanie wiadomości na inny adres e-mail**, a następnie wpisz adres e-mail administratora zabezpieczeń; na przykład *Alicja<span><span>@contoso. com*.          Jeśli wiadomość e-mail jest wysyłana przez personisperowaną domenę: Wybierz **wiadomość z kwarantanny**.  <br/> |
|Inteligencja skrzynki pocztowej  <br/> |Domyślnie inteligencja skrzynki pocztowej jest zaznaczona podczas tworzenia nowej zasady anty-phishing. Pozostaw to ustawienie **na** najlepsze wyniki.  <br/> |
|Dodawanie zaufanych nadawców i domen  <br/> |Tutaj możesz dodać własną domenę lub inne zaufane domeny.  <br/> |
|Zastosowane do  <br/> |Wybierz **domenę adresata**. W **dowolnym z nich**wybierz **Wybierz**. Wybierz **+ Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso.<span> com <span>*, na liście, a następnie wybierz **Dodaj**. Wybierz **gotowe**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Chroń przed złośliwymi załącznikami i plikami za pomocą bezpiecznych załączników ATP

Użytkownicy regularnie wysyłają, odbierają i współużytkują załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Nie zawsze łatwo jest stwierdzić, czy załącznik jest bezpieczny, czy złośliwy, patrząc na wiadomość e-mail. Zaawansowana ochrona przed zagrożeniami w pakiecie Office 365 obejmuje ochronę bezpiecznego załącznika ATP, ale ta ochrona nie jest domyślnie włączona. Zaleca się utworzenie nowej reguły, aby rozpocząć korzystanie z tej ochrony. Ta ochrona rozciąga się na pliki w programie SharePoint, OneDrive i Microsoft Teams.
  
Aby utworzyć zasadę bezpiecznego załącznika ATP, Obejrzyj [ten krótki film](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)lub wykonaj następujące czynności:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu konta administratora. 
    
2. W Office 365 Security &amp; Compliance Center, w okienku nawigacyjnym po lewej stronie, w obszarze **zarządzania zagrożeniem**, wybierz polecenie **zasad**.
    
3. Na stronie zasady wybierz **bezpieczne załączniki ATP**.
    
4. Na stronie bezpieczne załączniki Zastosuj tę ochronę szeroko, zaznaczając pole wyboru **Włącz ATP dla programu SharePoint, OneDrive i Microsoft Teams** . 
    
5. Wybierz **+** , aby utworzyć nową zasadę. 
    
6. Zastosuj ustawienia w poniższej tabeli. 
    
7. Po dokonaniu przeglądu ustawień wybierz opcję **Utwórz tę zasadę** lub **Zapisz**, stosownie do potrzeb.
    

|**Ustawienie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Blokuj bieżące i przyszłe wiadomości e-mail z wykrytym złośliwym oprogramowaniem.  <br/> |
|Opis  <br/> |Blokuj bieżące i przyszłe e-maile i załączniki z wykrytym złośliwym oprogramowaniem.  <br/> |
|Zapisz załączniki nieznana odpowiedź na złośliwe oprogramowanie  <br/> |Wybierz **Blokuj-Blokuj bieżące i przyszłe e-maile i załączniki z wykrytym złośliwym oprogramowaniem**.  <br/> |
|Przekierowanie załącznika przy wykrywaniu  <br/> |Włącz przekierowywanie (zaznacz to pole) Wprowadź konto administratora lub konfigurację skrzynki pocztowej do kwarantanny.          Zastosuj powyższe zaznaczenie, jeśli skanowanie złośliwego oprogramowania w poszukiwaniu załączników upłynie lub wystąpi błąd (zaznacz to pole).  <br/> |
|Zastosowane do  <br/> |Domena adresata jest. . . Wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Konfigurowanie zasad ochrony przed phishingiem pakietu Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrona przed atakami phishingowymi za pomocą bezpiecznych linków ATP

Hakerzy czasami ukrywają złośliwe strony w linkach w wiadomościach e-mail lub innych plikach. Office 365 ATP bezpiecznych linków (ATP bezpiecznych linków), część pakietu Office 365 Zaawansowana ochrona przed zagrożeniami, może pomóc w ochronie organizacji, zapewniając czas kliknięcia weryfikacji adresów internetowych (adresów URL) w wiadomościach e-mail i dokumentach pakietu Office. Ochrona jest definiowana za pomocą zasad bezpiecznych linków ATP.
  
Zaleca się, aby wykonać następujące czynności:
  
- Modyfikowanie domyślnych zasad w celu zwiększenia ochrony.
    
- Dodaj nowe zasady skierowane do wszystkich adresatów w domenie.
    
Aby skonfigurować bezpieczne łącza ATP, Obejrzyj [ten krótki film treningowy](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)lub wykonaj następujące czynności:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu konta administratora. 
    
2. W Office 365 Security &amp; Compliance Center, w okienku nawigacyjnym po lewej stronie, w obszarze **zarządzania zagrożeniem**, wybierz polecenie **zasad**.
    
3. Na stronie zasady wybierz pozycję **bezpieczne łącza ATP**.
    
Aby zmodyfikować zasadę domyślną:
  
1. Na stronie bezpieczne łącza w obszarze **zasady, które mają zastosowanie do całej organizacji**, wybierz zasadę **domyślną** . 
    
2. W obszarze **Ustawienia, które mają zastosowanie do zawartości z wyjątkiem wiadomości e-mail**, wybierz **Office 365 ProPlus, Office dla iOS i Android**.
    
3. Kliknij pozycję **Zapisz**. 
    
Aby utworzyć nową zasadę skierowaną do wszystkich adresatów w domenie:
  
1. Na stronie bezpieczne łącza w obszarze **zasady, które mają zastosowanie do całej organizacji**, kliknij **+** , aby utworzyć nowe zasady. 
    
2. Zastosuj ustawienia wymienione w poniższej tabeli.
    
3. Kliknij pozycję **Zapisz**. 

|**Ustawienie lub opcja**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zasady bezpiecznego łącza dla wszystkich adresatów w domenie  <br/> |
|Wybierz akcję dla nieznanych potencjalnie złośliwych adresów URL w wiadomościach  <br/> |Wybierz **na-adresy URL zostaną przepisany i sprawdzane na liście znanych szkodliwych linków, gdy użytkownik kliknie łącze**.  <br/> |
|Użyj bezpiecznych załączników do skanowania zawartości do pobrania  <br/> |Zaznacz to pole.  <br/> |
|Zastosowane do  <br/> |Domena adresata jest. . . Wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji, zobacz [Office 365 ATP bezpiecznych linków](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do [witryny Azure Portal](https://portal.azure.com/).

2. Wybierz **wszystkie usługi** i wpisz w *usłudze Intune* w **polu wyszukiwania**.

3. Po wyświetleniu wyników kliknij przycisk Start obok **usługi Microsoft Intune** , aby uczynić go ulubionym i łatwo znaleźć później.

Oprócz centrum administracyjnego można używać usługi Intune do rejestrowania urządzeń w organizacji i zarządzania nimi. Aby uzyskać więcej informacji, zobacz [możliwości według metody rejestracji dla urządzeń z systemem Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) i [Opcje rejestracji dla urządzeń zarządzanych przez usługę Intune](https://docs.microsoft.com/intune/enrollment-options).
