---
title: Omówienie konfiguracji
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Zapoznaj się z instrukcjami dotyczącymi konfiguracji usługi Microsoft 365 Business Premium, od subskrybowania, dodawania domeny i użytkowników, konfigurowania zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: a808ae5761c1bc5706966a3f7de95f96f8f7c8c8
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785817"
---
# <a name="overview-of-setup"></a><span data-ttu-id="4cdbc-103">Omówienie konfiguracji</span><span class="sxs-lookup"><span data-stu-id="4cdbc-103">Overview of setup</span></span>

<span data-ttu-id="4cdbc-104">Obejrzyj krótki film o konfiguracji usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="4cdbc-105">Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="4cdbc-106">Większość czynności konfiguracyjnych można wykonać w kreatorze instalacji, ale inne opcje są również wymienione.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="4cdbc-107">Krok 1: Dodaj swoją domenę i użytkowników</span><span class="sxs-lookup"><span data-stu-id="4cdbc-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="4cdbc-108">**[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji,](sign-up.md)ten krok jest już wykonany).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="4cdbc-109">**Dodaj użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-109">**Add users**.</span></span> <span data-ttu-id="4cdbc-110">Użytkownicy można dodawać na dowolny z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="4cdbc-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="4cdbc-111">W [kreatorze](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="4cdbc-112">Użyj synchronizacji katalogów, aby [dodać użytkowników przy użyciu usługi Azure AD Connect,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) jeśli masz lokalną usługę Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="4cdbc-113">Można również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="4cdbc-114">Krok 2: Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń</span><span class="sxs-lookup"><span data-stu-id="4cdbc-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="4cdbc-115">Użyj [Kreatora instalacji,](set-up.md#protect-your-organization) aby skonfigurować zasady urządzeń.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="4cdbc-116">Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="4cdbc-117">Kreator konfiguracji skonfiguruje również podstawowe ustawienia ochrony przed zagrożeniami i utraty danych.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="4cdbc-118">Oprócz ustawień zabezpieczeń w kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="4cdbc-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="4cdbc-119">**Ochrona przed złośliwym oprogramowaniem pocztą e-mail**</span><span class="sxs-lookup"><span data-stu-id="4cdbc-119">**Email malware protection**</span></span>
- <span data-ttu-id="4cdbc-120">**Atp anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="4cdbc-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="4cdbc-121">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="4cdbc-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="4cdbc-122">**Ochrona informacji platformy Azure (Plan1)**</span><span class="sxs-lookup"><span data-stu-id="4cdbc-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="4cdbc-123">Aby rozpocząć, zobacz [zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) i [konfigurowanie funkcji zgodności](set-up-compliance.md).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="4cdbc-124">Zobacz też [10 najważniejszych sposobów zabezpieczenia usługi Microsoft 365 Business Premium, aby](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) uzyskać plan działania dotyczący najlepszych rozwiązań w zakresie zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="4cdbc-125">Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="4cdbc-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="4cdbc-126">Po uruchomieniu kreatora konfiguracji należy zwlekać z uruchomieniem wszystkich komputerów Windwos 10 w organizacji.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="4cdbc-127">Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla Microsoft 365 Business Premium, ale jeśli masz Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, twoja subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="4cdbc-128">Wykonaj kroki opisane w [bezpiecznych komputerach z systemem Windows 10,](secure-win-10-pcs.md) aby skonfigurować zasady dla urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="4cdbc-129">Po dołączeniu urządzenia z systemem Windows 10 do usługi Azure AD, zasady ustawione dla komputerów z systemem Windows 10 są stosowane do niego.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="4cdbc-130">Aby uzyskać więcej informacji, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="4cdbc-131">Krok 4: Instalowanie aplikacji usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="4cdbc-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="4cdbc-132">Pakiet Office można instalować automatycznie na urządzeniach z systemem Windows za pomocą [kreatora konfiguracji](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="4cdbc-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="4cdbc-133">Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="4cdbc-134">Zaawansowane</span><span class="sxs-lookup"><span data-stu-id="4cdbc-134">Advanced</span></span>
- <span data-ttu-id="4cdbc-135">**Konfigurowanie nowych urządzeń za pomocą autopilota**</span><span class="sxs-lookup"><span data-stu-id="4cdbc-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="4cdbc-136">Za pomocą [programu Windows Autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie skonfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="4cdbc-137">Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta w dziedzinie technologii w chmurze o skonfigurowanie zakupionych nowych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="4cdbc-138">**Dostęp do zasobów lokalnych**</span><span class="sxs-lookup"><span data-stu-id="4cdbc-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="4cdbc-139">Jeśli twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, można skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="4cdbc-140">Wykonaj kroki opisane w [obszarze Włączanie urządzeń z systemem Windows 10 przyłączonych do domeny, które mają być zarządzane przez usługę Microsoft 365 Business Premium,](manage-windows-devices.md) aby to skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="4cdbc-141">Jest to preferowana metoda, a urządzenia w tym stanie są nazywane urządzeniami przyłączanym do usługi Hybrid Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4cdbc-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="4cdbc-142">Jeśli twoja firma ma lokalną usługę Active Directory zawierającą pewne zasoby lokalne (takie jak udziały plików i drukarki), możesz przyznać urządzeniom korzystającym z usługi Azure AD dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [Dostęp do zasobów lokalnych z urządzenia przyłączanego do usługi Azure AD w usłudze Microsoft 365 Business Premium.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="4cdbc-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="4cdbc-143">Zobacz też</span><span class="sxs-lookup"><span data-stu-id="4cdbc-143">See also</span></span>

[<span data-ttu-id="4cdbc-144">Wideo dotyczące szkoleń dotyczących usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="4cdbc-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
