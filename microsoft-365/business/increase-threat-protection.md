---
title: Zwiększanie ochrony przed zagrożeniami na platformie Microsoft 365 dla firm
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
description: Skonfiguruj usługę Microsoft Defender dla usługi Office 365 i chroń poufne dane przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami.
ms.openlocfilehash: 6526ed9a849e83f19f74656004978089ce367ea9
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198396"
---
# <a name="increase-threat-protection"></a>Zwiększanie ochrony przed zagrożeniami

Ten artykuł ułatwia zwiększenie ochrony subskrypcji platformy Microsoft 365 w celu ochrony przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami. Te zalecenia są odpowiednie dla organizacji ze zwiększoną potrzebą zabezpieczeń, np. biura prawne i gabinety opieki zdrowotnej.

Przed rozpoczęciem sprawdź swój wynik bezpiecznego połączenia w usłudze Office 365. Bezpieczny wynik usługi Office 365 analizuje zabezpieczenia organizacji na podstawie twoich regularnych działań i ustawień zabezpieczeń, a następnie przypisuje wynik. Zacznij od notacji bieżącego wyniku. Aby zwiększyć wynik, wykonaj czynności zalecane w tym artykule. Celem nie jest osiągnięcie maksymalnej liczby wyników, ale świadomość możliwości ochrony środowiska, które nie mają negatywnego wpływu na wydajność pracy użytkowników.

Aby uzyskać więcej informacji, zobacz [Microsoft Secure Score](../security/defender/microsoft-secure-score.md).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podnoszenie poziomu ochrony przed złośliwym oprogramowaniem w wiadomościach e-mail

Środowisko usługi Office 365 lub platformy Microsoft 365 zapewnia ochronę przed złośliwym oprogramowaniem. Możesz zwiększyć tę ochronę, blokując załączniki za pomocą typów plików, które są często używane w przypadku złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomościach e-mail:

1. Przejdź do [https://protection.office.com](https://protection.office.com) konta administratora i zaloguj się przy użyciu jego poświadczeń.

2. W Centrum zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie zagrożeniami wybierz &amp; **pozycję Zasady** ochrony przed  \> **złośliwym oprogramowaniem.**

3. Kliknij dwukrotnie zasady domyślne, aby edytować te zasady dla całej firmy.

4. Wybierz **pozycję Ustawienia**.

5. W **obszarze Filtr typowych typów załączników** wybierz pozycję **Wł.** Blokowane typy plików są wyświetlane w oknie bezpośrednio poniżej tej kontrolki. Upewnij się, że dodano następujące typy plików:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   W razie potrzeby możesz później dodać lub usunąć typy plików.

6. Wybierz **pozycję Zapisz.**

Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem w uiece EOP.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Ochrona przed oprogramowaniem wymuszającym okup

Oprogramowanie wymuszające okup ogranicza dostęp do danych przez szyfrowanie plików lub blokowanie ekranów komputera. Następnie próbuje wyłudzić pieniądze od chwalenia, prosząc o "ransom" zwykle w formie banków, takich jak Waluty, w zamian za dostęp do danych.

Aby chronić przed oprogramowaniem wymuszającym okup, utwórz co najmniej jedną regułę przepływu poczty, aby blokować rozszerzenia plików, które są często używane dla oprogramowania wymuszającego okup. (Te reguły zostały dodane w kroku [podnieść poziom ochrony przed](#raise-the-level-of-protection-against-malware-in-mail) złośliwym oprogramowaniem). Możesz również ostrzegać użytkowników, którzy otrzymają te załączniki w wiadomościach e-mail.

Oprócz plików zablokowanych w poprzednim kroku warto utworzyć regułę ostrzegawczą użytkowników przed otwarciem plików załączników pakietu Office, które zawierają makra. Oprogramowanie wymuszające okup może być ukryte w makrach, więc ostrzegaj użytkowników, aby nie otwierali tych plików przed nieumiejętną wiedzą.

Aby utworzyć regułę transportu poczty:

1. Przejdź do centrum administracyjnego w <https://admin.microsoft.com> uciek i wybierz pozycję **Centra administracyjne programu** \> **Exchange.**

2. W kategorii **przepływ poczty** e-mail wybierz **pozycję reguły**.

3. Wybierz **+** pozycję , a następnie wybierz pozycję Utwórz **nową regułę**.

4. Wybierz **pozycję Więcej** opcji u dołu okna dialogowego, aby wyświetlić pełny zestaw opcji.

5. Zastosuj do reguły ustawienia z poniższej tabeli. Użyj wartości domyślnych pozostałych ustawień, chyba że chcesz je zmienić.

6. Wybierz **Zapisz**.

|Ustawienie|Ostrzegaj użytkowników przed otwieraniem załączników plików pakietu Office||
|---|---|---|
|Name (Nazwa)|Reguła ochrony przed oprogramowaniem wymuszającym okup: ostrzeganie użytkowników|
|Zastosuj tę regułę, jeśli . . .|Dowolny załącznik. . . rozszerzenie pliku jest do tego dopasowania. . .|
|Określanie wyrazów lub fraz|Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Wykonaj następujące czynności. . .|Powiadamianie adresata za pomocą wiadomości|
|Podaj tekst wiadomości|Tego typu pliki nie należy otwierać u osób, których nie znasz, ponieważ mogą zawierać makra ze złośliwym kodem.|

Aby uzyskać więcej informacji, zobacz:

- [Oprogramowanie wymuszające okup: jak zmniejszyć ryzyko](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Przywracanie usługi OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zatrzymywanie automatycznego przesyłania dalej wiadomości e-mail

Hakerzy, którzy uzyskają dostęp do skrzynki pocztowej użytkownika, mogą ukraść pocztę, ustawiając ją w celu automatycznego przesyłania dalej wiadomości e-mail. Może się to zdarzyć nawet bez wiedzy użytkownika. Aby temu zapobiec, skonfiguruj regułę przepływu poczty e-mail.

Aby utworzyć regułę transportu poczty, obejrzyj [ten krótki klip wideo](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) lub wykonaj następujące czynności:

1. W centrum administracyjnym platformy Microsoft 365 wybierz pozycję **Centra administracyjne programu** \> **Exchange**.

2. W kategorii **przepływ poczty** e-mail wybierz **pozycję reguły**.

3. Wybierz **+** pozycję , a następnie wybierz pozycję Utwórz **nową regułę**.

4. Aby wyświetlić wszystkie opcje, wybierz pozycję **Więcej opcji** u dołu okna dialogowego.

5. Zastosuj ustawienia z poniższej tabeli. Użyj wartości domyślnych pozostałych ustawień, chyba że chcesz je zmienić.

6. Wybierz **Zapisz**.

|Ustawienie|Ostrzegaj użytkowników przed otwieraniem załączników plików pakietu Office|
|---|---|
|Name (Nazwa)|Uniemożliwianie automatycznego przesyłania poczty e-mail do domen zewnętrznych|
|Zastosuj tę regułę, jeśli...|Nadawca . . . jest zewnętrzna/wewnętrzna. . . Wewnątrz organizacji|
|Dodaj warunek|Właściwości wiadomości. . . uwzględnij typ wiadomości . . . Automatyczne przesyłanie dalej|
|Wykonaj następujące czynności...|Zablokuj wiadomość. . . odrzuć wiadomość i dołącz wyjaśnienie.|
|Podaj tekst wiadomości|Automatyczne przesyłanie dalej poczty e-mail poza tę organizację jest blokowane ze względów bezpieczeństwa.|


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrona poczty e-mail przed atakami wyłudzających informacje

Jeśli skonfigurowano co najmniej jedną domenę niestandardową w środowisku usługi Office 365 lub platformy Microsoft 365, możesz skonfigurować ukierunkowaną ochronę przed wyłudzaniem informacji. Ochrona przed wyłudzaniem informacji, która jest częścią programu Microsoft Defender dla usługi Office 365, może pomóc chronić Twoją organizację przed atakami wyłudzania informacji opartymi na złośliwej personifikacji i przed innymi atakami wyłudzania informacji. Jeśli nie skonfigurowano domeny niestandardowej, nie musisz tego robić.

Zalecamy wprowadzenie do tej ochrony przez utworzenie zasad chroniących najważniejszych użytkowników i domenę niestandardową.

Aby utworzyć zasady ochrony przed wyłudzaniem informacji w [](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)usłudze Microsoft Defender dla usługi Office 365, obejrzyj ten krótki szkoleniowy klip wideo lub wykonaj następujące czynności:

1. Przejdź do witryny [https://protection.office.com](https://protection.office.com).

2. W Centrum &amp; zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie **zagrożeniami** wybierz pozycję **Zasady**.

3. Na stronie **Zasady** wybierz pozycję Ochrona **przed wyłudzaniem informacji**.

4. Na stronie **ochrony przed wyłudzaniem** informacji wybierz pozycję **+ Utwórz.** Kreator przeprowadzi Cię przez proces definiowania zasad ochrony przed wyłudzaniem informacji.

5. Określ nazwę, opis i ustawienia zasad zgodnie z zaleceniami w poniższej tabeli. Aby uzyskać więcej szczegółowych informacji, zobacz Informacje o zasadach ochrony przed wyłudzaniem informacji [w programie Microsoft Defender dla opcji usługi Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Po przejrzeniu ustawień wybierz pozycję Utwórz **te zasady** lub **Zapisz** odpowiednio do potrzeb.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Domena i najcenniejszy personel kampanii|
|Opis|Upewnij się, że nie podszywają się najważniejsze pracownicy i nasza domena.|
|Dodawanie użytkowników w celu ochrony|Wybierz **pozycję + Dodaj warunek, adresatem jest**. Wpisz nazwy użytkowników lub wprowadź adres e-mail kandydata, menedżera kampanii i innych ważnych członków personelu. Możesz dodać maksymalnie 20 wewnętrznych i zewnętrznych adresów, które chcesz chronić przed personifikacji.|
|Dodawanie domen w celu ochrony|Wybierz **pozycję + Dodaj warunek, domena adresata to**. Wprowadź domenę niestandardową skojarzoną z Twoją subskrypcją platformy Microsoft 365, jeśli została zdefiniowana. Możesz wprowadzić więcej niż jedną domenę.|
|Wybieranie akcji|Jeśli wiadomość e-mail zostanie wysłana przez spersonifikowanego użytkownika: Wybierz pozycję Przekieruj wiadomość na inny adres e-mail **,** a następnie wpisz adres e-mail administratora zabezpieczeń. na przykład *Alice <span> <span> @contoso.com*. Jeśli wiadomość e-mail jest wysyłana przez spersonifikowane domeny: Wybierz **pozycję Kwarantanna wiadomości**.|
|Inteligencja skrzynek pocztowych|Domyślnie podczas tworzenia nowych zasad ochrony przed wyłudzaniem informacji jest zaznaczona inteligencja skrzynek pocztowych. Aby uzyskać najlepsze **wyniki, pozostaw** to ustawienie wł.|
|Dodawanie zaufanych nadawców i domen|Tutaj możesz dodać własną domenę lub dowolne inne zaufane domeny.|
|Zastosowano do|Wybierz **pozycję Domena adresata to**. W **obszarze Dowolny z tych** wybierz pozycję **Wybierz**. Wybierz **pozycję + Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso. <span> <span> com*, na liście, a następnie wybierz pozycję **Dodaj**. Wybierz **pozycję Gotowe**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Ochrona przed złośliwymi załącznikami i plikami za pomocą bezpiecznych załączników

Osoby regularnie wysyłają, odbierają i udostępniają załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Samo patrząc na wiadomość e-mail, nie zawsze łatwo jest ustalić, czy załącznik jest bezpieczny, czy złośliwy. Program Microsoft Defender dla usługi Office 365 zawiera bezpieczną ochronę załączników, ale ta ochrona nie jest domyślnie włączona. Zalecamy utworzenie nowej reguły w celu rozpoczęcia korzystania z tej ochrony. Ta ochrona obejmuje również pliki w programie SharePoint, usłudze OneDrive i aplikacji Microsoft Teams.

Aby utworzyć zasady bezpiecznego załącznika, obejrzyj [ten krótki klip wideo](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)lub wykonaj następujące czynności:

1. Przejdź do [https://protection.office.com](https://protection.office.com) pozycji , a następnie zaloguj się przy użyciu konta administratora.

2. W Centrum &amp; zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie **zagrożeniami** wybierz pozycję **Zasady**.

3. Na stronie Zasady wybierz pozycję **Bezpieczne załączniki.**

4. Na stronie Bezpieczne załączniki zastosuj tę ochronę ogólnie, zaznaczając pole wyboru Włącz atP dla **programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams.**

5. Wybierz **+** pozycję , aby utworzyć nowe zasady.

6. Zastosuj ustawienia z poniższej tabeli.

7. Po przejrzeniu ustawień wybierz pozycję **Utwórz te zasady** lub **Zapisz** odpowiednio do potrzeb.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Blokuj bieżące i przyszłe wiadomości e-mail za pomocą wykrytego złośliwego oprogramowania.|
|Opis|Blokuj bieżące i przyszłe wiadomości e-mail oraz załączniki za pomocą wykrytego złośliwego oprogramowania.|
|Zapisywanie załączników z nieznanym złośliwym oprogramowaniem|Wybierz **pozycję Blokuj — blokuj bieżące i przyszłe wiadomości e-mail oraz załączniki za pomocą wykrytego złośliwego oprogramowania.**|
|Przekierowywanie załącznika przy wykrywaniu|Włącz przekierowywanie (zaznacz to pole) Wprowadź konto administratora lub konfigurację skrzynki pocztowej do kwarantanny.          Zastosowanie powyższej opcji w przypadku przecowania czasu lub błędu podczas skanowania w poszukiwaniu załączników (zaznacz to pole).|
|Zastosowano do|Domeną adresata jest . . . wybierz domenę.|

Aby uzyskać więcej informacji, zobacz Konfigurowanie zasad ochrony przed wyłudzaniem [informacji w usłudze Microsoft Defender dla usługi Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Ochrona przed atakami wyłudzających informacje za pomocą bezpiecznych linków

Hakerzy czasami ukrywają złośliwe witryny internetowe w linkach w wiadomościach e-mail lub innych plikach. Bezpieczne linki, część programu Microsoft Defender dla usługi Office 365, może pomóc chronić Twoją organizację, zapewniając weryfikację adresów internetowych (adresów URL) za pomocą kliknięcia w wiadomościach e-mail i dokumentach pakietu Office. Ochrona jest definiowana za pomocą zasad bezpiecznych linków.

Zalecamy:

- Zmodyfikuj zasady domyślne, aby zwiększyć ochronę.

- Dodaj nowe zasady kierowane do wszystkich adresatów w domenie.

Aby skonfigurować bezpieczne linki, obejrzyj ten krótki film [szkoleniowy](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)lub wykonaj następujące czynności:

1. Przejdź do [https://protection.office.com](https://protection.office.com) pozycji , a następnie zaloguj się przy użyciu konta administratora.

2. W Centrum &amp; zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie **zagrożeniami** wybierz pozycję **Zasady**.

3. Na stronie Zasady wybierz pozycję **Bezpieczne linki.**

Aby zmodyfikować zasady domyślne:

1. Na stronie Bezpieczne linki w obszarze **Zasady stosowane do** całej organizacji wybierz zasady domyślne. 

2. W **obszarze Ustawienia, które dotyczą zawartości z** wyjątkiem wiadomości e-mail wybierz pozycję **Aplikacje Microsoft 365 dla przedsiębiorstw, Office dla systemów iOS i Android.**

3. Wybierz **Zapisz**.

Aby utworzyć nowe zasady kierowane do wszystkich adresatów w domenie:

1. Na stronie Bezpieczne linki w obszarze Zasady stosowane **do** całej organizacji wybierz pozycję **+** , aby utworzyć nowe zasady.

2. Zastosuj ustawienia wymienione w poniższej tabeli.

3. Wybierz **Zapisz**.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Zasady bezpiecznych linków dla wszystkich adresatów w domenie|
|Wybierz akcję dla nieznanych, potencjalnie złośliwych adresów URL w wiadomościach|Wybierz **pozycję W — po kliknięciu linku** przez użytkownika adresy URL zostaną ponownie napisane i zaewidencjonowane pod kątem listy znanych złośliwych linków.|
|Używanie bezpiecznych załączników do skanowania zawartości do pobrania|Zaznacz to pole.|
|Zastosowano do|Domeną adresata jest . . . wybierz domenę.|

Aby uzyskać więcej informacji, zobacz [Bezpieczne linki.](../security/office-365-security/safe-links.md)

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/)

2. Wybierz **pozycję Wszystkie usługi** i wpisz *intune* w polu **wyszukiwania**.

3. Po wyświetlonej stronie wyników wybierz start obok usługi **Microsoft Intune,** aby dodać ją do ulubionych i ułatwić jej późniejsze znalezienie.

Oprócz centrum administracyjnego do rejestrowania urządzeń organizacji i zarządzania nimi możesz użyć usługi Intune. Aby uzyskać więcej informacji, zobacz Funkcje według [metody rejestracji](/intune/enrollment/enrollment-method-capab) dla urządzeń z systemem Windows i Opcje rejestracji dla urządzeń [zarządzanych przez usługę Intune.](/intune/enrollment-options)
