---
title: Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS
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
description: Dowiedz się, jak tworzyć, edytować i usuwać zasady zarządzania aplikacjami oraz chronić pliki robocze na urządzeniach z systemem Android lub iOS.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321850"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="ec2ce-103">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="ec2ce-103">Set app protection settings for Android or iOS devices</span></span>

![Banner, który wskaż https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="ec2ce-105">Tworzenie zasad zarządzania aplikacjami</span><span class="sxs-lookup"><span data-stu-id="ec2ce-105">Create an app management policy</span></span>

1. <span data-ttu-id="ec2ce-106">Przejdź do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="ec2ce-107">W lewym NAV wybierz pozycję **zasady** \> **urządzeń** \> **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="ec2ce-108">W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="ec2ce-109">W obszarze **Typ zasad**, wybierz **Zarządzanie aplikacjami dla systemu Android** lub **Zarządzanie aplikacjami dla systemu iOS**, w zależności od tego, który zestaw zasad, które chcesz utworzyć.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="ec2ce-110">Rozwiń pozycję **Chroń pliki robocze, gdy urządzenia zostaną utracone lub skradzione** , i Zarządzaj tym, **jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych**.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="ec2ce-111">Skonfiguruj ustawienia tak, jak chcesz.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-111">Configure the settings how you would like.</span></span> <span data-ttu-id="ec2ce-112">**Zarządzaj tym, jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych** jest domyślnie **wyłączona** , ale zaleca się **włączenie go i** zaakceptuj wartości domyślne.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="ec2ce-113">Aby uzyskać więcej informacji, zobacz [dostępne ustawienia](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="ec2ce-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="ec2ce-114">Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="ec2ce-116">Next decide **Who will get these settings?**</span><span class="sxs-lookup"><span data-stu-id="ec2ce-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="ec2ce-117">Jeśli nie chcesz używać domyślnej grupy zabezpieczeń **Wszyscy użytkownicy** , wybierz polecenie **Zmień**, wybierz grupy zabezpieczeń, które mają te ustawienia \> **Wybierz**.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="ec2ce-118">Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="ec2ce-119">Edytowanie zasad zarządzania aplikacjami</span><span class="sxs-lookup"><span data-stu-id="ec2ce-119">Edit an app management policy</span></span>

1. <span data-ttu-id="ec2ce-120">Na karcie **zasady** wybierz pozycję **Edytuj zasadę**.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="ec2ce-121">W okienku **Edytowanie zasad** wybierz zasadę, którą chcesz zmienić.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="ec2ce-122">Wybierz opcję **Edytuj** obok poszczególnych ustawień, aby zmienić wartości zasad.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="ec2ce-123">Zmiana wartości jest automatycznie zapisywana w zasadach.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="ec2ce-124">Gdy skończysz, Zamknij Edytuj okienko **zasad** .</span><span class="sxs-lookup"><span data-stu-id="ec2ce-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="ec2ce-125">Usuwanie zasad zarządzania aplikacjami</span><span class="sxs-lookup"><span data-stu-id="ec2ce-125">Delete an app management policy</span></span>

1. <span data-ttu-id="ec2ce-126">Na stronie **zasady** wybierz zasadę, a następnie **Usuń**.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="ec2ce-127">W okienku **zasady usuwania** wybierz pozycję **Potwierdź** , aby usunąć wybrane zasady lub zasady.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="ec2ce-128">Dostępne ustawienia</span><span class="sxs-lookup"><span data-stu-id="ec2ce-128">Available settings</span></span>

<span data-ttu-id="ec2ce-129">Poniższe tabele dają szczegółowe informacje na temat ustawień dostępnych do ochrony plików roboczych na urządzeniach i ustawień, które kontrolują, jak użytkownicy uzyskują dostęp do plików pakietu Office z ich urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="ec2ce-130">Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="ec2ce-130">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="ec2ce-131">Ustawienia chroniące pliki służbowe</span><span class="sxs-lookup"><span data-stu-id="ec2ce-131">Settings that protect work files</span></span>

<span data-ttu-id="ec2ce-132">W przypadku zgubienia lub kradzieży urządzenia użytkownika dostępne są następujące ustawienia chroniące pliki służbowe:</span><span class="sxs-lookup"><span data-stu-id="ec2ce-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ec2ce-133">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="ec2ce-133">Setting</span></span>  <br/> |<span data-ttu-id="ec2ce-134">Opis</span><span class="sxs-lookup"><span data-stu-id="ec2ce-134">Description</span></span>  <br/> |
|<span data-ttu-id="ec2ce-135">Usuń pliki służbowe z nieaktywnego urządzenia po określonej liczbie dni</span><span class="sxs-lookup"><span data-stu-id="ec2ce-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="ec2ce-136">Jeśli urządzenie nie jest używane przez liczbę dni, które określisz w tym miejscu, wszystkie pliki robocze zapisane na urządzeniu zostaną automatycznie usunięte.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="ec2ce-137">Wymuszaj na użytkownikach zapisywanie wszystkich plików służbowych w usłudze OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="ec2ce-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="ec2ce-138">Jeśli to ustawienie jest **włączone**, jedyną dostępną lokalizacją zapisywania plików roboczych jest usługa OneDrive dla firm.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="ec2ce-139">Szyfruj pliki służbowe</span><span class="sxs-lookup"><span data-stu-id="ec2ce-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="ec2ce-140">Zachowaj to ustawienie **Włączone**, aby chronić pliki służbowe przy użyciu szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="ec2ce-141">Nawet jeśli urządzenie zostanie zgubione lub skradzione, nikt nie może odczytać danych firmowych.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="ec2ce-142">Ustawienia, które sterują dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="ec2ce-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="ec2ce-143">Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="ec2ce-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ec2ce-144">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="ec2ce-144">Setting</span></span>  <br/> |<span data-ttu-id="ec2ce-145">Opis</span><span class="sxs-lookup"><span data-stu-id="ec2ce-145">Description</span></span>  <br/> |
|<span data-ttu-id="ec2ce-146">Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ec2ce-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="ec2ce-147">Jeśli to ustawienie jest **na** użytkowników, należy podać inną formę uwierzytelniania, oprócz nazwy użytkownika i hasła, zanim będą mogli korzystać z aplikacji pakietu Office na swoich urządzeniach przenośnych.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="ec2ce-148">Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania</span><span class="sxs-lookup"><span data-stu-id="ec2ce-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="ec2ce-149">Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="ec2ce-150">Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ec2ce-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="ec2ce-151">To ustawienie określa, jak długo użytkownik może być bezczynny, zanim zostanie wyświetlony monit o ponowne zalogowanie.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="ec2ce-152">Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta</span><span class="sxs-lookup"><span data-stu-id="ec2ce-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="ec2ce-p105">Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta. Umożliwia to użytkownikowi modyfikowanie systemu operacyjnego, co może uczynić urządzenie bardziej podatnym na złośliwe oprogramowanie. Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.  </span><span class="sxs-lookup"><span data-stu-id="ec2ce-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="ec2ce-156">Zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych</span><span class="sxs-lookup"><span data-stu-id="ec2ce-156">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="ec2ce-157">Domyślnie jest to dozwolone, ale gdy to ustawienie jest **włączone**, użytkownik może kopiować informacje z pliku służbowego do osobistego.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="ec2ce-158">Jeśli to ustawienie jest **wyłączone**, użytkownik nie będzie mógł kopiować informacji z konta służbowego do aplikacji osobistej ani na konto osobiste.</span><span class="sxs-lookup"><span data-stu-id="ec2ce-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
