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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z instrukcjami konfiguracji usługi Microsoft 365 Business, od subskrypcji po dodawanie domeny i użytkowników, po konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 9bb536b52981966f6c4c487f8400577b896261e0
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561207"
---
# <a name="overview-of-setup"></a><span data-ttu-id="ef23f-103">Omówienie konfiguracji</span><span class="sxs-lookup"><span data-stu-id="ef23f-103">Overview of setup</span></span>

<span data-ttu-id="ef23f-104">Obejrzyj krótki film o konfiguracji usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ef23f-104">Watch a short video about Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="ef23f-105">Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników platformy Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="ef23f-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="ef23f-106">Większość kroków konfiguracji można wykonać w kreatorze konfiguracji, ale inne opcje są również wymienione.</span><span class="sxs-lookup"><span data-stu-id="ef23f-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="ef23f-107">Krok 1: Dodaj domenę i użytkowników</span><span class="sxs-lookup"><span data-stu-id="ef23f-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="ef23f-108">**[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji,](sign-up.md)ten krok jest już wykonany).</span><span class="sxs-lookup"><span data-stu-id="ef23f-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="ef23f-109">**Dodaj użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="ef23f-109">**Add users**.</span></span> <span data-ttu-id="ef23f-110">Możesz dodać użytkowników na jeden z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="ef23f-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="ef23f-111">W [kreatorze](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="ef23f-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="ef23f-112">Synchronizacja katalogów umożliwia [dodawanie użytkowników przy użyciu usługi Azure AD Connect,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) jeśli masz lokalny katalog Active.</span><span class="sxs-lookup"><span data-stu-id="ef23f-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="ef23f-113">Możesz również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="ef23f-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="ef23f-114">Krok 2: Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń</span><span class="sxs-lookup"><span data-stu-id="ef23f-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="ef23f-115">Użyj [Kreatora instalacji,](set-up.md#protect-your-organization) aby skonfigurować zasady dotyczące urządzeń.</span><span class="sxs-lookup"><span data-stu-id="ef23f-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="ef23f-116">Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="ef23f-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="ef23f-117">Kreator konfiguracji skonfiguruj również podstawowe ustawienia ochrony przed zagrożeniami i zapobiegania utracie danych.</span><span class="sxs-lookup"><span data-stu-id="ef23f-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="ef23f-118">Oprócz ustawień zabezpieczeń w kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="ef23f-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="ef23f-119">**Ochrona przed złośliwym oprogramowaniem poczty e-mail**</span><span class="sxs-lookup"><span data-stu-id="ef23f-119">**Email malware protection**</span></span>
- <span data-ttu-id="ef23f-120">**Ochrona przed phishingiem atp**</span><span class="sxs-lookup"><span data-stu-id="ef23f-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="ef23f-121">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="ef23f-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="ef23f-122">**Usługa Azure Information Protection (Plan1)**</span><span class="sxs-lookup"><span data-stu-id="ef23f-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="ef23f-123">Aby rozpocząć, zobacz [zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) i [konfigurowanie funkcji zgodności](set-up-compliance.md).</span><span class="sxs-lookup"><span data-stu-id="ef23f-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="ef23f-124">Zobacz też [10 najważniejszych sposobów zabezpieczenia usługi Microsoft 365 Business,](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) aby zapoznać się z planem najlepszych rozwiązań w zakresie zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="ef23f-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="ef23f-125">Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="ef23f-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="ef23f-126">Po uruchomieniu kreatora konfiguracji należy zwiększyć wszystkie komputery Windwos 10 w organizacji.</span><span class="sxs-lookup"><span data-stu-id="ef23f-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="ef23f-127">Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla microsoft 365 Business, ale jeśli masz Windows 7 Pro, Windows 8 Pro, lub Windows 8.1 Pro, subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="ef23f-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="ef23f-128">Wykonaj kroki opisane w [bezpiecznych komputerach z systemem Windows 10,](secure-win-10-pcs.md) aby skonfigurować zasady dla urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ef23f-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="ef23f-129">Po dołączeniu urządzenia z systemem Windows 10 do usługi Azure AD zasady ustawione dla komputerów z systemem Windows 10 są do niego stosowane.</span><span class="sxs-lookup"><span data-stu-id="ef23f-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="ef23f-130">Aby uzyskać więcej informacji, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="ef23f-130">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="ef23f-131">Krok 4: Instalowanie usługi Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="ef23f-131">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="ef23f-132">Pakiet Office można zainstalować automatycznie na urządzeniach z systemem Windows za pomocą [kreatora instalacji](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="ef23f-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="ef23f-133">Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="ef23f-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="ef23f-134">Zaawansowane</span><span class="sxs-lookup"><span data-stu-id="ef23f-134">Advanced</span></span>
- <span data-ttu-id="ef23f-135">**Konfigurowanie nowych urządzeń za pomocą programu Autopilot**</span><span class="sxs-lookup"><span data-stu-id="ef23f-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="ef23f-136">Za pomocą [programu Windows Autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie skonfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie.</span><span class="sxs-lookup"><span data-stu-id="ef23f-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="ef23f-137">Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta w dziedzinie technologii w chmurze o skonfigurowanie nowych kupowanego urządzeń.</span><span class="sxs-lookup"><span data-stu-id="ef23f-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="ef23f-138">**Dostęp do zasobów lokalnych**</span><span class="sxs-lookup"><span data-stu-id="ef23f-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="ef23f-139">Jeśli organizacja korzysta z lokalnego usługi Windows Server Active Directory, można skonfigurować usługę Microsoft 365 Business do ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="ef23f-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="ef23f-140">Wykonaj kroki opisane w [artykule Włącz urządzenia z systemem Windows 10 przyłączone do domeny, które mają być zarządzane przez firmę Microsoft 365 Business,](manage-windows-devices.md) aby to skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="ef23f-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="ef23f-141">Jest to preferowana metoda, a urządzenia w tym stanie są nazywane hybrydowymi urządzeniami usługi Azure AD przyłączonymi.</span><span class="sxs-lookup"><span data-stu-id="ef23f-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="ef23f-142">Jeśli twoja firma ma lokalną usługę Active Directory zawierającą pewne zasoby lokalne (takie jak udziały plików i drukarki), można przyznać urządzeniom przyłączonym do usługi Azure AD dostęp do tych zasobów, wykonując następujące kroki w tym miejscu: [Dostęp do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="ef23f-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="ef23f-143">Zobacz też</span><span class="sxs-lookup"><span data-stu-id="ef23f-143">See also</span></span>

[<span data-ttu-id="ef23f-144">Szkoleniowe klipy wideo dotyczące rozwiązania Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="ef23f-144">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
