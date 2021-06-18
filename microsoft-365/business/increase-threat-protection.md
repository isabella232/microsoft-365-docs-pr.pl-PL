---
title: Zwiększanie ochrony przed zagrożeniami Microsoft 365 dla firm
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Skonfiguruj usługę Microsoft Defender na Office 365 i chroń poufne dane przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami.
ms.openlocfilehash: a995063cef6fdc42ad62079d49d58edc9d07b52c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924324"
---
# <a name="increase-threat-protection"></a>Zwiększanie ochrony przed zagrożeniami

Ten artykuł ułatwia zwiększenie ochrony subskrypcji usługi Microsoft 365 w celu ochrony przed wyłudzaniem informacji, złośliwym oprogramowaniem i innymi zagrożeniami. Te zalecenia są odpowiednie dla organizacji ze zwiększoną potrzebą zabezpieczeń, np. biura prawne i gabinety opieki zdrowotnej.

Przed rozpoczęciem należy sprawdzić Office 365 wyniku bezpiecznego. Office 365 Secure Score analizuje zabezpieczenia organizacji na podstawie twoich zwykłych działań i ustawień zabezpieczeń, a następnie przypisuje wynik. Zacznij od notacji bieżącego wyniku. Aby zwiększyć wynik, wykonaj czynności zalecane w tym artykule. Celem nie jest osiągnięcie maksymalnej liczby wyników, ale świadomość możliwości ochrony środowiska, które nie mają negatywnego wpływu na wydajność pracy użytkowników.

Aby uzyskać więcej informacji, zobacz [Microsoft Secure Score](../security/defender/microsoft-secure-score.md).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podnoszenie poziomu ochrony przed złośliwym oprogramowaniem w wiadomościach e-mail

Twoje Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem. Możesz zwiększyć tę ochronę, blokując załączniki za pomocą typów plików, które są często używane w przypadku złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomościach e-mail:

1. Przejdź do [https://protection.office.com](https://protection.office.com) konta administratora i zaloguj się przy użyciu jego poświadczeń.

2. W Centrum zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie zagrożeniami wybierz &amp; **pozycję Zasady** ochrony przed  \> **złośliwym oprogramowaniem.**

3. Kliknij dwukrotnie zasady domyślne, aby edytować te zasady dla całej firmy.

4. Wybierz **Ustawienia**.

5. W **obszarze Filtr typowych typów załączników** wybierz pozycję **Wł.** Blokowane typy plików są wyświetlane w oknie bezpośrednio poniżej tej kontrolki. Upewnij się, że dodano następujące typy plików:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   W razie potrzeby możesz później dodać lub usunąć typy plików.

6. Wybierz **pozycję Zapisz.**

Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem w uiece EOP.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Ochrona przed oprogramowaniem wymuszającym okup

Oprogramowanie wymuszające okup ogranicza dostęp do danych przez szyfrowanie plików lub blokowanie ekranów komputera. Następnie próbuje wyłudzić pieniądze od chwalenia, prosząc o "ransom" zwykle w formie banków, takich jak Waluty, w zamian za dostęp do danych.

Aby chronić przed oprogramowaniem wymuszającym okup, utwórz co najmniej jedną regułę przepływu poczty, aby blokować rozszerzenia plików, które są często używane dla oprogramowania wymuszającego okup. (Te reguły zostały dodane w kroku [podnieść poziom ochrony przed](#raise-the-level-of-protection-against-malware-in-mail) złośliwym oprogramowaniem). Możesz również ostrzegać użytkowników, którzy otrzymają te załączniki w wiadomościach e-mail.

Oprócz plików zablokowanych w poprzednim kroku warto utworzyć regułę ostrzegawczą użytkowników przed otwieraniem załączników z plikami Office, które zawierają makra. Oprogramowanie wymuszające okup może być ukryte w makrach, więc ostrzegaj użytkowników, aby nie otwierali tych plików przed nieumiejętną wiedzą.

Aby utworzyć regułę transportu poczty:

1. Przejdź do centrum administracyjnego w <https://admin.microsoft.com> miejscu , a następnie wybierz pozycję Centra **administracyjne** \> **Exchange.**

2. W kategorii **przepływ poczty** e-mail wybierz **pozycję reguły**.

3. Wybierz **+** pozycję , a następnie wybierz pozycję Utwórz **nową regułę**.

4. Wybierz **pozycję Więcej** opcji u dołu okna dialogowego, aby wyświetlić pełny zestaw opcji.

5. Zastosuj do reguły ustawienia z poniższej tabeli. Użyj wartości domyślnych pozostałych ustawień, chyba że chcesz je zmienić.

6. Wybierz **Zapisz**.

|Ustawienie|Ostrzegaj użytkowników przed otwieraniem załączników Office plików|
|---|---|
|Name (Nazwa)|Reguła ochrony przed oprogramowaniem wymuszającym okup: ostrzeganie użytkowników|
|Zastosuj tę regułę, jeśli . . .|Dowolny załącznik. . . rozszerzenie pliku jest do tego dopasowania. . .|
|Określanie wyrazów lub fraz|Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Wykonaj następujące czynności. . .|Powiadamianie adresata za pomocą wiadomości|
|Podaj tekst wiadomości|Tego typu pliki nie należy otwierać u osób, których nie znasz, ponieważ mogą zawierać makra ze złośliwym kodem.|

Aby uzyskać więcej informacji, zobacz:

- [Oprogramowanie wymuszające okup: jak zmniejszyć ryzyko](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Przywracanie OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zatrzymywanie automatycznego przesyłania dalej wiadomości e-mail

Hakerzy, którzy uzyskają dostęp do skrzynki pocztowej użytkownika, mogą ukraść pocztę, ustawiając ją w celu automatycznego przesyłania dalej wiadomości e-mail. Może się to zdarzyć nawet bez wiedzy użytkownika. Aby temu zapobiec, skonfiguruj regułę przepływu poczty e-mail.

Aby utworzyć regułę transportu poczty, obejrzyj [ten krótki klip wideo](../business-video/stop-email-auto-forward.md) lub wykonaj następujące czynności:

1. W centrum administracyjne platformy Microsoft 365 wybierz pozycję **Centra administracyjne** \> **Exchange**.

2. W kategorii **przepływ poczty** e-mail wybierz **pozycję reguły**.

3. Wybierz **+** pozycję , a następnie wybierz pozycję Utwórz **nową regułę**.

4. Aby wyświetlić wszystkie opcje, wybierz pozycję **Więcej opcji** u dołu okna dialogowego.

5. Zastosuj ustawienia z poniższej tabeli. Użyj wartości domyślnych pozostałych ustawień, chyba że chcesz je zmienić.

6. Wybierz **Zapisz**.

|Ustawienie|Ostrzegaj użytkowników przed otwieraniem załączników Office plików|
|---|---|
|Name (Nazwa)|Uniemożliwianie automatycznego przesyłania poczty e-mail do domen zewnętrznych|
|Zastosuj tę regułę, jeśli...|Nadawca . . . jest zewnętrzna/wewnętrzna. . . Wewnątrz organizacji|
|Dodaj warunek|Właściwości wiadomości. . . uwzględnij typ wiadomości . . . Automatyczne przesyłanie dalej|
|Wykonaj następujące czynności...|Zablokuj wiadomość. . . odrzuć wiadomość i dołącz wyjaśnienie.|
|Podaj tekst wiadomości|Automatyczne przesyłanie dalej poczty e-mail poza tę organizację jest blokowane ze względów bezpieczeństwa.|


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrona poczty e-mail przed atakami wyłudzających informacje

Jeśli skonfigurowano co najmniej jedną domenę niestandardową dla środowiska Office 365 lub Microsoft 365, możesz skonfigurować ukierunkowaną ochronę przed wyłudzaniem informacji. Ochrona przed wyłudzaniem informacji, która jest częścią usługi Microsoft Defender for Office 365, może pomóc chronić Twoją organizację przed atakami wyłudzania informacji opartymi na złośliwej personifikacji i przed innymi atakami wyłudzania informacji. Jeśli nie skonfigurowano domeny niestandardowej, nie musisz tego robić.

Zalecamy wprowadzenie do tej ochrony przez utworzenie zasad chroniących najważniejszych użytkowników i domenę niestandardową.

Aby utworzyć zasady ochrony przed wyłudzaniem informacji [](../business-video/setup-anti-phishing.md)w programie Microsoft Defender dla systemu Office 365, obejrzyj ten krótki szkoleniowy klip wideo lub wykonaj następujące czynności:

1. Przejdź do witryny [https://protection.office.com](https://protection.office.com).

2. W Centrum &amp; zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie **zagrożeniami** wybierz pozycję **Zasady**.

3. Na stronie **Zasady** wybierz pozycję Ochrona **przed wyłudzaniem informacji**.

4. Na stronie **ochrony przed wyłudzaniem** informacji wybierz pozycję **+ Utwórz.** Kreator przeprowadzi Cię przez proces definiowania zasad ochrony przed wyłudzaniem informacji.

5. Określ nazwę, opis i ustawienia zasad zgodnie z zaleceniami w poniższej tabeli. Aby uzyskać więcej szczegółowych informacji, zobacz Informacje o zasadach ochrony przed wyłudzaniem informacji w [programie Microsoft Defender, aby Office 365 opcje.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Po przejrzeniu ustawień wybierz pozycję Utwórz **te zasady** lub **Zapisz** odpowiednio do potrzeb.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Domena i najcenniejszy personel kampanii|
|Opis|Upewnij się, że nie podszywają się najważniejsze pracownicy i nasza domena.|
|Dodawanie użytkowników w celu ochrony|Wybierz **pozycję + Dodaj warunek, adresatem jest**. Wpisz nazwy użytkowników lub wprowadź adres e-mail kandydata, menedżera kampanii i innych ważnych członków personelu. Możesz dodać maksymalnie 20 wewnętrznych i zewnętrznych adresów, które chcesz chronić przed personifikacji.|
|Dodawanie domen w celu ochrony|Wybierz **pozycję + Dodaj warunek, domena adresata to**. Wprowadź domenę niestandardową skojarzoną Microsoft 365 subskrypcji usługi( jeśli zdefiniowano subskrypcję). Możesz wprowadzić więcej niż jedną domenę.|
|Wybieranie akcji|Jeśli wiadomość e-mail zostanie wysłana przez spersonifikowanego użytkownika: Wybierz pozycję Przekieruj wiadomość na inny adres e-mail **,** a następnie wpisz adres e-mail administratora zabezpieczeń. na przykład *Alice <span> <span> @contoso.com*. Jeśli wiadomość e-mail jest wysyłana przez spersonifikowane domeny: Wybierz **pozycję Kwarantanna wiadomości**.|
|Inteligencja skrzynek pocztowych|Domyślnie podczas tworzenia nowych zasad ochrony przed wyłudzaniem informacji jest zaznaczona inteligencja skrzynek pocztowych. Aby uzyskać najlepsze **wyniki, pozostaw** to ustawienie wł.|
|Dodawanie zaufanych nadawców i domen|Tutaj możesz dodać własną domenę lub dowolne inne zaufane domeny.|
|Zastosowano do|Wybierz **pozycję Domena adresata to**. W **obszarze Dowolny z tych** wybierz pozycję **Wybierz**. Wybierz **pozycję + Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso. <span> <span> com*, na liście, a następnie wybierz pozycję **Dodaj**. Wybierz **pozycję Gotowe**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Ochrona przed złośliwymi załącznikami i plikami za pomocą Sejf załączników

Osoby regularnie wysyłają, odbierają i udostępniają załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i inne. Samo patrząc na wiadomość e-mail, nie zawsze łatwo jest ustalić, czy załącznik jest bezpieczny, czy złośliwy. Program Microsoft Defender dla Office 365 zawiera Sejf ochronę załączników, ale ta ochrona nie jest domyślnie włączona. Zalecamy utworzenie nowej reguły w celu rozpoczęcia korzystania z tej ochrony. Ta ochrona obejmuje pliki w SharePoint, OneDrive i Microsoft Teams.

Aby utworzyć zasady Sejf załączników, obejrzyj [ten krótki](../business-video/safe-attachments.md)klip wideo lub wykonaj następujące czynności:

1. Przejdź do [https://protection.office.com](https://protection.office.com) pozycji , a następnie zaloguj się przy użyciu konta administratora.

2. W Centrum &amp; zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie **zagrożeniami** wybierz pozycję **Zasady**.

3. Na stronie Zasady wybierz pozycję Sejf **załączników.**

4. Na stronie Sejf załączników zastosuj tę ochronę ogólnie, zaznaczając pole wyboru Włącz **atP SharePoint,** OneDrive i Microsoft Teams atp.

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

Aby uzyskać więcej informacji, zobacz Konfigurowanie zasad ochrony przed wyłudzaniem [informacji w programie Microsoft Defender dla Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Ochrona przed atakami wyłudzających informacje za pomocą Sejf informacji

Hakerzy czasami ukrywają złośliwe witryny internetowe w linkach w wiadomościach e-mail lub innych plikach. Sejf Linki, część usługi Microsoft Defender dla systemu Office 365, mogą pomóc chronić Twoją organizację, udostępniając weryfikację adresów internetowych (adresów URL) za pomocą kliknięcia w wiadomościach e-mail i Office dokumentach. Ochrona jest definiowana za pomocą Sejf linków sieciowych.

Zalecamy:

- Zmodyfikuj zasady domyślne, aby zwiększyć ochronę.

- Dodaj nowe zasady kierowane do wszystkich adresatów w domenie.

Aby skonfigurować linki Sejf, obejrzyj [ten krótki szkoleniowy](../business-video/safe-links.md)klip wideo lub wykonaj następujące czynności:

1. Przejdź do [https://protection.office.com](https://protection.office.com) pozycji , a następnie zaloguj się przy użyciu konta administratora.

2. W Centrum &amp; zgodności zabezpieczeń w lewym okienku nawigacji w obszarze Zarządzanie **zagrożeniami** wybierz pozycję **Zasady**.

3. Na stronie Zasady wybierz pozycję **Sejf sieci Web.**

Aby zmodyfikować zasady domyślne:

1. Na stronie Sejf w obszarze **Zasady** stosowane do całej organizacji wybierz pozycję **Zasady** domyślne.

2. W **Ustawienia, które dotyczą zawartości** z wyjątkiem wiadomości e-mail, wybierz pozycję Aplikacje Microsoft 365 dla przedsiębiorstw, Office dla systemów **iOS i Android.**

3. Wybierz **Zapisz**.

Aby utworzyć nowe zasady kierowane do wszystkich adresatów w domenie:

1. Na stronie Sejf w obszarze **Zasady** stosowane do całej organizacji wybierz pozycję , **+** aby utworzyć nowe zasady.

2. Zastosuj ustawienia wymienione w poniższej tabeli.

3. Wybierz **Zapisz**.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Sejf łączy zasad dla wszystkich adresatów w domenie|
|Wybierz akcję dla nieznanych, potencjalnie złośliwych adresów URL w wiadomościach|Wybierz **pozycję W — po kliknięciu linku** przez użytkownika adresy URL zostaną ponownie napisane i zaewidencjonowane pod kątem listy znanych złośliwych linków.|
|Używanie załączników Sejf do skanowania zawartości do pobrania|Zaznacz to pole.|
|Zastosowano do|Domeną adresata jest . . . wybierz domenę.|

Aby uzyskać więcej informacji, [zobacz Sejf linki](../security/office-365-security/safe-links.md).

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/)

2. Wybierz **pozycję Wszystkie usługi** i wpisz *intune* w polu **wyszukiwania**.

3. Po wyświetlonej liście wyników wybierz  początek obok Microsoft Intune, aby dodać go do ulubionych i ułatwić jego późniejsze znalezienie.

Oprócz centrum administracyjnego do rejestrowania urządzeń organizacji i zarządzania nimi możesz użyć usługi Intune. Aby uzyskać więcej informacji, zobacz Funkcje według [metody rejestracji Windows urządzeń](/intune/enrollment/enrollment-method-capab) i Opcje rejestracji dla urządzeń [zarządzanych przez usługę Intune.](/intune/enrollment-options)
