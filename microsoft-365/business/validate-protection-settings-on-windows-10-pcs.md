---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Sprawdź poprawność ustawień ochrony aplikacji usługi Microsoft 365 Business Premium na urządzeniach z systemem Windows 10 i upewnij się, że użytkownicy nie mogą kopiować danych firmowych do plików osobistych ani do aplikacji nieza zarządzanych.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579867"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="e50bb-103">Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="e50bb-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="e50bb-104">Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych</span><span class="sxs-lookup"><span data-stu-id="e50bb-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="e50bb-105">Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e50bb-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="e50bb-106">Jeśli zostało  włączone ustawienie Uniemożliwiaj użytkownikom kopiowanie danych firmowych do plików osobistych i wymusz na nich zapisywanie plików służbowych w usłudze **OneDrive** dla Firm dla urządzeń należących do firmy, możesz to sprawdzić na urządzeniu użytkownika po połączeniu się przez tego użytkownika z usługą Azure AD i zalogowaniu.</span><span class="sxs-lookup"><span data-stu-id="e50bb-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="e50bb-107">**Sprawdzanie ustawień połączenia**</span><span class="sxs-lookup"><span data-stu-id="e50bb-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="e50bb-108">Po zalogowaniu się przy użyciu poświadczeń usługi Microsoft 365 Business Premium i nawiązyniu połączenia z usługą Azure AD zgodnie z opisem w tece Konfigurowanie urządzeń z systemem Windows dla użytkowników [usługi Microsoft 365 Business Premium](set-up-windows-devices.md)przejdź do strony Ustawienia systemu **Windows** Konta Dostępu do pracy lub \>  \> **nauki.**</span><span class="sxs-lookup"><span data-stu-id="e50bb-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="e50bb-109">Wybierz **pozycję Połączono z \<tenant name\> usługą Azure AD,** a następnie wybierz **pozycję Informacje.**</span><span class="sxs-lookup"><span data-stu-id="e50bb-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="e50bb-111">Na stronie **Zarządzane przez** możesz zobaczyć informacje o połączeniu, które zawierają adres serwera zarządzania, jak pokazano na \<tenant name\> poniższym rysunku.  </span><span class="sxs-lookup"><span data-stu-id="e50bb-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="e50bb-113">**Sprawdzanie, czy nie można wkleić danych firmowych w aplikacji nieza zarządzanych**</span><span class="sxs-lookup"><span data-stu-id="e50bb-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="e50bb-114">Otwórz program Outlook 2016 zainstalowany przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e50bb-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="e50bb-115">Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.</span><span class="sxs-lookup"><span data-stu-id="e50bb-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="e50bb-116">Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.</span><span class="sxs-lookup"><span data-stu-id="e50bb-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="e50bb-117">Zostanie wyświetlony komunikat o błędzie z komunikatem, że aplikacja nie może uzyskać dostępu do zawartości.</span><span class="sxs-lookup"><span data-stu-id="e50bb-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="e50bb-119">Można jednak wkleić tę zawartość w programie Word 2016.</span><span class="sxs-lookup"><span data-stu-id="e50bb-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="e50bb-120">Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych</span><span class="sxs-lookup"><span data-stu-id="e50bb-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="e50bb-121">**Sprawdzanie ustawień połączenia**</span><span class="sxs-lookup"><span data-stu-id="e50bb-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="e50bb-122">Na urządzeniu osobistym z systemem Windows 10, na którym zalogowano się jako użytkownik lokalny, przejdź do ustawień systemu **Windows** i kliknij lub naciśnij **pozycję** Konta Uzyskaj dostęp do miejsca pracy \> **lub nauki.**</span><span class="sxs-lookup"><span data-stu-id="e50bb-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="e50bb-123">W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="e50bb-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="e50bb-124">Wprowadź poświadczenia usługi Microsoft 365 Business Premium w oknie dialogowym Konfigurowanie **konta służbowego Zaloguj** \> **się.**</span><span class="sxs-lookup"><span data-stu-id="e50bb-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="e50bb-125">Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="e50bb-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kliknij lub naciśnij pozycję Informacje w oknie dialogowym Konto służbowe.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="e50bb-127">Na stronie Uzyskaj **dostęp** do pracy  lub nauki widoczne  są informacje o połączeniu, które zawierają adres serwera zarządzania, taki jak przedstawiony na poniższej ilustracji, oraz *wyrazy wip* i *mam* w obrębie.</span><span class="sxs-lookup"><span data-stu-id="e50bb-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="e50bb-129">**Sprawdzanie, czy nie można wkleić danych firmowych w aplikacji nieza zarządzanych**</span><span class="sxs-lookup"><span data-stu-id="e50bb-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="e50bb-130">Otwórz program Outlook 2016 i w razie potrzeby dodaj konto Microsoft 365 Business Premium i zaloguj się przy użyciu poświadczeń platformy Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e50bb-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="e50bb-131">Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.</span><span class="sxs-lookup"><span data-stu-id="e50bb-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="e50bb-132">Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.</span><span class="sxs-lookup"><span data-stu-id="e50bb-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="e50bb-133">Zostanie wyświetlony komunikat o błędzie z komunikatem Aplikacja nie może uzyskać dostępu do zawartości.</span><span class="sxs-lookup"><span data-stu-id="e50bb-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="e50bb-135">Można jednak wkleić tę zawartość w programie Word 2016.</span><span class="sxs-lookup"><span data-stu-id="e50bb-135">You can, however, paste the same content into Word 2016.</span></span>
    

