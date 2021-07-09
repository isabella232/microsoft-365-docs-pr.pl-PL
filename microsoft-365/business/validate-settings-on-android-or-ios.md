---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na urządzeniach z systemem Android lub iOS
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
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Dowiedz się, jak sprawdzić poprawność Microsoft 365 Business Premium ochrony aplikacji na urządzeniach z systemem Android lub iOS.
ms.openlocfilehash: 43e74b548711550090021c39096b1647cee9e039
ms.sourcegitcommit: 0d1b065c94125b495e9886200f7918de3bda40b3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339335"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="00524-103">Sprawdzanie poprawności ustawień ochrony aplikacji na urządzeniach z systemem Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="00524-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="00524-104">Postępuj zgodnie z instrukcjami w poniższych sekcjach, aby sprawdzić poprawność ustawień ochrony aplikacji na urządzeniach z systemem Android lub iOS.</span><span class="sxs-lookup"><span data-stu-id="00524-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="00524-105">Android</span><span class="sxs-lookup"><span data-stu-id="00524-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="00524-106">Sprawdzanie, czy na urządzeniach użytkowników działają ustawienia ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="00524-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="00524-107">Gdy [skonfigurujesz aplikacje dla urządzeń z systemem Android](app-protection-settings-for-android-and-ios.md) w celu ochrony aplikacji, możesz wykonać czynności opisane poniżej, aby sprawdzić działanie wybranych ustawień.</span><span class="sxs-lookup"><span data-stu-id="00524-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="00524-108">Najpierw upewnij się, że zasady dotyczą aplikacji, w której chcesz ją zweryfikować.</span><span class="sxs-lookup"><span data-stu-id="00524-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="00524-109">W centrum Microsoft 365 Business Premium [przejdź](https://admin.microsoft.com)do **pozycji** Zasady \> **Edytuj zasady.**</span><span class="sxs-lookup"><span data-stu-id="00524-109">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="00524-110">Wybierz **pozycję Zasady aplikacji** dla systemu Android dla ustawień utworzonych podczas konfiguracji lub innych utworzonych zasad i sprawdź, czy są wymuszane na przykład Outlook urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="00524-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="00524-112">Sprawdzanie działania ustawienia Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu</span><span class="sxs-lookup"><span data-stu-id="00524-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="00524-113">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="00524-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Upewnij się, że dla ustawienia Wymagaj numeru PIN lub odcisku palca Office dostępu do aplikacji jest ustawiona wartość Wł.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="00524-115">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook zaloguj się przy użyciu jego poświadczeń logowania Microsoft 365 Business Premium Android.</span><span class="sxs-lookup"><span data-stu-id="00524-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="00524-116">Zostanie również wyświetlony monit o wprowadzenie numeru PIN lub użycie odcisku palca.</span><span class="sxs-lookup"><span data-stu-id="00524-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="00524-118">Sprawdzanie działania ustawienia Resetuj numer PIN po określonej liczbie nieudanych prób</span><span class="sxs-lookup"><span data-stu-id="00524-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="00524-119">W  okienku Edytuj  zasady wybierz pozycję Edytuj obok opcji Kontrola dostępu do dokumentów programu Office , **rozwiń** pozycję Zarządzaj dostępem użytkowników do plików programu **Office** na urządzeniach przenośnych i upewnij się, że po liczbie nieudanych prób jest ustawiona wartość Resetuj numer **PIN.**</span><span class="sxs-lookup"><span data-stu-id="00524-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="00524-120">Domyślnie jest to 5.</span><span class="sxs-lookup"><span data-stu-id="00524-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="00524-121">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook zaloguj się przy użyciu jego poświadczeń logowania Microsoft 365 Business Premium Android.</span><span class="sxs-lookup"><span data-stu-id="00524-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="00524-122">Wprowadź nieprawidłowy numer PIN więcej razy niż zezwalają na to obowiązujące zasady.</span><span class="sxs-lookup"><span data-stu-id="00524-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="00524-123">Zostanie wyświetlony monit z komunikatem Osiągnięto limit prób numeru **PIN,** aby zresetować ten numer.</span><span class="sxs-lookup"><span data-stu-id="00524-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="00524-125">Naciśnij pozycję **Resetuj numer PIN**.</span><span class="sxs-lookup"><span data-stu-id="00524-125">Press **Reset PIN**.</span></span> <span data-ttu-id="00524-126">Zostanie wyświetlony monit o zalogowanie się przy użyciu poświadczeń logowania Microsoft 365 Business Premium, a następnie ustawienie nowego numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="00524-127">Sprawdzanie działania ustawienia Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="00524-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="00524-128">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="00524-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="00524-130">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook zaloguj się przy użyciu jego poświadczeń logowania Microsoft 365 Business Premium, a w razie prośby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="00524-131">Otwórz wiadomość e-mail zawierającą załącznik, a następnie naciśnij ikonę strzałki w dół obok informacji o załączniku.</span><span class="sxs-lookup"><span data-stu-id="00524-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="00524-133">U dołu ekranu zostanie wyświetlony **obraz** Nie można zapisać na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="00524-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="00524-135">Zapisywanie w usłudze OneDrive dla Firm nie jest obecnie włączone dla systemu Android, więc jest tylko wyświetlana informacja o zablokowanej możliwości zapisywania lokalnie.</span><span class="sxs-lookup"><span data-stu-id="00524-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="00524-136">Sprawdzanie działania ustawienia Wymagaj ponownego logowania użytkownika po określonym czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="00524-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="00524-137">W  okienku Edytuj  zasady wybierz pozycję Edytuj obok opcji Kontrola dostępu do dokumentów programu **Office**, rozwiń  pozycję Zarządzaj dostępem użytkowników do plików programu **Office** na urządzeniach przenośnych i upewnij się, że ustawienie Wymagaj ponownego logowania użytkowników po Office, gdy aplikacje nie są bezczynne, ma ustawioną wartość pewnymi minutami.</span><span class="sxs-lookup"><span data-stu-id="00524-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="00524-138">Domyślnie jest to 30 minut.</span><span class="sxs-lookup"><span data-stu-id="00524-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="00524-139">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook zaloguj się przy użyciu jego poświadczeń logowania Microsoft 365 Business Premium, a w razie prośby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="00524-p105">Powinna zostać wyświetlona skrzynka odbiorcza aplikacji Outlook. Nie dotykaj urządzenia z systemem Android przez co najmniej 30 minut (lub inny czas dłuższy niż wartość określona w zasadach). Ekran urządzenia prawdopodobnie zostanie wygaszony.</span><span class="sxs-lookup"><span data-stu-id="00524-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="00524-143">Ponownie Outlook na urządzeniu z systemem Android.</span><span class="sxs-lookup"><span data-stu-id="00524-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="00524-144">Zanim będzie można ponownie uzyskać dostęp do swojego numeru PIN, zostanie Outlook monit o wprowadzenie numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="00524-145">Sprawdzanie działania ustawienia Chroń pliki służbowe przy użyciu szyfrowania</span><span class="sxs-lookup"><span data-stu-id="00524-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="00524-146">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Chroń pliki służbowe przy użyciu szyfrowania** jest **włączona**, a funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **wyłączona**.</span><span class="sxs-lookup"><span data-stu-id="00524-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="00524-147">Na urządzeniu użytkownika z systemem Android otwórz aplikację Outlook zaloguj się przy użyciu jego poświadczeń logowania Microsoft 365 Business Premium, a w razie prośby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="00524-148">Otwórz wiadomość e-mail zawierającą kilka załączników do pliku obrazu.</span><span class="sxs-lookup"><span data-stu-id="00524-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="00524-149">Naciśnij ikonę strzałki w dół obok informacji o załączniku, aby go zapisać.</span><span class="sxs-lookup"><span data-stu-id="00524-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="00524-p106">Może pojawić się monit o zezwolenie programowi Outlook na dostęp do zdjęć, multimediów i plików na urządzeniu. Naciśnij pozycję **Zezwalaj**.</span><span class="sxs-lookup"><span data-stu-id="00524-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="00524-153">U dołu ekranu wybierz pozycję **Zapisz na urządzeniu**, a następnie otwórz aplikację **Galeria**.</span><span class="sxs-lookup"><span data-stu-id="00524-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="00524-p107">Na liście powinno zostać wyświetlone zaszyfrowane zdjęcie (lub kilka zdjęć, jeśli zapisano ich więcej). Może ono być wyświetlane na liście obrazów w postaci szarego kwadratu z białym wykrzyknikiem w białym okręgu w środku szarego kwadratu.</span><span class="sxs-lookup"><span data-stu-id="00524-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="00524-157">iOS</span><span class="sxs-lookup"><span data-stu-id="00524-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="00524-158">Sprawdzanie, czy na urządzeniach użytkowników działają ustawienia ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="00524-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="00524-159">Gdy [skonfigurujesz aplikacje dla urządzeń z systemem iOS](app-protection-settings-for-android-and-ios.md) w celu ochrony aplikacji, możesz wykonać czynności opisane poniżej, aby sprawdzić działanie wybranych ustawień.</span><span class="sxs-lookup"><span data-stu-id="00524-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="00524-160">Najpierw upewnij się, że zasady dotyczą aplikacji, w której chcesz ją zweryfikować.</span><span class="sxs-lookup"><span data-stu-id="00524-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="00524-161">W centrum Microsoft 365 Business Premium [przejdź](https://admin.microsoft.com)do **pozycji** Zasady \> **Edytuj zasady.**</span><span class="sxs-lookup"><span data-stu-id="00524-161">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="00524-162">Wybierz pozycję Zasady aplikacji dla systemu **iOS** dla ustawień utworzonych podczas instalacji lub innych utworzonych zasad i sprawdź, czy są wymuszane na przykład Outlook konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="00524-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="00524-164">Sprawdzanie działania ustawienia Wymagaj numeru PIN w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="00524-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="00524-165">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Kontrola dostępu do dokumentów pakietu Office**, rozwiń pozycję **Zarządzaj dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych** i upewnij się, że funkcja **Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="00524-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Upewnij się, że dla ustawienia Wymagaj numeru PIN lub odcisku palca Office dostępu do aplikacji jest ustawiona wartość Wł.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="00524-167">Na urządzeniu użytkownika z systemem iOS otwórz Outlook zaloguj się przy użyciu poświadczeń logowania Microsoft 365 Business Premium użytkownika.</span><span class="sxs-lookup"><span data-stu-id="00524-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="00524-168">Zostanie również wyświetlony monit o wprowadzenie numeru PIN lub użycie odcisku palca.</span><span class="sxs-lookup"><span data-stu-id="00524-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="00524-170">Sprawdzanie działania ustawienia Resetuj numer PIN po określonej liczbie nieudanych prób</span><span class="sxs-lookup"><span data-stu-id="00524-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="00524-171">W  okienku Edytuj  zasady wybierz pozycję Edytuj obok opcji Kontrola dostępu do dokumentów programu Office , **rozwiń** pozycję Zarządzaj dostępem użytkowników do plików programu **Office** na urządzeniach przenośnych i upewnij się, że po liczbie nieudanych prób jest ustawiona wartość Resetuj numer **PIN.**</span><span class="sxs-lookup"><span data-stu-id="00524-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="00524-172">Domyślnie jest to 5.</span><span class="sxs-lookup"><span data-stu-id="00524-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="00524-173">Na urządzeniu użytkownika z systemem iOS otwórz Outlook zaloguj się przy użyciu poświadczeń logowania Microsoft 365 Business Premium użytkownika.</span><span class="sxs-lookup"><span data-stu-id="00524-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="00524-174">Wprowadź nieprawidłowy numer PIN więcej razy niż zezwalają na to obowiązujące zasady.</span><span class="sxs-lookup"><span data-stu-id="00524-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="00524-175">Zostanie wyświetlony monit z komunikatem Osiągnięto limit prób numeru **PIN,** aby zresetować ten numer.</span><span class="sxs-lookup"><span data-stu-id="00524-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="00524-177">Naciśnij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="00524-177">Press **OK**.</span></span> <span data-ttu-id="00524-178">Zostanie wyświetlony monit o zalogowanie się przy użyciu poświadczeń logowania Microsoft 365 Business Premium, a następnie ustawienie nowego numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="00524-179">Sprawdzanie działania ustawienia Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="00524-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="00524-180">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **włączona**.</span><span class="sxs-lookup"><span data-stu-id="00524-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="00524-182">Na urządzeniu użytkownika z systemem iOS otwórz program Outlook zaloguj się przy użyciu poświadczeń logowania Microsoft 365 Business Premium i w razie prośby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="00524-183">Otwórz wiadomość e-mail z załącznikiem, otwórz ten załącznik i wybierz pozycję **Zapisz** u dołu ekranu.</span><span class="sxs-lookup"><span data-stu-id="00524-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="00524-185">Powinna być widoczna tylko jedna opcja umożliwiająca zapisanie pliku w usłudze OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="00524-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="00524-186">Jeśli nie, naciśnij **pozycję Dodaj konto** i wybierz pozycję **OneDrive dla Firm** na ekranie **Storage konto.**</span><span class="sxs-lookup"><span data-stu-id="00524-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="00524-187">Podaj nazwę użytkownika końcowego, Microsoft 365 Business Premium się po wyświetleniu monitu.</span><span class="sxs-lookup"><span data-stu-id="00524-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="00524-188">Naciśnij przycisk **Zapisz** i wybierz opcję **OneDrive dla Firm**.</span><span class="sxs-lookup"><span data-stu-id="00524-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="00524-189">Sprawdzanie działania ustawienia Wymagaj ponownego logowania użytkownika po określonym czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="00524-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="00524-190">W  okienku Edytuj  zasady wybierz pozycję Edytuj obok opcji Kontrola dostępu do dokumentów programu **Office**, rozwiń  pozycję Zarządzaj dostępem użytkowników do plików programu **Office** na urządzeniach przenośnych i upewnij się, że ustawienie Wymagaj ponownego logowania użytkowników po Office, gdy aplikacje nie są bezczynne, ma ustawioną wartość pewnymi minutami.</span><span class="sxs-lookup"><span data-stu-id="00524-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="00524-191">Domyślnie jest to 30 minut.</span><span class="sxs-lookup"><span data-stu-id="00524-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="00524-192">Na urządzeniu użytkownika z systemem iOS otwórz program Outlook zaloguj się przy użyciu poświadczeń logowania Microsoft 365 Business Premium i w razie prośby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="00524-p113">Powinna zostać wyświetlona skrzynka odbiorcza aplikacji Outlook. Nie dotykaj urządzenia z systemem iOS przez co najmniej 30 minut (lub inny czas, który jest dłuższy od wartości określonej w zasadach). Ekran urządzenia prawdopodobnie zostanie wygaszony.</span><span class="sxs-lookup"><span data-stu-id="00524-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="00524-196">Ponownie Outlook na urządzeniu z systemem iOS.</span><span class="sxs-lookup"><span data-stu-id="00524-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="00524-197">Zanim będzie można ponownie uzyskać dostęp do swojego numeru PIN, zostanie Outlook monit o wprowadzenie numeru PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="00524-198">Sprawdzanie działania ustawienia Chroń pliki służbowe przy użyciu szyfrowania</span><span class="sxs-lookup"><span data-stu-id="00524-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="00524-199">W okienku **Edytuj zasady** wybierz pozycję **Edytuj** obok pozycji **Ochrona w razie utraty lub kradzieży urządzenia**, rozwiń pozycję **Chroń pliki służbowe w przypadku zgubienia lub kradzieży urządzenia** i upewnij się, że funkcja **Chroń pliki służbowe przy użyciu szyfrowania** jest **włączona**, a funkcja **Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm** jest **wyłączona**.</span><span class="sxs-lookup"><span data-stu-id="00524-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="00524-200">Na urządzeniu użytkownika z systemem iOS otwórz program Outlook zaloguj się przy użyciu poświadczeń logowania Microsoft 365 Business Premium i w razie prośby wprowadź numer PIN.</span><span class="sxs-lookup"><span data-stu-id="00524-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="00524-201">Otwórz wiadomość e-mail zawierającą kilka załączników do pliku obrazu.</span><span class="sxs-lookup"><span data-stu-id="00524-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="00524-202">Naciśnij załącznik i wybierz pod nim opcję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="00524-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="00524-p114">Otwórz aplikację **Zdjęcia** na ekranie głównym. Zobaczysz zapisane zdjęcie (lub kilka, jeśli zapiszesz ich więcej) w zaszyfrowanej postaci.</span><span class="sxs-lookup"><span data-stu-id="00524-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

