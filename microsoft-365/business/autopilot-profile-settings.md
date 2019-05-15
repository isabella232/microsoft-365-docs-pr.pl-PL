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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile autopilota można kontrolować, jak system Windows zostanie zainstalowany na urządzeniach użytkowników. Profile zawierają domyślne i ustawienia opcjonalne, takie jak pominąć instalację Cortana.
ms.openlocfilehash: adc8112861b67fd96a91ff24dc155aeb0c394532
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071865"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="7787e-104">Ustawienia profilu rozwiązania AutoPilot  informacje</span><span class="sxs-lookup"><span data-stu-id="7787e-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="7787e-105">Ustawienia profilu autopilota</span><span class="sxs-lookup"><span data-stu-id="7787e-105">AutoPilot profile settings</span></span>

<span data-ttu-id="7787e-106">Można kontrolować, jak system Windows zostanie zainstalowany na urządzenia użytkownika przy użyciu profilów autopilota.</span><span class="sxs-lookup"><span data-stu-id="7787e-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="7787e-107">Profile zawierają następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="7787e-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="7787e-108">**Autopilota domyślne funkcje (pole wymagane), które są ustawiane automatycznie:**</span><span class="sxs-lookup"><span data-stu-id="7787e-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="7787e-109">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="7787e-109">**Setting**</span></span>|<span data-ttu-id="7787e-110">**Opis**</span><span class="sxs-lookup"><span data-stu-id="7787e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7787e-111">Pomijanie rejestracji Cortana, OneDrive i OEM</span><span class="sxs-lookup"><span data-stu-id="7787e-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="7787e-112">Pomija instalacji aplikacji konsumenta, takich jak Cortana i OneDrive osobistych.</span><span class="sxs-lookup"><span data-stu-id="7787e-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="7787e-113">Urządzenie użytkownika można zainstalować później, tak długo, jak długo dany użytkownik jest administratorem lokalnym na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="7787e-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="7787e-114">Pierwotnej rejestracji producenta jest pomijane, ponieważ urządzenie będzie zarządzany przez Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="7787e-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="7787e-115">Zaloguj się doświadczenie do marki firmy</span><span class="sxs-lookup"><span data-stu-id="7787e-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="7787e-116">Jeśli Twoja firma ma, [Dodaj firmę znakowania do Office 365 stronę logowania](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), użytkownik urządzenia otrzyma tego doświadczenia podczas logowania się.</span><span class="sxs-lookup"><span data-stu-id="7787e-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="7787e-117">MDM autorejestrowania z skonfigurowanych kont AAD.</span><span class="sxs-lookup"><span data-stu-id="7787e-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="7787e-118">Tożsamość użytkownika będą zarządzane przez usługę Azure Active directory, a użytkownicy będą logują się do systemu Windows i Office 365 przy użyciu poświadczeń Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="7787e-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="7787e-119">**Ustawienia opcjonalne:**</span><span class="sxs-lookup"><span data-stu-id="7787e-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="7787e-120">**Ustawienie**</span><span class="sxs-lookup"><span data-stu-id="7787e-120">**Setting**</span></span>|<span data-ttu-id="7787e-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="7787e-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7787e-122">Pomiń ustawienia prywatności (domyślnie wyłączone)</span><span class="sxs-lookup"><span data-stu-id="7787e-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="7787e-123">Jeśli ta opcja jest ustawiona na **On**, urządzenie użytkownika nie zobaczą umowy licencyjnej dla urządzenia i Windows podczas po raz pierwszy zaloguje się.</span><span class="sxs-lookup"><span data-stu-id="7787e-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="7787e-124">Niezezwalanie użytkownikowi stać się administratorem lokalnym</span><span class="sxs-lookup"><span data-stu-id="7787e-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="7787e-125">Jeśli ta opcja jest ustawiona na **On**, użytkownik urządzenia nie będzie mógł zainstalować wszystkie aplikacje osobistych, takich jak Cortana.</span><span class="sxs-lookup"><span data-stu-id="7787e-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
