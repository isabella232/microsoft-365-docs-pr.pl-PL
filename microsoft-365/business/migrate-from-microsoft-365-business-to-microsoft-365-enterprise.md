---
title: Migrowanie z programu Microsoft 365 Business do firmy Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Dowiedz się, jak przenieść firmę z witryny Microsoft 365 Business Premium do firmy Microsoft 365 E3.
ms.openlocfilehash: 3f840a27cdcf50bba7710681135f6c2e241ad14b
ms.sourcegitcommit: 001e64f89f9c3cd6bbd4a25459f5bee3b966820c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/20/2020
ms.locfileid: "49367060"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="b3241-103">Migrowanie z usługi Microsoft 365 Business Premium do firmy Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="b3241-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="b3241-104">Aplikacja Microsoft 365 Business Premium ma wszystko, czego potrzebujesz dla małych firm, łącząc aplikacje biurowe najlepiej obsługujące się w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają pracownikom wykonywanie ich najlepszej pracy.</span><span class="sxs-lookup"><span data-stu-id="b3241-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="b3241-105">Jednak w niektórych przypadkach konieczne może być Migrowanie subskrypcji programu Microsoft 365 Business Premium do firmy Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b3241-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="b3241-106">Na przykład Twoja firma rozwinęła się i potrzebuje więcej niż 300 licencji (Gratulacje, w drodze).</span><span class="sxs-lookup"><span data-stu-id="b3241-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="b3241-107">Ponadto firma potrzebuje funkcji organizacji, takich jak aplikacje Microsoft 365 dla przedsiębiorstw, Windows 10 Enterprise E3 lub licencje dostępu klienta (CAL) dla przedsiębiorstw.</span><span class="sxs-lookup"><span data-stu-id="b3241-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="b3241-108">Uaktualnienie jest proste: możesz rozpocząć uaktualnianie [w centrum administracyjnym](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="b3241-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="b3241-109">Wszystkie dane i konfiguracja w bieżącej subskrypcji są zachowywane.</span><span class="sxs-lookup"><span data-stu-id="b3241-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="b3241-110">Nie trzeba nic robić, aby przygotować się do migracji i nic nie robić, z wyjątkiem możliwości skorzystania z nowych funkcji.</span><span class="sxs-lookup"><span data-stu-id="b3241-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="b3241-111">Możesz również skorzystać z abonamentu Microsoft 365 Business Premium dla maksymalnie 300 stanowisk i uzyskać abonament Microsoft 365 E3 na więcej niż 300 miejsc.</span><span class="sxs-lookup"><span data-stu-id="b3241-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="b3241-112">Program Microsoft Defender dla Office 365 nie jest jednak dostępny w witrynie Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b3241-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="b3241-113">Aby zapewnić ciągłą ochronę przed zagrożeniami, należy dodać dodatkowe usługi Defender for Office 365, aby uzyskać licencję wszystkich użytkowników w zakresie usługi Defender dla Office 365.</span><span class="sxs-lookup"><span data-stu-id="b3241-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="b3241-114">Różnice między programem Microsoft 365 Business Premium a programem Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="b3241-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="b3241-115">W poniższej tabeli przedstawiono różnice między programami Microsoft 365 Business Premium i Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b3241-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="b3241-116">Funkcja</span><span class="sxs-lookup"><span data-stu-id="b3241-116">Feature</span></span>    | <span data-ttu-id="b3241-117">Pomoc techniczna w programie Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b3241-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="b3241-118">Pomoc techniczna w witrynie Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="b3241-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="b3241-119">**Lokalnie**</span><span class="sxs-lookup"><span data-stu-id="b3241-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="b3241-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b3241-120">Windows 10</span></span>    | <span data-ttu-id="b3241-121">System Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="b3241-121">Windows 10 Business</span></span>  |     <span data-ttu-id="b3241-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="b3241-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="b3241-123">Aplikacje pakietu Office \*</span><span class="sxs-lookup"><span data-stu-id="b3241-123">Office apps\*</span></span>    | [<span data-ttu-id="b3241-124">Aplikacje Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="b3241-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="b3241-125">Aplikacje usługi Microsoft 365 dla przedsiębiorstw</span><span class="sxs-lookup"><span data-stu-id="b3241-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="b3241-126">**Aplikacje do pracy w chmurze**</span><span class="sxs-lookup"><span data-stu-id="b3241-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="b3241-127">Exchange Online i Outlook</span><span class="sxs-lookup"><span data-stu-id="b3241-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="b3241-128">50 GB limitu magazynowania na skrzynkę pocztową i funkcję archiwizacji usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b3241-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="b3241-129">100 GB limitu magazynowania na skrzynkę pocztową i funkcję archiwizacji usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b3241-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="b3241-130">Teams</span><span class="sxs-lookup"><span data-stu-id="b3241-130">Teams</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-133">OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="b3241-133">OneDrive for Business</span></span>    | <span data-ttu-id="b3241-134">1 TB limitu magazynowania na użytkownika</span><span class="sxs-lookup"><span data-stu-id="b3241-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="b3241-135">Czas</span><span class="sxs-lookup"><span data-stu-id="b3241-135">Unlimited</span></span> | 
| <span data-ttu-id="b3241-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="b3241-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-139">MileIQ</span><span class="sxs-lookup"><span data-stu-id="b3241-139">MileIQ</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="b3241-141">**Ochrona przed zagrożeniami**</span><span class="sxs-lookup"><span data-stu-id="b3241-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="b3241-142">Funkcje ograniczania powierzchni ataku</span><span class="sxs-lookup"><span data-stu-id="b3241-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="b3241-143">Zobacz tę listę</span><span class="sxs-lookup"><span data-stu-id="b3241-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="b3241-144">Zarządzanie przedsiębiorstwem izolacji opartej na sprzęcie dla przeglądarki Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b3241-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="b3241-145">Defender dla Office 365 (plan 1)</span><span class="sxs-lookup"><span data-stu-id="b3241-145">Defender for Office 365 Plan 1</span></span> | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="b3241-147">Nieuwzględniona, ale można ją dodać</span><span class="sxs-lookup"><span data-stu-id="b3241-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="b3241-148">**Zarządzanie tożsamościami**</span><span class="sxs-lookup"><span data-stu-id="b3241-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="b3241-149">Samoobsługowe resetowanie hasła dla kont hybrydowych usługi Azure Active Directory (MFA), usługi Azure Multi-Factor Authentication (MFA), dostęp warunkowy, Stornowanie hasła dla tożsamości lokalnych</span><span class="sxs-lookup"><span data-stu-id="b3241-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-152">Odnajdowanie aplikacji w chmurze, usługa Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="b3241-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-154">Aplikacje usługi Azure AD Office 365 pojedyncza Sign-On (SSO): 10 aplikacji na użytkownika (aplikacje galerii SaaS, takie jak usługi Salesforce) \*</span><span class="sxs-lookup"><span data-stu-id="b3241-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-157">Usługa Azure AD Premium 1 SSO: brak limitu (aplikacje lokalne za pośrednictwem serwera proxy aplikacji Azure AD i aplikacji nienależących do galerii przy użyciu szablonów integracji aplikacji Self-Service)</span><span class="sxs-lookup"><span data-stu-id="b3241-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-159">**Zarządzanie urządzeniami i aplikacjami**</span><span class="sxs-lookup"><span data-stu-id="b3241-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="b3241-160">Microsoft Intune, Windows dla autopilota</span><span class="sxs-lookup"><span data-stu-id="b3241-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b3241-163">Wirtualny dostęp do pulpitu (VDA)</span><span class="sxs-lookup"><span data-stu-id="b3241-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b3241-165">Pulpit wirtualny systemu Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="b3241-165">Windows Virtual Desktop (WVD)</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b3241-168">Aktywacja na komputerze współużytkowanym (BRIDGED)</span><span class="sxs-lookup"><span data-stu-id="b3241-168">Shared Computer Activation (SCA)</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-171">Pakiet optymalizacji Microsoft Desktop</span><span class="sxs-lookup"><span data-stu-id="b3241-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-173">**Ochrona informacji**</span><span class="sxs-lookup"><span data-stu-id="b3241-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="b3241-174">Ochrona przed utratą danych w pakiecie Office 365 i usługa Azure Information Protection Plan 1</span><span class="sxs-lookup"><span data-stu-id="b3241-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-177">Ochrona informacji o oknach dla punktu końcowego DLP</span><span class="sxs-lookup"><span data-stu-id="b3241-177">Window Information Protection for endpoint DLP</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-180">**Licencja dostępu klienta (prawa CAL)**</span><span class="sxs-lookup"><span data-stu-id="b3241-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="b3241-181">Pakiet Enterprise CAL (Exchange, SharePoint, Skype, Windows, Menedżer konfiguracji programu Microsoft Endpoint, zarządzanie prawami dostępu w systemie Windows)</span><span class="sxs-lookup"><span data-stu-id="b3241-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-183">**Spełnienia**</span><span class="sxs-lookup"><span data-stu-id="b3241-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="b3241-184">Archiwizowanie wiadomości e-mail bez ograniczeń</span><span class="sxs-lookup"><span data-stu-id="b3241-184">Unlimited email archiving</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-187">Menedżer zgodności</span><span class="sxs-lookup"><span data-stu-id="b3241-187">Compliance Manager</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-190">Materiałów</span><span class="sxs-lookup"><span data-stu-id="b3241-190">eDiscovery</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-193">Przechowywanie w miejscu i w ramach postępowania sądowego</span><span class="sxs-lookup"><span data-stu-id="b3241-193">In-place hold and litigation hold</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b3241-196">Znaczniki przechowywania i zasady przechowywania rekordów funkcji zarządzania rekordami wiadomości (MRM)</span><span class="sxs-lookup"><span data-stu-id="b3241-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="b3241-199">\* Użytkownicy, którym przypisano dostęp do aplikacji SaaS, mogą uzyskać dostęp SSO do 10 aplikacji.</span><span class="sxs-lookup"><span data-stu-id="b3241-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="b3241-200">Administratorzy mogą konfigurować Logowanie jednokrotne i zmieniać dostęp użytkowników do różnych aplikacji SaaS, ale dostęp SSO jest dozwolony tylko dla 10 aplikacji na użytkownika naraz.</span><span class="sxs-lookup"><span data-stu-id="b3241-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="b3241-201">Wszystkie aplikacje pakietu Office 365 są liczone jako pojedyncza aplikacja.</span><span class="sxs-lookup"><span data-stu-id="b3241-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="b3241-202">Migracj</span><span class="sxs-lookup"><span data-stu-id="b3241-202">Migration</span></span>

<span data-ttu-id="b3241-203">Aby przeprowadzić migrację, należy współpracować z partnerem w celu przeniesienia abonamentu i licencji programu Microsoft 365 Business Premium na odpowiednią subskrypcję Microsoft 365 E3 z jej licencjami.</span><span class="sxs-lookup"><span data-stu-id="b3241-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="b3241-204">W poniższych sekcjach opisano, jakie zmiany należy wprowadzić, jeśli istnieją, oraz jakie czynności można wykonać po zakończeniu migracji.</span><span class="sxs-lookup"><span data-stu-id="b3241-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="b3241-205">Konfiguracja i dane subskrypcji programu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b3241-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="b3241-206">Przed przeprowadzeniem migracji nie trzeba wprowadzać żadnych zmian w bieżącym abonamentu ani danych, co obejmuje następujące funkcje:</span><span class="sxs-lookup"><span data-stu-id="b3241-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="b3241-207">Konfiguracja subskrypcji, na przykład nazwy domen DNS.</span><span class="sxs-lookup"><span data-stu-id="b3241-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="b3241-208">Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="b3241-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="b3241-209">Konfiguracje usług biurowych i ich dane, takie jak zespoły, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla firm i Notesy programu OneNote.</span><span class="sxs-lookup"><span data-stu-id="b3241-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="b3241-210">Użytkownicy mogą teraz korzystać z przestrzeni dyskowej bez ograniczeń w folderach skrzynek pocztowych Exchange Online i OneDrive dla firm.</span><span class="sxs-lookup"><span data-stu-id="b3241-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="b3241-211">Możesz zacząć korzystać z funkcji Odnajdowanie aplikacji w chmurze, Azure AD Connect Health i SSO na więcej niż 10 aplikacji.</span><span class="sxs-lookup"><span data-stu-id="b3241-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="b3241-212">Użytkownicy zmigrowani do programu Microsoft 365 E3 nie mogą już korzystać z MileIQ.</span><span class="sxs-lookup"><span data-stu-id="b3241-212">Users migrated to Microsoft 365 E3 can no longer use MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="b3241-213">Ochrona przed zagrożeniami</span><span class="sxs-lookup"><span data-stu-id="b3241-213">Threat protection</span></span>

<span data-ttu-id="b3241-214">System Windows 10 Business obejmuje następujące funkcje:</span><span class="sxs-lookup"><span data-stu-id="b3241-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="b3241-215">Proces wdrażania integralności procesu uruchamiania systemu operacyjnego</span><span class="sxs-lookup"><span data-stu-id="b3241-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="b3241-216">Egzekwowanie integralności wrażliwych składników operacyjnych</span><span class="sxs-lookup"><span data-stu-id="b3241-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="b3241-217">Zaawansowana Luka w zabezpieczeniach oraz łagodzenie wykorzystania zer</span><span class="sxs-lookup"><span data-stu-id="b3241-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="b3241-218">Ochrona sieci oparta na reputacji w programie Microsoft Edge, Internet Explorer i w programie Chrome</span><span class="sxs-lookup"><span data-stu-id="b3241-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="b3241-219">Zapora oparta na hoście</span><span class="sxs-lookup"><span data-stu-id="b3241-219">Host-based firewall</span></span>
- <span data-ttu-id="b3241-220">Ograniczenia dotyczące oprogramowania wymuszającego okup</span><span class="sxs-lookup"><span data-stu-id="b3241-220">Ransomware mitigations</span></span>
- <span data-ttu-id="b3241-221">Izolacja sprzętowa przeglądarki Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b3241-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="b3241-222">Sterowanie aplikacjami obsługiwane przez wykres inteligentne zabezpieczenia</span><span class="sxs-lookup"><span data-stu-id="b3241-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="b3241-223">Sterowanie urządzeniem (USB)</span><span class="sxs-lookup"><span data-stu-id="b3241-223">Device control (USB)</span></span>
- <span data-ttu-id="b3241-224">Ochrona sieci na potrzeby zagrożeń opartych na sieci Web</span><span class="sxs-lookup"><span data-stu-id="b3241-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="b3241-225">Reguły zapobiegania włamaniom hosta</span><span class="sxs-lookup"><span data-stu-id="b3241-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="b3241-226">System Windows 10 Enterprise E3 obejmuje również zarządzanie przedsiębiorstwem izolacji opartej na sprzęcie dla przeglądarki Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b3241-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="b3241-227">Użytkownicy zmigrowani do programu Microsoft 365 E3 będą musieli wymagać licencji usługi Microsoft Defender for Office 365 na kontynuację ochrony przed zagrożeniami.</span><span class="sxs-lookup"><span data-stu-id="b3241-227">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="b3241-228">Pamiętaj, aby zakupić dodatkowe usługi Defender dla licencji Office 365, aby uzyskać licencję wszystkich użytkowników w zakresie usługi Defender dla Office 365.</span><span class="sxs-lookup"><span data-stu-id="b3241-228">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="b3241-229">Zarządzanie urządzeniami za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="b3241-229">Device management with Intune</span></span>

<span data-ttu-id="b3241-230">Przed przeprowadzeniem migracji nie trzeba wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, obejmującym zarejestrowane urządzenia i ustawienia urządzeń oraz aplikacji.</span><span class="sxs-lookup"><span data-stu-id="b3241-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="b3241-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b3241-231">Windows 10</span></span>

<span data-ttu-id="b3241-232">Pakiet Microsoft 365 Business Premium obejmuje system Windows 10 Business, który można zainstalować za pomocą autopilota systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="b3241-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="b3241-233">Podczas migrowania do programu Microsoft 365 E3 każda Licencja użytkownika obejmuje system Windows 10 Enterprise E3, który można też zainstalować za pomocą autopilota systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="b3241-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="b3241-234">Aplikacje Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="b3241-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="b3241-235">Program Microsoft 365 Apps dla firm zainstalowany na urządzeniach automatycznie rozpocznie korzystanie z funkcji aplikacji Microsoft 365 w wersji Enterprise.</span><span class="sxs-lookup"><span data-stu-id="b3241-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="b3241-236">Po zakończeniu migracji możesz teraz używać następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="b3241-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="b3241-237">Aktywacja Zbiorcza za pomocą zasad grupy</span><span class="sxs-lookup"><span data-stu-id="b3241-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="b3241-238">Telemetria aplikacji</span><span class="sxs-lookup"><span data-stu-id="b3241-238">App telemetry</span></span>
 - <span data-ttu-id="b3241-239">Aktualizowanie kontrolek</span><span class="sxs-lookup"><span data-stu-id="b3241-239">Update controls</span></span>
 - <span data-ttu-id="b3241-240">Porównywanie arkuszy kalkulacyjnych i zapytanie</span><span class="sxs-lookup"><span data-stu-id="b3241-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="b3241-241">Analiza biznesowa</span><span class="sxs-lookup"><span data-stu-id="b3241-241">Business intelligence</span></span>

