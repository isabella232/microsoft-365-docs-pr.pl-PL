---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Sprawdź poprawność ustawień ochrony aplikacji usługi Microsoft 365 Business Premium na urządzeniach z systemem Windows 10 i sprawdź, czy użytkownicy nie mogą kopiować danych firmowych do plików osobistych lub aplikacji niezarządzalnych.
ms.openlocfilehash: 589d2fc25cc1425a775523595881660cc03e152e
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403395"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="cf480-103">Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf480-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="cf480-104">Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych</span><span class="sxs-lookup"><span data-stu-id="cf480-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="cf480-105">Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="cf480-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="cf480-106">Jeśli **włączono ustawienie Uniemożliwić użytkownikom kopiowanie danych firmowych do plików osobistych i wymusić na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm** dla urządzeń należących do firmy, możesz to sprawdzić na urządzeniu użytkownika po nawiązaniu połączenia z usługą Azure AD i zalogowaniu się. **On**</span><span class="sxs-lookup"><span data-stu-id="cf480-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="cf480-107">**Sprawdzanie ustawień połączenia**</span><span class="sxs-lookup"><span data-stu-id="cf480-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="cf480-108">Po zalogowaniu się przy użyciu poświadczeń usługi Microsoft 365 Business Premium i nawiązaniu połączenia z usługą Azure AD zgodnie z opisem w [sekcji Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium](set-up-windows-devices.md)przejdź do sekcji Dostęp do kont ustawień systemu **Windows** w pracy \> **Accounts** \> **lub szkole**.</span><span class="sxs-lookup"><span data-stu-id="cf480-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="cf480-109">Wybierz pozycję **Połączono z \<tenant name\> usługą Azure AD**, a następnie wybierz pozycję **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="cf480-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="cf480-111">Na stronie **Zarządzane według** \<tenant name\> można wyświetlić informacje o **połączeniu,** które zawierają **adres serwera zarządzania,** taki jak ten pokazany na poniższym rysunku.</span><span class="sxs-lookup"><span data-stu-id="cf480-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="cf480-113">**Sprawdź, czy nie można wkleić danych firmy w aplikacji niezarządkowej**</span><span class="sxs-lookup"><span data-stu-id="cf480-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="cf480-114">Otwórz program Outlook 2016, który został zainstalowany przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cf480-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="cf480-115">Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.</span><span class="sxs-lookup"><span data-stu-id="cf480-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="cf480-116">Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.</span><span class="sxs-lookup"><span data-stu-id="cf480-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="cf480-117">Zostanie wyświetlony błąd informujący, że aplikacja nie może uzyskać dostępu do zawartości.</span><span class="sxs-lookup"><span data-stu-id="cf480-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="cf480-119">Można jednak wkleić tę zawartość w programie Word 2016.</span><span class="sxs-lookup"><span data-stu-id="cf480-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="cf480-120">Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych</span><span class="sxs-lookup"><span data-stu-id="cf480-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="cf480-121">**Sprawdzanie ustawień połączenia**</span><span class="sxs-lookup"><span data-stu-id="cf480-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="cf480-122">Na urządzeniu osobistym z systemem Windows 10, na którym użytkownik lokalny jesteś zalogowany, przejdź do **ustawień systemu Windows**i kliknij lub naciśnij pozycję Dostęp do **kont** w pracy \> **lub szkole**.</span><span class="sxs-lookup"><span data-stu-id="cf480-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="cf480-123">W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="cf480-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="cf480-124">Wprowadź poświadczenia usługi Microsoft 365 Business Premium w **oknie dialogowym Konfigurowanie konta służbowego** \> **Zaloguj się**.</span><span class="sxs-lookup"><span data-stu-id="cf480-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="cf480-125">Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="cf480-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kliknij lub naciśnij pozycję Informacje w oknie dialogowym Praca lub konto szkolne.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="cf480-127">Na stronie **Praca programu Access lub szkoła** można wyświetlić informacje o **połączeniu,** które zawierają **adres serwera zarządzania,** taki jak ten pokazany na poniższym rysunku, i zawierają słowa *wip* i *mam* wewnątrz.</span><span class="sxs-lookup"><span data-stu-id="cf480-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="cf480-129">**Sprawdź, czy nie można wkleić danych firmy w aplikacji niezarządkowej**</span><span class="sxs-lookup"><span data-stu-id="cf480-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="cf480-130">Otwórz program Outlook 2016 i w razie potrzeby dodaj konto usługi Microsoft 365 Business Premium i zaloguj się przy użyciu poświadczeń usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cf480-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="cf480-131">Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.</span><span class="sxs-lookup"><span data-stu-id="cf480-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="cf480-132">Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.</span><span class="sxs-lookup"><span data-stu-id="cf480-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="cf480-133">Zostanie wyświetlony błąd informujący, że aplikacja nie może uzyskać dostępu do zawartości.</span><span class="sxs-lookup"><span data-stu-id="cf480-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="cf480-135">Można jednak wkleić tę zawartość w programie Word 2016.</span><span class="sxs-lookup"><span data-stu-id="cf480-135">You can, however, paste the same content into Word 2016.</span></span>
    

