---
title: "Ustawienia profilu rozwiązania AutoPilot \x97 informacje"
f1.keywords:
- NOCSH
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
description: Profile programu AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkownika. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pominięcie instalacji Cortany.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593338"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="d4eef-104">Ustawienia profilu rozwiązania AutoPilot  informacje</span><span class="sxs-lookup"><span data-stu-id="d4eef-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="d4eef-105">Ustawienia profilu Programu AutoPilot</span><span class="sxs-lookup"><span data-stu-id="d4eef-105">AutoPilot profile settings</span></span>

<span data-ttu-id="d4eef-106">Za pomocą profilów programu AutoPilot można kontrolować sposób instalowania systemu Windows na urządzeniach użytkownika.</span><span class="sxs-lookup"><span data-stu-id="d4eef-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="d4eef-107">Profile zawierają następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="d4eef-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="d4eef-108">**Domyślne funkcje AutoPilota (wymagane), które są ustawiane automatycznie:**</span><span class="sxs-lookup"><span data-stu-id="d4eef-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="d4eef-109">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="d4eef-109">**Setting**</span></span>|<span data-ttu-id="d4eef-110">**Opis**</span><span class="sxs-lookup"><span data-stu-id="d4eef-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4eef-111">Pomiń cortanę, onedrive i rejestrację oem</span><span class="sxs-lookup"><span data-stu-id="d4eef-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="d4eef-112">Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobista usługa OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4eef-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="d4eef-113">Użytkownik urządzenia może zainstalować je później, o ile użytkownik jest administratorem lokalnym na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="d4eef-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="d4eef-114">Oryginalna rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d4eef-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="d4eef-115">Zaloguj się do marki swojej firmy</span><span class="sxs-lookup"><span data-stu-id="d4eef-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="d4eef-116">Jeśli twoja firma ma [markę Dodaj firmę do strony logowania do usługi Office 365,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)użytkownik urządzenia otrzyma to środowisko podczas logowania.</span><span class="sxs-lookup"><span data-stu-id="d4eef-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="d4eef-117">Automatyczna rejestracja usługi MDM przy skonfigurowanych kontach add.</span><span class="sxs-lookup"><span data-stu-id="d4eef-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="d4eef-118">Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemów Windows i usługi Office 365 przy użyciu poświadczeń usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d4eef-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="d4eef-119">**Ustawienia opcjonalne:**</span><span class="sxs-lookup"><span data-stu-id="d4eef-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="d4eef-120">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="d4eef-120">**Setting**</span></span>|<span data-ttu-id="d4eef-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="d4eef-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4eef-122">Pomijanie ustawień prywatności (domyślnie wyłączone)</span><span class="sxs-lookup"><span data-stu-id="d4eef-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="d4eef-123">Jeśli ta opcja jest ustawiona na **Włączone,** użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy po raz pierwszy się zaloguje.</span><span class="sxs-lookup"><span data-stu-id="d4eef-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="d4eef-124">Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym</span><span class="sxs-lookup"><span data-stu-id="d4eef-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="d4eef-125">Jeśli ta opcja jest ustawiona na **Włączone,** użytkownik urządzenia nie będzie mógł zainstalować żadnych osobistych aplikacji, takich jak Cortana.</span><span class="sxs-lookup"><span data-stu-id="d4eef-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
