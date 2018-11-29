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
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982827"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="a07e7-103">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="a07e7-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="a07e7-104">Tworzenie zasad zarządzania aplikacjami dla systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="a07e7-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="a07e7-105">Jeśli użytkownicy mają urządzenia osobiste z systemem Windows 10, na których wykonują zadania służbowe, możesz również chronić dane na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="a07e7-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="a07e7-p101">Zaloguj się do usługi [Microsoft 365 Business](https://portal.office.com) za pomocą poświadczeń administratora globalnego. Wybierz kafelek **Administrator**, aby przejść do centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="a07e7-p101">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="a07e7-108">Na karcie **Zasady dotyczące urządzenia** portalu administracyjnego wybierz pozycję **Dodaj zasady**.</span><span class="sxs-lookup"><span data-stu-id="a07e7-108">On the **Device policies** card of the admin portal, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="a07e7-110">W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad.</span><span class="sxs-lookup"><span data-stu-id="a07e7-110">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="a07e7-111">W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="a07e7-111">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="a07e7-112">W obszarze \*\* typu urządzenia \*\*, wybierz **osobiste** lub **Właścicielem firmy**.</span><span class="sxs-lookup"><span data-stu-id="a07e7-112">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="a07e7-113">Opcja **Szyfruj pliki służbowe** zostanie włączona automatycznie.</span><span class="sxs-lookup"><span data-stu-id="a07e7-113">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="a07e7-114">Jeśli nie chcesz, aby użytkownicy mogli zapisywać pliki służbowe na swoich komputerach, **włącz** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm**.</span><span class="sxs-lookup"><span data-stu-id="a07e7-114">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="a07e7-p102">Rozwiń **Zarządzanie dostęp użytkowników do plików pakietu Office na urządzeniach** \> skonfigurować ustawienia jak. **Zarządzanie dostęp użytkowników do urządzeń biurowych na urządzeniach przenośnych** jest domyślnie **wyłączone** , ale zaleca się **ją włączyć** , a następnie zaakceptuj wartości domyślne. Aby uzyskać więcej informacji, zobacz temat [dostępne ustawienia](protection-settings-for-windows-10-devices.md#bkmk_settings) .</span><span class="sxs-lookup"><span data-stu-id="a07e7-p102">Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](protection-settings-for-windows-10-devices.md#bkmk_settings) for more information.</span></span> 
    
    <span data-ttu-id="a07e7-118">Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**.</span><span class="sxs-lookup"><span data-stu-id="a07e7-118">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="a07e7-119">Rozwiń sekcję **Odzyskiwanie danych na urządzeniach z systemem Windows** i **włącz** tę opcję (jest to zalecane).</span><span class="sxs-lookup"><span data-stu-id="a07e7-119">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="a07e7-p103">Aby móc przejść do lokalizacji certyfikatu agenta odzyskiwania danych, musisz najpierw go utworzyć. Odpowiednie instrukcje znajdziesz w artykule na temat [tworzenia i weryfikowania certyfikatu agenta odzyskiwania danych systemu szyfrowania plików](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="a07e7-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="a07e7-p104">Domyślnie pliki robocze są szyfrowane przy użyciu klucza tajnego, który jest przechowywany na urządzeniu i skojarzony z profilem użytkownika. Tylko użytkownik może otwierać i odszyfrowywać plik. Jednak w razie utraty urządzenia lub usunięcia użytkownika plik może utknąć w stanie zaszyfrowania. Administrator może użyć certyfikatu agenta odzyskiwania danych (DRA) do odszyfrowania pliku.</span><span class="sxs-lookup"><span data-stu-id="a07e7-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="a07e7-p105">Rozwiń sekcję **Chroń dodatkowe lokalizacje sieciowe i w chmurze**, jeśli chcesz dodać więcej domen lub lokalizacji usługi SharePoint Online. W ten sposób możesz się upewnić, że pliki we wszystkich wymienionych aplikacjach będą chronione. Poszczególne pozycje wprowadzane w polach oddzielaj średnikami.</span><span class="sxs-lookup"><span data-stu-id="a07e7-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="a07e7-p106">Następnie zdecydować **kto otrzyma te ustawienia?** Jeśli nie chcesz używać domyślnej grupy zabezpieczeń **Wszyscy użytkownicy** , **Zmień**, wybierz polecenie grupy zabezpieczeń, którzy otrzymają te ustawienia \> **Wybierz**.</span><span class="sxs-lookup"><span data-stu-id="a07e7-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="a07e7-132">Na koniec wybierz przycisk **Dodaj**, aby zapisać zasady i zastosować je na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="a07e7-132">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="a07e7-133">Dostępne ustawienia</span><span class="sxs-lookup"><span data-stu-id="a07e7-133">Available settings</span></span>

<span data-ttu-id="a07e7-134">Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="a07e7-134">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="a07e7-135">Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="a07e7-135">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="a07e7-136">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="a07e7-136">**Setting**</span></span>|<span data-ttu-id="a07e7-137">**Opis**</span><span class="sxs-lookup"><span data-stu-id="a07e7-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a07e7-138">Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="a07e7-138">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="a07e7-139">Gdy to ustawienie jest **włączone**, użytkownicy muszą się dodatkowo uwierzytelnić, korzystając z innej metody (oprócz podania nazwy użytkownika i hasła), aby uzyskać dostęp do aplikacji pakietu Office na urządzeniach przenośnych.</span><span class="sxs-lookup"><span data-stu-id="a07e7-139">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="a07e7-140">Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania</span><span class="sxs-lookup"><span data-stu-id="a07e7-140">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="a07e7-141">Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.</span><span class="sxs-lookup"><span data-stu-id="a07e7-141">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="a07e7-142">Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="a07e7-142">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="a07e7-143">To ustawienie określa, jak długo użytkownik może nie korzystać z aplikacji, zanim będzie wymagane ponowne zalogowanie się.</span><span class="sxs-lookup"><span data-stu-id="a07e7-143">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

