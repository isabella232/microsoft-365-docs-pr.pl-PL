---
title: Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS
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
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Dowiedz się, jak tworzyć, edytować lub usuwać zasady zarządzania aplikacjami oraz chronić pliki służbowe na urządzeniach z systemem Android lub iOS.
ms.openlocfilehash: f4366230805c50fe82183431e3bd2bdfa9fddd68
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42068657"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS

![Baner, który https://aka.ms/aboutM365previewwskazuje na .](../media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Tworzenie zasad zarządzania aplikacjami

1. Przejdź do centrum <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administracyjnego pod adresem . 
    
2. W lewej nav wybierz pozycję **Dodaj** **zasady** \> **urządzeń** \> .
  
3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
    
4. W obszarze **Typ zasad**wybierz pozycję **Zarządzanie aplikacjami dla systemu Android** lub Zarządzanie **aplikacjami dla systemu iOS**, w zależności od zestawu zasad, które chcesz utworzyć. 
    
5. Rozwiń **Chroń pliki służbowe, gdy urządzenia zostaną utracone lub skradzione,** a **zarządzanie dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych**. Skonfiguruj ustawienia, jak chcesz. **Domyślnie można zarządzać tym, jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych,** **ale** zaleca się **włączenie** i zaakceptowanie wartości domyślnych. Aby uzyskać więcej informacji, zobacz [Dostępne ustawienia](#available-settings). 
    
    Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** Jeśli nie chcesz używać domyślnej grupy zabezpieczeń **Wszyscy użytkownicy,** wybierz **pozycję Zmień** \> , wybierz grupy zabezpieczeń, które otrzymują te ustawienia **Wybierz**.
    
7. Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach. 
    
## <a name="edit-an-app-management-policy"></a>Edytowanie zasad zarządzania aplikacjami

1. Na karcie **Zasady** wybierz pozycję **Edytowanie zasad**.
    
2. W okienku **Edytowanie zasad** wybierz zasadę, którą chcesz zmienić. 
    
3. Wybierz opcję **Edytuj** obok poszczególnych ustawień, aby zmienić wartości zasad. Po zmianie wartości jest ona automatycznie zapisywana w zasadach.
    
4. Po zakończeniu zamknij okienko **zasad Edytowanie.** 
    
## <a name="delete-an-app-management-policy"></a>Usuwanie zasad zarządzania aplikacjami

1. Na stronie **Zasady** wybierz zasadę, a następnie **usuń**.
    
2. W okienku **zasad Usuwanie** wybierz pozycję **Potwierdź,** aby usunąć wybrane zasady lub zasady. 
    
## <a name="available-settings"></a>Dostępne ustawienia

Poniższe tabele udostępniają szczegółowe informacje o dostępnych ustawieniach w celu ochrony plików służbowych na urządzeniach oraz ustawienia, które kontrolują sposób, w jaki użytkownicy uzyskują dostęp do plików pakietu Office ze swoich urządzeń przenośnych.
  
 Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Ustawienia chroniące pliki służbowe

W przypadku zgubienia lub kradzieży urządzenia użytkownika dostępne są następujące ustawienia chroniące pliki służbowe:
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Usuń pliki służbowe z nieaktywnego urządzenia po określonej liczbie dni  <br/> |Jeśli urządzenie nie jest używane przez określoną tutaj liczbę dni, wszystkie pliki robocze przechowywane na urządzeniu zostaną automatycznie usunięte.  <br/> |
|Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm  <br/> |Jeśli to ustawienie jest **włączone,** jedyną dostępną lokalizacją zapisu dla plików służbowych jest OneDrive dla Firm.  <br/> |
|Szyfruj pliki służbowe  <br/> |Zachowaj to ustawienie **Włączone**, aby chronić pliki służbowe przy użyciu szyfrowania. Nawet jeśli urządzenie zostanie zgubione lub skradzione, nikt nie może odczytać danych twojej firmy.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Ustawienia, które sterują dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych

Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office  <br/> |Jeśli to ustawienie jest **Włączone** użytkownicy muszą podać inną formę uwierzytelniania, oprócz nazwy użytkownika i hasła, zanim będą mogli korzystać z aplikacji pakietu Office na swoich urządzeniach przenośnych.<br/> |
|Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania  <br/> |Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.  <br/> |
|Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office  <br/> |To ustawienie określa, jak długo użytkownik może być bezczynny, zanim zostanie poproszony o ponowne zalogowanie się.  <br/> |
|Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta  <br/> |Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta. Umożliwia to użytkownikowi modyfikowanie systemu operacyjnego, co może uczynić urządzenie bardziej podatnym na złośliwe oprogramowanie. Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.  <br/> |
|Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych  <br/> |Domyślnie jest to dozwolone, ale gdy to ustawienie jest **włączone**, użytkownik może kopiować informacje z pliku służbowego do osobistego. Jeśli to ustawienie jest **wyłączone**, użytkownik nie będzie mógł kopiować informacji z konta służbowego do aplikacji osobistej ani na konto osobiste.  <br/> |
