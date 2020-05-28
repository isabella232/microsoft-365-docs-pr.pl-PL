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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Dowiedz się, jak tworzyć, edytować lub usuwać zasady zarządzania aplikacjami oraz chronić pliki robocze na urządzeniach z systemem Android lub iOS.
ms.openlocfilehash: 01c50e6660d8d8640a2bff2794ee0ea8a69188c8
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401059"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS

![Banner, który wskazuje na https://aka.ms/aboutM365preview .](../media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Tworzenie zasad zarządzania aplikacjami

1. Przejdź do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. W lewym urządzeniu nawigacyjnym wybierz pozycję **Dodawanie** zasad urządzeń \> **Policies** \> **Add**.
  
3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
    
4. W obszarze **Typ zasad**wybierz pozycję **Zarządzanie aplikacjami dla systemu Android** lub Zarządzanie **aplikacjami dla systemu iOS**, w zależności od tego, który zestaw zasad chcesz utworzyć. 
    
5. Rozwiń **pozycję Chroń pliki robocze, gdy urządzenia zostaną zgubione lub skradzione,** a także **zarządzaj tym, jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych.** Skonfiguruj ustawienia, jak chcesz. **Zarządzanie tym, jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych** jest domyślnie **wyłączone,** ale zalecamy włączenie **go** i zaakceptowanie wartości domyślnych. Aby uzyskać więcej informacji, zobacz [Dostępne ustawienia](#available-settings). 
    
    Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** Jeśli nie chcesz używać domyślnej grupy zabezpieczeń **Wszyscy użytkownicy,** wybierz pozycję **Zmień**, wybierz grupy zabezpieczeń, które otrzymują te ustawienia \> **Wybierz**.
    
7. Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach. 
    
## <a name="edit-an-app-management-policy"></a>Edytowanie zasad zarządzania aplikacjami

1. Na karcie **Zasady** wybierz pozycję **Edytuj zasady**.
    
2. W okienku **Edytowanie zasad** wybierz zasadę, którą chcesz zmienić. 
    
3. Wybierz opcję **Edytuj** obok poszczególnych ustawień, aby zmienić wartości zasad. Po zmianie wartości jest ona automatycznie zapisywana w zasadach.
    
4. Po zakończeniu zamknij okienko **Edytowanie zasad.** 
    
## <a name="delete-an-app-management-policy"></a>Usuwanie zasad zarządzania aplikacjami

1. Na stronie **Zasady** wybierz pozycję zasad, a następnie **pozycję Usuń**.
    
2. W okienku **Usuwanie zasad** wybierz pozycję **Potwierdź,** aby usunąć wybrane zasady lub zasady. 
    
## <a name="available-settings"></a>Dostępne ustawienia

Poniższe tabele zawiera szczegółowe informacje o ustawieniach dostępnych do ochrony plików służbowych na urządzeniach i ustawieniach, które kontrolują sposób uzyskiwania dostępu użytkowników do plików pakietu Office z urządzeń przenośnych.
  
 Aby uzyskać więcej informacji, zobacz [Jak funkcje ochrony w usłudze Microsoft 365 Business Premium są mapowane na ustawienia usługi Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Ustawienia chroniące pliki służbowe

W przypadku zgubienia lub kradzieży urządzenia użytkownika dostępne są następujące ustawienia chroniące pliki służbowe:
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Usuń pliki służbowe z nieaktywnego urządzenia po określonej liczbie dni  <br/> |Jeśli urządzenie nie jest używane przez określoną w tym miejscu liczbę dni, wszystkie pliki robocze przechowywane na urządzeniu zostaną automatycznie usunięte.  <br/> |
|Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm  <br/> |Jeśli to ustawienie to **Włączone,** jedyną dostępną lokalizacją zapisu dla plików służbowych jest usługa OneDrive dla Firm.  <br/> |
|Szyfruj pliki służbowe  <br/> |Zachowaj to ustawienie **Włączone**, aby chronić pliki służbowe przy użyciu szyfrowania. Nawet jeśli urządzenie zostanie zgubione lub skradzione, nikt nie może odczytać danych twojej firmy.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Ustawienia, które sterują dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych

Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:
  
|||
|:-----|:-----|
|Ustawienie  <br/> |Opis  <br/> |
|Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office  <br/> |Jeśli to ustawienie jest **Włączone użytkownicy** muszą podać inną formę uwierzytelniania, oprócz nazwy użytkownika i hasła, zanim będą mogli korzystać z aplikacji pakietu Office na swoich urządzeniach przenośnych.<br/> |
|Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania  <br/> |Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.  <br/> |
|Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office  <br/> |To ustawienie określa, jak długo użytkownik może być bezczynny, zanim zostanie wyświetlony monit o ponowne zalogowanie się.  <br/> |
|Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta  <br/> |Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta. Umożliwia to użytkownikowi modyfikowanie systemu operacyjnego, co może uczynić urządzenie bardziej podatnym na złośliwe oprogramowanie. Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.  <br/> |
|Nie zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych  <br/> |Domyślnie jest to dozwolone, ale gdy to ustawienie jest **włączone**, użytkownik może kopiować informacje z pliku służbowego do osobistego. Jeśli to ustawienie jest **wyłączone**, użytkownik nie będzie mógł kopiować informacji z konta służbowego do aplikacji osobistej ani na konto osobiste.  <br/> |
