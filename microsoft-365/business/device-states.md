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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Informacje o różnych stanach urządzeń na liście Akcje urządzenia w domu administratora w usłudze Microsoft 365 Business.
ms.openlocfilehash: 878050fbe11acca1d5d434a5d2ab0b5b48510e45
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415670"
---
# <a name="device-states"></a><span data-ttu-id="358c8-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="358c8-103">Device states</span></span>

<span data-ttu-id="358c8-104">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="358c8-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="358c8-106">**Stan**</span><span class="sxs-lookup"><span data-stu-id="358c8-106">**Status**</span></span>|<span data-ttu-id="358c8-107">**Opis**</span><span class="sxs-lookup"><span data-stu-id="358c8-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="358c8-108">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="358c8-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="358c8-109">Zarządzane przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="358c8-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="358c8-110">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="358c8-110">Retire pending</span></span>  <br/> |<span data-ttu-id="358c8-111">Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="358c8-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="358c8-112">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="358c8-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="358c8-113">Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="358c8-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="358c8-114">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="358c8-114">Retire failed</span></span>  <br/> | <span data-ttu-id="358c8-115">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="358c8-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="358c8-116">Wycofana anulowana</span><span class="sxs-lookup"><span data-stu-id="358c8-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="358c8-117">Wycofaj akcję została anulowana.</span><span class="sxs-lookup"><span data-stu-id="358c8-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="358c8-118">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="358c8-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="358c8-119">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="358c8-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="358c8-120">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="358c8-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="358c8-121">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="358c8-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="358c8-122">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="358c8-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="358c8-123">Nie można zrobić reset fabryczny.</span><span class="sxs-lookup"><span data-stu-id="358c8-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="358c8-124">Wytrzeć anulowane</span><span class="sxs-lookup"><span data-stu-id="358c8-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="358c8-125">Fabryczna chusteczka została anulowana.</span><span class="sxs-lookup"><span data-stu-id="358c8-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="358c8-126">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="358c8-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="358c8-127">Akcja jest w toku (lub w toku), ale urządzenie nie zaewidencjonowało się przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="358c8-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="358c8-128">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="358c8-128">Delete pending</span></span>  <br/> |<span data-ttu-id="358c8-129">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="358c8-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="358c8-130">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="358c8-130">Discovered</span></span>  <br/> |<span data-ttu-id="358c8-131">Usługa Microsoft 365 Business wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="358c8-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
