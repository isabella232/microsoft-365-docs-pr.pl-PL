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
description: Zapoznaj się z krokami konfiguracji Microsoft 365 Business Premium, od subskrybowania, dodawania domeny i użytkowników po konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245069"
---
# <a name="overview-of-setup"></a><span data-ttu-id="178b8-103">Omówienie konfiguracji</span><span class="sxs-lookup"><span data-stu-id="178b8-103">Overview of setup</span></span>

<span data-ttu-id="178b8-104">Obejrzyj krótki klip wideo na temat Microsoft 365 Business Premium konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="178b8-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="178b8-105">Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="178b8-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>

<span data-ttu-id="178b8-106">Większość kroków konfiguracji można wykonać przy instalacji ze przewodnikiem, ale wymienione są również inne opcje.</span><span class="sxs-lookup"><span data-stu-id="178b8-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="178b8-107">Krok 1. Dodawanie domeny i użytkowników</span><span class="sxs-lookup"><span data-stu-id="178b8-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="178b8-108">**[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji](sign-up.md), ten krok jest już wykonane).</span><span class="sxs-lookup"><span data-stu-id="178b8-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="178b8-109">**Dodaj użytkowników.**</span><span class="sxs-lookup"><span data-stu-id="178b8-109">**Add users**.</span></span> <span data-ttu-id="178b8-110">Użytkowników możesz dodać na jeden z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="178b8-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="178b8-111">W konfiguracji [z przewodnikiem](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="178b8-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="178b8-112">Użyj synchronizacji [katalogów, aby dodać użytkowników przy użyciu usługi Azure AD Połączenie,](../enterprise/set-up-directory-synchronization.md) jeśli masz lokalną usługę Active Directory.</span><span class="sxs-lookup"><span data-stu-id="178b8-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="178b8-113">Użytkowników możesz [również dodać w dalszej](../admin/add-users/add-users.md) części centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="178b8-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="178b8-114">Krok 2. Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń</span><span class="sxs-lookup"><span data-stu-id="178b8-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="178b8-115">Skonfiguruj zasady dotyczące urządzeń [przy](set-up.md#protect-your-organization) użyciu konfiguracji ze przewodnikiem.</span><span class="sxs-lookup"><span data-stu-id="178b8-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="178b8-116">Możesz również dodać więcej lub edytować je później w centrum administracyjnym i w [portalu Intune.](/intune/tutorial-walkthrough-intune-portal) [](view-policies-and-devices.md)</span><span class="sxs-lookup"><span data-stu-id="178b8-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="178b8-117">Kreator konfiguracji skonfiguruje również podstawowe ustawienia ochrony przed zagrożeniami i utratą danych.</span><span class="sxs-lookup"><span data-stu-id="178b8-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="178b8-118">Oprócz ustawień zabezpieczeń w kreatorze konfiguracji możesz zwiększyć poziom zabezpieczeń, dodając następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="178b8-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="178b8-119">**Ochrona przed złośliwym oprogramowaniem w wiadomościach e-mail**</span><span class="sxs-lookup"><span data-stu-id="178b8-119">**Email malware protection**</span></span>
- <span data-ttu-id="178b8-120">**Ochrona przed wyłudzaniem informacji w programie Defender dla Office 365**</span><span class="sxs-lookup"><span data-stu-id="178b8-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="178b8-121">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="178b8-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="178b8-122">**Azure Information Protection (plan1)**</span><span class="sxs-lookup"><span data-stu-id="178b8-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="178b8-123">Aby rozpocząć, zobacz [Zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) [i konfigurowanie funkcji zgodności.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="178b8-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="178b8-124">Zobacz [również 10 najlepszych](/office365/admin/security-and-compliance/secure-your-business-data) sposobów zabezpieczania konta Microsoft 365 Business Premium, aby uzyskać plan najlepszych rozwiązań w zakresie zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="178b8-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="178b8-125">Krok 3. Konfigurowanie urządzeń przenośnych i Windows 10 zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="178b8-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="178b8-126">Po zakończeniu konfiguracji ze przewodnikiem należy chronić wszystkie Windows 10 w organizacji.</span><span class="sxs-lookup"><span data-stu-id="178b8-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="178b8-127">Windows 10 Pro wymaga wstępnie [](pre-requisites-for-data-protection.md) wersji Microsoft 365 Business Premium, ale jeśli masz subskrypcję usługi Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja uprawnia do uaktualnienia do systemu [Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="178b8-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="178b8-128">Postępuj zgodnie z instrukcjami w [zabezpieczaniu Windows 10 PC,](secure-win-10-pcs.md) aby skonfigurować zasady dotyczące Windows 10 komputerach.</span><span class="sxs-lookup"><span data-stu-id="178b8-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="178b8-129">Po dołączeniu urządzenia Windows 10 do usługi Azure AD są do niej stosowane zasady ustawione dla Windows 10 komputerów.</span><span class="sxs-lookup"><span data-stu-id="178b8-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="178b8-130">Aby uzyskać więcej informacji, [zobacz Konfigurowanie Windows dla Microsoft 365 użytkowników.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="178b8-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="178b8-131">Krok 4. Instalowanie Aplikacje Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="178b8-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="178b8-132">Możesz automatycznie zainstalować Office urządzeniach Windows urządzeniach przy użyciu [kreatora konfiguracji.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="178b8-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="178b8-133">Umożliwianie [użytkownikom Office aplikacji dla](/office365/admin/setup/install-applications) Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="178b8-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="178b8-134">Advanced</span><span class="sxs-lookup"><span data-stu-id="178b8-134">Advanced</span></span>
- <span data-ttu-id="178b8-135">**Konfigurowanie nowych urządzeń za pomocą rozwiązania Autopilot**</span><span class="sxs-lookup"><span data-stu-id="178b8-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="178b8-136">Możesz użyć rozwiązania [Windows Autopilot,](add-autopilot-devices-and-profile.md) aby  automatycznie wstępnie skonfigurować nowe urządzenia Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie.</span><span class="sxs-lookup"><span data-stu-id="178b8-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="178b8-137">Możesz również przejść do [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), a następnie poprosić eksperta z technologii w chmurze o skonfigurowanie nowych kupowanych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="178b8-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="178b8-138">**Zasoby lokalne programu Access**</span><span class="sxs-lookup"><span data-stu-id="178b8-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="178b8-139">Jeśli Twoja organizacja korzysta z lokalnej usługi Windows Server Active Directory, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="178b8-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="178b8-140">Postępuj zgodnie z instrukcjami w włączanie zarządzania przez Windows 10 [przyłączone](manage-windows-devices.md) do domeny przez Microsoft 365 Business Premium, aby to skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="178b8-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="178b8-141">Jest to preferowana metoda, a urządzenia w tym stanie mają nazwę Urządzenia sprzężenia hybrydowego usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="178b8-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="178b8-142">Jeśli Twoja firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udzielić swoim urządzeniu przyłączony do usługi Azure AD dostępu do tych zasobów, korzystając z procedury opisanej tutaj: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie [Microsoft 365 Business Premium.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="178b8-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="related-content"></a><span data-ttu-id="178b8-143">Zawartość powiązana</span><span class="sxs-lookup"><span data-stu-id="178b8-143">Related content</span></span>

<span data-ttu-id="178b8-144">[Microsoft 365 szkoleniowe klipy wideo dla firm](../business-video/index.yml) (strona linku)</span><span class="sxs-lookup"><span data-stu-id="178b8-144">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>