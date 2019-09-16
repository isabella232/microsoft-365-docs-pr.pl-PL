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
description: Dowiedz się, jak włączyć Microsoft 365 do ochrony lokalnych urządzeń z systemem Windows 10 przyłączonych do usługi AD.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992234"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="a99a2-103">Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="a99a2-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="a99a2-104">Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="a99a2-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="a99a2-105">Można to skonfigurować, najpierw synchronizowanie usługi Active Directory z usługą Azure Active Directory, a następnie rejestrowanie urządzeń z systemem Windows 10 z usługą Azure AD i rejestrowanie ich do zarządzania urządzeniami przenośnymi przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="a99a2-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="a99a2-106">Następujące wideo szczegóły kroki dotyczące sposobu ustawiania tego w najbardziej typowym scenariuszu.</span><span class="sxs-lookup"><span data-stu-id="a99a2-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="a99a2-107">Konfigurowanie urządzeń przyłączonych do domeny, które mają być zarządzane przez firmę Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="a99a2-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="a99a2-108">Aby skonfigurować urządzenia przyłączone do domeny w organizacji, aby korzystać z możliwości oferowanych przez usługę Azure Active Directory oprócz lokalnej usługi Active Directory, można zaimplementować **urządzeń przyłączonych do usługi Azure AD hybrydowy**.</span><span class="sxs-lookup"><span data-stu-id="a99a2-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="a99a2-109">Są to urządzenia, które są przyłączone do lokalnej usługi Active Directory i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a99a2-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="a99a2-110">Hybrydowe urządzenia przyłączone do usługi Azure AD mogą być chronione i zarządzane przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="a99a2-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="a99a2-111">Wykonaj poniższe kroki, aby urządzenia z systemem Windows 10 Hybrid Azure AD dołączył i zarządzane przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="a99a2-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="a99a2-112">Aby zsynchronizować użytkowników, grup i kontaktów z lokalnej usługi Active Directory w usłudze Azure Active Directory, uruchom Kreatora synchronizacji katalogów i Azure Active Directory Connect zgodnie z opisem w [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="a99a2-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="a99a2-113">Kroki są dokładnie takie same dla Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="a99a2-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="a99a2-114">Przed wykonaniem kroku 3, aby włączyć urządzenia systemu Windows 10 do hybrydowego usługi Azure AD dołączył, należy upewnić się, że spełniają następujące wymagania wstępne:</span><span class="sxs-lookup"><span data-stu-id="a99a2-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="a99a2-115">Używasz najnowszej wersji programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a99a2-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="a99a2-116">Azure AD Connect zsynchronizował wszystkie obiekty komputerów urządzeń, które mają być hybrydowego usługi Azure AD dołączył.</span><span class="sxs-lookup"><span data-stu-id="a99a2-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="a99a2-117">Jeśli obiekty komputera należą do określonych jednostek organizacyjnych (OU), upewnij się, że te jednostki organizacyjne są ustawione do synchronizacji w usłudze Azure AD Connect, jak również.</span><span class="sxs-lookup"><span data-stu-id="a99a2-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="a99a2-118">Zarejestruj istniejące urządzenia przyłączone do domeny systemu Windows 10 do hybrydowego usługi Azure AD dołączył i zarejestrować je do zarządzania urządzeniami przenośnymi przez usługę Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="a99a2-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="a99a2-119">Postępuj zgodnie z instrukcjami krok po kroku w [sposobie konfigurowania hybrydowego usługi Azure Active Directory przyłączonych urządzeń](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="a99a2-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="a99a2-120">Umożliwi to synchronizację lokalnej usługi Active Directory przyłączonych komputerów z systemem Windows 10 i sprawi, że będą gotowe do chmury.</span><span class="sxs-lookup"><span data-stu-id="a99a2-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="a99a2-121">Aby zarejestrować urządzenie z systemem Windows 10 do zarządzania urządzeniami przenośnymi, zobacz [Rejestrowanie urządzenia z systemem Windows 10 przy użyciu usługi Intune za pomocą zasad grupy](https://go.microsoft.com/fwlink/p/?linkid=872871) , aby uzyskać instrukcje.</span><span class="sxs-lookup"><span data-stu-id="a99a2-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="a99a2-122">Można ustawić zasady grupy na poziomie komputera lokalnego lub dla operacji zbiorczych, można utworzyć to ustawienie zasad grupy na serwerze kontrolera domeny.</span><span class="sxs-lookup"><span data-stu-id="a99a2-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>