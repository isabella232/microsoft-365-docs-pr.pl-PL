---
title: Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Dowiedz się, jak tworzyć, edytować, lub usuwanie aplikacji zasad zarządzania i ochrony plików praca na urządzeniach Android lub iOS.
ms.openlocfilehash: 04479360bf13a8ff685a91ed95440c08f8cf80b4
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660580"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS

![Transparent odsyłających do https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Tworzenie zasad zarządzania aplikacjami

1. Przejdź do Centrum administracyjnego o <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. W nawigacji z lewej strony wybierz **urządzenia** \> **zasady** \> **Dodaj**.
  
3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
    
4. W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Android** lub **Zarządzanie aplikacjami dla systemu iOS** w zależności od tego, jaki zestaw zasad chcesz utworzyć. 
    
5. Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. Aby uzyskać więcej informacji, zobacz temat [dostępne ustawienia](#available-settings) . 
    
    Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
7. Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach. 
    
## <a name="edit-an-app-management-policy"></a>Edytowanie zasad zarządzania aplikacjami

1. Na karcie **zasady** wybierz polecenie **Edytuj zasady**.
    
2. W okienku **Edytowanie zasad** wybierz zasadę, którą chcesz zmienić. 
    
3. Wybierz opcję **Edytuj** obok poszczególnych ustawień, aby zmienić wartości zasad. Wszystkie zmiany są zapisywane automatycznie. 
    
4. Gdy skończysz wprowadzać zmiany, zamknij okienko **Edytowanie zasad**. 
    
## <a name="delete-an-app-management-policy"></a>Usuwanie zasad zarządzania aplikacjami

1. Na stronie **zasady** wybierz zasady, a następnie **usunąć**.
    
2. **Usuwanie zasady** w okienku wybierz **Potwierdź** , aby usunąć zasadę lub zasady, które wybrałeś. 
    
## <a name="available-settings"></a>Dostępne ustawienia

W poniższych tabelach szczegółowo opisano dostępne ustawienia umożliwiające ochronę służbowych plików na urządzeniach i kontrolowanie dostępu użytkowników do plików pakietu Office na urządzeniach przenośnych.
  
 Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Ustawienia chroniące pliki służbowe

W przypadku zgubienia lub kradzieży urządzenia użytkownika dostępne są następujące ustawienia chroniące pliki służbowe:
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Usuń pliki służbowe z nieaktywnego urządzenia po określonej liczbie dni  <br/> |Jeśli urządzenie nie będzie używane przez określoną w tym miejscu liczbę dni, wszelkie pliki służbowe znajdujące się na urządzeniu zostaną automatycznie usunięte.  <br/> |
|Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm  <br/> |Gdy to ustawienie jest **Włączone**, jedyną dostępną lokalizacją zapisu plików służbowych jest usługa OneDrive dla Firm.  <br/> |
|Szyfruj pliki służbowe  <br/> |Zachowaj to ustawienie **Włączone**, aby chronić pliki służbowe przy użyciu szyfrowania. Nawet jeśli urządzenie zostanie zgubione lub ukradzione, nikt nie będzie mógł odczytać danych firmowych.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Ustawienia umożliwiające kontrolę dostępu użytkowników do plików pakietu Office na urządzeniach przenośnych

Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office  <br/> |Gdy to ustawienie jest **włączone**, użytkownicy muszą się dodatkowo uwierzytelnić, korzystając z innej metody (oprócz podania nazwy użytkownika i hasła), aby uzyskać dostęp do aplikacji pakietu Office na urządzeniach przenośnych.  <br/> |
|Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania  <br/> |Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.  <br/> |
|Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office  <br/> |To ustawienie określa, jak długo użytkownik może nie korzystać z aplikacji, zanim będzie wymagane ponowne zalogowanie się.  <br/> |
|Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta  <br/> |Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta. Umożliwia to użytkownikowi modyfikowanie systemu operacyjnego, co może uczynić urządzenie bardziej podatnym na złośliwe oprogramowanie. Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.  <br/> |
|Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych  <br/> |Domyślnie jest to dozwolone, ale gdy to ustawienie jest **włączone**, użytkownik może kopiować informacje z pliku służbowego do osobistego. Jeśli to ustawienie jest **wyłączone**, użytkownik nie będzie mógł kopiować informacji z konta służbowego do aplikacji osobistej ani na konto osobiste.  <br/> |
   

  

