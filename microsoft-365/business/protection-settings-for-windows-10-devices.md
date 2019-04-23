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
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Dowiedz się, jak utworzyć zasady aplikacji zarządzania i ochrony plików praca na urządzeniach Windows 10.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278191"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10

## <a name="create-an-app-management-policy-for-windows-10"></a>Tworzenie zasad zarządzania aplikacjami dla systemu Windows 10

Jeśli użytkownicy mają urządzenia osobiste z systemem Windows 10, na których wykonują zadania służbowe, możesz również chronić dane na tych urządzeniach.
  
1. Zaloguj się do [Centrum administracyjnego](https://go.microsoft.com/fwlink/p/?linkid=837890) z poświadczeniami administratora globalnego. Wybierz kafelek **Administrator**, aby przejść do centrum administracyjnego. 
    
2. Na nawigacji z lewej strony wybierz **urządzenia** \> **zasady** \> **Dodaj**.

3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
    
4. W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Windows 10**.
    
5. Under ** Device type **, choose either **Personal** or **Company Owned**.
    
6. Opcja **Szyfruj pliki służbowe** zostanie włączona automatycznie. 
    
7. Jeśli nie chcesz, aby użytkownicy mogli zapisywać pliki służbowe na swoich komputerach, **włącz** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm**. 
    
8. Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. Aby uzyskać więcej informacji, zobacz temat [dostępne ustawienia](#available-settings). 
    
    Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**. 
    
9. Rozwiń sekcję **Odzyskiwanie danych na urządzeniach z systemem Windows** i **włącz** tę opcję (jest to zalecane).
    
    Aby móc przejść do lokalizacji certyfikatu agenta odzyskiwania danych, musisz najpierw go utworzyć. Odpowiednie instrukcje znajdziesz w artykule na temat [tworzenia i weryfikowania certyfikatu agenta odzyskiwania danych systemu szyfrowania plików](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Domyślnie pliki robocze są szyfrowane przy użyciu klucza tajnego, który jest przechowywany na urządzeniu i skojarzony z profilem użytkownika. Tylko użytkownik może otwierać i odszyfrowywać plik. Jednak w razie utraty urządzenia lub usunięcia użytkownika plik może utknąć w stanie zaszyfrowania. Administrator może użyć certyfikatu agenta odzyskiwania danych (DRA) do odszyfrowania pliku.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Rozwiń sekcję **Chroń dodatkowe lokalizacje sieciowe i w chmurze**, jeśli chcesz dodać więcej domen lub lokalizacji usługi SharePoint Online. W ten sposób możesz się upewnić, że pliki we wszystkich wymienionych aplikacjach będą chronione. Poszczególne pozycje wprowadzane w polach oddzielaj średnikami. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
12. Na koniec wybierz przycisk **Dodaj**, aby zapisać zasady i zastosować je na urządzeniach. 
    
## <a name="available-settings"></a>Dostępne ustawienia

Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia.
  
Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md).
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office  <br/> |Gdy to ustawienie jest **włączone**, użytkownicy muszą się dodatkowo uwierzytelnić, korzystając z innej metody (oprócz podania nazwy użytkownika i hasła), aby uzyskać dostęp do aplikacji pakietu Office na urządzeniach przenośnych.  <br/> |
|Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania  <br/> |Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.  <br/> |
|Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office  <br/> |To ustawienie określa, jak długo użytkownik może nie korzystać z aplikacji, zanim będzie wymagane ponowne zalogowanie się.  <br/> |
   

