---
title: Migrowanie z platformy Microsoft 365 Business do platformy Microsoft 365 E3
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
description: Dowiedz się, jak przenieść swoją firmę z usługi Microsoft 365 Business Premium do platformy Microsoft 365 E3.
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126206"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="cef48-103">Migrowanie z usługi Microsoft 365 Business Premium do platformy Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="cef48-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="cef48-104">Usługa Microsoft 365 Business Premium oferuje wszystko, czego potrzebujesz dla Twojej małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają Twoim pracownikom wydajną pracę.</span><span class="sxs-lookup"><span data-stu-id="cef48-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="cef48-105">Jednak w niektórych przypadkach może być konieczne przeprowadzenie migracji subskrypcji platformy Microsoft 365 Business Premium do platformy Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cef48-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="cef48-106">Na przykład Twoja firma rozrosła się i potrzebuje ponad 300 licencji (gratulacje, przy okazji).</span><span class="sxs-lookup"><span data-stu-id="cef48-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="cef48-107">Albo Twoja firma potrzebuje funkcji dla przedsiębiorstw, takich jak aplikacje Microsoft 365 dla przedsiębiorstw, licencje CALs (Enterprise Client Access License) dla systemu Windows 10 Enterprise lub Enterprise Client Access License.</span><span class="sxs-lookup"><span data-stu-id="cef48-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="cef48-108">Uaktualnienie jest łatwe: możesz rozpocząć uaktualnienie [z centrum administracyjnego.](../commerce/subscriptions/upgrade-to-different-plan.md)</span><span class="sxs-lookup"><span data-stu-id="cef48-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="cef48-109">Wszystkie dane i konfiguracja w bieżącej subskrypcji są zachowywane.</span><span class="sxs-lookup"><span data-stu-id="cef48-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="cef48-110">Nie musisz nic robić, aby przygotować się do migracji i nie musisz później nic robić, poza skorzystaniem z nowych funkcji.</span><span class="sxs-lookup"><span data-stu-id="cef48-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="cef48-111">Możesz również użyć subskrypcji usługi Microsoft 365 Business Premium dla maksymalnie 300 stanowisk i uzyskać subskrypcję Microsoft 365 E3 dla ponad 300 stanowisk.</span><span class="sxs-lookup"><span data-stu-id="cef48-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="cef48-112">Program Microsoft Defender dla Office 365 nie jest jednak dołączony do platformy Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cef48-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="cef48-113">W celu dalszej ochrony przed zagrożeniami należy dodać kolejne licencje usługi Defender dla usługi Office 365, aby wszyscy użytkownicy w zakresie działań w ramach działań w ramach programu Defender dla usługi Office 365 posiadali licencje.</span><span class="sxs-lookup"><span data-stu-id="cef48-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="cef48-114">Różnice między usługami Microsoft 365 Business Premium i Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="cef48-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="cef48-115">W poniższej tabeli przedstawiono różnice między usługami Microsoft 365 Business Premium i Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cef48-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="cef48-116">Funkcja</span><span class="sxs-lookup"><span data-stu-id="cef48-116">Feature</span></span>    | <span data-ttu-id="cef48-117">Pomoc techniczna w uwitrynie Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="cef48-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="cef48-118">Pomoc techniczna na microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="cef48-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="cef48-119">**Lokalnie**</span><span class="sxs-lookup"><span data-stu-id="cef48-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="cef48-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="cef48-120">Windows 10</span></span>    | <span data-ttu-id="cef48-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="cef48-121">Windows 10 Business</span></span>  |     <span data-ttu-id="cef48-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="cef48-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="cef48-123">Aplikacje pakietu Office\*</span><span class="sxs-lookup"><span data-stu-id="cef48-123">Office apps\*</span></span>    | [<span data-ttu-id="cef48-124">Aplikacje Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="cef48-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="cef48-125">Aplikacje Microsoft 365 dla przedsiębiorstw</span><span class="sxs-lookup"><span data-stu-id="cef48-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="cef48-126">**Aplikacje zwiększające produktywność w chmurze**</span><span class="sxs-lookup"><span data-stu-id="cef48-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="cef48-127">Exchange Online i Outlook</span><span class="sxs-lookup"><span data-stu-id="cef48-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="cef48-128">Limit miejsca do magazynowania 50 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cef48-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="cef48-129">Limit przestrzeni dyskowej 100 GB na skrzynkę pocztową i nieograniczona archiwizacja w u usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cef48-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="cef48-130">Teams</span><span class="sxs-lookup"><span data-stu-id="cef48-130">Teams</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-133">OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="cef48-133">OneDrive for Business</span></span>    | <span data-ttu-id="cef48-134">Limit przestrzeni dyskowej do 1 TB na użytkownika</span><span class="sxs-lookup"><span data-stu-id="cef48-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="cef48-135">Bez ograniczeń</span><span class="sxs-lookup"><span data-stu-id="cef48-135">Unlimited</span></span> | 
| <span data-ttu-id="cef48-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="cef48-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-139">MileIQ</span><span class="sxs-lookup"><span data-stu-id="cef48-139">MileIQ</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="cef48-141">**Ochrona przed zagrożeniami**</span><span class="sxs-lookup"><span data-stu-id="cef48-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="cef48-142">Funkcje zmniejszania powierzchni ataków</span><span class="sxs-lookup"><span data-stu-id="cef48-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="cef48-143">Zobacz tę listę</span><span class="sxs-lookup"><span data-stu-id="cef48-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="cef48-144">Zarządzanie przedsiębiorstwem izolacji na podstawie sprzętu dla programu Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cef48-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="cef48-145">Defender dla Office 365 (plan 1)</span><span class="sxs-lookup"><span data-stu-id="cef48-145">Defender for Office 365 Plan 1</span></span> | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="cef48-147">Nie są uwzględniane, ale można dodać do</span><span class="sxs-lookup"><span data-stu-id="cef48-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="cef48-148">**Zarządzanie tożsamościami**</span><span class="sxs-lookup"><span data-stu-id="cef48-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="cef48-149">Samodzielne resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego usługi Azure AD, dostępu warunkowego, zapisu zwrotnego haseł dla tożsamości lokalnych</span><span class="sxs-lookup"><span data-stu-id="cef48-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-152">Odnajdowanie aplikacji w chmurze, usługa Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="cef48-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-154">Aplikacje usługi Azure AD usługi Office 365 single Sign-On (SSO): 10 aplikacji na użytkownika (aplikacje Galerii SaaS, takie jak Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="cef48-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-157">Logowanie jednokrotne usługi Azure AD Premium 1: bez ograniczeń (aplikacje lokalne za pośrednictwem serwera proxy aplikacji usługi Azure AD i aplikacje nieu galerii przy użyciu szablonów integracji aplikacji usługi Self-Service)</span><span class="sxs-lookup"><span data-stu-id="cef48-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-159">**Zarządzanie urządzeniami i aplikacją**</span><span class="sxs-lookup"><span data-stu-id="cef48-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="cef48-160">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="cef48-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="cef48-163">Virtual Desktop Access (VDA)</span><span class="sxs-lookup"><span data-stu-id="cef48-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="cef48-165">Pulpit wirtualny systemu Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="cef48-165">Windows Virtual Desktop (WVD)</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="cef48-168">Aktywacja na komputerze udostępnionym (SCA, Shared Computer Activation)</span><span class="sxs-lookup"><span data-stu-id="cef48-168">Shared Computer Activation (SCA)</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-171">Pakiet optymalizacji pulpitu firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="cef48-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-173">**Ochrona informacji**</span><span class="sxs-lookup"><span data-stu-id="cef48-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="cef48-174">Ochrona przed utratą danych w usłudze Office 365, Azure Information Protection Plan 1</span><span class="sxs-lookup"><span data-stu-id="cef48-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-177">Ochrona informacji o oknie dla ochrony przed DLP punktu końcowego</span><span class="sxs-lookup"><span data-stu-id="cef48-177">Window Information Protection for endpoint DLP</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-180">**Licencja dostępu klienta (prawa cal)**</span><span class="sxs-lookup"><span data-stu-id="cef48-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="cef48-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Menedżer konfiguracji, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="cef48-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-183">**Zgodność**</span><span class="sxs-lookup"><span data-stu-id="cef48-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="cef48-184">Nieograniczona archiwizacja wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="cef48-184">Unlimited email archiving</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-187">Menedżer zgodności</span><span class="sxs-lookup"><span data-stu-id="cef48-187">Compliance Manager</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-190">zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="cef48-190">eDiscovery</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-193">Zawieszenie w miejscu i postępowanie sądowe</span><span class="sxs-lookup"><span data-stu-id="cef48-193">In-place hold and litigation hold</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cef48-196">Tagi przechowywania i zasady przechowywania zarządzania rekordami wiadomości (MRM)</span><span class="sxs-lookup"><span data-stu-id="cef48-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="cef48-199">\* Użytkownicy, którym przypisano dostęp do aplikacji SaaS, mogą uzyskać dostęp do logowania jednokrotnego do maksymalnie 10 aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cef48-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="cef48-200">Administratorzy mogą konfigurować logowanie jednokrotne i zmieniać dostęp użytkowników do różnych aplikacji SaaS, ale dostęp do logowania jednokrotnego jest dozwolony tylko dla 10 aplikacji na użytkownika jednocześnie.</span><span class="sxs-lookup"><span data-stu-id="cef48-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="cef48-201">Wszystkie aplikacje usługi Office 365 są liczone jako jedna aplikacja.</span><span class="sxs-lookup"><span data-stu-id="cef48-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="cef48-202">Migracja</span><span class="sxs-lookup"><span data-stu-id="cef48-202">Migration</span></span>

<span data-ttu-id="cef48-203">Aby przeprowadzić migrację, we współpracy z partnerem przenieś subskrypcję i licencje Microsoft 365 Business Premium do odpowiedniej subskrypcji Microsoft 365 E3 wraz z jej licencjami.</span><span class="sxs-lookup"><span data-stu-id="cef48-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="cef48-204">W poniższych sekcjach opisano, jakie zmiany należy wprowadzić, jeśli są, oraz co można zrobić po migracji.</span><span class="sxs-lookup"><span data-stu-id="cef48-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="cef48-205">Dane i konfiguracja subskrypcji platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cef48-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="cef48-206">Nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych przed migracją, co obejmuje:</span><span class="sxs-lookup"><span data-stu-id="cef48-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="cef48-207">Konfiguracja subskrypcji, taka jak nazwy domen DNS.</span><span class="sxs-lookup"><span data-stu-id="cef48-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="cef48-208">Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="cef48-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="cef48-209">Konfiguracje usługi zwiększającej produktywność i ich dane, takie jak zespoły, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.</span><span class="sxs-lookup"><span data-stu-id="cef48-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="cef48-210">Użytkownicy mogą teraz korzystać z nieograniczonej przestrzeni dyskowej w skrzynkach pocztowych usługi Exchange Online i folderach usługi OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="cef48-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="cef48-211">Możesz zacząć korzystać z funkcji odnajdowania aplikacji w chmurze, usługi Azure AD Connect Health i logowania jednokrotnego dla ponad 10 aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cef48-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="cef48-212">Użytkownicy zmigrowany do platformy Microsoft 365 E3 nie mogą już korzystać z usługi MileIQ.</span><span class="sxs-lookup"><span data-stu-id="cef48-212">Users migrated to Microsoft 365 E3 can no longer use MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="cef48-213">Ochrona przed zagrożeniami</span><span class="sxs-lookup"><span data-stu-id="cef48-213">Threat protection</span></span>

<span data-ttu-id="cef48-214">System Windows 10 Business zapewnia następujące zabezpieczenia:</span><span class="sxs-lookup"><span data-stu-id="cef48-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="cef48-215">Wymuszanie integralności procesu rozruchu systemu operacyjnego</span><span class="sxs-lookup"><span data-stu-id="cef48-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="cef48-216">Wymuszanie integralności poufnych składników operacyjnych</span><span class="sxs-lookup"><span data-stu-id="cef48-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="cef48-217">Zaawansowana luki w zabezpieczeniach i środki zaradcze wykorzystujące luki w zabezpieczeniach typu "zero-day"</span><span class="sxs-lookup"><span data-stu-id="cef48-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="cef48-218">Ochrona sieci oparta na reputacji dla przeglądarek Microsoft Edge, Internet Explorer i Chrome</span><span class="sxs-lookup"><span data-stu-id="cef48-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="cef48-219">Zapora oparta na hoście</span><span class="sxs-lookup"><span data-stu-id="cef48-219">Host-based firewall</span></span>
- <span data-ttu-id="cef48-220">Środki zaradcze oprogramowania wymuszającego okup</span><span class="sxs-lookup"><span data-stu-id="cef48-220">Ransomware mitigations</span></span>
- <span data-ttu-id="cef48-221">Izolowanie oparte na sprzęcie dla programu Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cef48-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="cef48-222">Sterowanie aplikacją obsługiwane przez funkcja Intelligent Security Graph</span><span class="sxs-lookup"><span data-stu-id="cef48-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="cef48-223">Sterowanie urządzeniem (USB)</span><span class="sxs-lookup"><span data-stu-id="cef48-223">Device control (USB)</span></span>
- <span data-ttu-id="cef48-224">Ochrona sieci przed zagrożeniami internetowymi</span><span class="sxs-lookup"><span data-stu-id="cef48-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="cef48-225">Reguły zapobiegania intruzom hostów</span><span class="sxs-lookup"><span data-stu-id="cef48-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="cef48-226">System Windows 10 Enterprise E3 obejmuje również zarządzanie przedsiębiorstwem izolacji na podstawie sprzętu dla programu Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="cef48-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="cef48-227">Użytkownicy migrowany do platformy Microsoft 365 E3 będą wymagali licencji programu Microsoft Defender dla usługi Office 365 na kontynuowanie ochrony przed zagrożeniami.</span><span class="sxs-lookup"><span data-stu-id="cef48-227">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="cef48-228">Pamiętaj o zakupie dodatkowych licencji usługi Defender dla usługi Office 365, tak aby wszyscy użytkownicy korzystający z usług Defender dla office 365 posiadali licencje.</span><span class="sxs-lookup"><span data-stu-id="cef48-228">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="cef48-229">Zarządzanie urządzeniami za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="cef48-229">Device management with Intune</span></span>

<span data-ttu-id="cef48-230">Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, która obejmuje zarejestrowane urządzenia oraz ustawienia urządzeń i aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cef48-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="cef48-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="cef48-231">Windows 10</span></span>

<span data-ttu-id="cef48-232">Usługa Microsoft 365 Business Premium zawiera system Windows 10 Business, który można zainstalować za pomocą rozwiązania Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="cef48-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="cef48-233">Podczas migracji do platformy Microsoft 365 E3 każda licencja użytkownika obejmuje system Windows 10 Enterprise E3, który można również zainstalować za pomocą rozwiązania Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="cef48-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="cef48-234">Aplikacje Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="cef48-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="cef48-235">Klient aplikacji Microsoft 365 dla firm zainstalowany na Twoich urządzeniach automatycznie zacznie korzystać z funkcji aplikacji platformy Microsoft 365 dla przedsiębiorstw.</span><span class="sxs-lookup"><span data-stu-id="cef48-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="cef48-236">Po migracji możesz teraz użyć:</span><span class="sxs-lookup"><span data-stu-id="cef48-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="cef48-237">zasady grupy pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="cef48-237">Group Policy support</span></span>
 - <span data-ttu-id="cef48-238">Porównywanie arkuszy kalkulacyjnych i inquire</span><span class="sxs-lookup"><span data-stu-id="cef48-238">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="cef48-239">Funkcje analizy biznesowej</span><span class="sxs-lookup"><span data-stu-id="cef48-239">Business intelligence</span></span>

