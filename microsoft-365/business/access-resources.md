---
title: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business
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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki, z urządzenia z systemem Windows 10, do których dołączyć usługa Azure Active Directory.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445353"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="728e7-103">Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="728e7-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="728e7-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="728e7-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="728e7-105">Każde urządzenie z systemem Windows 10, do których dołączyć jest usługa Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje platformy Microsoft 365, i może być chronione przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="728e7-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="728e7-106">Możesz również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje firmowe (LOB), udziały plików i drukarki.</span><span class="sxs-lookup"><span data-stu-id="728e7-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="728e7-107">Aby zezwolić na dostęp, użyj programu [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) do zsynchronizowania lokalnej usługi Active Directory z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="728e7-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="728e7-108">Aby dowiedzieć się więcej, [zobacz Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="728e7-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="728e7-109">Kroki te zostały również podsumowane w poniższych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="728e7-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="728e7-110">Uruchamianie programu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="728e7-110">Run Azure AD Connect</span></span>

<span data-ttu-id="728e7-111">Wykonaj poniższe czynności, aby umożliwić organizacji urządzenia przyłączone do usługi Azure AD w celu uzyskiwania dostępu do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="728e7-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="728e7-112">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom kreatora synchronizacji katalogów i programu Azure AD Connect zgodnie z opisem w tesłudze Konfigurowanie synchronizacji katalogów dla usługi [Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="728e7-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>
    
2. <span data-ttu-id="728e7-113">Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia Organizacji z systemem Windows 10 są przyłączone do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="728e7-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="728e7-114">Ten krok jest wykonywane pojedynczo na każdym urządzeniu z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="728e7-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="728e7-115">Aby uzyskać szczegółowe informacje, zobacz Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi [Microsoft 365 Business Premium.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="728e7-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="728e7-116">Gdy urządzenia z systemem Windows 10 dołączą do usługi Azure AD, każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń platformy Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="728e7-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="728e7-117">Wszystkie urządzenia mają teraz również dostęp do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="728e7-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="728e7-118">Aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączony do usługi Azure AD, nie są wymagane żadne dodatkowe czynności.</span><span class="sxs-lookup"><span data-stu-id="728e7-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="728e7-119">Ta funkcja jest wbudowana w system Windows 10.</span><span class="sxs-lookup"><span data-stu-id="728e7-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="728e7-120">Jeśli planujesz zalogować się do urządzenia AADJ inną niż metoda haseł Like PIN/Bio-metric za pośrednictwem logowania poświadczeń WHFB, a następnie uzyskać dostęp do zasobów lokalnych (udziałów,drukarek). itp.), postępuj zgodnie z https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="728e7-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="728e7-121">Jeśli Twoja organizacja nie jest jeszcze gotowa do wdrożenia w opisanej powyżej konfiguracji urządzenia połączonego z usługą Azure AD, rozważ skonfigurowanie hybrydowej konfiguracji urządzenia przyłączonego do usługi [Azure AD.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="728e7-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="728e7-122">Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="728e7-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="728e7-123">Jeśli urządzenie z systemem Windows, do których dodano usługę Azure-AD, było wcześniej przyłączone do domeny lub w grupie roboczej, rozważ następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="728e7-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="728e7-124">Gdy urządzenie dołącza do usługi Azure AD, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu.</span><span class="sxs-lookup"><span data-stu-id="728e7-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="728e7-125">Profile należy migrować ręcznie.</span><span class="sxs-lookup"><span data-stu-id="728e7-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="728e7-126">Profil użytkownika zawiera informacje, takie jak ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start.</span><span class="sxs-lookup"><span data-stu-id="728e7-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="728e7-127">Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień na nowy profil.</span><span class="sxs-lookup"><span data-stu-id="728e7-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="728e7-128">Jeśli urządzenie używa obiektów zasady grupy (GPO), niektóre obiekty GPOs [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) mogą nie mieć porównywalnego dostawcy usług konfiguracji (CSP) w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="728e7-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="728e7-129">Uruchom narzędzie [MMAT, aby](https://www.microsoft.com/download/details.aspx?id=45520) znaleźć porównywalne pliki CSP dla istniejących gpOs.</span><span class="sxs-lookup"><span data-stu-id="728e7-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="728e7-130">Użytkownicy mogą nie być w stanie uwierzytelnić się w aplikacjach zależnych od uwierzytelniania usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="728e7-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="728e7-131">Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnego uwierzytelniania, jeśli to możliwe.</span><span class="sxs-lookup"><span data-stu-id="728e7-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="728e7-132">Odnajdowanie drukarek usługi Active Directory nie będzie działać.</span><span class="sxs-lookup"><span data-stu-id="728e7-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="728e7-133">Możesz udostępnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [drukowania uniwersalnego.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="728e7-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="728e7-134">Artykuły pokrewne</span><span class="sxs-lookup"><span data-stu-id="728e7-134">Related Articles</span></span>

[<span data-ttu-id="728e7-135">Wymagania wstępne programu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="728e7-135">Prerequisites for Azure AD Connect</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
