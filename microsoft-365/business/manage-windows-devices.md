---
title: Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dowiedz się, jak włączyć Microsoft 365 do ochrony AD lokalnych połączonych urządzeń Windows 10.
ms.openlocfilehash: af0e78ef6e79bfd612b11a16538e7afcd377ffb0
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071555"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="90eb7-103">Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="90eb7-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="90eb7-104">Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych.</span><span class="sxs-lookup"><span data-stu-id="90eb7-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="90eb7-105">Możesz ustawić to dzięki pierwszej synchronizacji usługi Active Directory z usługą Active Directory, a następnie rejestracji urządzeń 10 systemu Windows Azure AD i zapisywania ich do zarządzania urządzeniami przenośnymi przez Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="90eb7-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="90eb7-106">Konfigurowanie urządzeń przyłączonych do domeny mają być zarządzane przez Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="90eb7-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="90eb7-107">Aby skonfigurować urządzenia przyłączone do domeny organizacji do korzystania z możliwości oferowane przez usługę Active Directory Azure oprócz lokalnej usługi Active Directory, można zaimplementować **hybrydowy Azure AD dołączył do urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="90eb7-107">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="90eb7-108">Są to urządzenia, które są połączone, zarówno w usłudze Active Directory na lokalnym i usługi Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="90eb7-108">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="90eb7-109">Urządzeniach hybrydowych Azure AD dołączył do mogą być chronione i zarządzane przez Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="90eb7-109">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="90eb7-110">Należy wykonać poniższe kroki, aby utworzyć urządzeniach 10 systemu Windows Azure AD przyłączony i zarządzany przez Microsoft 365 Business hybrydowy.</span><span class="sxs-lookup"><span data-stu-id="90eb7-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="90eb7-111">Aby zsynchronizować użytkowników, grup i kontakty z lokalną usługę Active Directory z usługą Active Directory Azure, uruchom Kreatora synchronizacji katalogu i Azure Active Directory połączyć zgodnie z opisem w [Konfigurowanie synchronizacji katalogów usługi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="90eb7-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="90eb7-112">Kroki są dokładnie takie same dla Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="90eb7-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="90eb7-113">Przed wykonaniem kroku 3, aby włączyć w urządzeniach Windows 10 za hybrydowe dołączył do Azure AD, należy upewnić się, że spełniasz następujące wymagania wstępne:</span><span class="sxs-lookup"><span data-stu-id="90eb7-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="90eb7-114">Używasz najnowszej wersji programu Azure AD connect.</span><span class="sxs-lookup"><span data-stu-id="90eb7-114">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="90eb7-115">Połączyć Azure AD został zsynchronizowany wszystkie obiekty komputera ma być hybrydowy Azure AD dołączył do urządzeń.</span><span class="sxs-lookup"><span data-stu-id="90eb7-115">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="90eb7-116">Jeśli obiekty komputerów należą do poszczególnych jednostek organizacyjnych (OU), a następnie upewnij się, że te jednostki organizacyjne są ustawione dla synchronizacji w Azure AD również połączyć.</span><span class="sxs-lookup"><span data-stu-id="90eb7-116">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="90eb7-117">Zarejestruj istniejących urządzeniach Windows 10 domeny hybrydowy Azure AD połączonych i zapisać je do zarządzania urządzeniami przenośnymi przez Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="90eb7-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="90eb7-118">Postępuj zgodnie z instrukcjami krok po kroku, w [jaki sposób skonfigurować hybrydowy Azure Active Directory dołączył do urządzenia](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="90eb7-118">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="90eb7-119">Spowoduje to włączenie synchronizacji usługi Active Directory na lokalnym przyłączony systemie Windows 10 komputerów i ich gotowości w chmurze.</span><span class="sxs-lookup"><span data-stu-id="90eb7-119">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="90eb7-120">Aby zarejestrować urządzenie Windows 10 do zarządzania urządzeniami przenośnymi, zobacz [Rejestrowanie urządzeń systemu Windows 10 z Windows Intune za pomocą zasady grupy](https://go.microsoft.com/fwlink/p/?linkid=872871) instrukcje.</span><span class="sxs-lookup"><span data-stu-id="90eb7-120">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="90eb7-121">Poziom można ustawić zasady grupy na komputerze lokalnym lub operacje zbiorcze można utworzyć ustawienie zasad grupy na serwerze kontrolera domeny.</span><span class="sxs-lookup"><span data-stu-id="90eb7-121">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>