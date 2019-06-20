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
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086371"
---
# <a name="increase-threat-protection"></a>Zwiększ ochronę przed zagrożeniami

Ten artykuł pomoże Ci zwiększyć ochronę w ramach subskrypcji usługi Microsoft 365 do ochrony przed phishingiem, przed złośliwym oprogramowaniem i innymi zagrożeniami. Zalecenia te są odpowiednie dla organizacji z zwiększone zapotrzebowanie na zabezpieczenia, jak prawa biura i kliniki zdrowia.

Przed rozpoczęciem należy sprawdzić wynik Secure Office 365. Office 365 Secure wynik analizuje zabezpieczenia organizacji usługi Office 365 na podstawie regularnych działań i ustawienia zabezpieczeń i przypisuje wynik. Rozpocznij od biorąc pod uwagę aktualny wynik. Wykonywanie akcji zalecane w tym artykule zwiększa wynik. Celem jest nie do osiągnięcia ocena max, ale należy pamiętać o możliwości ochrony środowiska nie negatywnie wpływają na wydajność pracy użytkowników. 

Aby uzyskać więcej informacji zobacz [Microsoft Secure wynik](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podnoszenie poziomu ochrony przed złośliwym oprogramowaniem w korespondencji

Środowiska usługi Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem, ale może zwiększyć tę ochronę przez blokowanie załączników z typami plików, które są powszechnie stosowane w poszukiwaniu złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomości e-mail:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu poświadczeń konta administratora. 
    
2. W zabezpieczeniach pakietu Office 365 &amp; Centrum zgodności w okienku nawigacyjnym z lewej strony, w obszarze **Zarządzanie zagrożeniami**, wybierz **zasadę** \> **Wykrywającego złośliwe oprogramowanie**.
    
3. Kliknij dwukrotnie zasadę domyślną do edytowania tej zasady całej firmy.
    
4. Kliknij przycisk **Ustawienia**.
    
5. W obszarze **Typowe Filtr typów załączników**zaznacz **na**. Typy plików, które są blokowane są wymienione w oknie się poniżej tego formantu.  Upewnij się, że możesz dodać te typy plików:
   - ade, adp, ani, dolny, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, zadania, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> Można dodać lub usunąć typy plików później, w razie potrzeby.
    
6. Kliknij **zapisać.**
    
Aby uzyskać więcej informacji zobacz temat [Ochrona antywirusowa](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochronę przed szkodnika

Szkodnika ogranicza dostęp do danych przez system szyfrowania plików lub blokowania monitorach komputerowych. Następnie próbuje wyłudzić pieniądze od ofiar, prosząc o "okup", zazwyczaj w postaci kryptowaluty jak Bitcoin, w zamian za dostęp do danych. 
  
Można ochronić się przed szkodnika przez utworzenie reguły przepływu, aby zablokować rozszerzenia plików, które są powszechnie stosowane do szkodnika (te zostały dodane w kroku [podnieść poziom ochrony przed złośliwym oprogramowaniem w programie Poczta](#raise-the-level-of-protection-against-malware-in-mail) ) lub ostrzec użytkowników, którzy otrzymują te poczty jeden lub więcej załączniki do wiadomości e-mail.

Oprócz plików, które są blokowane w poprzednim kroku również jest dobrym rozwiązaniem jest utworzenie reguły ostrzec użytkowników przed otwarciem załączników pliku pakietu Office, które zawierają makra. Szkodnika może być ukryte wewnątrz makra, więc możemy ostrzec użytkowników nie otworzyć te pliki od osób, które nie znają.

Aby utworzyć regułę transportu poczty:
  
1. Przejdź do Centrum administracyjnego o <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> i wybierz polecenie **Admin centers** \> **programu Exchange**.
    
2. W kategorii **przepływu poczty** kliknij przycisk **reguły**.
    
3. Kliknij **+**, a następnie kliknij przycisk **Utwórz nową regułę**.
    
4. Kliknij przycisk **Więcej opcji** w dolnej części okna dialogowego, aby zobaczyć pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli dla reguły. Pozostaw pozostałe ustawienia domyślnego, chyba że chcesz zmienić.
    
6. Kliknij pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzec użytkowników przed otwarciem załączników plików pakietu Office**||
|:-----|:-----|:-----|
|Name (Nazwa)  <br/> |Reguła anty szkodnika: ostrzec użytkowników  <br/>  |
|Zastosuj tę regułę, jeśli. . .  <br/> |Żadnego załącznika. . . rozszerzenie pliku jest zgodne. . .  <br/> |
|Podaj wyrazy lub frazy  <br/> |Dodaj te typy plików:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Wykonaj następujące czynności. . .  <br/> |Powiadamia adresata z wiadomości  <br/> |
|Przekaż wiadomość  <br/> |Nie należy otwierać tego typu pliki od osób, które nie wiadomo, ponieważ mogą zawierać makra z złośliwego kodu.  <br/> |
   
Aby uzyskać więcej informacji, zobacz:
  
- [Jak radzić sobie z szkodnika](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Przywracanie OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Zatrzymaj automatyczne przekazywanie wiadomości e-mail

Hakerzy, uzyskujących dostęp do skrzynki pocztowej użytkownika, mogą wykraść poczty przez ustawienie skrzynek pocztowych, aby automatycznie przesłać dalej wiadomości e-mail. Może się to zdarzyć nawet bez wiedzy użytkownika. Można temu zapobiec sytuacjom, konfigurując reguły przepływu poczty. 
  
Aby utworzyć regułę transportu poczty, ten krótki klip [wideo](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) lub wykonaj następujące kroki:
  
1. W Centrum administracyjnego usługi Microsoft 365 kliknij **Admin centers** \> **programu Exchange**.
    
2. W kategorii **przepływu poczty** kliknij przycisk **reguły**.
    
3. Kliknij **+**, a następnie kliknij przycisk **Utwórz nową regułę**.
    
4. Kliknij przycisk **Więcej opcji** w dolnej części okna dialogowego, aby zobaczyć pełny zestaw opcji. 
    
5. Zastosuj ustawienia w poniższej tabeli. Pozostaw pozostałe ustawienia domyślnego, chyba że chcesz zmienić.
    
6. Kliknij pozycję **Zapisz**.
    
|**Ustawienie**|**Ostrzec użytkowników przed otwarciem załączników plików pakietu Office**|
|:-----|:-----|
|Name (Nazwa)  <br/> |Uniemożliwić automatyczne przesyłanie dalej wiadomości e-mail do domen zewnętrznych  <br/> |
|Zastosuj tę regułę, jeśli...  <br/> |Nadawca. . . jest zewnętrzny/wewnętrzny. . . Wewnątrz organizacji  <br/> |
|Dodaj warunek  <br/> |Właściwości wiadomości. . . Uwzględnij typ wiadomości. . . Automatyczne przekazywanie  <br/> |
|Wykonaj następujące czynności...  <br/> |Blokowanie wiadomości. . . Odrzuć wiadomość i zawierać wyjaśnienie.  <br/> |
|Przekaż wiadomość  <br/> |Ze względów bezpieczeństwa nie będzie mógł automatyczne przekazywanie wiadomości e-mail spoza tej organizacji.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrona poczty e-mail przed wyłudzeniami informacji

Jeśli masz skonfigurowane jednej lub kilku domen niestandardowych dla danego środowiska usługi Office 365 lub Microsoft 365, można skonfigurować odpowiednią ochronę anti-phishing. Ochrona anti-phishing ATP, część pakietu Office 365 Zaawansowana ochrona przed zagrożeniami, może pomóc chronić organizacji przed złośliwego podstawie personifikacji wyłudzania i innymi atakami typu phishing. Jeśli nie skonfigurowano własnej domeny, nie trzeba to zrobić.
  
Zaleca się, że możesz rozpocząć objętej tą ochroną, poprzez utworzenie zasady ochrony najważniejsze użytkowników i domeny niestandardowej. 

  
Aby utworzyć zasady anti-phishing ATP, obejrzyj [to wideo szkolenie krótki](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)lub wykonaj następujące kroki:
  
1. Przejdź do witryny [https://protection.office.com](https://protection.office.com). 
    
2. W zabezpieczeniach pakietu Office 365 &amp; Centrum zgodności w okienku nawigacyjnym z lewej strony, w obszarze **Zarządzanie zagrożeniami**, wybierz **zasadę**.
    
3. Na stronie **zasad** wybierz **ATP anti-phishing**.
    
4. Na stronie **Anti-phishing** wybierz **+ Utwórz**. Uruchamia kreatora, który przeprowadza użytkownika przez definiowanie zasad anti-phishing.
    
5. Określ nazwę, opis i ustawienia zasad sieci zgodnie z zaleceniami w poniższej tabeli. Więcej szczegółów znajdziesz [więcej informacji na temat opcji zasad anti-phishing ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) . 
    
6. Po przejrzeniu ustawień, wybierz opcję **Utwórz tej zasady** lub **Zapisz**, stosownie do przypadku.
    

|**Ustawienie lub opcji**<br/>|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Domeny i najbardziej wartościową personelu kampanii  <br/> |
|Opis  <br/> |Upewnij się, coraz ważniejsze, personel i naszej domenie są nie są traktowane.  <br/> |
|Dodaj użytkowników do ochrony  <br/> |Wybierz opcję **+ Dodaj warunek, odbiorca jest**. Wpisz nazwy użytkowników lub wpisz adres e-mail kandydata, Menedżer kampanii i innych członków personelu ważne. Można dodać maksymalnie 20 adresów wewnętrznych i zewnętrznych, które chcesz chronić przed personifikacji.  <br/> |
|Dodawanie domen do ochrony  <br/> |Wybierz opcję **+ Dodaj warunek domeny adresata jest**. Wprowadź domenę niestandardowych skojarzone z subskrypcją usługi Microsoft 365, jeśli zdefiniowano jedną. Można wprowadzić więcej niż jednej domeny.  <br/> |
|Wybierz akcje  <br/> |Jeśli wiadomość e-mail jest wysyłana przez personifikowanym użytkownikiem: Wybierz **Przekierowanie wiadomości na inny adres e-mail**, a następnie wpisz adres e-mail administratora zabezpieczeń; na przykład *Alicja<span><span>@contoso.com*.          Jeśli wiadomość e-mail jest wysyłana przez domenę personifikowanego: Wybierz **komunikat kwarantanny**.  <br/> |
|Analizy skrzynki pocztowej  <br/> |Analizy skrzynki pocztowej jest zaznaczone domyślnie, podczas tworzenia nowej zasady anti-phishing. Pozostawić to ustawienie **na** najlepsze wyniki.  <br/> |
|Dodawanie zaufanych nadawców i domen  <br/> |W tym miejscu można dodać własnej domeny lub innych zaufanych domen.  <br/> |
|Stosowane do  <br/> |Wybierz **domeny adresata**. W **żadnej z tych**wybierz opcję **Wybierz**. Wybierz **+ Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład contoso *.<span> <span>com*, na liście, a następnie wybierz polecenie **Dodaj**. Wybierz **Gotowe**.  <br/> |
   
Aby uzyskać więcej informacji zobacz [Konfigurowanie zasad anti-phishing Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochronę przed złośliwymi załącznikami i plików z bezpiecznych załączników ATP

Osoby regularnie wysyłać, odbierać i udostępniać załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Nie zawsze jest łatwo stwierdzić, czy załącznik jest bezpieczny lub złośliwego tylko przeglądając wiadomości e-mail. Office 365 Zaawansowana ochrona przed zagrożeniami obejmuje ochronę ATP bezpieczne załączniki, ale tej ochrony nie jest włączony domyślnie. Zaleca się, można utworzyć nową regułę do rozpoczęcia korzystania z tej ochrony. Ochrona ta rozciąga się do plików w programie SharePoint, OneDrive i Teams firmy Microsoft.
  
Aby utworzyć zasady bezpieczne załączniki ATP, ten krótki klip [wideo](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)lub wykonaj następujące kroki:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się na konto administratora. 
    
2. W zabezpieczeniach pakietu Office 365 &amp; Centrum zgodności w okienku nawigacyjnym z lewej strony, w obszarze **Zarządzanie zagrożeniami**, wybierz **zasadę**.
    
3. Na stronie zasady wybierz **bezpieczne załączniki ATP**.
    
4. Na stronie bezpiecznych załączników tej ochrony mają szerokie zastosowanie przez zaznaczenie pola wyboru **Włącz ATP, SharePoint, usługi i zespoły pracowników firmy Microsoft** . 
    
5. Wybierz **+** Aby utworzyć nową zasadę. 
    
6. Zastosuj ustawienia w poniższej tabeli. 
    
7. Po przejrzeniu ustawień, wybierz opcję **Utwórz tej zasady** lub **Zapisz**, stosownie do przypadku.
    

|**Ustawienie lub opcji**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Blok bieżących i przyszłych wiadomości z wykryto złośliwe oprogramowanie.  <br/> |
|Opis  <br/> |Zablokowanie bieżących i przyszłych wiadomości e-mail i załączniki z wykryto złośliwe oprogramowanie.  <br/> |
|Zapisz załączniki nieznanym złośliwym oprogramowaniem odpowiedzi  <br/> |Zaznacz **Blok - zablokowanie bieżących i przyszłych wiadomości e-mail i załączniki z wykryto złośliwe oprogramowanie**.  <br/> |
|Załącznik przekierowanie dla wykrywania  <br/> |Należy włączyć funkcję przekierowywania (Zaznacz to pole) wprowadź konto administratora lub Konfiguracja skrzynki pocztowej dla kwarantanny.          Zastosowanie powyższego wyboru jeśli złośliwego oprogramowania skanowanie załączników do przekroczenia limitu czasu lub wystąpi błąd (Zaznaczenie tego pola).  <br/> |
|Stosowane do  <br/> |Jest domeną adresata. . . Wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji zobacz [Konfigurowanie zasad anti-phishing Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrona przed atakami typu phishing z bezpiecznego łącza ATP

Czasami hakerzy ukryć złośliwych witryn z łącza w wiadomości e-mail lub innych plików. Office 365 ATP bezpiecznego łącza (ATP bezpiecznego łącza), część pakietu Office 365 Zaawansowana ochrona przed zagrożeniami, może pomóc chronić organizacji poprzez zapewnienie czasu kliknij weryfikację adresów sieci web (URL) w wiadomości e-mail i dokumentów pakietu Office. Ochrona jest zdefiniowany za pomocą zasad bezpiecznego łącza ATP.
  
Firma Microsoft zaleca, należy wykonać następujące czynności:
  
- Modyfikowanie domyślnych zasad do zwiększenia ochrony.
    
- Dodać nową zasadę kierowane do wszystkich odbiorców w domenie.
    
Aby skonfigurować bezpiecznego łącza ATP, obejrzyj [to wideo, krótkie szkolenie](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa), lub wykonaj następujące kroki:
  
1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się na konto administratora. 
    
2. W zabezpieczeniach pakietu Office 365 &amp; Centrum zgodności w okienku nawigacyjnym z lewej strony, w obszarze **Zarządzanie zagrożeniami**, wybierz **zasadę**.
    
3. Na stronie zasady wybierz **ATP bezpiecznego łącza**.
    
Aby zmodyfikować domyślne zasady:
  
1. Na stronie bezpiecznego łącza w obszarze **zasady, które dotyczą całej organizacji**wybierz **domyślne** zasady. 
    
2. W obszarze **Ustawienia, które dotyczą zawartości z wyjątkiem wiadomości e-mail**zaznacz **Office 365 ProPlus, Urząd iOS i Android**.
    
3. Kliknij pozycję **Zapisz**. 
    
Aby utworzyć nową zasadę kierowane do wszystkich odbiorców w domenie:
  
1. Na stronie bezpiecznego łącza w ramach **zasady, które dotyczą całej organizacji**, kliknij przycisk **+** Aby utworzyć nową zasadę. 
    
2. Zastosuj ustawienia wymienione w poniższej tabeli.
    
3. Kliknij pozycję **Zapisz**. 

|**Ustawienie lub opcji**|**Zalecane ustawienie** <br/>|
|:-----|:-----|
|Name (Nazwa)  <br/> |Zasady bezpiecznego łącza dla wszystkich adresatów w domenie  <br/> |
|Wybierz akcję dla nieznanych potencjalnie złośliwe adresy URL w wiadomości  <br/> |Zaznacz **na - adresy URL będzie przebudowywany i porównywane z listą znanych niebezpiecznego łącza, gdy użytkownik kliknie na łącze**.  <br/> |
|Umożliwia bezpieczne załączniki skanują zawartość do pobrania  <br/> |Zaznacz to pole.  <br/> |
|Stosowane do  <br/> |Jest domeną adresata. . . Wybierz domenę.  <br/> |
   
Aby uzyskać więcej informacji zobacz [bezpieczne łącza Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Przejdź do Centrum administracyjnego Windows Intune

1. Zalogować się do [portalu Azure](https://portal.azure.com/).

2. Zaznacz **wszystkie usługi** i wpisz *Windows Intune* w **Polu wyszukiwania**.

3. Gdy wyniki są wyświetlane, kliknij przycisk start, obok **Intune firmy Microsoft** , aby dodać ją do ulubionych i łatwo później odnaleźć.

Oprócz Centrum administracyjnego Intune służy do rejestrowania i zarządzać urządzeniami w organizacji. Aby uzyskać więcej informacji zobacz [możliwości przez metodę rejestracji dla urządzeń z systemem Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) i [Opcje rejestrowania dla urządzeń zarządzanych przez usługę Intune](https://docs.microsoft.com/intune/enrollment-options).
