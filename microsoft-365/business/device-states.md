---
title: Stany urządzeń
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Dowiedz się więcej o Stany urządzeń w Microsoft 365 Business.
ms.openlocfilehash: 06e5c800e6a104785c1fd0724223e05d7729722e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072725"
---
# <a name="device-states"></a><span data-ttu-id="70491-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="70491-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="70491-104">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="70491-104">Device states</span></span>

<span data-ttu-id="70491-105">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="70491-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="70491-107">**Stan**</span><span class="sxs-lookup"><span data-stu-id="70491-107">**Status**</span></span>|<span data-ttu-id="70491-108">**Opis**</span><span class="sxs-lookup"><span data-stu-id="70491-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70491-109">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="70491-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="70491-110">Zarządzane przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="70491-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="70491-111">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="70491-111">Retire pending</span></span>  <br/> |<span data-ttu-id="70491-112">Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="70491-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="70491-113">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="70491-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="70491-114">Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="70491-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="70491-115">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="70491-115">Retire failed</span></span>  <br/> | <span data-ttu-id="70491-116">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="70491-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="70491-117">Anulowano wycofywanie</span><span class="sxs-lookup"><span data-stu-id="70491-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="70491-118">Akcja wycofywania została anulowana.</span><span class="sxs-lookup"><span data-stu-id="70491-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="70491-119">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="70491-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="70491-120">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="70491-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="70491-121">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="70491-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="70491-122">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="70491-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="70491-123">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="70491-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="70491-124">Nie można przywrócić ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="70491-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="70491-125">Anulowano czyszczenie</span><span class="sxs-lookup"><span data-stu-id="70491-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="70491-126">Przywracanie ustawień fabrycznych zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="70491-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="70491-127">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="70491-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="70491-128">Trwa oczekiwanie na rozpoczęcie akcji (lub jest ona w toku), ale urządzenie nie zostało zaewidencjonowane przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="70491-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="70491-129">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="70491-129">Delete pending</span></span>  <br/> |<span data-ttu-id="70491-130">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="70491-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="70491-131">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="70491-131">Discovered</span></span>  <br/> |<span data-ttu-id="70491-132">Usługa Microsoft 365 Business wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="70491-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
