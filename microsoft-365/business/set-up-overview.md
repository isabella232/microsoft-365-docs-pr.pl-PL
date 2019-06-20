---
title: Omówienie konfiguracji
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Przegląd ustaw kroki dla Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086368"
---
# <a name="overview-of-setup"></a><span data-ttu-id="5f5ef-103">Przegląd ustawień</span><span class="sxs-lookup"><span data-stu-id="5f5ef-103">Overview of setup</span></span>

<span data-ttu-id="5f5ef-104">Większość ustawień czynności może odbywać się w Kreatorze instalacji, ale inne opcje są również wyświetlane.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="5f5ef-105">Krok 1: Dodawanie użytkownika domeny i użytkownicy</span><span class="sxs-lookup"><span data-stu-id="5f5ef-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="5f5ef-106">**[Dodawanie domeny](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli kupiłeś domeny podczas [zarejestrować się](sign-up.md), ten krok jest już zrobione.)</span><span class="sxs-lookup"><span data-stu-id="5f5ef-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="5f5ef-107">**Dodaj użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-107">**Add users**.</span></span> <span data-ttu-id="5f5ef-108">Możesz to zrobić na jeden z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="5f5ef-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="5f5ef-109">W oknie [Kreatora](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="5f5ef-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="5f5ef-110">Użyj synchronizacji katalogów, aby [dodać użytkowników za pomocą Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jeśli masz lokalnej usługi Active directory.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="5f5ef-111">Można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="5f5ef-112">Krok 2: Ustawianie zasad zabezpieczeń i konfigurowania urządzeń</span><span class="sxs-lookup"><span data-stu-id="5f5ef-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="5f5ef-113">[Kreator konfiguracji](set-up.md#set-up-security-policies-and-device-configurations) umożliwia skonfigurowanie urządzenia i zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="5f5ef-114">Można również dodać więcej lub edytować je później w [Centrum administracyjnego](view-policies-and-devices.md) i [portal Windows Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="5f5ef-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="5f5ef-115">Oprócz ustawień zabezpieczeń w Kreatorze instalacji ze względów bezpieczeństwa można zwiększyć przez dodanie następujących ustawień:</span><span class="sxs-lookup"><span data-stu-id="5f5ef-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="5f5ef-116">**E-mail, ochrona przed złośliwym oprogramowaniem**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-116">**Email malware protection**</span></span>
      - <span data-ttu-id="5f5ef-117">**Zaawansowane zagrożenia ochrony (ATP) bezpiecznego łącza**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="5f5ef-118">**Załączników bezpieczne ATP**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="5f5ef-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="5f5ef-120">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="5f5ef-121">**Zapobieganie utracie danych (DLP)**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="5f5ef-122">**Ochrony informacji azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="5f5ef-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="5f5ef-123">Aby rozpocząć, zobacz [Konfigurowanie zasad zabezpieczeń zaawansowanych](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="5f5ef-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="5f5ef-124">Zobacz też [top 10 sposobów zabezpieczenia firmy Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) do utworzenia planu działań najważniejsze wskazówki dotyczące zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="5f5ef-125">Krok 3: Konfigurowanie urządzeń i zarządzanie nimi 10 systemu Windows</span><span class="sxs-lookup"><span data-stu-id="5f5ef-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="5f5ef-126">Po dołączeniu urządzenia Windows 10 do Azure AD, zasady ustawione w [kroku 2](#step-2-set-up-security-policies-and-configure-devices) będzie stosowane do niego.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="5f5ef-127">Windows 10 Pro jest [wstępnie wymagane](pre-requisites-for-data-protection.md) dla Microsoft 365 Business, ale jeśli masz system Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro subskrypcji uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="5f5ef-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="5f5ef-128">[Kreator konfiguracji](set-up.md#set-up-security-policies-and-device-configurations) umożliwia konfigurowanie zasad dla urządzeń Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="5f5ef-129">Wprowadzają 4: Zainstalować Business Office 365</span><span class="sxs-lookup"><span data-stu-id="5f5ef-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="5f5ef-130">Można automatycznie zainstalować pakiet Office w urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="5f5ef-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="5f5ef-131">Automatycznie [zainstalować pakiet Office](auto-install-or-uninstall-office.md) z Centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="5f5ef-132">Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="5f5ef-133">Zaawansowane</span><span class="sxs-lookup"><span data-stu-id="5f5ef-133">Advanced</span></span>
- <span data-ttu-id="5f5ef-134">**Służy do definiowania nowych urządzeń autopilota**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="5f5ef-135">Można użyć [Windows Autopilot](add-autopilot-devices-and-profile.md) automatycznie wstępnie skonfigurować **Nowe** urządzenia Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może zrobić to dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="5f5ef-136">Można także przejść do [Magazyn Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) i zapytać specjalisty w zakresie technologii cloud Ustawianie nowych urządzeń, które kupić dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="5f5ef-137">**Dostęp do zasobów lokalnych**</span><span class="sxs-lookup"><span data-stu-id="5f5ef-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="5f5ef-138">Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="5f5ef-139">Postępuj zgodnie z instrukcjami [włączyć przyłączonych do domeny Windows 10 urządzenia mają być zarządzane przez Microsoft 365 Business](manage-windows-devices.md) można wybrać tę opcję.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="5f5ef-140">Jest to preferowana metoda i urządzeń, w tym stanie są nazywane hybrydowy Azure AD dołączył do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="5f5ef-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="5f5ef-141">Jeśli Twoja firma ma lokalnej usługi Active Directory, który zawiera niektóre zasobów lokalnych (takich jak udziały plików i drukarek), może dać Azure AD przyłączony urządzeniom dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostępu do zasobów lokalnych z Azure AD dołączył do urządzenia w Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="5f5ef-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  