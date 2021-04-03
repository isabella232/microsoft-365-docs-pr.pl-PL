---
title: "Ustawienia profilu rozwiązania AutoPilot \x97 informacje"
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile rozwiązania AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pominięcie instalacji Cortany.
ms.openlocfilehash: 86f8718131f0a0b93e18e65e39e02e7d65aded1a
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578512"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="c3c22-104">Ustawienia profilu rozwiązania AutoPilot  informacje</span><span class="sxs-lookup"><span data-stu-id="c3c22-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="c3c22-105">Ustawienia profilu rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c3c22-105">AutoPilot profile settings</span></span>

<span data-ttu-id="c3c22-106">Profile rozwiązania AutoPilot mogą pomóc w kontrolowaniu sposobu instalowania systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c3c22-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="c3c22-107">Profile zawierają następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="c3c22-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="c3c22-108">**Funkcje domyślne rozwiązania AutoPilot ustawiane automatycznie (wymagane):**</span><span class="sxs-lookup"><span data-stu-id="c3c22-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="c3c22-109">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="c3c22-109">**Setting**</span></span>|<span data-ttu-id="c3c22-110">**Opis**</span><span class="sxs-lookup"><span data-stu-id="c3c22-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c3c22-111">Pomiń rejestrację Cortany, usługi OneDrive i OEM</span><span class="sxs-lookup"><span data-stu-id="c3c22-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="c3c22-112">Pomija instalację aplikacji dla klientów konsumenckich, takich jak Cortana i osobista aplikacja OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c3c22-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="c3c22-113">Użytkownik urządzenia może je zainstalować później, o ile użytkownik jest administratorem lokalnym na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="c3c22-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="c3c22-114">Rejestracja oryginalnego producenta zostanie pominięta, ponieważ urządzeniem będzie zarządzana usługa Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c3c22-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="c3c22-115">Logowanie się za pomocą marki firmowej</span><span class="sxs-lookup"><span data-stu-id="c3c22-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="c3c22-116">Jeśli twoja firma ma znakowanie Dodaj markę twojej firmy do strony logowania na platformie [Microsoft 365,](../admin/setup/customize-sign-in-page.md)użytkownik urządzenia będzie miał to doświadczenie podczas logowania.</span><span class="sxs-lookup"><span data-stu-id="c3c22-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="c3c22-117">Automatyczne rejestrowanie w uścisku usługi MDM ze skonfigurowanymi kontami AAD.</span><span class="sxs-lookup"><span data-stu-id="c3c22-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="c3c22-118">Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy logują się do systemu Windows i platformy Microsoft 365 za pomocą poświadczeń platformy Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c3c22-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="c3c22-119">**Ustawienia opcjonalne:**</span><span class="sxs-lookup"><span data-stu-id="c3c22-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="c3c22-120">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="c3c22-120">**Setting**</span></span>|<span data-ttu-id="c3c22-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="c3c22-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c3c22-122">Pomiń ustawienia prywatności (domyślnie wyłączone)</span><span class="sxs-lookup"><span data-stu-id="c3c22-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="c3c22-123">Jeśli ta opcja jest ustawiona **na** Wł., użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy tylko się wcześniej pojawi.</span><span class="sxs-lookup"><span data-stu-id="c3c22-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="c3c22-124">Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym</span><span class="sxs-lookup"><span data-stu-id="c3c22-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="c3c22-125">Jeśli ta opcja jest ustawiona na Wł., użytkownik urządzenia nie będzie mógł zainstalować żadnych aplikacji osobistych, takich jak Cortana.</span><span class="sxs-lookup"><span data-stu-id="c3c22-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
