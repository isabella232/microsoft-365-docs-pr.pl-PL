---
title: Dostęp do zasobów lokalnych z urządzenia przyłączanego do usługi Azure AD w usłudze Microsoft 365 Business
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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki z usługi Azure Active Directory przyłączone do urządzenia z systemem Windows 10.
ms.openlocfilehash: 9615ecc9469992d3e5a7479f4799c610db11fb41
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471256"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="aa2c2-103">Dostęp do zasobów lokalnych z urządzenia przyłączanego do usługi Azure AD w usłudze Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="aa2c2-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="aa2c2-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="aa2c2-105">Każde urządzenie z systemem Windows 10, do którego dołączona jest usługa Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje usługi Microsoft 365, i może być chronione przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="aa2c2-106">Można również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje biznesowe (LOB), udziały plików i drukarki.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="aa2c2-107">Aby zezwolić na dostęp, użyj [usługi Azure AD Connect,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) aby zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="aa2c2-108">Aby dowiedzieć się więcej, zobacz [Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="aa2c2-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="aa2c2-109">Kroki są również podsumowane w poniższych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-109">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="aa2c2-110">Ta procedura ma zastosowanie tylko do OAuth i NTLM.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-110">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="aa2c2-111">Protokół Kerberos nie jest obsługiwany.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-111">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="aa2c2-112">Uruchamianie usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="aa2c2-112">Run Azure AD Connect</span></span>

<span data-ttu-id="aa2c2-113">Wykonaj następujące kroki, aby umożliwić urządzeniom przyłączanym do usługi Azure AD w organizacji dostęp do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-113">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="aa2c2-114">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom Kreatora synchronizacji katalogów i usługi Azure AD Connect zgodnie z opisem w [obszarze Konfigurowanie synchronizacji katalogów dla usługi Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="aa2c2-114">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="aa2c2-115">Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są przyłączone do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-115">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="aa2c2-116">Ten krok jest wykonywany indywidualnie na każdym urządzeniu z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-116">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="aa2c2-117">Szczegółowe informacje można znaleźć w witrynie [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="aa2c2-117">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="aa2c2-118">Gdy urządzenia z systemem Windows 10 są przyłączone do usługi Azure AD, każdy użytkownik musi ponownie uruchomić swoje urządzenia i zalogować się przy użyciu poświadczeń usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-118">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="aa2c2-119">Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych, jak również.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-119">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="aa2c2-120">Żadne dodatkowe kroki nie są wymagane, aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączonych do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-120">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="aa2c2-121">Ta funkcja jest wbudowana w system Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-121">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="aa2c2-122">Jeśli masz plany logowania się do urządzenia AADJ inne niż metoda hasła, takie jak PIN/Bio-metryka za pośrednictwem logowania poświadczeń WHFB, a następnie dostęp do zasobów lokalnych (udziały,drukarki.. itp.), należy postępować zgodnie zhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="aa2c2-122">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="aa2c2-123">Jeśli twoja organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia przyłączanym do usługi Azure AD, opisana powyżej, należy rozważyć skonfigurowanie [konfiguracji urządzenia przyłączone do usługi Azure AD.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="aa2c2-123">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="aa2c2-124">Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="aa2c2-124">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="aa2c2-125">Jeśli urządzenie z systemem Windows, do którego przyłączono usługę Azure-AD, było wcześniej przyłączone do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="aa2c2-125">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="aa2c2-126">Gdy urządzenie usługi Azure AD sprzężenia, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-126">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="aa2c2-127">Profile muszą być migrowane ręcznie.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-127">Profiles must be manually migrated.</span></span> <span data-ttu-id="aa2c2-128">Profil użytkownika zawiera informacje, takie jak ulubione pliki, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-128">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="aa2c2-129">Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień do nowego profilu.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-129">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="aa2c2-130">Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty zasad grupy mogą nie mieć porównywalnego [dostawcy usług konfiguracji](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-130">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="aa2c2-131">Uruchom [narzędzie MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) aby znaleźć porównywalne dostawcy usług internetowych dla istniejących zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-131">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="aa2c2-132">Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-132">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="aa2c2-133">Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnej eru, jeśli to możliwe.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-133">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="aa2c2-134">Odnajdowanie drukarek usługi Active Directory nie będzie działać.</span><span class="sxs-lookup"><span data-stu-id="aa2c2-134">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="aa2c2-135">Można zapewnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [hybrid cloud print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="aa2c2-135">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
