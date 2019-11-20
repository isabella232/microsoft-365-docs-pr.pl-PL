---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak zweryfikować ustawienia ochrony aplikacji biznesowych firmy Microsoft 365 w urządzeniach z systemem Windows 10.
ms.openlocfilehash: c54b053c1f6efbca8fd02431c416793a044c6821
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721865"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="0336f-103">Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="0336f-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="0336f-104">Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych</span><span class="sxs-lookup"><span data-stu-id="0336f-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="0336f-105">Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="0336f-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="0336f-106">Jeśli **włączono** **uniemożliwić użytkownikom kopiowanie danych firmowych do plików osobistych i wymusić ich zapisać pliki robocze do OneDrive dla firmy** ustawienie dla urządzeń należących do firmy, można to sprawdzić na urządzeniu użytkownika po nawiązaniu połączenia z usługą Azure AD i zalogowany.</span><span class="sxs-lookup"><span data-stu-id="0336f-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="0336f-107">**Sprawdzanie ustawień połączenia**</span><span class="sxs-lookup"><span data-stu-id="0336f-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="0336f-p102">Po zalogowaniu się przy użyciu poświadczeń Microsoft 365 Business i połączeniu z usługą Azure AD zgodnie z opisem w artykule [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md) przejdź do obszaru **Ustawienia systemu Windows** \> **Konta** \> **Uzyskaj dostęp do miejsca pracy lub nauki**. Wybierz pozycję **Połączono z usługą Azure AD \<nazwa dzierżawy\>**, a następnie wybierz pozycję **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="0336f-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="0336f-111">Na **zarządzanych przez** \<nazwę\> dzierżawcy strony, możesz zobaczyć informacje o **połączeniu** , który zawiera **adres serwera zarządzania** , jak pokazano na poniższej ilustracji.</span><span class="sxs-lookup"><span data-stu-id="0336f-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="0336f-113">**Sprawdź, czy nie można wkleić danych firmowych w aplikacji niezarządzanej**</span><span class="sxs-lookup"><span data-stu-id="0336f-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="0336f-114">Otwórz program Outlook 2016 zainstalowany przez usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0336f-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="0336f-115">Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.</span><span class="sxs-lookup"><span data-stu-id="0336f-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="0336f-116">Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.</span><span class="sxs-lookup"><span data-stu-id="0336f-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="0336f-117">Zostanie wyświetlony komunikat o błędzie informujący, że aplikacja nie może uzyskać dostępu do zawartości.</span><span class="sxs-lookup"><span data-stu-id="0336f-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="0336f-119">Można jednak wkleić tę zawartość w programie Word 2016.</span><span class="sxs-lookup"><span data-stu-id="0336f-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="0336f-120">Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych</span><span class="sxs-lookup"><span data-stu-id="0336f-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="0336f-121">**Sprawdzanie ustawień połączenia**</span><span class="sxs-lookup"><span data-stu-id="0336f-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="0336f-122">Na urządzeniu osobistym z systemem Windows 10, w którym użytkownik jest zalogowany jako użytkownik lokalny, przejdź do pozycji **Ustawienia systemu Windows**i kliknij \*\*\*\* \> lub naciśnij pozycję **dostęp do kont w pracy lub szkole**.</span><span class="sxs-lookup"><span data-stu-id="0336f-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="0336f-123">W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="0336f-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="0336f-124">W oknie dialogowym **Konfigurowanie konta służbowego** \> **Zaloguj się** wprowadź poświadczenia Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0336f-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="0336f-125">Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="0336f-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kliknij lub naciśnij pozycję informacje w oknie dialogowym konto służbowe lub szkolne.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="0336f-127">Na stronie **dostęp do pracy lub szkoły** możesz zobaczyć **Informacje o połączeniu** , które zawierają **adres serwera zarządzania** , taki jak pokazany na poniższym rysunku, i zawiera słowa *PWT* i *mam* w.</span><span class="sxs-lookup"><span data-stu-id="0336f-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="0336f-129">**Sprawdź, czy nie można wkleić danych firmowych w aplikacji niezarządzanej**</span><span class="sxs-lookup"><span data-stu-id="0336f-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="0336f-130">Otwórz program Outlook 2016 i dodaj konto Microsoft 365 Business, jeśli to konieczne, a następnie zaloguj się przy użyciu poświadczeń Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0336f-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="0336f-131">Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.</span><span class="sxs-lookup"><span data-stu-id="0336f-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="0336f-132">Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.</span><span class="sxs-lookup"><span data-stu-id="0336f-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="0336f-133">Otrzymasz komunikat o błędzie informujący, że aplikacja nie może uzyskać dostępu do zawartości.</span><span class="sxs-lookup"><span data-stu-id="0336f-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="0336f-135">Można jednak wkleić tę zawartość w programie Word 2016.</span><span class="sxs-lookup"><span data-stu-id="0336f-135">You can, however, paste the same content into Word 2016.</span></span>
    

