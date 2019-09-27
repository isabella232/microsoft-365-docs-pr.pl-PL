---
title: Omówienie konfigurowania
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Omówienie konfigurowania kroków dla Microsoft 365 Business.
ms.openlocfilehash: f156d236a783942ec06d457c9b7ca087d12d6f58
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288580"
---
# <a name="overview-of-setup"></a><span data-ttu-id="a7312-103">Przegląd ustawień</span><span class="sxs-lookup"><span data-stu-id="a7312-103">Overview of setup</span></span>

<span data-ttu-id="a7312-104">Większość kroków konfiguracji można wykonać w Kreatorze instalacji, ale inne opcje są również wymienione.</span><span class="sxs-lookup"><span data-stu-id="a7312-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="a7312-105">Krok 1: Dodaj domenę i użytkowników</span><span class="sxs-lookup"><span data-stu-id="a7312-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="a7312-106">**[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (Jeśli Twoja domena została [kupiona podczas rejestracji](sign-up.md), ten krok jest już zrobione).</span><span class="sxs-lookup"><span data-stu-id="a7312-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="a7312-107">**Dodawanie użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="a7312-107">**Add users**.</span></span> <span data-ttu-id="a7312-108">Można to zrobić na trzy sposoby:</span><span class="sxs-lookup"><span data-stu-id="a7312-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="a7312-109">W [Kreatorze](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="a7312-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="a7312-110">Użyj synchronizacji katalogów, aby [dodać użytkowników przy użyciu programu Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jeśli masz lokalną usługę Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a7312-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="a7312-111">Możesz także [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="a7312-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="a7312-112">Krok 2: Konfigurowanie zasad zabezpieczeń i Konfigurowanie urządzeń</span><span class="sxs-lookup"><span data-stu-id="a7312-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="a7312-113">Skonfiguruj zasady dotyczące urządzeń i zabezpieczeń za pomocą [Kreatora instalacji](set-up.md#set-up-security-policies-and-device-configurations) .</span><span class="sxs-lookup"><span data-stu-id="a7312-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="a7312-114">Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="a7312-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="a7312-115">Oprócz ustawień zabezpieczeń w Kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="a7312-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="a7312-116">**Ochrona przed złośliwym oprogramowaniem poczty e-mail**</span><span class="sxs-lookup"><span data-stu-id="a7312-116">**Email malware protection**</span></span>
      - <span data-ttu-id="a7312-117">**Zaawansowane zabezpieczenia przed zagrożeniami (ATP) bezpieczne łącza**</span><span class="sxs-lookup"><span data-stu-id="a7312-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="a7312-118">**Bezpieczne załączniki ATP**</span><span class="sxs-lookup"><span data-stu-id="a7312-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="a7312-119">**ATP anty-phishing**</span><span class="sxs-lookup"><span data-stu-id="a7312-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="a7312-120">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="a7312-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="a7312-121">**Zapobieganie utracie danych (DLP)**</span><span class="sxs-lookup"><span data-stu-id="a7312-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="a7312-122">**Ochrona informacji Azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="a7312-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="a7312-123">Aby rozpocząć, zobacz [Konfigurowanie zaawansowanych zasad zabezpieczeń](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="a7312-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="a7312-124">Zobacz także [10 najlepszych sposobów zabezpieczania Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) dla planu najlepszych praktyk w zakresie bezpieczeństwa.</span><span class="sxs-lookup"><span data-stu-id="a7312-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="a7312-125">Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="a7312-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="a7312-126">Po przyłączeniu urządzenia systemu Windows 10 do usługi Azure AD, zasady skonfigurowane w [kroku 2](#step-2-set-up-security-policies-and-configure-devices) Get stosowane do niego.</span><span class="sxs-lookup"><span data-stu-id="a7312-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="a7312-127">Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla Microsoft 365 Business, ale jeśli masz Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="a7312-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="a7312-128">Użyj [Kreatora konfiguracji](set-up.md#set-up-security-policies-and-device-configurations) , aby skonfigurować zasady dla urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a7312-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="a7312-129">Stes 4: instalacja pakietu Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="a7312-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="a7312-130">Pakiet Office można automatycznie zainstalować na urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="a7312-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="a7312-131">Automatycznie [Zainstaluj pakiet Office](auto-install-or-uninstall-office.md) z centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="a7312-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="a7312-132">Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="a7312-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="a7312-133">Zaawansowane</span><span class="sxs-lookup"><span data-stu-id="a7312-133">Advanced</span></span>
- <span data-ttu-id="a7312-134">**Konfigurowanie nowych urządzeń za pomocą autopilota**</span><span class="sxs-lookup"><span data-stu-id="a7312-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="a7312-135">Za pomocą programu [Windows autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie konfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może to zrobić dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="a7312-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="a7312-136">Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) i poprosić eksperta w zakresie technologii chmurowej o ustawienie nowych urządzeń, które zakupisz.</span><span class="sxs-lookup"><span data-stu-id="a7312-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="a7312-137">**Dostęp do zasobów lokalnych**</span><span class="sxs-lookup"><span data-stu-id="a7312-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="a7312-138">Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="a7312-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="a7312-139">Wykonaj kroki opisane w [Włączanie przyłączonych do domeny urządzeń z systemem Windows 10, które mają być zarządzane przez firmę Microsoft 365 Business](manage-windows-devices.md) , aby to skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="a7312-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="a7312-140">Jest to preferowana metoda i urządzenia w tym stanie są nazywane hybrydowych urządzeń przyłączonych do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a7312-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="a7312-141">Jeśli Twoja firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz nadać urządzeniom przyłączonym do usługi Azure AD dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostęp do zasobów lokalnych z Urządzenie przyłączone do usługi Azure AD w Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="a7312-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  