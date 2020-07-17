---
title: Synchronizowanie użytkowników domeny z platformą Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Synchronizuj użytkowników kontrolowanych przez domenę z platformą Microsoft 365 dla firm.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081908"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="591be-103">Synchronizowanie użytkowników domeny z platformą Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="591be-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="591be-104">1. Przygotowanie do synchronizacji katalogów</span><span class="sxs-lookup"><span data-stu-id="591be-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="591be-105">Przed zsynchronizowanie użytkowników i komputerów z lokalnej domeny usługi Active Directory należy zapoznać się z recenzją [Prepare for directory synchronizacji do usługi Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="591be-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="591be-106">W szczególności:</span><span class="sxs-lookup"><span data-stu-id="591be-106">In particular:</span></span>

   - <span data-ttu-id="591be-107">Upewnij się, że w katalogu nie istnieją duplikaty dla następujących atrybutów: **poczta,** **proxyAddresses**i **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="591be-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="591be-108">Wartości te muszą być unikatowe i wszystkie duplikaty muszą zostać usunięte.</span><span class="sxs-lookup"><span data-stu-id="591be-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="591be-109">Zaleca się skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego w taki sposób, aby odpowiadał podstawowemu adresowi e-mail odpowiadającemu licencjonowanemu użytkownikowi usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="591be-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="591be-110">Na przykład: *mary.shelley@contoso.com,* a nie *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="591be-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="591be-111">Jeśli domena usługi Active Directory kończy się sufiksem niesygnawalnym, takim jak *.local* lub *.lan,* zamiast sufiksu z routingiem internetowym, takim jak *.com* lub *.org,* dostosuj sufiks nazwy UPN kont użytkowników lokalnych, zgodnie z opisem w [polu Przygotuj domenę nie rutowalną do synchronizacji katalogów.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="591be-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="591be-112">**Uruchom IdFix** w kroku czwartym (4) poniżej, upewnij się również, że lokalna usługa Active Directory jest gotowa do synchronizacji dir.</span><span class="sxs-lookup"><span data-stu-id="591be-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="591be-113">2. Instalowanie i konfigurowanie usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="591be-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="591be-114">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory w usłudze Azure Active Directory, zainstaluj usługę Azure Active Directory Connect i skonfiguruj synchronizację katalogów.</span><span class="sxs-lookup"><span data-stu-id="591be-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="591be-115">W centrum administracyjnym przy <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> wyborze **Instalatora** w lewej konsoli.</span><span class="sxs-lookup"><span data-stu-id="591be-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="591be-116">W obszarze **Logowanie i zabezpieczenia**wybierz pozycję **Wyświetl** w obszarze **Synchronizuj użytkowników z katalogu organizacji**.</span><span class="sxs-lookup"><span data-stu-id="591be-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="591be-117">Na stronie **Synchronizuj użytkowników z katalogu organizacji** wybierz pozycję **Wprowadzenie**.</span><span class="sxs-lookup"><span data-stu-id="591be-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="591be-118">W pierwszym kroku uruchom narzędzie IdFix, aby przygotować się do synchronizacji katalogu.</span><span class="sxs-lookup"><span data-stu-id="591be-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="591be-119">Wykonaj kroki kreatora, aby pobrać usługę Azure AD Connect i użyj jej do zsynchronizowania użytkowników kontrolowanych przez domenę z usługą Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="591be-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="591be-120">Aby dowiedzieć się więcej, zobacz [Konfigurowanie synchronizacji katalogów dla usługi Microsoft 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="591be-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="591be-121">Podczas konfigurowania opcji usługi Azure AD Connect zaleca się włączenie **synchronizacji haseł,** **bezproblemowego logowania jednokrotnego**i funkcji **zapisywania zwrotnego hasła,** która jest również obsługiwana w usłudze Microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="591be-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="591be-122">Istnieje kilka dodatkowych kroków dotyczących zapisywania zwrotnego hasła poza polem wyboru w usłudze Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="591be-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="591be-123">Aby uzyskać więcej informacji, zobacz [Instrukcje: konfigurowanie storamentu hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="591be-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="591be-124">Jeśli chcesz również zarządzać urządzeniami z systemem Windows 10 przyłączonych do domeny, zobacz [Włączanie urządzeń z systemem Windows 10 przyłączonych do domeny, którymi ma zarządzać usługa Microsoft 365 Business Premium](manage-windows-devices.md) w celu skonfigurowania hybrydowego dołączania do usługi Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="591be-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 