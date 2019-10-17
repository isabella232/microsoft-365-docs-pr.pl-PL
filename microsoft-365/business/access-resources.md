---
title: Dostęp do zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business
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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje linii biznesowych, udziałów plików i drukarek z usługi Azure Active Directory przyłączony do systemu Windows 10 urządzenia.
ms.openlocfilehash: 92e8ccb99dfece7687c25db84b81fc7bc7158d71
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574683"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="30ee0-103">Dostęp do zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="30ee0-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="30ee0-104">Wszystkie urządzenia z systemem Windows 10, które są przyłączone do usługi Azure Active Directory, będą miały dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje pakietu Office 365 i mogą być chronione przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="30ee0-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="30ee0-105">Aby również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje linii biznesowych (LOB), udziałów plików i drukarek, należy zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory przy użyciu programu [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="30ee0-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> 

<span data-ttu-id="30ee0-106">Zobacz [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) , aby dowiedzieć się więcej.</span><span class="sxs-lookup"><span data-stu-id="30ee0-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="30ee0-107">Kroki są również podsumowane w poniższych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="30ee0-107">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="30ee0-108">Uruchom program Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="30ee0-108">Run Azure AD Connect</span></span>

<span data-ttu-id="30ee0-109">Wykonaj następujące kroki, aby włączyć urządzenia przyłączone do usługi Azure AD w organizacji dostępu do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="30ee0-109">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="30ee0-110">Aby zsynchronizować użytkowników, grup i kontaktów z lokalnej usługi Active Directory w usłudze Azure Active Directory, uruchom Kreatora synchronizacji katalogów i Azure AD Connect zgodnie z opisem w [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="30ee0-110">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="30ee0-111">Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są przyłączone do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30ee0-111">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="30ee0-112">Ten krok jest wykonywana indywidualnie na każdym urządzeniu z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="30ee0-112">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="30ee0-113">Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników Microsoft 365 Business](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="30ee0-113">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="30ee0-114">Po przyłączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik powinien ponownie uruchomić swoje urządzenia i zalogować się przy użyciu poświadczeń firmy Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="30ee0-114">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="30ee0-115">Wszystkie urządzenia będą teraz mieć dostęp do zasobów lokalnych, jak również.</span><span class="sxs-lookup"><span data-stu-id="30ee0-115">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="30ee0-116">Nie dodatkowe kroki są wymagane, aby uzyskać dostęp do zasobów lokalnych dla usługi Azure AD przyłączonych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="30ee0-116">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="30ee0-117">Jest to wbudowana funkcja dostępna w systemie Windows 10.</span><span class="sxs-lookup"><span data-stu-id="30ee0-117">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="30ee0-118">Jeśli organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia przyłączone do usługi Azure AD opisanych powyżej, należy rozważyć skonfigurowanie [konfiguracji urządzenia przyłączone do hybrydowej usługi Azure AD](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="30ee0-118">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="30ee0-119">Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="30ee0-119">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="30ee0-120">Jeśli usługi Azure AD przyłączanie urządzenia systemu Windows, który wcześniej został przyłączony do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="30ee0-120">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="30ee0-121">Gdy urządzenie dołącza do usługi Azure AD, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu.</span><span class="sxs-lookup"><span data-stu-id="30ee0-121">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="30ee0-122">Aby rozwiązać ten problem, profile muszą być migrowane ręcznie.</span><span class="sxs-lookup"><span data-stu-id="30ee0-122">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="30ee0-123">Profil użytkownika zawiera takie informacje, jak Ulubione, pliki lokalne, ustawienia przeglądarki, ustawienia menu Start itp. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień do nowego profilu</span><span class="sxs-lookup"><span data-stu-id="30ee0-123">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="30ee0-124">Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty GPO mogą nie mieć porównywalnego [dostawcy usług konfiguracji (CSP, Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) ) w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="30ee0-124">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="30ee0-125">Uruchom [Narzędzie MMat](https://www.microsoft.com/download/details.aspx?id=45520) , aby znaleźć porównywalne dostawcy CSP dla istniejących obiektów zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="30ee0-125">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="30ee0-126">Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="30ee0-126">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="30ee0-127">Aby poradzić sobie z tym ocenić za pomocą starszej wersji aplikacji i rozważyć aktualizację do aplikacji, która korzysta z nowoczesnych auth, jeśli to możliwe.</span><span class="sxs-lookup"><span data-stu-id="30ee0-127">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="30ee0-128">Odnajdowanie drukarek usługi Active Directory nie będzie działać.</span><span class="sxs-lookup"><span data-stu-id="30ee0-128">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="30ee0-129">Aby rozwiązać ten problem, należy zapewnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub wykorzystać [hybrydowy Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="30ee0-129">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
