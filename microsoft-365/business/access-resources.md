---
title: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje firmowe, udziały plików i drukarki, za pomocą Azure Active Directory urządzenia Windows 10 firmowego.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843327"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="57b1f-103">Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="57b1f-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="57b1f-104">Ten artykuł dotyczy Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="57b1f-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="57b1f-105">Każde Windows 10, do których jest dołączany komputer Azure Active Directory ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje Microsoft 365, i może być chronione przez Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="57b1f-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="57b1f-106">Możesz również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje firmowe (LOB), udziały plików i drukarki.</span><span class="sxs-lookup"><span data-stu-id="57b1f-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="57b1f-107">Aby zezwolić na dostęp, użyj usługi [Azure AD Połączenie](/azure/active-directory/connect/active-directory-aadconnect) w celu zsynchronizowania lokalnej usługi Active Directory z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57b1f-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="57b1f-108">Aby dowiedzieć się więcej, [zobacz Wprowadzenie do zarządzania urządzeniami w programie Azure Active Directory.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="57b1f-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="57b1f-109">Kroki te zostały również podsumowane w poniższych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="57b1f-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="57b1f-110">Uruchamianie narzędzia Azure AD Połączenie</span><span class="sxs-lookup"><span data-stu-id="57b1f-110">Run Azure AD Connect</span></span>

<span data-ttu-id="57b1f-111">Wykonaj poniższe czynności, aby umożliwić organizacji urządzenia przyłączone do usługi Azure AD w celu uzyskiwania dostępu do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="57b1f-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="57b1f-112">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom kreatora synchronizacji katalogów i usługi Azure AD Połączenie zgodnie z opisem w tesłudze Konfigurowanie synchronizacji katalogów dla usługi [Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="57b1f-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="57b1f-113">Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia firmowe Windows 10 dołączyć do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="57b1f-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="57b1f-114">Ten krok jest wykonywane osobno na każdym Windows 10 urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="57b1f-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="57b1f-115">Zobacz [Konfigurowanie Windows dla Microsoft 365 Business Premium, aby](set-up-windows-devices.md) uzyskać szczegółowe informacje.</span><span class="sxs-lookup"><span data-stu-id="57b1f-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="57b1f-116">Po dołączeniu Windows 10 Azure AD każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń logowania Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="57b1f-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="57b1f-117">Wszystkie urządzenia mają teraz również dostęp do zasobów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="57b1f-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="57b1f-118">Aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączony do usługi Azure AD, nie są wymagane żadne dodatkowe czynności.</span><span class="sxs-lookup"><span data-stu-id="57b1f-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="57b1f-119">Ta funkcja jest wbudowana w Windows 10.</span><span class="sxs-lookup"><span data-stu-id="57b1f-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="57b1f-120">Jeśli planujesz zalogowanie się do urządzenia AADJ inną niż metoda haseł Like PIN/Bio-metric za pośrednictwem logowania poświadczeń WHFB, a następnie dostęp do zasobów lokalnych (udziałów, drukarek itp.), zapoznaj się z tym [artykułem.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="57b1f-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="57b1f-121">Jeśli Twoja organizacja nie jest jeszcze gotowa do wdrożenia w opisanej powyżej konfiguracji urządzenia połączonego z usługą Azure AD, rozważ skonfigurowanie hybrydowej konfiguracji urządzenia przyłączonego do usługi [Azure AD.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="57b1f-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="57b1f-122">Zagadnienia dotyczące dołączania urządzeń Windows do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="57b1f-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="57b1f-123">Jeśli urządzenie Windows przyłączone do usługi Azure-AD było wcześniej przyłączone do domeny lub w grupie roboczej, rozważ następujące ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="57b1f-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="57b1f-124">Gdy urządzenie dołącza do usługi Azure AD, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu.</span><span class="sxs-lookup"><span data-stu-id="57b1f-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="57b1f-125">Profile należy migrować ręcznie.</span><span class="sxs-lookup"><span data-stu-id="57b1f-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="57b1f-126">Profil użytkownika zawiera informacje, takie jak ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start.</span><span class="sxs-lookup"><span data-stu-id="57b1f-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="57b1f-127">Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień na nowy profil.</span><span class="sxs-lookup"><span data-stu-id="57b1f-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="57b1f-128">Jeśli urządzenie używa obiektów zasady grupy (GPO), niektóre obiekty GPOs [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) mogą nie mieć porównywalnego dostawcy usług konfiguracji (CSP) w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="57b1f-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="57b1f-129">Uruchom narzędzie [MMAT, aby](https://www.microsoft.com/download/details.aspx?id=45520) znaleźć porównywalne pliki CSP dla istniejących gpOs.</span><span class="sxs-lookup"><span data-stu-id="57b1f-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="57b1f-130">Użytkownicy mogą nie być w stanie uwierzytelnić się w aplikacjach zależnych od uwierzytelniania usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57b1f-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="57b1f-131">Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnego uwierzytelniania, jeśli to możliwe.</span><span class="sxs-lookup"><span data-stu-id="57b1f-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="57b1f-132">Odnajdowanie drukarek usługi Active Directory nie będzie działać.</span><span class="sxs-lookup"><span data-stu-id="57b1f-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="57b1f-133">Możesz udostępnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [drukowania uniwersalnego.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="57b1f-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="57b1f-134">Artykuły pokrewne</span><span class="sxs-lookup"><span data-stu-id="57b1f-134">Related Articles</span></span>

[<span data-ttu-id="57b1f-135">Wymagania wstępne usługi Azure AD Połączenie</span><span class="sxs-lookup"><span data-stu-id="57b1f-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
