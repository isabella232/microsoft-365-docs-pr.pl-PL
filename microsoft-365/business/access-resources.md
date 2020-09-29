---
title: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak linia aplikacji biznesowych, udziały plików i drukarki z urządzenia usługi Azure Active Directory połączonego z systemem Windows 10.
ms.openlocfilehash: 2144268f5cbab67c39d5902622c61c0c35e6481c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295315"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="03e13-103">Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="03e13-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="03e13-104">Ten artykuł dotyczy programu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="03e13-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="03e13-105">Wszystkie urządzenia z systemem Windows 10, które są połączone z usługą Azure Active Directory, mają dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje Microsoft 365, i mogą być chronione przez firmę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="03e13-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="03e13-106">Możesz również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje LOB, udziały plików i drukarki.</span><span class="sxs-lookup"><span data-stu-id="03e13-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="03e13-107">Aby zezwolić na dostęp, użyj funkcji [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) w celu zsynchronizowania lokalnej usługi Active Directory z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03e13-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="03e13-108">Aby dowiedzieć się więcej, zobacz [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="03e13-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="03e13-109">Instrukcje te zostały również podsumowane w poniższych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="03e13-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="03e13-110">Uruchamianie usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="03e13-110">Run Azure AD Connect</span></span>

<span data-ttu-id="03e13-111">Wykonaj poniższe czynności, aby włączyć dostęp do zasobów lokalnych w Twojej organizacji z dołączonymi urządzeniami usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="03e13-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="03e13-112">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom Kreatora synchronizacji katalogów i usługi Azure AD Connect zgodnie z opisem w obszarze [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="03e13-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="03e13-113">Po zakończeniu synchronizacji katalogów upewnij się, że na urządzeniach z systemem Windows 10 organizacji jest przyłączony system Azure AD.</span><span class="sxs-lookup"><span data-stu-id="03e13-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="03e13-114">Ten krok należy przeprowadzić indywidualnie na każdym urządzeniu z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="03e13-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="03e13-115">Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla programu Microsoft 365 Business Premium](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="03e13-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="03e13-116">Po przełączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń programu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="03e13-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="03e13-117">Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="03e13-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="03e13-118">Aby uzyskać dostęp do zasobów lokalnych dla przyłączonych urządzeń Azure AD, nie są wymagane żadne dodatkowe czynności.</span><span class="sxs-lookup"><span data-stu-id="03e13-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="03e13-119">Ta funkcja jest wbudowana w systemie Windows 10.</span><span class="sxs-lookup"><span data-stu-id="03e13-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="03e13-120">Jeśli masz plan logowania na urządzeniu AADJ innym niż Metoda Password, taką jak PIN/Bio-Metric za pomocą WHFB poświadczenia logowania, a następnie uzyskujesz dostęp do zasobów lokalnymi (udziałów, drukarek. itd.), wykonaj https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="03e13-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="03e13-121">Jeśli Twoja organizacja nie jest gotowa do wdrożenia w opisanej powyżej konfiguracji urządzenia połączonego z usługą Azure AD, spróbuj skonfigurować [konfigurację hybrydowego urządzenia z usługą Azure AD](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="03e13-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="03e13-122">Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="03e13-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="03e13-123">Jeśli urządzenie z systemem Windows, na którym znajduje się usługa Azure-AD, była już przyłączone do domeny lub w grupie roboczej, należy uwzględnić następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="03e13-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="03e13-124">Po dołączeniu do usługi Azure AD program tworzy nowego użytkownika bez odwołania do istniejącego profilu.</span><span class="sxs-lookup"><span data-stu-id="03e13-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="03e13-125">Profile należy poddać ręcznej migracji.</span><span class="sxs-lookup"><span data-stu-id="03e13-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="03e13-126">Profil użytkownika zawiera informacje, takie jak Ulubione, lokalne pliki, ustawienia przeglądarki i ustawienia menu Start.</span><span class="sxs-lookup"><span data-stu-id="03e13-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="03e13-127">Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy służącego do mapowania istniejących plików i ustawień na nowy profil.</span><span class="sxs-lookup"><span data-stu-id="03e13-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="03e13-128">Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty GPO mogą nie mieć porównywalnego [dostawcy usług konfiguracji](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="03e13-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="03e13-129">Uruchom [Narzędzie MMAT](https://www.microsoft.com/download/details.aspx?id=45520) , aby znaleźć porównywalnych dostawców CSP dla istniejących obiektów zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="03e13-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="03e13-130">Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03e13-130">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="03e13-131">Oceń starszą aplikację i spróbuj zaktualizować aplikację, która korzysta z nowoczesnego uwierzytelniania, jeśli to możliwe.</span><span class="sxs-lookup"><span data-stu-id="03e13-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="03e13-132">Odnajdowanie drukarek w usłudze Active Directory nie będzie działać.</span><span class="sxs-lookup"><span data-stu-id="03e13-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="03e13-133">Możesz udostępniać bezpośrednie ścieżki drukarek wszystkim użytkownikom lub korzystać z funkcji [drukowania w chmurze hybrydowej](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="03e13-133">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
