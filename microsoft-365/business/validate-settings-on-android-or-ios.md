---
title: Sprawdź poprawność ustawień ochrony aplikacji na urządzeniach Android lub iOS
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
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: d4ed70290b21b40ca9ecd5601954c429a27dc528
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072375"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="10187-103">Sprawdź poprawność ustawień ochrony aplikacji na urządzeniach Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="10187-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="10187-104">Postępuj zgodnie z instrukcjami na kartach, aby sprawdzić poprawność ustawień ochrony aplikacji na urządzeniach Android lub iOS.</span><span class="sxs-lookup"><span data-stu-id="10187-104">Follow the instructions in the tabs to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="androidtab"></a>[<span data-ttu-id="10187-105">Android</span><span class="sxs-lookup"><span data-stu-id="10187-105">Android</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="10187-106">Sprawdzanie, czy na urządzeniach użytkowników działają ustawienia ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="10187-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="10187-107">Gdy [skonfigurujesz aplikacje dla urządzeń z systemem Android](app-protection-settings-for-android-and-ios.md) w celu ochrony aplikacji, możesz wykonać czynności opisane poniżej, aby sprawdzić działanie wybranych ustawień.</span><span class="sxs-lookup"><span data-stu-id="10187-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="10187-108">Najpierw upewnij się, że zasady obejmują aplikację, której działanie chcesz sprawdzić.</span><span class="sxs-lookup"><span data-stu-id="10187-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="10187-109">W [centrum administracyjnym](https://portal.office.com) usługi Microsoft 365 Business wybierz pozycję **Zasady** \> **Edytuj zasady**.</span><span class="sxs-lookup"><span data-stu-id="10187-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="10187-110">Wybierz pozycję **Zasady dotyczące aplikacji dla systemu Android** obok ustawień utworzonych podczas konfiguracji lub innych utworzonych zasad i sprawdź, czy są one zastosowane na przykład do programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="10187-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="10187-112">Sprawdzanie działania ustawienia Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu</span><span class="sxs-lookup"><span data-stu-id="10187-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="10187-113">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="10187-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="10187-115">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usług Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="10187-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="10187-116">Zostanie też wyświetlony monit o wprowadzenie numeru PIN lub użycie odcisku palca.</span><span class="sxs-lookup"><span data-stu-id="10187-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="10187-118">Sprawdzanie działania ustawienia Resetuj numer PIN po określonej liczbie nieudanych prób</span><span class="sxs-lookup"><span data-stu-id="10187-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="10187-119">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Resetuj numer PIN po określonej liczbie nieudanych prób** jest ustawiona na dowolną wartość (domyślnie jest to 5).</span><span class="sxs-lookup"><span data-stu-id="10187-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="10187-120">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usług Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="10187-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="10187-p101">Wprowadź nieprawidłowy numer PIN więcej razy niż zezwalają na to obowiązujące zasady. Pojawi się komunikat z informacją o **Osiągnięto limit prób wprowadzenia numeru PIN** i monit o zresetowanie tego numeru.</span><span class="sxs-lookup"><span data-stu-id="10187-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="10187-p102">Naciśnij pozycję **Resetuj numer PIN**. Zostanie wyświetlony monit o zalogowanie się przy użyciu poświadczeń użytkownika do usług Microsoft 365 Business i ustawienie nowego numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="10187-126">Sprawdzanie działania ustawienia Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="10187-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="10187-127">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="10187-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="10187-129">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook, zaloguj się za pomocą poświadczeń użytkownika do usług Microsoft 365 Business i w razie potrzeby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="10187-130">Otwórz wiadomość e-mail zawierającą załącznik, a następnie naciśnij ikonę strzałki w dół obok informacji o załączniku.</span><span class="sxs-lookup"><span data-stu-id="10187-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="10187-132">U dołu ekranu zostanie wyświetlony komunikat **Nie można zapisać na urządzeniu**.</span><span class="sxs-lookup"><span data-stu-id="10187-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="10187-134">Zapisywanie w usłudze OneDrive dla Firm nie jest obecnie włączone dla systemu Android, więc jest tylko wyświetlana informacja o zablokowanej możliwości zapisywania lokalnie.</span><span class="sxs-lookup"><span data-stu-id="10187-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="10187-135">Sprawdzanie działania ustawienia Wymagaj ponownego logowania użytkownika po określonym czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="10187-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="10187-136">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office** ma ustawioną dowolną wartość (domyślnie jest to 30 minut).</span><span class="sxs-lookup"><span data-stu-id="10187-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="10187-137">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook, zaloguj się za pomocą poświadczeń użytkownika do usług Microsoft 365 Business i w razie potrzeby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="10187-p103">Powinna zostać wyświetlona skrzynka odbiorcza aplikacji Outlook. Nie dotykaj urządzenia z systemem Android przez co najmniej 30 minut (lub inny czas dłuższy niż wartość określona w zasadach). Ekran urządzenia prawdopodobnie zostanie wygaszony.</span><span class="sxs-lookup"><span data-stu-id="10187-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="10187-141">Ponownie otwórz aplikację Outlook na urządzeniu z systemem Android.</span><span class="sxs-lookup"><span data-stu-id="10187-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="10187-142">Przed ponownym uzyskaniem dostępu do aplikacji Outlook pojawi się monit o wprowadzenie numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="10187-143">Sprawdzanie działania ustawienia Chroń pliki służbowe przy użyciu szyfrowania</span><span class="sxs-lookup"><span data-stu-id="10187-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="10187-144">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Chroń pliki służbowe przy użyciu szyfrowania** jest **włączona**, a funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **wyłączona**.</span><span class="sxs-lookup"><span data-stu-id="10187-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="10187-145">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook, zaloguj się za pomocą poświadczeń użytkownika do usług Microsoft 365 Business i w razie potrzeby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="10187-146">Otwórz wiadomość e-mail z załączonymi kilkoma plikami obrazu.</span><span class="sxs-lookup"><span data-stu-id="10187-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="10187-147">Naciśnij ikonę strzałki w dół obok informacji o załączniku, aby go zapisać.</span><span class="sxs-lookup"><span data-stu-id="10187-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="10187-p104">Może pojawić się monit o zezwolenie programowi Outlook na dostęp do zdjęć, multimediów i plików na urządzeniu. Naciśnij pozycję **Zezwalaj**.</span><span class="sxs-lookup"><span data-stu-id="10187-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="10187-151">U dołu ekranu wybierz pozycję **Zapisz na urządzeniu**, a następnie otwórz aplikację **Galeria**.</span><span class="sxs-lookup"><span data-stu-id="10187-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="10187-p105">Na liście powinno zostać wyświetlone zaszyfrowane zdjęcie (lub kilka zdjęć, jeśli zapisano ich więcej). Może ono być wyświetlane na liście obrazów w postaci szarego kwadratu z białym wykrzyknikiem w białym okręgu w środku szarego kwadratu.</span><span class="sxs-lookup"><span data-stu-id="10187-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[<span data-ttu-id="10187-155">iOS</span><span class="sxs-lookup"><span data-stu-id="10187-155">iOS</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="10187-156">Sprawdzanie, czy na urządzeniach użytkowników działają ustawienia ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="10187-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="10187-157">Gdy [skonfigurujesz aplikacje dla urządzeń z systemem iOS](app-protection-settings-for-android-and-ios.md) w celu ochrony aplikacji, możesz wykonać czynności opisane poniżej, aby sprawdzić działanie wybranych ustawień.</span><span class="sxs-lookup"><span data-stu-id="10187-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="10187-158">Najpierw upewnij się, że zasady obejmują aplikację, której działanie chcesz sprawdzić.</span><span class="sxs-lookup"><span data-stu-id="10187-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="10187-159">W [centrum administracyjnym](https://portal.office.com) usługi Microsoft 365 Business wybierz pozycję **Zasady** \> **Edytuj zasady**.</span><span class="sxs-lookup"><span data-stu-id="10187-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="10187-160">Wybierz pozycję **Zasady aplikacji dla systemu iOS** obok ustawień utworzonych podczas konfiguracji lub innych utworzonych zasad i sprawdź, czy są one wymuszane na przykład w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="10187-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="10187-162">Sprawdzanie działania ustawienia Wymagaj numeru PIN w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="10187-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="10187-163">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="10187-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="10187-165">Na urządzeniu użytkownika z systemem iOS otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="10187-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="10187-166">Zostanie też wyświetlony monit o wprowadzenie numeru PIN lub użycie odcisku palca.</span><span class="sxs-lookup"><span data-stu-id="10187-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="10187-168">Sprawdzanie działania ustawienia Resetuj numer PIN po określonej liczbie nieudanych prób</span><span class="sxs-lookup"><span data-stu-id="10187-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="10187-169">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Resetuj numer PIN po określonej liczbie nieudanych prób** jest ustawiona na dowolną wartość (domyślnie jest to 5).</span><span class="sxs-lookup"><span data-stu-id="10187-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="10187-170">Na urządzeniu użytkownika z systemem iOS otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="10187-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="10187-p106">Wprowadź nieprawidłowy numer PIN więcej razy niż zezwalają na to obowiązujące zasady. Pojawi się komunikat z informacją o **Osiągnięto limit prób wprowadzenia numeru PIN** i monit o zresetowanie tego numeru.</span><span class="sxs-lookup"><span data-stu-id="10187-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="10187-p107">Naciśnij przycisk **OK**. Zostanie wyświetlony monit o zalogowanie się przy użyciu poświadczeń użytkownika do usług Microsoft 365 Business i ustawienie nowego numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="10187-176">Sprawdzanie działania ustawienia Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="10187-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="10187-177">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="10187-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="10187-179">Na urządzeniu użytkownika z systemem iOS otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usługi Microsoft 365 Business. W razie potrzeby wprowadź kod PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="10187-180">Otwórz wiadomość e-mail z załącznikiem, otwórz ten załącznik i wybierz pozycję **Zapisz** u dołu ekranu.</span><span class="sxs-lookup"><span data-stu-id="10187-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="10187-p108">Powinna być widoczna tylko jedna opcja umożliwiająca zapisanie pliku w usłudze OneDrive dla Firm. Jeśli jej nie ma, naciśnij opcję **Dodaj konto** i wybierz pozycję **OneDrive dla Firm** na ekranie **Dodawanie konta magazynu**. Zaloguj się do usługi Microsoft 365 Business przez wprowadzenie poświadczeń użytkownika.</span><span class="sxs-lookup"><span data-stu-id="10187-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="10187-185">Naciśnij przycisk **Zapisz** i wybierz opcję **OneDrive dla Firm**.</span><span class="sxs-lookup"><span data-stu-id="10187-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="10187-186">Sprawdzanie działania ustawienia Wymagaj ponownego logowania użytkownika po określonym czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="10187-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="10187-187">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office** ma ustawioną dowolną wartość (domyślnie jest to 30 minut).</span><span class="sxs-lookup"><span data-stu-id="10187-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="10187-188">Na urządzeniu użytkownika z systemem iOS otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usługi Microsoft 365 Business. W razie potrzeby wprowadź kod PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="10187-p109">Powinna zostać wyświetlona skrzynka odbiorcza aplikacji Outlook. Nie dotykaj urządzenia z systemem iOS przez co najmniej 30 minut (lub inny czas, który jest dłuższy od wartości określonej w zasadach). Ekran urządzenia prawdopodobnie zostanie wygaszony.</span><span class="sxs-lookup"><span data-stu-id="10187-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="10187-192">Ponownie otwórz aplikację Outlook na urządzeniu z systemem iOS.</span><span class="sxs-lookup"><span data-stu-id="10187-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="10187-193">Przed ponownym uzyskaniem dostępu do aplikacji Outlook pojawi się monit o wprowadzenie numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="10187-194">Sprawdzanie działania ustawienia Chroń pliki służbowe przy użyciu szyfrowania</span><span class="sxs-lookup"><span data-stu-id="10187-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="10187-195">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Chroń pliki służbowe przy użyciu szyfrowania** jest **włączona**, a funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **wyłączona**.</span><span class="sxs-lookup"><span data-stu-id="10187-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="10187-196">Na urządzeniu użytkownika z systemem iOS otwórz aplikację Outlook i zaloguj się za pomocą poświadczeń użytkownika do usługi Microsoft 365 Business. W razie potrzeby wprowadź kod PIN.</span><span class="sxs-lookup"><span data-stu-id="10187-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="10187-197">Otwórz wiadomość e-mail z załączonymi kilkoma plikami obrazu.</span><span class="sxs-lookup"><span data-stu-id="10187-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="10187-198">Naciśnij załącznik i wybierz pod nim opcję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="10187-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="10187-p110">Otwórz aplikację **Zdjęcia** na ekranie głównym. Zobaczysz zapisane zdjęcie (lub kilka, jeśli zapiszesz ich więcej) w zaszyfrowanej postaci.</span><span class="sxs-lookup"><span data-stu-id="10187-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

