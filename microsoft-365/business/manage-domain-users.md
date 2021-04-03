---
title: Synchronizowanie użytkowników domeny z usługą Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Synchronizowanie użytkowników kontrolowanych domeną z platformą Microsoft 365 dla firm.
ms.openlocfilehash: b477b8a1f35a790d6c49937c973c141ad9f90ad4
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578412"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="87777-103">Synchronizowanie użytkowników domeny z usługą Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="87777-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="87777-104">1. Przygotowywanie do synchronizacji katalogów</span><span class="sxs-lookup"><span data-stu-id="87777-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="87777-105">Przed zsynchronizowaniem użytkowników i komputerów z lokalnej domeny usługi Active Directory zapoznaj się z tematem Przygotowanie do synchronizacji katalogów [z platformą Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="87777-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="87777-106">W szczególności:</span><span class="sxs-lookup"><span data-stu-id="87777-106">In particular:</span></span>

   - <span data-ttu-id="87777-107">Upewnij się, że w katalogu nie występują duplikaty następujących atrybutów: **mail,** **proxyAddresses** i **userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="87777-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="87777-108">Te wartości muszą być unikatowe, a wszelkie duplikaty muszą zostać usunięte.</span><span class="sxs-lookup"><span data-stu-id="87777-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="87777-109">Zalecamy skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego tak, aby był on taki, jak podstawowy adres e-mail odpowiadający licencjonowanemu użytkownikowi platformy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="87777-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="87777-110">Na przykład: *mary.shelley@contoso.com* zamiast *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="87777-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="87777-111">Jeśli domena usługi Active Directory kończy się sufiksem nie routowalnym, takim jak *.local* lub *lan,* zamiast sufiksu routowalnego przez Internet, takiego jak *.com* lub *.org,* najpierw dostosuj sufiks upn kont użytkowników lokalnych zgodnie z opisem w tesłudze Przygotowywanie domeny nie routowalnej do synchronizacji [katalogów.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="87777-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="87777-112">Uruchomienie **programu IdFix** w kroku 4 (4) poniżej spowoduje również upewninie się, że lokalna usługa Active Directory jest gotowa do synchronizacji katalogów.</span><span class="sxs-lookup"><span data-stu-id="87777-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="87777-113">2. Instalowanie i konfigurowanie programu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="87777-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="87777-114">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, zainstaluj narzędzie Azure Active Directory Connect i skonfiguruj synchronizację katalogów.</span><span class="sxs-lookup"><span data-stu-id="87777-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="87777-115">W centrum [administracyjnym wybierz](https://go.microsoft.com/fwlink/p/?linkid=2024339) **pozycję Konfiguracja w** lewym okienku narracji.</span><span class="sxs-lookup"><span data-stu-id="87777-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="87777-116">W **obszarze Logowanie i zabezpieczenia wybierz** pozycję **Wyświetl** w obszarze Synchronizowanie użytkowników z **katalogu organizacji.**</span><span class="sxs-lookup"><span data-stu-id="87777-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="87777-117">Na stronie **Synchronizuj użytkowników** z katalogu organizacji wybierz pozycję **Wprowadzenie.**</span><span class="sxs-lookup"><span data-stu-id="87777-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="87777-118">W pierwszym kroku uruchom narzędzie IdFix, aby przygotować się do synchronizacji katalogów.</span><span class="sxs-lookup"><span data-stu-id="87777-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="87777-119">Postępuj zgodnie z instrukcjami kreatora, aby pobrać program Azure AD Connect i za jego pomocą zsynchronizować użytkowników kontrolowanych domeną z platformą Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="87777-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="87777-120">Aby dowiedzieć się więcej, zobacz Konfigurowanie synchronizacji katalogów na platformie [Microsoft 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="87777-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="87777-121">Podczas konfigurowania opcji dla programu Azure AD Connect zalecamy włączenie synchronizacji **haseł,**  bezproblemowego logowania pojedynczego i funkcji zapisu hasła, która jest również obsługiwana na platformie Microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="87777-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="87777-122">Istnieje kilka dodatkowych kroków zapisu hasła poza polem wyboru w programie Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="87777-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="87777-123">Aby uzyskać więcej informacji, zobacz [Jak skonfigurować pisanie hasła.](/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="87777-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="87777-124">Jeśli chcesz również zarządzać urządzeniami z systemem Windows 10 przyłączanych do domeny, zobacz Włączanie zarządzania przez platformę [Microsoft 365 Business Premium](manage-windows-devices.md) dla urządzeń przyłącznych do domeny w celu skonfigurowania hybrydowego dołączenia do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="87777-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>