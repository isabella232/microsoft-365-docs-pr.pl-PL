---
title: Jak funkcje ochrony w usłudze Microsoft 365 Business Premium mapują ustawienia usługi Intune
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 8/13/2018
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Dowiedz się, jak funkcje ochrony w usłudze Microsoft 365 Business Premium mapują ustawienia usługi Intune. Subskrypcja zapewnia licencję na modyfikowanie ustawień usługi Intune.
ms.openlocfilehash: 572d3364e465067536e8369b49404d3d1de1bb5b
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633248"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Jak funkcje ochrony w usłudze Microsoft 365 Business Premium mapują ustawienia usługi Intune

## <a name="android-and-ios-application-protection-settings"></a>Ustawienia ochrony aplikacji dla systemów Android lub iOS

W poniższej tabeli przedstawiono mapowanie ustawień zasad aplikacji systemów Android i iOS na ustawienia usługi Intune.
  
Aby znaleźć ustawienie usługi Intune, zaloguj się przy użyciu poświadczeń administratora usługi Microsoft 365 Business Premium i przejdź do **centrów administracyjnych**, a następnie **usługi Intune**.
  
 > [!IMPORTANT]
 > 
 > Subskrypcja usługi Microsoft 365 Business Premium daje licencję na modyfikowanie wszystkich ustawień usługi Intune. Aby [rozpocząć, zobacz Wprowadzenie do usługi Intune.](https://docs.microsoft.com/intune/introduction-intune)
  
Wybierz nazwę zasad, &mdash; na przykład zasady &mdash; aplikacji dla systemu Android, a następnie wybierz pozycję **Ustawienia zasad**.
  
W obszarze **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia**
  
|**Ustawienie zasad aplikacji dla systemu Android lub iOS**|**Ustawienia usługi Intune**|
|:-----|:-----|
|Usuń pliki służbowe z nieaktywnego urządzenia po  <br/> |Interwał przebywania w trybie offline (w dniach) przed wyczyszczeniem danych aplikacji  <br/> |
|Wymuszaj na użytkownikach zapisywanie plików służbowych w usłudze OneDrive dla Firm  <br/> Uwaga: dozwolona jest tylko usługa OneDrive dla Firm  <br/> |Wybierz, w których usługach magazynu można zapisywać dane firmowe  <br/> |
|||
   
W obszarze **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych**
  
|**Ustawienie zasad aplikacji dla systemu Android lub iOS**|**Ustawienia usługi Intune**|
|:-----|:-----|
|Usuń pliki służbowe z nieaktywnego urządzenia po  <br/> |Interwał przebywania w trybie offline (w dniach) przed wyczyszczeniem danych aplikacji  <br/> |
|Wymuszaj na użytkownikach zapisywanie plików służbowych w usłudze OneDrive dla Firm  <br/> Uwaga: dozwolona jest tylko usługa OneDrive dla Firm  <br/> |Wybierz, w których usługach magazynu można zapisywać dane firmowe  <br/> |
|Szyfruj pliki służbowe  <br/> |Szyfruj dane aplikacji  <br/> |
|W obszarze **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** <br/> ||
|Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office  <br/> | Wymagaj numeru PIN w celu uzyskania dostępu  <br/>  Spowoduje to również ustawienie:  <br/> **Zezwalaj na prosty numer PIN** na **Tak** <br/> **Długość numeru PIN** na 4  <br/> **Zezwalaj na używanie odcisku palca zamiast numeru PIN** na **Tak** <br/> **Wyłącz numer PIN aplikacji, gdy zarządzany jest numer PIN urządzenia** na **Tak** <br/> |
|Resetowanie kodu PIN, gdy logowanie nie powiedzie się wiele razy (jest to wyłączone, jeśli kod PIN nie jest wymagany)  <br/> |Liczba prób przed zresetowaniem numeru PIN  <br/> |
|Wymagaj od użytkowników ponownego zalogowania się po tym, jak aplikacje pakietu Office zostały bezczynne (jest to wyłączone, jeśli numer PIN nie jest wymagany)  <br/> | Ponownie sprawdź wymagania dostępu po (w minutach)  <br/>  Spowoduje to również ustawienie:  <br/> **Limit czasu**  zostają ustawione minuty  <br/>  Jest to ta sama liczba minut, która jest ustawiana w usłudze Microsoft 365 Business.  <br/> **Okres karencji w trybie offline**  zostaje domyślnie ustawiona wartość 720 minut  <br/> |
|Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta  <br/> |Blokuj uruchamianie aplikacji zarządzanych na urządzeniach ze zdjętymi zabezpieczeniami systemu lub odblokowanym dostępem do konta administratora  <br/> |
|Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych  <br/> | Ograniczanie wycinania, kopiowania i wklejania z innymi aplikacjami  <br/>  Jeśli opcja Microsoft 365 Business Premium jest ustawiona **na Włączone,** te trzy opcje są również ustawione na **Wszystkie aplikacje** w usłudze Intune:  <br/> **Zezwalaj aplikacji na przesyłanie danych do innych aplikacji** <br/> **Zezwalaj aplikacji na odbieranie danych z innych aplikacji** <br/> **Ogranicz wycinanie, kopiowanie i wklejanie w innych aplikacjach** <br/>  Jeśli dla opcji Microsoft 365 Business została ustawiona wartość **Włączone**, to dla wszystkich tych opcji w usłudze Intune zostają ustawione wskazane wartości:  <br/> **Zezwalaj aplikacji na przesyłanie danych do innych aplikacji**  zostaje ustawiona wartość **Aplikacje zarządzane przez zasady** <br/> **Zezwalaj aplikacji na odbieranie danych z innych aplikacji**  zostaje ustawiona wartość **Wszystkie aplikacje** <br/> **Ogranicz wycinanie, kopiowanie i wklejanie w innych aplikacjach**  zostaje ustawiona wartość **Aplikacje zarządzane przez zasady z funkcją wklejania** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Ustawienia ochrony aplikacji dla systemu Windows 10

W poniższej tabeli przedstawiono mapowanie ustawień zasad aplikacji systemu Windows 10 na ustawienia usługi Intune.
  
Aby znaleźć ustawienie usługi Intune, zaloguj się przy użyciu poświadczeń administratora usługi Microsoft 365 Business Premium i przejdź do [witryny Azure portal](https://portal.azure.com). Wybierz **pozycję Więcej usług**i wpisz intune w **filtrze**. Wybierz pozycję **Zasady aplikacji**ochrony aplikacji \> **usługi Intune** .
  
 > [!IMPORTANT]
 >
 >Subskrypcja usługi Microsoft 365 Business Premium daje licencję na modyfikowanie tylko ustawień usługi Intune, które mapują ustawienia dostępne w usłudze Microsoft 365 Business Premium. 
  
Aby eksplorować dostępne ustawienia, wybierz odpowiednią nazwę zasad, a następnie w lewym okienku nawigacji wybierz pozycję **Ogólne, Przydziały,** **Dozwolone aplikacje,** **Zwolnione aplikacje,** **Ustawienia wymagane**lub **Ustawienia zaawansowane.** 
  
|**Ustawienie zasad aplikacji dla systemu Windows 10**|**Ustawienia usługi Intune**|
|:-----|:-----|
|Szyfruj pliki służbowe  <br/> |**Ustawienia zaawansowane** \> **Ochrona danych**: **Odwołaj klucze szyfrowania po wyrejestrowaniu** i **Odwołaj dostęp do chronionych danych po zarejestrowaniu urządzenia w usłudze MDM**  dla obu zasad zostaje ustawiona wartość **Włączone**.  <br/> |
|Uniemożliwia użytkownikom kopiowanie danych firmy do plików osobistych.  <br/> |**Wymagane ustawienia** \> **Tryb funkcji Windows Information Protection**. **Na** mapach Microsoft 365 Business Premium do: **Ukryj overrides**, **Off** w Microsoft 365 Business Premium map do: **Off**.  <br/> |
|Kontrola dostępu do dokumentów pakietu Office  <br/> | Jeśli jest to ustawione **na Włączone** w usłudze Microsoft 365 Business Premium,  <br/> dla zasady **Ustawienia zaawansowane** \> **Dostęp**, **Użyj usługi Windows Hello dla firm jako metody logowania się do systemu Windows** zostaje ustawiona wartość **Włączone** z następującymi ustawieniami dodatkowymi:  <br/> **Ustaw minimalną wymaganą liczbę znaków kodu PIN**  zostaje ustawiona wartość **4**.  <br/> **Skonfiguruj użycie wielkich liter w kodzie PIN usługi Windows Hello dla firm**  zostaje ustawiona wartość **Nie zezwalaj na użycie wielkich liter w kodzie PIN**.  <br/> **Skonfiguruj użycie małych liter w kodzie PIN usługi Windows Hello dla firm**  zostaje ustawiona wartość **Nie zezwalaj na użycie małych liter w kodzie PIN**.  <br/> **Skonfiguruj użycie znaków specjalnych w kodzie PIN usługi Windows Hello dla firm**  zostaje ustawiona wartość **Nie zezwalaj na użycie znaków specjalnych w kodzie PIN**.  <br/> **Określ okres (w dniach), przez który może być używany numer PIN, zanim system wymaga, aby użytkownik mógł zmienić,** jest ustawiony na **0**.  <br/> **Określ liczbę ostatnich numerów PIN skojarzonych z kontem użytkownika, które nie mogą zostać ponownie użyte**  zostaje ustawiona wartość **0**.  <br/> **Liczba dozwolonych niepowodzeń uwierzytelniania, po przekroczeniu której urządzenie zostanie wyczyszczone**  zostaje ustawiona wartość taka sama jak w usłudze Microsoft 365 Business (domyślnie: 5).  <br/> **Maksymalny czas (w minutach) bezczynności urządzenia, po którym urządzenie zostanie zablokowane przy użyciu kodu PIN lub hasła**  zostaje ustawiona wartość taka sama jak w usłudze Microsoft 365 Business.  <br/> |
|Włącz odzyskiwanie chronionych danych  <br/> |**Ustawienia zaawansowane** \> **Ochrona danych**: **Pokaż ikonę ochrony danych przedsiębiorstwa** i **Użyj usługi Azure RMS na potrzeby funkcji WIP**  dla obu zasad zostaje ustawiona wartość **Włączone**.  <br/> |
|Chroń dodatkowe lokalizacje firmowe w chmurze  <br/> |**Ustawienia zaawansowane** \> **Domeny chronione** i **Zasoby w chmurze**  są tu wskazywane domeny i witryny programu SharePoint.  <br/> |
|Pliki używane przez te aplikacje są chronione  <br/> |Listę chronionych aplikacji można znaleźć w obszarze **Dozwolone aplikacje**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Ustawienia ochrony urządzeń dla systemu Windows 10

W poniższej tabeli przedstawiono mapowanie ustawień konfiguracji urządzeń systemu Windows 10 na ustawienia usługi Intune.
  
Aby znaleźć ustawienie Usługi Intune, zaloguj się przy użyciu poświadczeń administratora usługi Microsoft 365 Business Premium i przejdź do [portalu Azure](https://portal.azure.com)portal , a następnie wybierz pozycję **Więcej usług**i wpisz w usłudze Intune w **filtrze**, wybierz pozycję **Profile** **konfiguracji** \> urządzenia **usługi Intune** \> . Then select **Device policy for Windows 10** \> **Properties** \> **Settings**.
  
|**Ustawienie zasad urządzeń dla systemu Windows 10**|**Ustawienia usługi Intune**|
|:-----|:-----|
|Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender  <br/> |Zezwalaj na monitorowanie w czasie rzeczywistym = włączone  <br/> Zezwalaj na ochronę w chmurze = włączone  <br/> Pytaj użytkowników o przesyłane próbki = Wyślij bezpieczne próbki automatycznie (domyślnie bez automatycznego wysyłania identyfikowalnych danych osobowych)  <br/> |
|Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge  <br/> |**SmartScreen** w obszarze **Ustawienia przeglądarki Edge**  zostaje ustawiona wartość **Wymagane**.  <br/> |
|Wyłącz ekran urządzenia po takim czasie (minuty)  <br/> |Maksymalna liczba minut braku aktywności przed zablokowaniem ekranu (minuty)  <br/> |
|Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store  <br/> |Niestandardowe zasady URI  <br/> |
|Zezwalaj użytkownikom na korzystanie z Cortany  <br/> |**Ogólne** \> **Cortana** jest ustawiona na **blokowanie** w usłudze Intune po **ustawieniu wyłączony** w usłudze Microsoft 365 Business Premium.  <br/> |
|Zezwalaj użytkownikom na otrzymywanie porad i reklam dotyczących systemu Windows od firmy Microsoft  <br/> |**Windows spotlight**, wszystkie zablokowane, jeśli jest to ustawione na **wyłączony** w usłudze Microsoft 365 Business Premium.  <br/> |
|Automatycznie aktualizuj urządzenia z systemem Windows 10  <br/> | To ustawienie znajduje się w aktualizacji usługi **usługi Microsoft Intune** \> **— windows 10 Update Rings**wybierz pozycję Aktualizuj zasady dla urządzeń z systemem Windows **10**, a następnie **ustawienia** **właściwości** \> .  <br/>  Gdy ustawienie Usługi Microsoft 365 Business Premium jest ustawione **na Włączone,** zostaną ustawione wszystkie następujące ustawienia:  <br/> **Gałąź usługi** jest ustawiona na **CB** (CBB, gdy jest wyłączona w usłudze Microsoft 365 Business Premium).  <br/> **Aktualizacje produktów firmy Microsoft**  zostaje ustawiona wartość **Zezwalaj**.  <br/> **Sterowniki systemu Windows**  zostaje ustawiona wartość **Zezwalaj**.  <br/> **Zachowanie automatycznych aktualizacji**  zostaje ustawiona wartość **Automatycznie zainstaluj podczas konserwacji** oraz:  <br/> **Początek godzin aktywnego użytkowania**  zostaje ustawiona wartość **6:00**.  <br/> **Koniec godzin aktywnego użytkowania**  zostaje ustawiona wartość **22:00**.  <br/> **Okres odroczenia aktualizacji dotyczących jakości (dni)**  zostaje ustawiona wartość **0**.  <br/> **Okres odroczenia aktualizacji funkcji (dni)**  zostaje ustawiona wartość **0**.  <br/> **Tryb pobierania optymalizacji dostarczania**  zostaje ustawiona wartość **HTTP w połączeniu z komunikacją równorzędną za tym samym translatorem adresów sieciowych**.  <br/> |
|||
   

