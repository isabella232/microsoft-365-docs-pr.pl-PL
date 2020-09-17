---
title: Zwiększanie ochrony przed zagrożeniami dla programu Microsoft 365 dla firm
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
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami pakietu Office 365 i Zabezpiecz ważne dane przed phishingiem, złośliwym oprogramowaniem i innymi zagrożeniami.
ms.openlocfilehash: d56a5371bc5fc4da22f4625024769cc0325a25ca
ms.sourcegitcommit: dffb9b72acd2e0bd286ff7e79c251e7ec6e8ecae
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/17/2020
ms.locfileid: "47948593"
---
# <a name="increase-threat-protection"></a>Zwiększanie ochrony przed zagrożeniami

Ten artykuł ułatwia zwiększenie ochrony subskrypcji programu Microsoft 365 w celu ochrony przed phishingiem, złośliwym oprogramowaniem i innymi zagrożeniami. Te rekomendacje są odpowiednie dla organizacji z zwiększonym zapotrzebowaniem na bezpieczeństwo, takich jak biura praw i kliniki medyczne.

Przed rozpoczęciem Sprawdź, czy pakiet Office 365 ma zabezpieczoną ocenę. Dodatek Office 365 Security Score analizuje zabezpieczenia organizacji na podstawie regularnych działań i ustawień zabezpieczeń oraz przypisuje wynik. Zacznij od wzięcia pod uwagę bieżącego wyniku. Aby zwiększyć wynik, wykonaj czynności zalecane w tym artykule. Celem nie jest osiągnięcie maksymalnego wyniku, ale uwzględnienie możliwości ochrony środowiska, które nie wpływają negatywnie na wydajność użytkowników.

Aby uzyskać więcej informacji, zobacz [bezpieczny wynik firmy Microsoft](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Podnoszenie poziomu ochrony przed złośliwym oprogramowaniem w aplikacji Poczta

Środowisko pakietu Office 365 lub Microsoft 365 obejmuje ochronę przed złośliwym oprogramowaniem. Ochronę można zwiększyć, blokując załączniki za pomocą typów plików, które są często używane w przypadku złośliwego oprogramowania. Aby zwiększyć ochronę przed złośliwym oprogramowaniem w wiadomości e-mail:

1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu poświadczeń konta administratora.

2. W &amp; Centrum zgodności zabezpieczeń w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **zasady** chroniące \> **przed złośliwym oprogramowaniem**.

3. Kliknij dwukrotnie zasadę domyślną, aby edytować te zasady dotyczące całej firmy.

4. Wybierz pozycję **Ustawienia**.

5. W obszarze **typowe filtry typów załączników**wybierz pozycję **włączone**. Zablokowane typy plików są wyświetlane w oknie bezpośrednio pod tą kontrolką. Upewnij się, że dodajesz następujące typy plików:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   W razie potrzeby możesz później dodać lub usunąć typy plików.

6. Wybierz pozycję **Zapisz.**

Aby uzyskać więcej informacji, zobacz [Ochrona przed złośliwym oprogramowaniem w EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection).

## <a name="protect-against-ransomware"></a>Ochrona przed działaniem oprogramowania wymuszającego okup

Oprogramowanie wymuszającego okup ogranicza dostęp do danych przez szyfrowanie plików lub blokowanie ekranów komputerowych. Następnie próbuje extort pieniądze od ofiar, pytając o "wymuszającego okup", zazwyczaj w formie cryptocurrencies, na przykład Bitcoin, w programie Exchange w celu uzyskania dostępu do danych.

Aby chronić się przed działaniem oprogramowania wymuszającego okup, Utwórz co najmniej jeden Regulamin przepływu poczty, aby zablokować rozszerzenia plików używane powszechnie na potrzeby oprogramowania wymuszającego okup. (Te reguły zostały dodane w kroku [podnieść poziom ochrony przed złośliwym oprogramowaniem w wiadomości e-mail](#raise-the-level-of-protection-against-malware-in-mail) ). Możesz również ostrzec użytkowników, którzy otrzymają te załączniki w wiadomościach e-mail.

Oprócz plików zablokowanych w poprzednim kroku warto utworzyć regułę ostrzegającą użytkowników przed otwarciem załączników do plików pakietu Office, które zawierają makra. Oprogramowanie wymuszającego okup może być ukryte w makrach, dlatego należy ostrzec użytkowników, że pliki te nie są otwierane przez osoby, które ich nie znają.

Aby utworzyć regułę transportu poczty:

1. Przejdź do centrum administracyjnego w witrynie <https://admin.microsoft.com> , a następnie wybierz pozycję Centrum **administracyjne** \> **programu Exchange**.

2. W kategorii **przepływ poczty** wybierz pozycję **reguły**.

3. Wybierz pozycję **+** , a następnie wybierz pozycję **Utwórz nową regułę**.

4. Wybierz pozycję **więcej opcji** u dołu okna dialogowego, aby wyświetlić pełny zestaw opcji.

5. Zastosuj ustawienia w poniższej tabeli dla reguły. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.

6. Wybierz **Zapisz**.

|Ustawienie|Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office||
|---|---|---|
|Name (Nazwa)|Reguła anty-wymuszającego okup: ostrzeganie użytkowników|
|Zastosuj tę regułę, jeśli. . .|Dowolny załącznik. . . dopasowania rozszerzeń plików. . .|
|Określanie wyrazów lub fraz|Dodaj następujące typy plików:  <br/> dotm, docm, xlsm, sltm, XLA, XLAM, XLL, pptm, potm, PPAM, PPSM, SLDM|
|Wykonaj poniższe czynności. . .|Powiadamianie adresata za pomocą wiadomości|
|Przekazywanie tekstu wiadomości|Nie otwieraj plików tego typu od osób, których nie znasz, ponieważ mogą one zawierać makra ze złośliwym kodem.|

Aby uzyskać więcej informacji, zobacz:

- [Oprogramowanie wymuszającego okup: jak zmniejszyć ryzyko](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Przywracanie usługi OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zatrzymywanie automatycznego przesyłania dalej wiadomości e-mail

Hakerzy, którzy uzyskają dostęp do skrzynki pocztowej użytkownika, mogą ukraść pocztę, ustawiając skrzynkę pocztową na automatyczne przesyłanie dalej wiadomości e-mail. Może się to zdarzyć nawet bez świadomości użytkownika. Aby uniknąć tego problemu, skonfiguruj regułę przepływu poczty.

Aby utworzyć regułę transportu poczty, Obejrzyj [ten krótki klip wideo](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) lub wykonaj następujące czynności:

1. W centrum administracyjnym usługi Microsoft **365 wybierz pozycję Center Center** \> **Exchange**.

2. W kategorii **przepływ poczty** wybierz pozycję **reguły**.

3. Wybierz pozycję **+** , a następnie wybierz pozycję **Utwórz nową regułę**.

4. Aby wyświetlić wszystkie opcje, wybierz pozycję **więcej opcji** u dołu okna dialogowego.

5. Zastosuj ustawienia w poniższej tabeli. Użyj wartości domyślnych dla pozostałych ustawień, chyba że chcesz je zmienić.

6. Wybierz **Zapisz**.

|Ustawienie|Ostrzegaj użytkowników przed otwarciem załączników plików pakietu Office|
|---|---|
|Name (Nazwa)|Zapobieganie automatycznemu przekazywaniu poczty e-mail do domen zewnętrznych|
|Zastosuj tę regułę, jeśli...|Nadawca. . . jest zewnętrznym/wewnętrznym. . . W organizacji|
|Dodaj warunek|Właściwości wiadomości. . . Uwzględnij typ wiadomości. . . Automatyczne przesyłanie dalej|
|Wykonaj następujące czynności...|Zablokowanie wiadomości. . . Odrzuć wiadomość i Dołącz wyjaśnienie.|
|Przekazywanie tekstu wiadomości|Automatyczne przesyłanie dalej wiadomości e-mail spoza tej organizacji jest zabronione ze względów bezpieczeństwa.|


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrona poczty e-mail przed atakami przy użyciu phishingu

Jeśli co najmniej jedna domena niestandardowa jest skonfigurowana dla środowiska pakietu Office 365 lub Microsoft 365, możesz skonfigurować nacelową ochronę przed phishingiem. Ochrona ATP zapewnia ochronę przed phishingiem, część zaawansowanej ochrony przed zagrożeniami pakietu Office 365, ułatwia ochronę organizacji przed złośliwym atakiem wykorzystującym phishing i innymi atakami na phishing. Jeśli nie skonfigurowano domeny niestandardowej, nie trzeba tego robić.

Zalecamy rozpoczęcie korzystania z tej ochrony przez utworzenie zasad chroniących najważniejszych użytkowników i domenę niestandardową.

Aby utworzyć zasady walki z phishingiem, Obejrzyj  [ten krótki szkoleniowy klip wideo](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)lub wykonaj następujące czynności:

1. Przejdź do witryny [https://protection.office.com](https://protection.office.com).

2. W &amp; Centrum zgodności zabezpieczeń w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **zasady**.

3. Na stronie **zasady** wybierz pozycję **ATP — ochrona przed phishingiem**.

4. Na stronie **Ochrona przed phishingiem** wybierz pozycję **+ Utwórz**. Zostanie uruchomiony Kreator, który poprowadzi Cię przez zdefiniowanie zasad ochrony przed phishingiem.

5. W poniższej tabeli Określ nazwę, opis i ustawienia zasad, zgodnie z zaleceniami. Aby uzyskać więcej informacji, zobacz [Informacje o opcjach zasad ochrony przed phishingiem](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

6. Po przejrzeniu ustawień wybierz pozycję **Utwórz te zasady** lub **Zapisz**, zależnie od potrzeb.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Domena i najbardziej cenny personel kampanii|
|Opis|Upewnij się, że najważniejsze osoby i nasze domeny nie są personifikowane.|
|Dodawanie użytkowników do ochrony|Wybierz pozycję **+ Dodaj warunek**. Wpisz nazwy użytkowników lub wprowadź adres e-mail kandydata, menedżera kampanii i innych ważnych członków personelu. Możesz dodać maksymalnie 20 adresów wewnętrznych i zewnętrznych, które chcesz chronić przed personifikacją.|
|Dodawanie domen do ochrony|Wybierz pozycję **+ Dodaj warunek, a domena adresata to**. Wprowadź domenę niestandardową skojarzoną z subskrypcją programu Microsoft 365, jeśli ją zdefiniowano. Możesz wprowadzić więcej niż jeden program Domain.|
|Wybieranie akcji|Jeśli wiadomość e-mail jest wysyłana przez personifikowanego użytkownika: wybierz pozycję **Przekieruj wiadomość na inny adres e-mail**, a następnie wpisz adres e-mail administratora zabezpieczeń. na przykład *alicja <span> <span> @contoso. com*. Jeśli wiadomość e-mail jest wysyłana przez personifikowaną domenę: wybierz pozycję **komunikat kwarantanny**.|
|Analiza skrzynek pocztowych|Podczas tworzenia nowych zasad ochrony przed phishingiem domyślnie jest wybierana analiza skrzynki pocztowej. **Ustawienie to** należy zostawić, aby uzyskać optymalne rezultaty.|
|Dodawanie zaufanych nadawców i domen|W tym miejscu możesz dodać własną domenę lub inne zaufane domeny.|
|Zastosowane do|Wybierz **domenę adresata**. W obszarze **dowolnego z tych**opcji wybierz pozycję **Wybierz**. Wybierz pozycję **+ Dodaj**. Zaznacz pole wyboru obok nazwy domeny, na przykład *contoso. <span> <span> com*, na liście, a następnie wybierz pozycję **Dodaj**. Wybierz pozycję **gotowy**.|

## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrona przed złośliwymi załącznikami i plikami za pomocą bezpiecznych załączników ATP

Osoby regularnie wysyłają, odbierają i udostępniają załączniki, takie jak dokumenty, prezentacje, arkusze kalkulacyjne i nie tylko. Nie zawsze można stwierdzić, czy załącznik jest bezpieczny, czy szkodliwy, przeglądając wiadomość e-mail. Zaawansowana ochrona przed zagrożeniami w pakiecie Office 365 obejmuje ochronę za pomocą bezpiecznych załączników, ale ta ochrona nie jest domyślnie włączona. Zalecamy utworzenie nowej reguły, aby zacząć korzystać z tej ochrony. Ta ochrona rozszerza się na pliki w programach SharePoint, OneDrive i Microsoft Teams.

Aby utworzyć zasady bezpiecznego przyłączeń ATP, Obejrzyj [ten krótki klip wideo](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)lub wykonaj następujące czynności:

1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu konta administratora.

2. W &amp; Centrum zgodności zabezpieczeń w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **zasady**.

3. Na stronie zasady wybierz pozycję **bezpieczne załączniki ATP**.

4. Na stronie bezpieczne załączniki Zastosuj tę ochronę w szerokim zakresie, zaznaczając pole wyboru **Włącz ATP dla programu SharePoint, OneDrive i Microsoft Teams** .

5. Wybierz **+** , aby utworzyć nowe zasady.

6. Zastosuj ustawienia w poniższej tabeli.

7. Po przejrzeniu ustawień wybierz pozycję **Utwórz te zasady** lub **Zapisz**, zależnie od potrzeb.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Blokuj bieżące i przyszłe wiadomości e-mail z wykrytym złośliwym oprogramowaniem.|
|Opis|Blokowanie bieżących i przyszłych wiadomości e-mail oraz załączników z wykrytym złośliwym oprogramowaniem.|
|Zapisywanie załączników nieznana odpowiedź na ataki|Wybierz pozycję **Blokuj — Blokuj bieżące i przyszłe wiadomości e-mail i załączniki z wykrytym złośliwym oprogramowaniem**.|
|Przekierowanie załącznika podczas wykrywania|Włącz przekierowywanie (zaznacz to pole) Wprowadź konto administratora lub konfigurację skrzynki pocztowej na potrzeby kwarantanny.          Zastosuj powyższe zaznaczenie, jeśli trwa skanowanie złośliwego oprogramowania dla załączników lub wystąpił błąd (zaznacz to pole).|
|Zastosowane do|Domena adresata to. . . Wybierz domenę.|

Aby uzyskać więcej informacji, zobacz [Konfigurowanie zasad zapobiegania phishingowi pakietu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrona przed atakami przy użyciu phishingu dzięki bezpiecznym linkom ATP

Hakerzy czasami ukrywają złośliwe witryny sieci Web w łączach w wiadomościach e-mail i innych plikach. Pakiet Office 365 ATP Links Safe (bezpieczne linki ATP), część pakietu Office 365 Advanced Threat Protection, ułatwia ochronę organizacji przez umożliwienie weryfikacji adresów internetowych (adresów URL) w wiadomościach e-mail i dokumentach pakietu Office. Ochrona jest definiowana za pośrednictwem zasad bezpiecznego łącza ATP.

Zalecamy wykonanie następujących czynności:

- Zmodyfikuj zasady domyślne, aby zwiększyć ochronę.

- Dodaj nowe zasady ukierunkowane na wszystkich adresatów w Twojej domenie.

Aby skonfigurować bezpieczne linki ATP, Obejrzyj [ten krótki szkoleniowy klip wideo](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)lub wykonaj następujące czynności:

1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu konta administratora.

2. W &amp; Centrum zgodności zabezpieczeń w lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **zasady**.

3. Na stronie zasady wybierz pozycję **bezpieczne linki ATP**.

Aby zmodyfikować zasadę domyślną:

1. Na stronie bezpieczne łącza w obszarze **zasady dotyczące całej organizacji**wybierz zasadę **domyślną** .

2. W obszarze **Ustawienia dotyczące zawartości z wyjątkiem wiadomości e-mail**wybierz pozycję **Microsoft 365 Apps dla przedsiębiorstw, Office dla systemu iOS i Android**.

3. Wybierz **Zapisz**.

Aby utworzyć nowe zasady ukierunkowane na wszystkich adresatów w Twojej domenie:

1. Na stronie bezpieczne łącza w obszarze **zasady dotyczące całej organizacji**wybierz pozycję, **+** Aby utworzyć nowe zasady.

2. Zastosuj ustawienia wymienione w poniższej tabeli.

3. Wybierz **Zapisz**.

|Ustawienie lub opcja|Zalecane ustawienie|
|---|---|
|Name (Nazwa)|Zasady bezpiecznego łącza dla wszystkich adresatów w domenie|
|Wybieranie akcji dla nieznanych potencjalnie złośliwych adresów URL w wiadomościach|**Po kliknięciu linku wybierz pozycję włączone — adresy URL będą ponownie zapisywane i sprawdzane na liście znanych złośliwych linków**.|
|Używanie bezpiecznych załączników do skanowania zawartości do pobrania|Zaznacz to pole wyboru.|
|Zastosowane do|Domena adresata to. . . Wybierz domenę.|

Aby uzyskać więcej informacji, zobacz [bezpieczne linki usługi ATP (Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)).

## <a name="go-to-intune-admin-center"></a>Przejdź do centrum administracyjnego usługi Intune

1. Zaloguj się do witryny [Azure Portal](https://portal.azure.com/).

2. Wybierz pozycję **wszystkie usługi** i wpisz w *usłudze Intune* w **polu wyszukiwania**.

3. Gdy pojawią się wyniki, wybierz przycisk Rozpocznij obok usługi **Microsoft Intune** , aby ułatwić mu znalezienie go jako ulubionego i łatwiejszego do późniejszego znalezienia.

Oprócz centrum administracyjnego za pomocą usługi Intune można rejestrować urządzenia organizacji i zarządzać nimi. Aby uzyskać więcej informacji, zobacz [funkcje na podstawie metody rejestracji urządzeń z systemem Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) i [opcji rejestracji dla urządzeń zarządzanych przez usługę Intune](https://docs.microsoft.com/intune/enrollment-options).
