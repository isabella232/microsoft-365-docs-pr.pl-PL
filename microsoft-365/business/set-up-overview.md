---
title: Omówienie konfiguracji
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z czynnościami konfiguracyjną usługi Microsoft 365 Business Premium, od subskrybowania, dodawania domeny i użytkowników po konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579939"
---
# <a name="overview-of-setup"></a><span data-ttu-id="62c72-103">Omówienie konfiguracji</span><span class="sxs-lookup"><span data-stu-id="62c72-103">Overview of setup</span></span>

<span data-ttu-id="62c72-104">Obejrzyj krótki klip wideo o konfiguracji usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="62c72-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="62c72-105">Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="62c72-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="62c72-106">Większość kroków konfiguracji można wykonać przy instalacji ze przewodnikiem, ale wymienione są również inne opcje.</span><span class="sxs-lookup"><span data-stu-id="62c72-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="62c72-107">Krok 1. Dodawanie domeny i użytkowników</span><span class="sxs-lookup"><span data-stu-id="62c72-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="62c72-108">**[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji](sign-up.md), ten krok jest już wykonane).</span><span class="sxs-lookup"><span data-stu-id="62c72-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="62c72-109">**Dodaj użytkowników.**</span><span class="sxs-lookup"><span data-stu-id="62c72-109">**Add users**.</span></span> <span data-ttu-id="62c72-110">Użytkowników możesz dodać na jeden z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="62c72-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="62c72-111">W konfiguracji [z przewodnikiem](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="62c72-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="62c72-112">Użyj synchronizacji [katalogów, aby dodać użytkowników za pomocą programu Azure AD Connect,](../enterprise/set-up-directory-synchronization.md) jeśli masz lokalną usługę Active Directory.</span><span class="sxs-lookup"><span data-stu-id="62c72-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="62c72-113">Użytkowników możesz [również dodać w dalszej](../admin/add-users/add-users.md) części centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="62c72-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="62c72-114">Krok 2. Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń</span><span class="sxs-lookup"><span data-stu-id="62c72-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="62c72-115">Skonfiguruj zasady dotyczące urządzeń [przy](set-up.md#protect-your-organization) użyciu konfiguracji ze przewodnikiem.</span><span class="sxs-lookup"><span data-stu-id="62c72-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="62c72-116">Możesz również dodać więcej lub edytować je później w centrum administracyjnym i w [portalu Intune.](/intune/tutorial-walkthrough-intune-portal) [](view-policies-and-devices.md)</span><span class="sxs-lookup"><span data-stu-id="62c72-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="62c72-117">Kreator konfiguracji skonfiguruje również podstawowe ustawienia ochrony przed zagrożeniami i utratą danych.</span><span class="sxs-lookup"><span data-stu-id="62c72-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="62c72-118">Oprócz ustawień zabezpieczeń w kreatorze konfiguracji możesz zwiększyć poziom zabezpieczeń, dodając następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="62c72-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="62c72-119">**Ochrona przed złośliwym oprogramowaniem w wiadomościach e-mail**</span><span class="sxs-lookup"><span data-stu-id="62c72-119">**Email malware protection**</span></span>
- <span data-ttu-id="62c72-120">**Ochrona przed wyłudzaniem informacji w usłudze Defender dla usługi Office 365**</span><span class="sxs-lookup"><span data-stu-id="62c72-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="62c72-121">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="62c72-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="62c72-122">**Azure Information Protection (plan1)**</span><span class="sxs-lookup"><span data-stu-id="62c72-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="62c72-123">Aby rozpocząć, zobacz [Zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) [i konfigurowanie funkcji zgodności.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="62c72-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="62c72-124">Zapoznaj się również z 10 najlepszymi sposobami zabezpieczania usługi [Microsoft 365 Business Premium,](/office365/admin/security-and-compliance/secure-your-business-data) aby uzyskać drogową mapę z najlepszymi rozwiązaniami w zakresie zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="62c72-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="62c72-125">Krok 3. Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="62c72-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="62c72-126">Po zakończeniu konfiguracji ze przewodnikiem należy chronić wszystkie komputery z systemem Windows 10 w organizacji.</span><span class="sxs-lookup"><span data-stu-id="62c72-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="62c72-127">System Windows 10 [](pre-requisites-for-data-protection.md) Pro stanowi wymaganie wstępne dla usługi Microsoft 365 Business Premium, ale jeśli masz system Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja uprawnia do uaktualnienia do systemu [Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="62c72-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="62c72-128">Postępuj zgodnie z instrukcjami w zabezpieczaniu komputerów z systemem [Windows 10,](secure-win-10-pcs.md) aby skonfigurować zasady dla urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="62c72-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="62c72-129">Po dołączeniu urządzenia z systemem Windows 10 do usługi Azure AD są do niej stosowane zasady ustawione dla komputerów z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="62c72-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="62c72-130">Aby uzyskać więcej informacji, [zobacz Konfigurowanie urządzeń z systemem Windows dla użytkowników platformy Microsoft 365.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="62c72-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="62c72-131">Krok 4. Instalowanie aplikacji platformy Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="62c72-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="62c72-132">Pakiet Office na urządzeniach z systemem Windows można zainstalować automatycznie za pomocą [kreatora konfiguracji.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="62c72-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="62c72-133">Umożliwianie [użytkownikom instalowania aplikacji pakietu Office](/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="62c72-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="62c72-134">Advanced</span><span class="sxs-lookup"><span data-stu-id="62c72-134">Advanced</span></span>
- <span data-ttu-id="62c72-135">**Konfigurowanie nowych urządzeń za pomocą rozwiązania Autopilot**</span><span class="sxs-lookup"><span data-stu-id="62c72-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="62c72-136">Rozwiązania [Windows Autopilot](add-autopilot-devices-and-profile.md) można użyć do automatycznego wstępnego skonfigurowania nowych urządzeń z systemem **Windows** 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie.</span><span class="sxs-lookup"><span data-stu-id="62c72-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="62c72-137">Możesz również przejść do [Sklepu Microsoft](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta z technologii w chmurze o skonfigurowanie nowych, kupowanych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="62c72-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="62c72-138">**Zasoby lokalne programu Access**</span><span class="sxs-lookup"><span data-stu-id="62c72-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="62c72-139">Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="62c72-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="62c72-140">Aby skonfigurować to ustawienie, wykonaj czynności opisane w tece Włączanie zarządzania przez usługę [Microsoft 365 Business Premium](manage-windows-devices.md) dla urządzeń przyłączanych do domeny systemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="62c72-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="62c72-141">Jest to preferowana metoda, a urządzenia w tym stanie mają nazwę Urządzenia sprzężenia hybrydowego usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="62c72-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="62c72-142">Jeśli Twoja firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udzielić swoim urządzeniu przyłączony do usługi Azure AD dostępu do tych zasobów, korzystając z procedury opisanej w tym miejscu: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze [Microsoft 365 Business Premium.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="62c72-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="62c72-143">Zobacz też</span><span class="sxs-lookup"><span data-stu-id="62c72-143">See also</span></span>

[<span data-ttu-id="62c72-144">Szkoleniowe klipy wideo dotyczące platformy Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="62c72-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)