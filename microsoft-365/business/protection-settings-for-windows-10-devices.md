---
title: Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Dowiedz się, jak utworzyć zasady aplikacji zarządzania i ochrony plików praca na urządzeniach Windows 10.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982827"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10

## <a name="create-an-app-management-policy-for-windows-10"></a>Tworzenie zasad zarządzania aplikacjami dla systemu Windows 10

Jeśli użytkownicy mają urządzenia osobiste z systemem Windows 10, na których wykonują zadania służbowe, możesz również chronić dane na tych urządzeniach.
  
1. Zaloguj się do usługi [Microsoft 365 Business](https://portal.office.com) za pomocą poświadczeń administratora globalnego. Wybierz kafelek **Administrator**, aby przejść do centrum administracyjnego. 
    
2. Na karcie **Zasady dotyczące urządzenia** portalu administracyjnego wybierz pozycję **Dodaj zasady**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
    
4. W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Windows 10**.
    
5. W obszarze ** typu urządzenia **, wybierz **osobiste** lub **Właścicielem firmy**.
    
6. Opcja **Szyfruj pliki służbowe** zostanie włączona automatycznie. 
    
7. Jeśli nie chcesz, aby użytkownicy mogli zapisywać pliki służbowe na swoich komputerach, **włącz** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm**. 
    
8. Rozwiń **Zarządzanie dostęp użytkowników do plików pakietu Office na urządzeniach** \> skonfigurować ustawienia jak. **Zarządzanie dostęp użytkowników do urządzeń biurowych na urządzeniach przenośnych** jest domyślnie **wyłączone** , ale zaleca się **ją włączyć** , a następnie zaakceptuj wartości domyślne. Aby uzyskać więcej informacji, zobacz temat [dostępne ustawienia](protection-settings-for-windows-10-devices.md#bkmk_settings) . 
    
    Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**. 
    
9. Rozwiń sekcję **Odzyskiwanie danych na urządzeniach z systemem Windows** i **włącz** tę opcję (jest to zalecane).
    
    Aby móc przejść do lokalizacji certyfikatu agenta odzyskiwania danych, musisz najpierw go utworzyć. Odpowiednie instrukcje znajdziesz w artykule na temat [tworzenia i weryfikowania certyfikatu agenta odzyskiwania danych systemu szyfrowania plików](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Domyślnie pliki robocze są szyfrowane przy użyciu klucza tajnego, który jest przechowywany na urządzeniu i skojarzony z profilem użytkownika. Tylko użytkownik może otwierać i odszyfrowywać plik. Jednak w razie utraty urządzenia lub usunięcia użytkownika plik może utknąć w stanie zaszyfrowania. Administrator może użyć certyfikatu agenta odzyskiwania danych (DRA) do odszyfrowania pliku.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Rozwiń sekcję **Chroń dodatkowe lokalizacje sieciowe i w chmurze**, jeśli chcesz dodać więcej domen lub lokalizacji usługi SharePoint Online. W ten sposób możesz się upewnić, że pliki we wszystkich wymienionych aplikacjach będą chronione. Poszczególne pozycje wprowadzane w polach oddzielaj średnikami. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Następnie zdecydować **kto otrzyma te ustawienia?** Jeśli nie chcesz używać domyślnej grupy zabezpieczeń **Wszyscy użytkownicy** , **Zmień**, wybierz polecenie grupy zabezpieczeń, którzy otrzymają te ustawienia \> **Wybierz**.
    
12. Na koniec wybierz przycisk **Dodaj**, aby zapisać zasady i zastosować je na urządzeniach. 
    
## <a name="available-settings"></a>Dostępne ustawienia

Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia.
  
Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md).
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office  <br/> |Gdy to ustawienie jest **włączone**, użytkownicy muszą się dodatkowo uwierzytelnić, korzystając z innej metody (oprócz podania nazwy użytkownika i hasła), aby uzyskać dostęp do aplikacji pakietu Office na urządzeniach przenośnych.  <br/> |
|Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania  <br/> |Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.  <br/> |
|Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office  <br/> |To ustawienie określa, jak długo użytkownik może nie korzystać z aplikacji, zanim będzie wymagane ponowne zalogowanie się.  <br/> |
   

