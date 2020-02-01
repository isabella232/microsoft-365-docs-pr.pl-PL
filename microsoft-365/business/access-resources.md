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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki z usługi Azure Active Directory przyłączonej do urządzenia z systemem Windows 10.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593238"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="e281a-103">Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e281a-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="e281a-104">Każde urządzenie z systemem Windows 10, przyłączone do usługi Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje usługi Office 365, i może być chronione przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e281a-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="e281a-105">Można również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje biznesowe (LOB), udziały plików i drukarki.</span><span class="sxs-lookup"><span data-stu-id="e281a-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="e281a-106">Aby zezwolić na dostęp, użyj [usługi Azure AD Connect,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) aby zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e281a-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="e281a-107">Aby dowiedzieć się więcej, zobacz [Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="e281a-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="e281a-108">Kroki są również podsumowane w poniższych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="e281a-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e281a-109">Ta procedura ma zastosowanie tylko do OAuth i NTLM.</span><span class="sxs-lookup"><span data-stu-id="e281a-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="e281a-110">Protokół Kerberos nie jest obsługiwany.</span><span class="sxs-lookup"><span data-stu-id="e281a-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="e281a-111">Uruchamianie usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e281a-111">Run Azure AD Connect</span></span>

<span data-ttu-id="e281a-112">Wykonaj następujące kroki, aby umożliwić urządzeniom przyłączonym do usługi Azure AD dostęp do zasobów lokalnych w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e281a-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="e281a-113">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom kreatora synchronizacji katalogu i usługę Azure AD Connect zgodnie z opisem w [obszarze Konfigurowanie synchronizacji katalogów dla usługi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="e281a-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="e281a-114">Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są połączone z usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e281a-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="e281a-115">Ten krok odbywa się indywidualnie na każdym urządzeniu z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e281a-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="e281a-116">Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="e281a-116">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="e281a-117">Po przyłączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e281a-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="e281a-118">Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="e281a-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="e281a-119">Nie są wymagane żadne dodatkowe kroki, aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączonych do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e281a-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="e281a-120">Ta funkcja jest wbudowana w system Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e281a-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="e281a-121">Jeśli masz plany, aby zalogować się do urządzenia AADJ innych niż metoda hasła Jak PIN / Bio-metryki za pośrednictwem logowania poświadczeń WHFB, a następnie uzyskać dostęp do zasobów lokalnych (udziały, drukarki.. itp.), należy postępować zgodnie zhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="e281a-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="e281a-122">Jeśli twoja organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia połączonego z usługą Azure AD opisanej powyżej, rozważ skonfigurowanie [konfiguracji urządzenia przyłączonego do usługi Azure AD](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="e281a-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="e281a-123">Zagadnienia podczas łączenia urządzeń z systemem Windows do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="e281a-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="e281a-124">Jeśli urządzenie z systemem Windows przyłączone do usługi Azure-AD było wcześniej przyłączone do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="e281a-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="e281a-125">Gdy urządzenie usługi Azure AD dołącza, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu.</span><span class="sxs-lookup"><span data-stu-id="e281a-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="e281a-126">Profile muszą być ręcznie migrowane.</span><span class="sxs-lookup"><span data-stu-id="e281a-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="e281a-127">Profil użytkownika zawiera informacje, takie jak ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start.</span><span class="sxs-lookup"><span data-stu-id="e281a-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="e281a-128">Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień na nowy profil.</span><span class="sxs-lookup"><span data-stu-id="e281a-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="e281a-129">Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty zasad grupy mogą nie mieć porównywalnego [dostawcy usług konfiguracji](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="e281a-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="e281a-130">Uruchom [narzędzie MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) aby znaleźć porównywalne usługi CSP dla istniejących obiektów zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="e281a-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="e281a-131">Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e281a-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="e281a-132">Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnej auth, jeśli to możliwe.</span><span class="sxs-lookup"><span data-stu-id="e281a-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="e281a-133">Odnajdowanie drukarki usługi Active Directory nie będzie działać.</span><span class="sxs-lookup"><span data-stu-id="e281a-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="e281a-134">Można udostępnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [funkcji Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="e281a-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
