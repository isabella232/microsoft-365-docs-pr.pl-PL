---
title: Konfigurowanie ustawień ochrony urządzeń dla komputerów z systemem Windows 10
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Dowiedz się więcej o domyślnych i innych ustawień, które są dostępne w Microsoft Business 365 do zabezpieczenia urządzeń Windows 10.
ms.openlocfilehash: 095aa2c2f32c3e7b5a5a4e560ea4bc7124d7146e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074515"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Konfigurowanie ustawień ochrony urządzeń dla komputerów z systemem Windows 10

## <a name="secure-windows-10-devices"></a>Zabezpieczanie urządzeń z systemem Windows 10

Obejrzyj klip wideo na temat zabezpieczania urządzeń z systemem Windows 10 za pomocą usługi Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. SGo do Centrum administracyjnego o <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. Na nawigacji z lewej strony wybierz **urządzenia** \> **zasady** \> **Dodaj**.
  
3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
    
4. W sekcji **Typ zasad** wybierz opcję **Konfiguracja urządzeń z systemem Windows 10**.
    
5. Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information. 
    
    Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
    
7. Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach. 
    
## <a name="available-settings"></a>Dostępne ustawienia

Domyślnie wszystkie ustawienia są **Włączone**. Dostępne są następujące ustawienia.
  
Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender  <br/> |Wymaga włączenia programu antywirusowego Windows Defender w celu ochrony komputerów przed zagrożeniami związanymi z połączeniem z Internetem.  <br/> |
|Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge  <br/> |Włącza w programie Microsoft Edge ustawienia ułatwiające ochronę użytkowników przed złośliwymi witrynami i złośliwą zawartością do pobrania.  <br/> |
|Użyj reguł, które zmniejszają obszar ataków na urządzenia  <br/> |Gdy zmniejszanie obszaru ataków jest włączone, pomaga blokować akcje i aplikacje zwykle używane przez złośliwe oprogramowanie do infekowania urządzeń. To ustawienie jest dostępne tylko wtedy, gdy jest włączona ochrona antywirusowa programu Windows Defender. Zobacz [Zmniejszanie obszarów ataków](https://go.microsoft.com/fwlink/?linkid=870417), aby dowiedzieć się więcej.  <br/> |
|Chroń foldery przed zagrożeniami, takimi jak oprogramowanie wymuszające okup  <br/> |To ustawienie używa kontrolowanego dostępu do folderów w celu ochrony danych firmy przed modyfikacją przez podejrzane lub złośliwe aplikacje, takie jak oprogramowanie wymuszające okup. Tego typu aplikacje mają zablokowaną możliwość wprowadzania zmian w chronionych folderach. To ustawienie jest dostępne tylko wtedy, gdy jest włączona ochrona antywirusowa programu Windows Defender. Zobacz [Chronienie folderów za pomocą kontrolowanego dostępu do folderów](https://go.microsoft.com/fwlink/?linkid=870418), aby dowiedzieć się więcej.  <br/> |
|Blokuj dostęp sieciowy do potencjalnie złośliwej zawartości w Internecie  <br/> |To ustawienie umożliwia blokowanie połączeń wychodzących użytkownika do lokalizacji internetowych o niskiej reputacji, które mogą wiązać się z wyłudzaniem informacji, oszustwami i złośliwą zawartością. To ustawienie jest dostępne tylko wtedy, gdy jest włączona ochrona antywirusowa programu Windows Defender. Zobacz [Chronienie sieci](https://go.microsoft.com/fwlink/?linkid=870419), aby uzyskać więcej informacji.  <br/> |
|Pomóż chronić pliki i foldery na komputerach przed nieautoryzowanym dostępem za pomocą funkcji BitLocker  <br/> |Funkcja BitLocker chroni dane przez zaszyfrowanie dysków twardych komputera i zapewnianie ochrony przed ujawnieniem danych w razie zagubienia lub kradzieży komputera. Zobacz [Często zadawane pytania dotyczące funkcji BitLocker](https://go.microsoft.com/fwlink/?linkid=871000), aby uzyskać więcej informacji.  <br/> |
|Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store  <br/> |Pozwala użytkownikom pobierać i instalować aplikacje z witryny Microsoft Store. Do aplikacji tych należą zarówno gry, jak i narzędzia biurowe, więc zostawiamy to ustawienie **włączone**, ale możesz je wyłączyć w celu dodatkowego zwiększenia bezpieczeństwa.  <br/> |
|Zezwalaj użytkownikom na korzystanie z Cortany  <br/> |Cortana może być bardzo pomocna. Może włączać lub wyłączać ustawienia, udzielać wskazówek i przypominać o spotkaniach, więc to ustawienie domyślnie jest **włączone**.  <br/> |
|Zezwalaj użytkownikom na otrzymywanie porad i reklam dotyczących systemu Windows od firmy Microsoft  <br/> |Porady dotyczące systemu Windows mogą być przydatne i ułatwiać użytkownikom zapoznawanie się nowymi funkcjami.  <br/> |
|Automatycznie aktualizuj urządzenia z systemem Windows 10  <br/> |Zapewnia, że urządzenia z systemem Windows 10 automatycznie otrzymują najnowsze aktualizacje.  <br/> |
|Wyłącz ekran urządzenia po takim czasie bezczynności  <br/> |Zapewnia bezpieczeństwo danych firmowych podczas bezczynności użytkownika. Jeśli użytkownik pracuje w miejscu publicznym, na przykład kawiarni, i odejdzie na chwilę od urządzenia lub skupi uwagę na czymś innym, przypadkowe osoby mogą obejrzeć zawartość ekranu. To ustawienie pozwala kontrolować czas bezczynności użytkownika, po którym ekran zostanie wyłączony.  <br/> |
   
  

