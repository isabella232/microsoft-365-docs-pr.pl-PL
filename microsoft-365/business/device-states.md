---
title: Stany urządzeń
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Poznaj różne stany urządzeń na liście Akcje urządzenia w witrynie głównej Administrator na platformie Microsoft 365 dla firm.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578472"
---
# <a name="device-states"></a><span data-ttu-id="a6b79-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="a6b79-103">Device states</span></span>

<span data-ttu-id="a6b79-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a6b79-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a6b79-105">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="a6b79-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="a6b79-107">**Stan**</span><span class="sxs-lookup"><span data-stu-id="a6b79-107">**Status**</span></span>|<span data-ttu-id="a6b79-108">**Opis**</span><span class="sxs-lookup"><span data-stu-id="a6b79-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6b79-109">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="a6b79-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="a6b79-110">Zarządzane przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a6b79-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="a6b79-111">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="a6b79-111">Retire pending</span></span>  <br/> |<span data-ttu-id="a6b79-112">Usługa Microsoft 365 Business Premium przygotowuje się do usunięcia danych firmowych z urządzenia.</span><span class="sxs-lookup"><span data-stu-id="a6b79-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="a6b79-113">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="a6b79-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="a6b79-114">Usługa Microsoft 365 Business Premium obecnie usuwa dane firmowe z urządzenia.</span><span class="sxs-lookup"><span data-stu-id="a6b79-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="a6b79-115">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="a6b79-115">Retire failed</span></span>  <br/> | <span data-ttu-id="a6b79-116">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="a6b79-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="a6b79-117">Anulowano wycofywanie</span><span class="sxs-lookup"><span data-stu-id="a6b79-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="a6b79-118">Akcja wycofywania została anulowana.</span><span class="sxs-lookup"><span data-stu-id="a6b79-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="a6b79-119">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="a6b79-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="a6b79-120">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="a6b79-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="a6b79-121">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="a6b79-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="a6b79-122">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="a6b79-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="a6b79-123">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="a6b79-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="a6b79-124">Nie można przywrócić ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="a6b79-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="a6b79-125">Czyszczenie anulowane</span><span class="sxs-lookup"><span data-stu-id="a6b79-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="a6b79-126">Czyszczenie fabryczne zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="a6b79-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="a6b79-127">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="a6b79-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="a6b79-128">Akcja jest oczekująca (lub jest w toku), ale urządzenie nie zostało zaewidencjonowane przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="a6b79-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="a6b79-129">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="a6b79-129">Delete pending</span></span>  <br/> |<span data-ttu-id="a6b79-130">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="a6b79-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="a6b79-131">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="a6b79-131">Discovered</span></span>  <br/> |<span data-ttu-id="a6b79-132">Urządzenie zostało wykryte przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a6b79-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
