---
title: Migracja z usługi Microsoft 365 Business do usługi Microsoft 365 E3
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
description: Dowiedz się, jak przenieść firmę z usługi Microsoft 365 Business Premium na usługę Microsoft 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081870"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="cac3f-103">Migracja z usługi Microsoft 365 Business Premium do usługi Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="cac3f-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="cac3f-104">Usługa Microsoft 365 Business Premium ma wszystko, czego potrzebujesz dla małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają pracownikom najlepszą pracę.</span><span class="sxs-lookup"><span data-stu-id="cac3f-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="cac3f-105">W niektórych przypadkach może być jednak konieczne migracja subskrypcji usługi Microsoft 365 Business Premium do usługi Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cac3f-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="cac3f-106">Na przykład Twoja firma rozrosła się i potrzebuje ponad 300 licencji (gratulacje, nawiasem mówiąc).</span><span class="sxs-lookup"><span data-stu-id="cac3f-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="cac3f-107">Twoja firma potrzebuje też funkcji korporacyjnych, takich jak Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3 lub Enterprise Client Access Licenses (CAL).</span><span class="sxs-lookup"><span data-stu-id="cac3f-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="cac3f-108">Uaktualnienie jest łatwe: uaktualnienie można rozpocząć [w centrum administracyjnym](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="cac3f-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="cac3f-109">Wszystkie dane i konfiguracja w bieżącej subskrypcji są obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="cac3f-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="cac3f-110">Nie ma nic do zrobienia, aby przygotować się do migracji i nic do zrobienia później, z wyjątkiem skorzystać z nowych funkcji.</span><span class="sxs-lookup"><span data-stu-id="cac3f-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="cac3f-111">Możesz również użyć subskrypcji Usługi Microsoft 365 Business Premium dla maksymalnie 300 miejsc i uzyskać subskrypcję usługi Microsoft 365 E3 na ponad 300 miejsc.</span><span class="sxs-lookup"><span data-stu-id="cac3f-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="cac3f-112">Jednak usługa Office 365 ATP nie jest dołączona do usługi Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cac3f-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="cac3f-113">Aby zapewnić ciągłą ochronę przed zagrożeniami, należy dodać dodatkowe licencje usługi Office 365 ATP, aby wszyscy użytkownicy w zakresie twoich policyjnych pakietów Office 365 ATP podlegali licencji.</span><span class="sxs-lookup"><span data-stu-id="cac3f-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="cac3f-114">Różnice między microsoft 365 Business Premium i Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="cac3f-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="cac3f-115">W tej tabeli przedstawiono różnice między usłudze Microsoft 365 Business Premium a microsoftem 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cac3f-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="cac3f-116">Funkcja</span><span class="sxs-lookup"><span data-stu-id="cac3f-116">Feature</span></span>    | <span data-ttu-id="cac3f-117">Pomoc techniczna w usłudze Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="cac3f-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="cac3f-118">Pomoc techniczna w usłudze Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="cac3f-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="cac3f-119">**Lokalnie**</span><span class="sxs-lookup"><span data-stu-id="cac3f-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="cac3f-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="cac3f-120">Windows 10</span></span>    | <span data-ttu-id="cac3f-121">Windows 10 Biznes</span><span class="sxs-lookup"><span data-stu-id="cac3f-121">Windows 10 Business</span></span>  |     <span data-ttu-id="cac3f-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="cac3f-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="cac3f-123">Aplikacje pakietu Office\*</span><span class="sxs-lookup"><span data-stu-id="cac3f-123">Office apps\*</span></span>    | [<span data-ttu-id="cac3f-124">Aplikacje usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="cac3f-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="cac3f-125">Aplikacje usługi Microsoft 365 dla przedsiębiorstw</span><span class="sxs-lookup"><span data-stu-id="cac3f-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="cac3f-126">**Aplikacje zwiększające produktywność w chmurze**</span><span class="sxs-lookup"><span data-stu-id="cac3f-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="cac3f-127">Usługa Exchange Online i Outlook</span><span class="sxs-lookup"><span data-stu-id="cac3f-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="cac3f-128">Limit miejsca 50 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cac3f-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="cac3f-129">Limit miejsca 100 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cac3f-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="cac3f-130">Zespołów</span><span class="sxs-lookup"><span data-stu-id="cac3f-130">Teams</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-133">OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="cac3f-133">OneDrive for Business</span></span>    | <span data-ttu-id="cac3f-134">Limit pojemności 1 TB na użytkownika</span><span class="sxs-lookup"><span data-stu-id="cac3f-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="cac3f-135">Nieograniczony</span><span class="sxs-lookup"><span data-stu-id="cac3f-135">Unlimited</span></span> | 
| <span data-ttu-id="cac3f-136">Yammer, SharePoint Online, Planner, Strumień</span><span class="sxs-lookup"><span data-stu-id="cac3f-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-139">Menedżer klienta programu Outlook, MileIQ</span><span class="sxs-lookup"><span data-stu-id="cac3f-139">Outlook Customer Manager, MileIQ</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="cac3f-141">**Ochrona przed zagrożeniami**</span><span class="sxs-lookup"><span data-stu-id="cac3f-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="cac3f-142">Możliwości redukcji powierzchni ataku</span><span class="sxs-lookup"><span data-stu-id="cac3f-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="cac3f-143">Zobacz tę listę</span><span class="sxs-lookup"><span data-stu-id="cac3f-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="cac3f-144">Zarządzanie izolacją sprzętową w przedsiębiorstwie dla przeglądarki Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cac3f-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="cac3f-145">Plan 1 zaawansowanej ochrony przed zagrożeniami usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="cac3f-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="cac3f-147">Nie jest dołączony, ale można go dodać na</span><span class="sxs-lookup"><span data-stu-id="cac3f-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="cac3f-148">**Zarządzanie tożsamościami**</span><span class="sxs-lookup"><span data-stu-id="cac3f-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="cac3f-149">Samoobsługowe resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego platformy Azure (MFA), dostępu warunkowego, zapisywania haseł dla tożsamości lokalnych</span><span class="sxs-lookup"><span data-stu-id="cac3f-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-152">Odnajdowanie aplikacji w chmurze, kondycja usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="cac3f-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-154">Aplikacje usługi Azure AD Office 365 Logowanie jednokrotne (logowanie jednokrotne): 10 aplikacji na użytkownika (aplikacje SaaS galerii, takie jak Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="cac3f-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-157">Samoustawne samouszczenia usługi Azure AD Premium 1: bez limitu (aplikacje lokalne za pośrednictwem serwera proxy aplikacji usługi Azure AD i aplikacji innych niż galeria przy użyciu szablonów integracji aplikacji samoobsługowych)</span><span class="sxs-lookup"><span data-stu-id="cac3f-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-159">**Zarządzanie urządzeniami i aplikacjami**</span><span class="sxs-lookup"><span data-stu-id="cac3f-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="cac3f-160">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="cac3f-160">Microsoft Intune, Windows Autopilot</span></span>|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="cac3f-163">Dostęp do pulpitu wirtualnego (VDA)</span><span class="sxs-lookup"><span data-stu-id="cac3f-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="cac3f-165">Pulpit wirtualny systemu Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="cac3f-165">Windows Virtual Desktop (WVD)</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png) |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="cac3f-168">Aktywacja komputera udostępnionego (SCA)</span><span class="sxs-lookup"><span data-stu-id="cac3f-168">Shared Computer Activation (SCA)</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png) |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-171">Pakiet optymalizacji pulpitu firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="cac3f-171">Microsoft Desktop Optimization Package</span></span>    | |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-173">**Ochrona informacji**</span><span class="sxs-lookup"><span data-stu-id="cac3f-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="cac3f-174">Zapobieganie utracie danych w usłudze Office 365, plan ochrony informacji platformy Azure 1</span><span class="sxs-lookup"><span data-stu-id="cac3f-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-177">Ochrona informacji o oknie dla punktu końcowego DLP</span><span class="sxs-lookup"><span data-stu-id="cac3f-177">Window Information Protection for endpoint DLP</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-180">**Licencja dostępu klienta (prawa CAL)**</span><span class="sxs-lookup"><span data-stu-id="cac3f-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="cac3f-181">Pakiet CAL dla przedsiębiorstw (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Zarządzanie prawami systemu Windows)</span><span class="sxs-lookup"><span data-stu-id="cac3f-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-183">**Zgodności**</span><span class="sxs-lookup"><span data-stu-id="cac3f-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="cac3f-184">Nieograniczona archiwizacja poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="cac3f-184">Unlimited email archiving</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-187">Menedżer wyników/zgodności zgodności</span><span class="sxs-lookup"><span data-stu-id="cac3f-187">Compliance Score/Compliance Manager</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-190">Zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="cac3f-190">eDiscovery</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-193">Wstrzymanie i zawieszenie w postępowaniu sądowym</span><span class="sxs-lookup"><span data-stu-id="cac3f-193">In-place hold and litigation hold</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cac3f-196">Tagi przechowywania i zasady przechowywania usługi Zarządzanie rekordami wiadomości (MRM)</span><span class="sxs-lookup"><span data-stu-id="cac3f-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="cac3f-199">\*Użytkownicy, którym przypisano dostęp do aplikacji SaaS, mogą uzyskać dostęp do aplikacji SSO do maksymalnie 10 aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cac3f-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="cac3f-200">Administratorzy mogą konfigurować jednokrotne i zmieniać dostęp użytkownika do różnych aplikacji SaaS, ale dostęp do jednokrotnego dostępu jest dozwolony tylko dla 10 aplikacji na użytkownika naraz.</span><span class="sxs-lookup"><span data-stu-id="cac3f-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="cac3f-201">Wszystkie aplikacje usługi Office 365 są liczone jako pojedyncza aplikacja.</span><span class="sxs-lookup"><span data-stu-id="cac3f-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="cac3f-202">Migracji</span><span class="sxs-lookup"><span data-stu-id="cac3f-202">Migration</span></span>

<span data-ttu-id="cac3f-203">Aby przeprowadzić migrację, skontaktuj się z partnerem, aby przenieść subskrypcję i licencje usługi Microsoft 365 Business Premium do odpowiedniej subskrypcji Usługi Microsoft 365 E3 z licencjami.</span><span class="sxs-lookup"><span data-stu-id="cac3f-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="cac3f-204">W poniższych sekcjach opisano, jakie zmiany należy wprowadzić, jeśli istnieją, i co można zrobić po migracji.</span><span class="sxs-lookup"><span data-stu-id="cac3f-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="cac3f-205">Konfiguracja i dane subskrypcji usługi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cac3f-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="cac3f-206">Przed migracją nie trzeba wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:</span><span class="sxs-lookup"><span data-stu-id="cac3f-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="cac3f-207">Konfiguracja subskrypcji, na przykład nazwy domen DNS.</span><span class="sxs-lookup"><span data-stu-id="cac3f-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="cac3f-208">Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="cac3f-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="cac3f-209">Konfiguracje usług zwiększających produktywność i ich dane, takie jak usługi Teams, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.</span><span class="sxs-lookup"><span data-stu-id="cac3f-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="cac3f-210">Użytkownicy mogą teraz korzystać z nieograniczonej przestrzeni dyskowej w skrzynkach pocztowych usługi Exchange Online i w folderach usługi OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="cac3f-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="cac3f-211">Możesz rozpocząć korzystanie z odnajdowania aplikacji w chmurze, usługi Azure AD Connect Health i aplikacji SSO dla ponad 10 aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cac3f-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="cac3f-212">Użytkownicy migrowani do usługi Microsoft 365 E3 nie mogą już korzystać z programu Outlook Customer Manager i MileIQ.</span><span class="sxs-lookup"><span data-stu-id="cac3f-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="cac3f-213">Ochrona przed zagrożeniami</span><span class="sxs-lookup"><span data-stu-id="cac3f-213">Threat protection</span></span>

<span data-ttu-id="cac3f-214">System Windows 10 Business zawiera następujące zabezpieczenia:</span><span class="sxs-lookup"><span data-stu-id="cac3f-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="cac3f-215">Wymuszanie integralności procesu rozruchu systemu operacyjnego</span><span class="sxs-lookup"><span data-stu-id="cac3f-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="cac3f-216">Egzekwowanie integralności wrażliwych komponentów operacyjnych</span><span class="sxs-lookup"><span data-stu-id="cac3f-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="cac3f-217">Zaawansowane środki zmniejszające podatność na zagrożenia i luki w zabezpieczeniach typu zero-day</span><span class="sxs-lookup"><span data-stu-id="cac3f-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="cac3f-218">Ochrona sieciowa oparta na reputacji dla przeglądarki Microsoft Edge, Internet Explorer i Chrome</span><span class="sxs-lookup"><span data-stu-id="cac3f-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="cac3f-219">Zapora oparta na hoście</span><span class="sxs-lookup"><span data-stu-id="cac3f-219">Host-based firewall</span></span>
- <span data-ttu-id="cac3f-220">Środki zaradcze związane z oprogramowaniem wymuszającym okup</span><span class="sxs-lookup"><span data-stu-id="cac3f-220">Ransomware mitigations</span></span>
- <span data-ttu-id="cac3f-221">Izolacja sprzętowa dla przeglądarki Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cac3f-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="cac3f-222">Sterowanie aplikacjami obsługiwane przez inteligentny wykres zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="cac3f-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="cac3f-223">Sterowanie urządzeniem (USB)</span><span class="sxs-lookup"><span data-stu-id="cac3f-223">Device control (USB)</span></span>
- <span data-ttu-id="cac3f-224">Ochrona sieci w przypadku zagrożeń internetowych</span><span class="sxs-lookup"><span data-stu-id="cac3f-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="cac3f-225">Zasady zapobiegania włamaniom hosta</span><span class="sxs-lookup"><span data-stu-id="cac3f-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="cac3f-226">System Windows 10 Enterprise E3 obejmuje również zarządzanie izolacją sprzętową dla przeglądarki Microsoft Edge w przedsiębiorstwie.</span><span class="sxs-lookup"><span data-stu-id="cac3f-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="cac3f-227">Użytkownicy migrowani do usługi Microsoft 365 E3 będą wymagać licencji usługi Office 365 ATP w celu ciągłej ochrony przed zagrożeniami.</span><span class="sxs-lookup"><span data-stu-id="cac3f-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="cac3f-228">Pamiętaj, aby zakupić dodatkowe licencje usługi Office 365 ATP, aby wszyscy użytkownicy w zakresie twoich policyjnych usługi Office 365 ATP były licencjonowane.</span><span class="sxs-lookup"><span data-stu-id="cac3f-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="cac3f-229">Zarządzanie urządzeniami za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="cac3f-229">Device management with Intune</span></span>

<span data-ttu-id="cac3f-230">Przed migracją nie trzeba wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, która obejmuje zarejestrowane urządzenia oraz ustawienia urządzeń i aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cac3f-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="cac3f-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="cac3f-231">Windows 10</span></span>

<span data-ttu-id="cac3f-232">Usługa Microsoft 365 Business Premium zawiera system Windows 10 Business, który można zainstalować za pomocą programu Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="cac3f-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="cac3f-233">Podczas migracji do usługi Microsoft 365 E3 każda licencja użytkownika zawiera system Windows 10 Enterprise E3, który można również zainstalować za pomocą programu Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="cac3f-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="cac3f-234">Aplikacje usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="cac3f-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="cac3f-235">Klient usługi Microsoft 365 Apps dla firm zainstalowany na twoich urządzeniach automatycznie zacznie korzystać z funkcji aplikacji usługi Microsoft 365 dla przedsiębiorstw.</span><span class="sxs-lookup"><span data-stu-id="cac3f-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="cac3f-236">Po migracji można teraz użyć:</span><span class="sxs-lookup"><span data-stu-id="cac3f-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="cac3f-237">Aktywacja zbiorcza za pośrednictwem zasad grupy</span><span class="sxs-lookup"><span data-stu-id="cac3f-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="cac3f-238">Telemetria aplikacji</span><span class="sxs-lookup"><span data-stu-id="cac3f-238">App telemetry</span></span>
 - <span data-ttu-id="cac3f-239">Kontrolki aktualizacji</span><span class="sxs-lookup"><span data-stu-id="cac3f-239">Update controls</span></span>
 - <span data-ttu-id="cac3f-240">Porównywanie arkuszy kalkulacyjnych i uzyskiwanie pytań</span><span class="sxs-lookup"><span data-stu-id="cac3f-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="cac3f-241">Analityka biznesowa</span><span class="sxs-lookup"><span data-stu-id="cac3f-241">Business intelligence</span></span>

