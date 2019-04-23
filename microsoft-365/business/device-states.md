---
title: Stany urządzeń
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Dowiedz się więcej o Stany urządzeń w Microsoft 365 Business.
ms.openlocfilehash: 15114835a5014f5bfac600eac79bcdffdaec481a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276991"
---
# <a name="device-states"></a><span data-ttu-id="c3557-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="c3557-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="c3557-104">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="c3557-104">Device states</span></span>

<span data-ttu-id="c3557-105">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="c3557-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="c3557-107">**Stan**</span><span class="sxs-lookup"><span data-stu-id="c3557-107">**Status**</span></span>|<span data-ttu-id="c3557-108">**Opis**</span><span class="sxs-lookup"><span data-stu-id="c3557-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c3557-109">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="c3557-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="c3557-110">Zarządzane przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c3557-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="c3557-111">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="c3557-111">Retire pending</span></span>  <br/> |<span data-ttu-id="c3557-112">Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c3557-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="c3557-113">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="c3557-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="c3557-114">Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c3557-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="c3557-115">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="c3557-115">Retire failed</span></span>  <br/> | <span data-ttu-id="c3557-116">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="c3557-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="c3557-117">Anulowano wycofywanie</span><span class="sxs-lookup"><span data-stu-id="c3557-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="c3557-118">Akcja wycofywania została anulowana.</span><span class="sxs-lookup"><span data-stu-id="c3557-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="c3557-119">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="c3557-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="c3557-120">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="c3557-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="c3557-121">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="c3557-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="c3557-122">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="c3557-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="c3557-123">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="c3557-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="c3557-124">Nie można przywrócić ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="c3557-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="c3557-125">Anulowano czyszczenie</span><span class="sxs-lookup"><span data-stu-id="c3557-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="c3557-126">Przywracanie ustawień fabrycznych zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="c3557-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="c3557-127">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="c3557-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="c3557-128">Trwa oczekiwanie na rozpoczęcie akcji (lub jest ona w toku), ale urządzenie nie zostało zaewidencjonowane przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="c3557-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="c3557-129">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="c3557-129">Delete pending</span></span>  <br/> |<span data-ttu-id="c3557-130">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="c3557-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="c3557-131">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="c3557-131">Discovered</span></span>  <br/> |<span data-ttu-id="c3557-132">Usługa Microsoft 365 Business wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="c3557-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
