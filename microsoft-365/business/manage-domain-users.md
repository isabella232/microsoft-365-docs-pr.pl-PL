---
title: Synchronizowanie użytkowników domeny z programem Microsoft 365
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
description: Synchronizowanie użytkowników kontrolowanych przez domeny z aplikacją Microsoft 365 dla firm.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306454"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="ff38b-103">Synchronizowanie użytkowników domeny z programem Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ff38b-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="ff38b-104">1. Przygotowywanie do synchronizacji katalogów</span><span class="sxs-lookup"><span data-stu-id="ff38b-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="ff38b-105">Przed zsynchronizowaniem użytkowników i komputerów z lokalnej domeny usługi Active Directory Przejrzyj [przygotowanie do synchronizacji katalogów z systemem Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ff38b-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="ff38b-106">W szczególności:</span><span class="sxs-lookup"><span data-stu-id="ff38b-106">In particular:</span></span>

   - <span data-ttu-id="ff38b-107">Upewnij się, że w katalogu nie ma żadnych duplikatów dla następujących atrybutów: **mail**, **proxyAddresses**i **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="ff38b-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="ff38b-108">Te wartości muszą być unikatowe i muszą być usunięte wszystkie duplikaty.</span><span class="sxs-lookup"><span data-stu-id="ff38b-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="ff38b-109">Zalecamy skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego, aby odpowiadał pierwotnemu adresowi e-mail, który odpowiada licencjonowanemu użytkownikowi usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ff38b-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="ff38b-110">Na przykład: *Mary.Shelley@contoso.com* , a nie *Mary@contoso. Local*</span><span class="sxs-lookup"><span data-stu-id="ff38b-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="ff38b-111">Jeśli domena usługi Active Directory kończy się na takim samym sufiksie, jak *. Local* lub. *LAN*, zamiast sufiksu internetowej obsługi routingu, takiego jak *com* lub *org*, należy dostosować sufiks głównej nazwy użytkownika konta użytkowników lokalnych zgodnie z opisem w części [Przygotowywanie do synchronizacji katalogów](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ff38b-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="ff38b-112">**Uruchomienie narzędzia IdFix** w kroku cztery (4) poniżej spowoduje również upewnienie się, że lokalna usługa Active Directory jest gotowa do synchronizacji katalogu.</span><span class="sxs-lookup"><span data-stu-id="ff38b-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="ff38b-113">2. Instalowanie i Konfigurowanie usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="ff38b-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="ff38b-114">Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, zainstaluj usługę Azure Active Directory Connect i skonfiguruj synchronizację katalogów.</span><span class="sxs-lookup"><span data-stu-id="ff38b-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="ff38b-115">W centrum administracyjnym po <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> wybraniu **Ustawienia** w lewym obszarze nawigacji.</span><span class="sxs-lookup"><span data-stu-id="ff38b-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="ff38b-116">W obszarze **Logowanie i zabezpieczenia**wybierz pozycję **Wyświetl**  w obszarze **Użytkownicy synchronizacji w katalogu**organizacji.</span><span class="sxs-lookup"><span data-stu-id="ff38b-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="ff38b-117">Na stronie **Synchronizuj użytkowników ze swojego katalogu w organizacji** **Wybierz pozycję wprowadzenie.**</span><span class="sxs-lookup"><span data-stu-id="ff38b-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="ff38b-118">W pierwszym kroku Uruchom narzędzie narzędzia IdFix, aby przygotować się do synchronizacji katalogów.</span><span class="sxs-lookup"><span data-stu-id="ff38b-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="ff38b-119">Postępuj zgodnie z instrukcjami kreatora, aby pobrać usługę Azure AD Connect, i użyć jej do zsynchronizowania użytkowników kontrolowanych przez domeny z systemem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ff38b-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="ff38b-120">Aby dowiedzieć się więcej, zobacz [Konfigurowanie synchronizacji katalogów dla programu Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .</span><span class="sxs-lookup"><span data-stu-id="ff38b-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="ff38b-121">Po skonfigurowaniu opcji usługi Azure AD Connect zalecamy włączenie **synchronizacji haseł**, **jednolite logowanie**jednokrotne oraz funkcji **zapisywania zwrotnego haseł** , która jest również obsługiwana w programie Microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="ff38b-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="ff38b-122">Istnieje kilka dodatkowych kroków dotyczących stornowania haseł poza polem wyboru w usłudze Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ff38b-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="ff38b-123">Aby uzyskać więcej informacji, zobacz [instrukcje: Konfigurowanie zapisywania zwrotnego hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="ff38b-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="ff38b-124">Jeśli chcesz zarządzać urządzeniami z systemem Windows 10 dołączonymi do domeny, zobacz [Włączanie zarządzania za pomocą programu Microsoft 365 Business Premium na urządzeniach z systemem Windows 10 przyłączonych do domeny](manage-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="ff38b-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 