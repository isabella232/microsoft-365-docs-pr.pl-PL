---
title: Dostęp do zasobów lokalnych z Azure urządzenia przyłączonych do AD w Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, jak linia biznesowych aplikacji, udziałów plików i drukarek z usługi Active Directory Azure dołączył do urządzenia systemu Windows 10.
ms.openlocfilehash: 0a5d4b0828888fcb99676223000c446479f84ddc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982257"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="d379c-103">Dostęp do zasobów lokalnych z Azure urządzenia przyłączonych do AD w Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="d379c-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="d379c-p101">Dowolnych urządzeń 10 systemu Windows Azure Active Directory połączonych będą mieli dostęp do wszystkich zasobów w chmurze takie jak aplikacje pakietu Office 365 i mogą być chronione przez Microsoft 365 Business. Aby również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje linii biznesowych (LOB), udziałów plików i drukarek, należy zsynchronizować usługi Active Directory na lokalnym z usługą Active Directory za pomocą [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). Zobacz [Wprowadzenie do zarządzania urządzeniami w usłudze Active Directory Azure](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) , aby dowiedzieć się więcej.</span><span class="sxs-lookup"><span data-stu-id="d379c-p101">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business. To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="d379c-107">Uruchom Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d379c-107">Run Azure AD Connect</span></span>

<span data-ttu-id="d379c-108">Wykonaj następujące kroki, aby włączyć w urządzeniach Azure AD dołączył do organizacji dostęp do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="d379c-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="d379c-109">Aby zsynchronizować użytkowników, grup i kontakty z lokalną usługę Active Directory z usługą Active Directory Azure, uruchom Kreatora synchronizacji katalogu i Azure Połącz AD jako opisane w [Konfigurowanie synchronizacji katalogów usługi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="d379c-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="d379c-p102">Po zakończeniu synchronizacji katalogów, upewnij się, że urządzenia Windows 10 organizacji są Azure AD przyłączony. Ten krok jest wykonywana indywidualnie na każde urządzenie Windows 10. Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń systemu Windows dla użytkowników biznesowych 365 Microsoft](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="d379c-p102">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined. This step is done individually on each Windows 10 device. See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="d379c-p103">Po zainstalowaniu urządzeń 10 systemu Windows Azure AD przyłączony, każdy użytkownik należy ponownie uruchomić komputer ich urządzenia i zaloguj się przy użyciu poświadczeń Microsoft 365 Business. Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych, jak również.</span><span class="sxs-lookup"><span data-stu-id="d379c-p103">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials. All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="d379c-p104">Żadne dodatkowe kroki są wymagane do uzyskania dostępu do lokalnego czy zasobów dla Azure AD dołączył do urządzenia. Jest to wbudowane funkcje dostępne w systemie Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d379c-p104">No additional steps are required to get access to on-premise resources for Azure AD joined devices. This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="d379c-117">Jeśli w organizacji nie jest gotowa do wdrożenia w Azure AD dołączył do konfiguracji urządzenia opisane powyżej, warto rozważyć skonfigurowanie [połączonych AD Azure hybrydowe konfiguracji urządzenia](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="d379c-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="d379c-118">Zagadnienia dotyczące przyłączania urządzenia z systemem Windows do Azure AD</span><span class="sxs-lookup"><span data-stu-id="d379c-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="d379c-119">Azure AD przyłączania urządzeń systemu Windows, który wcześniej został przyłączony do domeny czy do grupy roboczej, należy wziąć pod uwagę następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="d379c-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="d379c-p105">Gdy urządzenie Azure AD dołącza, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Aby rozwiązać ten problem, trzeba ręcznie można migrować profile. Profil użytkownika zawiera informacje, takie jak Ulubione, pliki lokalne, ustawienia przeglądarki, ustawienia menu Start, itp. Najlepszym rozwiązaniem jest znaleźć narzędzia innej firmy do mapowania istniejące pliki i ustawienia na nowy profil</span><span class="sxs-lookup"><span data-stu-id="d379c-p105">When a device Azure AD joins, it creates a new user without referencing an existing profile. To fix this, profiles need to be manually migrated. A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>
    
- <span data-ttu-id="d379c-p106">Jeśli urządzenie używa obiektów zasady grupy (GPO), niektóre obiekty zasad grupy może nie mieć porównywalne [Konfiguracji usługodawcy](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune. Uruchom [Narzędzie MMAT](https://www.microsoft.com/download/details.aspx?id=45520) odnaleźć dostawców CSP porównywalnych dla istniejących obiektów zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="d379c-p106">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune. Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span> 
    
- <span data-ttu-id="d379c-p107">Użytkownicy nie będą w stanie uwierzytelnić do aplikacji, które zależą od uwierzytelniania usługi Active Directory. Radzić sobie z oceny, za pomocą starszej wersji aplikacji i rozważyć aktualizację do aplikacji, która wykorzystuje nowoczesny Auth, jeśli jest to możliwe.</span><span class="sxs-lookup"><span data-stu-id="d379c-p107">Users will not be able to authenticate to applications that depend on Active Directory authentication. To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>
    
- <span data-ttu-id="d379c-p108">Odnajdywanie drukarki w usłudze Active Directory nie będzie działać. Aby rozwiązać ten problem, zapewnić bezpośrednie drukarki ścieżki dla wszystkich użytkowników lub wykorzystać [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="d379c-p108">Active Directory printer discovery will not work. To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
    

