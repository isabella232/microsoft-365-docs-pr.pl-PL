---
title: Migrowanie do Microsoft 365 Business z Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Jeśli masz subskrypcję Office 365 E3, ale nie masz więcej niż 300 pracowników, rozważ przełączenie się do Microsoft 365 Business Premium.
ms.openlocfilehash: d139d07c946ff3efed3db3a73eb5e1a4ae66c190
ms.sourcegitcommit: 686f192e1a650ec805fe8e908b46ca51771ed41f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52623610"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="daf43-103">Migrowanie z Office 365 E3 do Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="daf43-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="daf43-104">Microsoft 365 Business Premium wszystko, czego potrzebujesz dla swojej małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami.</span><span class="sxs-lookup"><span data-stu-id="daf43-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="daf43-105">Jeśli obecnie masz subskrypcję Office 365 E3, ale nie masz więcej niż 300 pracowników, rozważ przełączenie się do usługi Microsoft 365 Business Premium w celu uwzględnienia dodatkowych funkcji zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="daf43-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="daf43-106">Migracja jest łatwa: najpierw przełączasz licencje, a wszystkie dane i informacje o użytkownikach w bieżącej subskrypcji są zachowywane.</span><span class="sxs-lookup"><span data-stu-id="daf43-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="daf43-107">Po migracji musisz skonfigurować funkcje, które są dodawane w programie Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="daf43-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="daf43-108">Różnice między Office 365 E3 a Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="daf43-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="daf43-109">W poniższej tabeli przedstawiono różnice między Microsoft 365 Business Premium a Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="daf43-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="daf43-110">Funkcja</span><span class="sxs-lookup"><span data-stu-id="daf43-110">Feature</span></span>    | <span data-ttu-id="daf43-111">Pomoc techniczna w Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="daf43-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="daf43-112">Pomoc techniczna w Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="daf43-112">Support in Office 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="daf43-113">**Lokalnie**</span><span class="sxs-lookup"><span data-stu-id="daf43-113">**On-premises**</span></span>        | | |
| <span data-ttu-id="daf43-114">Office aplikacji<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="daf43-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="daf43-115">Aplikacje Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="daf43-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="daf43-116">Aplikacje usługi Microsoft 365 dla przedsiębiorstw</span><span class="sxs-lookup"><span data-stu-id="daf43-116">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="daf43-117">**Aplikacje zwiększające produktywność w chmurze**</span><span class="sxs-lookup"><span data-stu-id="daf43-117">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="daf43-118">Exchange Online i Outlook</span><span class="sxs-lookup"><span data-stu-id="daf43-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="daf43-119">50 GB miejsca do magazynowania na skrzynkę pocztową i nieograniczona liczba Exchange Online — archiwum</span><span class="sxs-lookup"><span data-stu-id="daf43-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="daf43-120">100 GB miejsca do magazynowania na skrzynkę pocztową i nieograniczona liczba Exchange Online — archiwum</span><span class="sxs-lookup"><span data-stu-id="daf43-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> |
| <span data-ttu-id="daf43-121">Teams</span><span class="sxs-lookup"><span data-stu-id="daf43-121">Teams</span></span>    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="daf43-124">OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="daf43-124">OneDrive for Business</span></span>    | <span data-ttu-id="daf43-125">1 TB miejsca do magazynowania na użytkownika</span><span class="sxs-lookup"><span data-stu-id="daf43-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="daf43-126">Bez ograniczeń</span><span class="sxs-lookup"><span data-stu-id="daf43-126">Unlimited</span></span> | 
| <span data-ttu-id="daf43-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="daf43-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="daf43-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="daf43-130">StaffHub</span></span>    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png) |
| <span data-ttu-id="daf43-133">**Ochrona przed zagrożeniami**</span><span class="sxs-lookup"><span data-stu-id="daf43-133">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="daf43-134">Defender dla Office 365 Plan 1</span><span class="sxs-lookup"><span data-stu-id="daf43-134">Defender for Office 365 Plan 1</span></span> | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="daf43-136">Nie dołączona, ale można ją dodać do</span><span class="sxs-lookup"><span data-stu-id="daf43-136">Not included, but can be added on</span></span> |
| <span data-ttu-id="daf43-137">**Zarządzanie tożsamościami**</span><span class="sxs-lookup"><span data-stu-id="daf43-137">**Identity management**</span></span>        | | |
| <span data-ttu-id="daf43-138">Samodzielne resetowanie hasła dla kont Azure Active Directory hybrydowych (Azure AD), uwierzytelnianie wieloskładnikowe (MFA), dostęp warunkowy, funkcja zapisu hasła dla tożsamości lokalnych</span><span class="sxs-lookup"><span data-stu-id="daf43-138">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="daf43-140">**Zarządzanie urządzeniami i aplikacją**</span><span class="sxs-lookup"><span data-stu-id="daf43-140">**Device and app management**</span></span>        | | |
| <span data-ttu-id="daf43-141">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="daf43-141">Microsoft Intune, Windows AutoPilot</span></span>|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="daf43-143">Aktywacja na komputerze udostępnionym</span><span class="sxs-lookup"><span data-stu-id="daf43-143">Shared computer activation</span></span>|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="daf43-146">Prawa do uaktualnienia do Windows 10 Pro z licencji win 7/8.1 Pro Windows</span><span class="sxs-lookup"><span data-stu-id="daf43-146">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    ||
| <span data-ttu-id="daf43-148">**Ochrona informacji**</span><span class="sxs-lookup"><span data-stu-id="daf43-148">**Information protection**</span></span>        | | |
|<span data-ttu-id="daf43-149">Office 365 Ochrona przed utratą danych</span><span class="sxs-lookup"><span data-stu-id="daf43-149">Office 365 Data Loss Prevention</span></span>|    ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)|![Dołączona do Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="daf43-152">Azure Information Protection Plan 1, funkcja BitLocker wymuszanie</span><span class="sxs-lookup"><span data-stu-id="daf43-152">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="daf43-154">Azure Information Protection Plan 1, Etykiety wrażliwości</span><span class="sxs-lookup"><span data-stu-id="daf43-154">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="daf43-156">**Licencja dostępu klienta (prawa calowe)**</span><span class="sxs-lookup"><span data-stu-id="daf43-156">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="daf43-157">Enterprise Cal Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="daf43-157">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Dołączona do Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="daf43-159"><sup>1</sup> Microsoft 365 Business Premium pakietu Office nie obejmuje aktywacji zbiorczej za pośrednictwem usługi zasady grupy, telemetrii aplikacji, kontrolek aktualizacji, porównywania i ineksji arkuszy kalkulacyjnych ani analizy biznesowej.</span><span class="sxs-lookup"><span data-stu-id="daf43-159"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="daf43-160">Migracja</span><span class="sxs-lookup"><span data-stu-id="daf43-160">Migration</span></span>

<span data-ttu-id="daf43-161">Aby przeprowadzić migrację subskrypcji, [zobacz](../commerce/subscriptions/change-plans-manually.md) Ręczne zmienianie planów, aby uzyskać instrukcje dotyczące przenoszenia tylko kilku osób do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="daf43-161">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="daf43-162">Możesz również [uaktualnić wszystkich automatycznie](../commerce/subscriptions/upgrade-to-different-plan.md)lub we współpracy z partnerem przenieść Twoją subskrypcję I licencje E3 do subskrypcji Microsoft 365 Business Premium subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="daf43-162">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="daf43-163">W poniższych sekcjach opisano zmiany, które należy wprowadzić (o ile są) oraz czynności, które można wprowadzić po migracji.</span><span class="sxs-lookup"><span data-stu-id="daf43-163">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="daf43-164">Office 365 Dane i konfiguracja subskrypcji E3</span><span class="sxs-lookup"><span data-stu-id="daf43-164">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="daf43-165">Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:</span><span class="sxs-lookup"><span data-stu-id="daf43-165">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="daf43-166">Konfiguracja subskrypcji, taka jak rekordy DNS i nazwy domen.</span><span class="sxs-lookup"><span data-stu-id="daf43-166">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="daf43-167">Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="daf43-167">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="daf43-168">Konfiguracje usługi zwiększającej produktywność i ich dane, takie Teams, Exchange Online pocztowe, SharePoint online, OneDrive dla Firm foldery i OneNote notesy.</span><span class="sxs-lookup"><span data-stu-id="daf43-168">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="daf43-169">Office aplikacja skaluje się automatycznie.</span><span class="sxs-lookup"><span data-stu-id="daf43-169">Office applications will scale automatically.</span></span> <span data-ttu-id="daf43-170">Office 365 nowoczesne licencjonowanie sprawdza przypisanie licencji użytkownika co 72 godziny i konwertuje aplikacje Office na wersję, która jest taka, jak subskrypcja użytkownika.</span><span class="sxs-lookup"><span data-stu-id="daf43-170">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="daf43-171">Windows 10</span><span class="sxs-lookup"><span data-stu-id="daf43-171">Windows 10</span></span>

<span data-ttu-id="daf43-172">Jeśli Twoje Windows nie są jeszcze w aktualizacji Windows Pro, uaktualnij je do Windows Pro [dla twórców.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="daf43-172">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="daf43-173">Konfigurowanie zasad ochrony urządzeń i plików użytkowników</span><span class="sxs-lookup"><span data-stu-id="daf43-173">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="daf43-174">Jeśli skonfigurujesz zasady Office 365 mdM, te urządzenia będą wyświetlane  na stronie Urządzenia w centrum administracyjnym usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="daf43-174">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="daf43-175">Wszystkie zasady, które skonfigurujsz, będą wyświetlane na liście zasad klasycznych w [portalu usługi Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="daf43-175">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="daf43-176">Po przypisaniu licencji do Microsoft 365 Business Premium możesz rozpocząć ochronę urządzeń i plików użytkowników.</span><span class="sxs-lookup"><span data-stu-id="daf43-176">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="daf43-177">Jeśli wszystkie osoby w organizacji zostały uaktualnione do programu Microsoft 365 Business Premium, na stronie głównej zostanie wyświetlony kreator konfiguracji, który może wykonać instrukcje Konfigurowanie usługi [Microsoft 365 Business Premium](set-up.md) w kreatorze konfiguracji w celu ochrony plików i urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="daf43-177">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="daf43-178">Na stronie Urządzenia możesz również wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="daf43-178">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="daf43-179">W centrum administracyjnym w lewym okienku narracji przejdź do **pozycji Zasady dotyczące** \> **urządzeń.**</span><span class="sxs-lookup"><span data-stu-id="daf43-179">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="daf43-180">Na stronie **Zasady dotyczące urządzeń** wybierz pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="daf43-180">On the **Device policies** page, choose **Add**.</span></span>

3. <span data-ttu-id="daf43-181">W **okienku Dodaj** zasady nadaj zasadom nazwę, **a** następnie z listy rozwijanej wybierz typ zasad.</span><span class="sxs-lookup"><span data-stu-id="daf43-181">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span>

     <span data-ttu-id="daf43-182">Możesz skonfigurować zasady aplikacji do ochrony plików na urządzeniach z systemami Android i iPhone, a także Windows 10, a także dla firmowych urządzeń Windows 10 urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="daf43-182">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="daf43-183">Aby uzyskać szczegółowe informacje, zobacz następujące linki:</span><span class="sxs-lookup"><span data-stu-id="daf43-183">See the following links for details:</span></span>

  - [<span data-ttu-id="daf43-184">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="daf43-184">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

  - [<span data-ttu-id="daf43-185">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="daf43-185">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

  - [<span data-ttu-id="daf43-186">Konfigurowanie ustawień ochrony urządzeń dla Windows 10 PC</span><span class="sxs-lookup"><span data-stu-id="daf43-186">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="daf43-187">Po skonfigurowaniu zasad Ty i Twoi pracownicy możecie skonfigurować urządzenia:</span><span class="sxs-lookup"><span data-stu-id="daf43-187">Once you set up policies, you and your employees can set up devices:</span></span>

  - <span data-ttu-id="daf43-188">Zobacz [Konfigurowanie Windows dla Microsoft 365 Business Premium,](set-up-windows-devices.md) aby uzyskać instrukcje dotyczące Windows urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="daf43-188">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 

  - <span data-ttu-id="daf43-189">Zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business Premium,](set-up-mobile-devices.md) aby uzyskać instrukcje dotyczące telefonów iPhone i telefonów z systemem Android.</span><span class="sxs-lookup"><span data-stu-id="daf43-189">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="daf43-190">Rozmiar skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="daf43-190">Mailbox Size</span></span>

<span data-ttu-id="daf43-191">Microsoft 365 Business Premium ma limit przestrzeni dyskowej 50 GB, ponieważ korzysta z Exchange Online Plan 1.</span><span class="sxs-lookup"><span data-stu-id="daf43-191">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="daf43-192">Jeśli podczas migracji do programu Microsoft 365 Business Premium żaden z użytkowników przekracza 50 GB miejsca do magazynowania skrzynki pocztowej, zaleca się przypisanie temu użytkownikowi planu Exchange Online 2 i usunięcie planu Exchange Online Plan 1, ponieważ nie jest możliwe przypisanie obu tych wartości.</span><span class="sxs-lookup"><span data-stu-id="daf43-192">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>

### <a name="threat-protection"></a><span data-ttu-id="daf43-193">Ochrona przed zagrożeniami</span><span class="sxs-lookup"><span data-stu-id="daf43-193">Threat protection</span></span>

<span data-ttu-id="daf43-194">Po zakończeniu migracji do programu Microsoft 365 Business Premium masz już programu Defender for Office 365.</span><span class="sxs-lookup"><span data-stu-id="daf43-194">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="daf43-195">Aby [uzyskać omówienie Office 365](../security/office-365-security/defender-for-office-365.md) zobacz Program Microsoft Defender, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="daf43-195">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="daf43-196">Aby to skonfigurować, zobacz konfigurowanie linków Sejf [,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [konfigurowanie](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)załączników Sejf i konfigurowanie ochrony przed wyłudzaniem informacji w programie Defender dla [systemu Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="daf43-196">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="daf43-197">Etykiety wrażliwości</span><span class="sxs-lookup"><span data-stu-id="daf43-197">Sensitivity labels</span></span>

<span data-ttu-id="daf43-198">Aby rozpocząć korzystanie z etykiet wrażliwości, zobacz [Omówienie etykiet wrażliwości](../compliance/sensitivity-labels.md) oraz tworzenie etykiet wrażliwości i zarządzanie nimi — [klip](../business-video/create-sensitivity-labels.md) wideo.</span><span class="sxs-lookup"><span data-stu-id="daf43-198">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>

## <a name="related-content"></a><span data-ttu-id="daf43-199">Zawartość pokrewna</span><span class="sxs-lookup"><span data-stu-id="daf43-199">Related content</span></span>

<span data-ttu-id="daf43-200">[Ręczne zmienianie planów](../commerce/subscriptions/change-plans-manually.md) (artykuł)</span><span class="sxs-lookup"><span data-stu-id="daf43-200">[Change plans manually](../commerce/subscriptions/change-plans-manually.md) (article)</span></span>\
<span data-ttu-id="daf43-201">[Uaktualnianie Windows do Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (wideo)</span><span class="sxs-lookup"><span data-stu-id="daf43-201">[Upgrade Windows devices to Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (video)</span></span>\
<span data-ttu-id="daf43-202">[Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS](app-protection-settings-for-android-and-ios.md) (artykuł)</span><span class="sxs-lookup"><span data-stu-id="daf43-202">[Set app protection settings for Android or iOS devices](app-protection-settings-for-android-and-ios.md) (article)</span></span>\
<span data-ttu-id="daf43-203">[Ustawianie lub edytowanie ustawień ochrony aplikacji dla Windows 10](protection-settings-for-windows-10-devices.md) (artykuł)</span><span class="sxs-lookup"><span data-stu-id="daf43-203">[Set or edit application protection settings for Windows 10 devices](protection-settings-for-windows-10-devices.md) (article)</span></span>\
<span data-ttu-id="daf43-204">[]</span><span class="sxs-lookup"><span data-stu-id="daf43-204">[]</span></span>

