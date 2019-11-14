---
title: "Ustawienia profilu rozwiązania AutoPilot \x97 informacje"
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają domyślne i opcjonalne ustawienia, takie jak Pomiń instalację Cortany.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321790"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="3da68-104">Ustawienia profilu rozwiązania AutoPilot  informacje</span><span class="sxs-lookup"><span data-stu-id="3da68-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="3da68-105">Ustawienia profilu AutoPilot</span><span class="sxs-lookup"><span data-stu-id="3da68-105">AutoPilot profile settings</span></span>

<span data-ttu-id="3da68-106">Profile AutoPilot można używać do kontrolowania sposobu instalowania systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3da68-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="3da68-107">Profile zawierają następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="3da68-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="3da68-108">**Domyślne funkcje autopilota (wymagane), które są ustawiane automatycznie:**</span><span class="sxs-lookup"><span data-stu-id="3da68-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="3da68-109">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="3da68-109">**Setting**</span></span>|<span data-ttu-id="3da68-110">**Opis**</span><span class="sxs-lookup"><span data-stu-id="3da68-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3da68-111">Pomiń rejestrację Cortany, OneDrive i OEM</span><span class="sxs-lookup"><span data-stu-id="3da68-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="3da68-112">Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobisty OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3da68-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="3da68-113">Użytkownik urządzenia może zainstalować je później, o ile użytkownik jest administratorem lokalnym na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="3da68-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="3da68-114">Oryginalna Rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3da68-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="3da68-115">Zaloguj się w swojej firmie</span><span class="sxs-lookup"><span data-stu-id="3da68-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="3da68-116">Jeśli Twoja firma ma [dodać marki firmy do pakietu Office 365 Zaloguj się na stronie](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), użytkownik urządzenia będzie uzyskać to doświadczenie podczas logowania.</span><span class="sxs-lookup"><span data-stu-id="3da68-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="3da68-117">Automatyczna rejestracja MDM z skonfigurowanymi kontami usługi AAD.</span><span class="sxs-lookup"><span data-stu-id="3da68-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="3da68-118">Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemu Windows i pakietu Office 365 za pomocą poświadczeń firmy Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3da68-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="3da68-119">**Ustawienia opcjonalne:**</span><span class="sxs-lookup"><span data-stu-id="3da68-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="3da68-120">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="3da68-120">**Setting**</span></span>|<span data-ttu-id="3da68-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="3da68-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3da68-122">Pomiń ustawienia prywatności (domyślnie wyłączone)</span><span class="sxs-lookup"><span data-stu-id="3da68-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="3da68-123">Jeśli ta opcja jest **włączona**, użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy on lub ona po raz pierwszy loguje się.</span><span class="sxs-lookup"><span data-stu-id="3da68-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="3da68-124">Nie Zezwalaj, aby użytkownik stał się administratorem lokalnym</span><span class="sxs-lookup"><span data-stu-id="3da68-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="3da68-125">Jeśli ta opcja jest **włączona**, użytkownik urządzenia nie będzie mógł instalować żadnych osobistych aplikacji, takich jak Cortana.</span><span class="sxs-lookup"><span data-stu-id="3da68-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
