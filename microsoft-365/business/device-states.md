---
title: Stany urządzeń
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Dowiedz się więcej o różnych stanach urządzeń na liście Akcje urządzenia w domu administratora w usłudze Microsoft 365 dla firm.
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400959"
---
# <a name="device-states"></a><span data-ttu-id="1612e-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="1612e-103">Device states</span></span>

<span data-ttu-id="1612e-104">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="1612e-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="1612e-106">**Stan**</span><span class="sxs-lookup"><span data-stu-id="1612e-106">**Status**</span></span>|<span data-ttu-id="1612e-107">**Opis**</span><span class="sxs-lookup"><span data-stu-id="1612e-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1612e-108">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="1612e-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="1612e-109">Zarządzane przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="1612e-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="1612e-110">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="1612e-110">Retire pending</span></span>  <br/> |<span data-ttu-id="1612e-111">Usługa Microsoft 365 Business Premium przygotowuje się do usunięcia danych firmowych z urządzenia.</span><span class="sxs-lookup"><span data-stu-id="1612e-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="1612e-112">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="1612e-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="1612e-113">Usługa Microsoft 365 Business Premium obecnie usuwa dane firmowe z urządzenia.</span><span class="sxs-lookup"><span data-stu-id="1612e-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="1612e-114">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="1612e-114">Retire failed</span></span>  <br/> | <span data-ttu-id="1612e-115">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="1612e-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="1612e-116">Wycofaj anulowano</span><span class="sxs-lookup"><span data-stu-id="1612e-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="1612e-117">Działanie na emeryturę zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="1612e-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="1612e-118">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="1612e-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="1612e-119">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="1612e-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="1612e-120">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="1612e-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="1612e-121">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="1612e-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="1612e-122">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="1612e-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="1612e-123">Nie można przywrócić ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="1612e-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="1612e-124">Wyczyść anulowane</span><span class="sxs-lookup"><span data-stu-id="1612e-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="1612e-125">Czyszczenie fabryczne zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="1612e-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="1612e-126">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="1612e-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="1612e-127">Akcja jest w toku (lub w toku), ale urządzenie nie zostało zaewidencjonowane przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="1612e-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="1612e-128">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="1612e-128">Delete pending</span></span>  <br/> |<span data-ttu-id="1612e-129">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="1612e-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="1612e-130">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="1612e-130">Discovered</span></span>  <br/> |<span data-ttu-id="1612e-131">Usługa Microsoft 365 Business Premium wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="1612e-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
