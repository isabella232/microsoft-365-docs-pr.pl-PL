---
title: Przegląd ustawień
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Omówienie kroków konfiguracji dla Microsoft 365 Business.
ms.openlocfilehash: 3447f06d031462a7bebc6f129238de9f0c5dee41
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721564"
---
# <a name="overview-of-setup"></a><span data-ttu-id="1f189-103">Przegląd ustawień</span><span class="sxs-lookup"><span data-stu-id="1f189-103">Overview of setup</span></span>

<span data-ttu-id="1f189-104">Większość czynności konfiguracyjnych można wykonać w Kreatorze instalacji, ale wyświetlane są również inne opcje.</span><span class="sxs-lookup"><span data-stu-id="1f189-104">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="1f189-105">Krok 1: Dodaj domenę i użytkowników</span><span class="sxs-lookup"><span data-stu-id="1f189-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="1f189-106">**[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (Jeśli Twoja domena została [kupiona podczas rejestracji](sign-up.md), ten krok jest już zrobione).</span><span class="sxs-lookup"><span data-stu-id="1f189-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="1f189-107">**Dodawanie użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="1f189-107">**Add users**.</span></span> <span data-ttu-id="1f189-108">Możesz dodać użytkowników na trzy sposoby:</span><span class="sxs-lookup"><span data-stu-id="1f189-108">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="1f189-109">W [Kreatorze](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="1f189-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="1f189-110">Użyj synchronizacji katalogów, aby [dodać użytkowników przy użyciu programu Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jeśli masz lokalną usługę Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1f189-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="1f189-111">Możesz także [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="1f189-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="1f189-112">Krok 2: Konfigurowanie zasad zabezpieczeń i Konfigurowanie urządzeń</span><span class="sxs-lookup"><span data-stu-id="1f189-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="1f189-113">Skonfiguruj zasady dotyczące urządzeń i zabezpieczeń za pomocą [Kreatora instalacji](set-up.md#protect-data-and-devices) .</span><span class="sxs-lookup"><span data-stu-id="1f189-113">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure device and security policies.</span></span> 
  - <span data-ttu-id="1f189-114">Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="1f189-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="1f189-115">Oprócz ustawień zabezpieczeń w Kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="1f189-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="1f189-116">**Ochrona przed złośliwym oprogramowaniem poczty e-mail**</span><span class="sxs-lookup"><span data-stu-id="1f189-116">**Email malware protection**</span></span>
      - <span data-ttu-id="1f189-117">**Zaawansowane zabezpieczenia przed zagrożeniami (ATP) bezpieczne łącza**</span><span class="sxs-lookup"><span data-stu-id="1f189-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="1f189-118">**Bezpieczne załączniki ATP**</span><span class="sxs-lookup"><span data-stu-id="1f189-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="1f189-119">**ATP anty-phishing**</span><span class="sxs-lookup"><span data-stu-id="1f189-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="1f189-120">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="1f189-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="1f189-121">**Zapobieganie utracie danych (DLP)**</span><span class="sxs-lookup"><span data-stu-id="1f189-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="1f189-122">**Ochrona informacji Azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="1f189-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="1f189-123">Aby rozpocząć, zobacz [Konfigurowanie zaawansowanych zasad zabezpieczeń](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="1f189-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="1f189-124">Zobacz także [10 najlepszych sposobów zabezpieczania Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) dla planu najlepszych praktyk w zakresie bezpieczeństwa.</span><span class="sxs-lookup"><span data-stu-id="1f189-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="1f189-125">Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="1f189-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="1f189-126">Po przyłączeniu urządzenia systemu Windows 10 do usługi Azure AD, zasady skonfigurowane w [kroku 2](#step-2-set-up-security-policies-and-configure-devices) Get stosowane do niego.</span><span class="sxs-lookup"><span data-stu-id="1f189-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="1f189-127">Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla Microsoft 365 Business, ale jeśli masz Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="1f189-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="1f189-128">Użyj [Kreatora konfiguracji](set-up.md#protect-data-and-devices) , aby skonfigurować zasady dla urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1f189-128">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure policies for Windows 10 devices.</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="1f189-129">Krok 4: instalacja pakietu Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="1f189-129">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="1f189-130">Pakiet Office można automatycznie zainstalować na urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="1f189-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="1f189-131">Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="1f189-131">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="1f189-132">Zaawansowane</span><span class="sxs-lookup"><span data-stu-id="1f189-132">Advanced</span></span>
- <span data-ttu-id="1f189-133">**Konfigurowanie nowych urządzeń za pomocą autopilota**</span><span class="sxs-lookup"><span data-stu-id="1f189-133">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="1f189-134">Za pomocą programu [Windows autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie konfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może to zrobić dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="1f189-134">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="1f189-135">Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta w zakresie technologii chmurowej o konfigurowanie nowych urządzeń, które kupujesz.</span><span class="sxs-lookup"><span data-stu-id="1f189-135">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="1f189-136">**Dostęp do zasobów lokalnych**</span><span class="sxs-lookup"><span data-stu-id="1f189-136">**Access on-premises resources**</span></span>

     - <span data-ttu-id="1f189-137">Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="1f189-137">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="1f189-138">Wykonaj kroki opisane w [Włączanie przyłączonych do domeny urządzeń z systemem Windows 10, które mają być zarządzane przez firmę Microsoft 365 Business](manage-windows-devices.md) , aby to skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="1f189-138">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="1f189-139">Jest to preferowana metoda, a urządzenia w tym stanie nazywane są urządzeniami przyłączone do hybrydowej usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1f189-139">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="1f189-140">Jeśli firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (na przykład udziały plików i drukarki), możesz nadać urządzeniom przyłączonym do usługi Azure AD dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: dostęp do [zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="1f189-140">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  