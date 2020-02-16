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
description: Informacje o stanach urządzeń w usłudze Microsoft 365 Business.
ms.openlocfilehash: 26b218cb7b6a14f17e33d34a2e712b06ac814c0c
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065776"
---
# <a name="device-states"></a><span data-ttu-id="ce3b0-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="ce3b0-103">Device states</span></span>

<span data-ttu-id="ce3b0-104">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="ce3b0-106">**Stan**</span><span class="sxs-lookup"><span data-stu-id="ce3b0-106">**Status**</span></span>|<span data-ttu-id="ce3b0-107">**Opis**</span><span class="sxs-lookup"><span data-stu-id="ce3b0-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce3b0-108">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="ce3b0-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="ce3b0-109">Zarządzane przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-110">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="ce3b0-110">Retire pending</span></span>  <br/> |<span data-ttu-id="ce3b0-111">Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-112">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="ce3b0-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="ce3b0-113">Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-114">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="ce3b0-114">Retire failed</span></span>  <br/> | <span data-ttu-id="ce3b0-115">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-116">Wycofana anulowana</span><span class="sxs-lookup"><span data-stu-id="ce3b0-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="ce3b0-117">Wycofaj akcję została anulowana.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-118">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="ce3b0-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="ce3b0-119">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-120">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="ce3b0-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="ce3b0-121">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-122">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="ce3b0-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="ce3b0-123">Nie można zrobić reset fabryczny.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-124">Wytrzeć anulowane</span><span class="sxs-lookup"><span data-stu-id="ce3b0-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="ce3b0-125">Fabryczna chusteczka została anulowana.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-126">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="ce3b0-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="ce3b0-127">Akcja jest w toku (lub w toku), ale urządzenie nie zaewidencjonowało się przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-128">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="ce3b0-128">Delete pending</span></span>  <br/> |<span data-ttu-id="ce3b0-129">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="ce3b0-130">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="ce3b0-130">Discovered</span></span>  <br/> |<span data-ttu-id="ce3b0-131">Usługa Microsoft 365 Business wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="ce3b0-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
