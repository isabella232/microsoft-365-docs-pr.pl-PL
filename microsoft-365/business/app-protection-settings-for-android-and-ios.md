---
title: Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983667"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="999db-103">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="999db-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="999db-104">Tworzenie zasad zarządzania aplikacjami</span><span class="sxs-lookup"><span data-stu-id="999db-104">Create an app management policy</span></span>

1. <span data-ttu-id="999db-105">Zaloguj się do usługi [Microsoft 365 Business](https://portal.office.com) za pomocą poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="999db-105">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="999db-106">W centrum administracyjnym na karcie **Zasady dotyczące urządzenia** wybierz pozycję **Dodaj zasady**.</span><span class="sxs-lookup"><span data-stu-id="999db-106">In the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="999db-108">W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad.</span><span class="sxs-lookup"><span data-stu-id="999db-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="999db-109">W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Android** lub **Zarządzanie aplikacjami dla systemu iOS** w zależności od tego, jaki zestaw zasad chcesz utworzyć.</span><span class="sxs-lookup"><span data-stu-id="999db-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="999db-p101">Rozwiń węzeł **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** i **zarządzać dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** \> skonfigurować ustawienia jak. **Zarządzaj dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** jest domyślnie **wyłączone** , ale zaleca się **ją włączyć** , a następnie zaakceptuj wartości domyślne. Aby uzyskać więcej informacji, zobacz temat [dostępne ustawienia](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) .</span><span class="sxs-lookup"><span data-stu-id="999db-p101">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="999db-113">Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**.</span><span class="sxs-lookup"><span data-stu-id="999db-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="999db-p102">Następnie zdecydować **kto otrzyma te ustawienia?** Jeśli nie chcesz używać domyślnej grupy zabezpieczeń **Wszyscy użytkownicy** , **Zmień**, wybierz polecenie grupy zabezpieczeń, którzy otrzymają te ustawienia \> **Wybierz**.</span><span class="sxs-lookup"><span data-stu-id="999db-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="999db-117">Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="999db-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="999db-118">Edytowanie zasad zarządzania aplikacjami</span><span class="sxs-lookup"><span data-stu-id="999db-118">Edit an app management policy</span></span>

1. <span data-ttu-id="999db-119">Na karcie **zasady** wybierz polecenie **Edytuj zasady**.</span><span class="sxs-lookup"><span data-stu-id="999db-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="999db-120">W okienku **Edytowanie zasad** wybierz zasadę, którą chcesz zmienić.</span><span class="sxs-lookup"><span data-stu-id="999db-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="999db-p103">Wybierz opcję **Edytuj** obok poszczególnych ustawień, aby zmienić wartości zasad. Wszystkie zmiany są zapisywane automatycznie.</span><span class="sxs-lookup"><span data-stu-id="999db-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="999db-123">Gdy skończysz wprowadzać zmiany, zamknij okienko **Edytowanie zasad**.</span><span class="sxs-lookup"><span data-stu-id="999db-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="999db-124">Usuwanie zasad zarządzania aplikacjami</span><span class="sxs-lookup"><span data-stu-id="999db-124">Delete an app management policy</span></span>

1. <span data-ttu-id="999db-125">Na karcie **Zasady** wybierz pozycję **Usuń zasady**.</span><span class="sxs-lookup"><span data-stu-id="999db-125">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="999db-126">**Usuwanie zasady** w okienku wybierz zasady do usunięcia \> **Zaznacz**, a następnie **Potwierdź** usunąć zasadę lub zasady wybrano.</span><span class="sxs-lookup"><span data-stu-id="999db-126">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="999db-127">Dostępne ustawienia</span><span class="sxs-lookup"><span data-stu-id="999db-127">Available settings</span></span>

<span data-ttu-id="999db-128">W poniższych tabelach szczegółowo opisano dostępne ustawienia umożliwiające ochronę służbowych plików na urządzeniach i kontrolowanie dostępu użytkowników do plików pakietu Office na urządzeniach przenośnych.</span><span class="sxs-lookup"><span data-stu-id="999db-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="999db-129">Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="999db-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="999db-130">Ustawienia chroniące pliki służbowe</span><span class="sxs-lookup"><span data-stu-id="999db-130">Settings that protect work files</span></span>

<span data-ttu-id="999db-131">W przypadku zagubienia lub kradzieży urządzenia użytkownika dostępne są następujące ustawienia chroniące pliki służbowe:</span><span class="sxs-lookup"><span data-stu-id="999db-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="999db-132">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="999db-132">Setting</span></span>  <br/> |<span data-ttu-id="999db-133">Opis</span><span class="sxs-lookup"><span data-stu-id="999db-133">Description</span></span>  <br/> |
|<span data-ttu-id="999db-134">Usuń pliki służbowe z nieaktywnego urządzenia po określonej liczbie dni</span><span class="sxs-lookup"><span data-stu-id="999db-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="999db-135">Jeśli urządzenie nie będzie używane przez określoną w tym miejscu liczbę dni, wszelkie pliki służbowe znajdujące się na urządzeniu zostaną automatycznie usunięte.</span><span class="sxs-lookup"><span data-stu-id="999db-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="999db-136">Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="999db-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="999db-137">Gdy to ustawienie jest **włączone**, pliki służbowe można zapisywać tylko w usłudze OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="999db-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="999db-138">Szyfruj pliki służbowe</span><span class="sxs-lookup"><span data-stu-id="999db-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="999db-p104">Pozostaw to ustawienie **włączone**, aby chronić pliki służbowe przy użyciu szyfrowania. Nawet jeśli urządzenie zostanie zgubione lub ukradzione, nikt nie będzie mógł odczytać danych firmowych.  </span><span class="sxs-lookup"><span data-stu-id="999db-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="999db-141">Ustawienia umożliwiające kontrolę dostępu użytkowników do plików pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="999db-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="999db-142">Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="999db-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="999db-143">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="999db-143">Setting</span></span>  <br/> |<span data-ttu-id="999db-144">Opis</span><span class="sxs-lookup"><span data-stu-id="999db-144">Description</span></span>  <br/> |
|<span data-ttu-id="999db-145">Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="999db-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="999db-146">Gdy to ustawienie jest **włączone**, użytkownicy muszą się dodatkowo uwierzytelnić, korzystając z innej metody (oprócz podania nazwy użytkownika i hasła), aby uzyskać dostęp do aplikacji pakietu Office na urządzeniach przenośnych.</span><span class="sxs-lookup"><span data-stu-id="999db-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="999db-147">Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania</span><span class="sxs-lookup"><span data-stu-id="999db-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="999db-148">Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.</span><span class="sxs-lookup"><span data-stu-id="999db-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="999db-149">Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="999db-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="999db-150">To ustawienie określa, jak długo użytkownik może nie korzystać z aplikacji, zanim będzie wymagane ponowne zalogowanie się.</span><span class="sxs-lookup"><span data-stu-id="999db-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="999db-151">Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta</span><span class="sxs-lookup"><span data-stu-id="999db-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="999db-p105">Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta. Umożliwia to użytkownikowi modyfikowanie systemu operacyjnego, co może narazić urządzenie na ataki złośliwym oprogramowaniem. Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.  </span><span class="sxs-lookup"><span data-stu-id="999db-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="999db-155">Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych</span><span class="sxs-lookup"><span data-stu-id="999db-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="999db-p106">Zezwalamy na to domyślnie, ale jeżeli to ustawienie jest **włączone**, użytkownik może skopiować informacje w pliku roboczego do pliku osobistego. Jeśli to ustawienie jest **wyłączone**, użytkownik będzie mógł skopiować informacje z konta służbowego do osobistych aplikacji lub konto osobiste.</span><span class="sxs-lookup"><span data-stu-id="999db-p106">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file. If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.  </span></span><br/> |
   

  

