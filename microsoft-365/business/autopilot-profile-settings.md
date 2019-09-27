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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają domyślne i opcjonalne ustawienia, takie jak Pomiń instalację Cortany.
ms.openlocfilehash: cd66627943301f4a4f2410bafeff6074919ec29d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287480"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="63618-104">Ustawienia profilu rozwiązania AutoPilot  informacje</span><span class="sxs-lookup"><span data-stu-id="63618-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="63618-105">Ustawienia profilu AutoPilot</span><span class="sxs-lookup"><span data-stu-id="63618-105">AutoPilot profile settings</span></span>

<span data-ttu-id="63618-106">Za pomocą profilów AutoPilot można kontrolować sposób instalowania systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="63618-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="63618-107">Profile zawierają następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="63618-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="63618-108">**Domyślne funkcje autopilota (wymagane), które są ustawiane automatycznie:**</span><span class="sxs-lookup"><span data-stu-id="63618-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="63618-109">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="63618-109">**Setting**</span></span>|<span data-ttu-id="63618-110">**Opis**</span><span class="sxs-lookup"><span data-stu-id="63618-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63618-111">Pomiń rejestrację Cortany, OneDrive i OEM</span><span class="sxs-lookup"><span data-stu-id="63618-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="63618-112">Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobisty OneDrive.</span><span class="sxs-lookup"><span data-stu-id="63618-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="63618-113">Użytkownik urządzenia można zainstalować te później tak długo, jak on lub ona jest administratorem lokalnym na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="63618-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="63618-114">Oryginalna Rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="63618-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="63618-115">Zaloguj się w swojej firmie</span><span class="sxs-lookup"><span data-stu-id="63618-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="63618-116">Jeśli Twoja firma ma [dodać marki firmy do pakietu Office 365 Zaloguj się na stronie](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), użytkownik urządzenia będzie uzyskać to doświadczenie podczas logowania.</span><span class="sxs-lookup"><span data-stu-id="63618-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="63618-117">Automatyczna rejestracja MDM z skonfigurowanymi kontami usługi AAD.</span><span class="sxs-lookup"><span data-stu-id="63618-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="63618-118">Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemu Windows i pakietu Office 365 za pomocą poświadczeń firmy Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="63618-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="63618-119">**Ustawienia opcjonalne:**</span><span class="sxs-lookup"><span data-stu-id="63618-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="63618-120">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="63618-120">**Setting**</span></span>|<span data-ttu-id="63618-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="63618-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63618-122">Pomiń ustawienia prywatności (domyślnie wyłączone)</span><span class="sxs-lookup"><span data-stu-id="63618-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="63618-123">Jeśli ta opcja jest **włączona**, użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy on lub ona po raz pierwszy loguje się.</span><span class="sxs-lookup"><span data-stu-id="63618-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="63618-124">Nie Zezwalaj, aby użytkownik stał się administratorem lokalnym</span><span class="sxs-lookup"><span data-stu-id="63618-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="63618-125">Jeśli ta opcja jest **włączona**, użytkownik urządzenia nie będzie mógł instalować żadnych osobistych aplikacji, takich jak Cortana.</span><span class="sxs-lookup"><span data-stu-id="63618-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
