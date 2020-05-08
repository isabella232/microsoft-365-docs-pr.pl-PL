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
description: Profile autopilot ułatwią kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pomiń instalację Cortany.
ms.openlocfilehash: 0c706d12ba262856ff40ea3bee57c64234fd77f7
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165846"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="d5f64-104">Ustawienia profilu rozwiązania AutoPilot  informacje</span><span class="sxs-lookup"><span data-stu-id="d5f64-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="d5f64-105">Ustawienia profilu autopilot</span><span class="sxs-lookup"><span data-stu-id="d5f64-105">AutoPilot profile settings</span></span>

<span data-ttu-id="d5f64-106">Za pomocą profilów programu AutoPilot można kontrolować sposób instalowania systemu Windows na urządzeniach użytkownika.</span><span class="sxs-lookup"><span data-stu-id="d5f64-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="d5f64-107">Profile zawierają następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="d5f64-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="d5f64-108">**Domyślne funkcje autopilot (wymagane), które są ustawiane automatycznie:**</span><span class="sxs-lookup"><span data-stu-id="d5f64-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="d5f64-109">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="d5f64-109">**Setting**</span></span>|<span data-ttu-id="d5f64-110">**Opis**</span><span class="sxs-lookup"><span data-stu-id="d5f64-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5f64-111">Pomiń rejestrację Cortany, Usługi OneDrive i OEM</span><span class="sxs-lookup"><span data-stu-id="d5f64-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="d5f64-112">Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobista usługa OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d5f64-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="d5f64-113">Użytkownik urządzenia może zainstalować je później, o ile użytkownik jest administratorem lokalnym na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="d5f64-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="d5f64-114">Oryginalna rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="d5f64-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="d5f64-115">Zaloguj się za pomocą marki firmy</span><span class="sxs-lookup"><span data-stu-id="d5f64-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="d5f64-116">Jeśli twoja firma ma [pozycję Dodaj markę firmy do strony logowania do usługi Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page)użytkownik urządzenia otrzyma to doświadczenie podczas logowania.</span><span class="sxs-lookup"><span data-stu-id="d5f64-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="d5f64-117">Automatyczna rejestracja mdm ze skonfigurowanymi kontami AAD.</span><span class="sxs-lookup"><span data-stu-id="d5f64-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="d5f64-118">Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemu Windows i usługi Microsoft 365 przy użyciu poświadczeń usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="d5f64-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="d5f64-119">**Ustawienia opcjonalne:**</span><span class="sxs-lookup"><span data-stu-id="d5f64-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="d5f64-120">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="d5f64-120">**Setting**</span></span>|<span data-ttu-id="d5f64-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="d5f64-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5f64-122">Pomiń ustawienia prywatności (domyślnie wyłączone)</span><span class="sxs-lookup"><span data-stu-id="d5f64-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="d5f64-123">Jeśli ta opcja jest ustawiona **na Włączone,** użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy po raz pierwszy się zaloguje.</span><span class="sxs-lookup"><span data-stu-id="d5f64-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="d5f64-124">Nie zezwalaj użytkownikowi na stanie się administratorem lokalnym</span><span class="sxs-lookup"><span data-stu-id="d5f64-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="d5f64-125">Jeśli ta opcja jest **ustawiona na Włączone,** użytkownik urządzenia nie będzie mógł zainstalować żadnych aplikacji osobistych, takich jak Cortana.</span><span class="sxs-lookup"><span data-stu-id="d5f64-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
