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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Informacje o różnych stanach urządzeń można dowiedzieć się na liście Akcje urządzenia w witrynie Admin home w usłudze Microsoft 365 Business.
ms.openlocfilehash: bed1610814ca0d60adb4b4b3d0018e3e7e6d763f
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560825"
---
# <a name="device-states"></a><span data-ttu-id="d45a1-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="d45a1-103">Device states</span></span>

<span data-ttu-id="d45a1-104">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="d45a1-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="d45a1-106">**Stan**</span><span class="sxs-lookup"><span data-stu-id="d45a1-106">**Status**</span></span>|<span data-ttu-id="d45a1-107">**Opis**</span><span class="sxs-lookup"><span data-stu-id="d45a1-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d45a1-108">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="d45a1-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="d45a1-109">Zarządzane przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d45a1-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="d45a1-110">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="d45a1-110">Retire pending</span></span>  <br/> |<span data-ttu-id="d45a1-111">Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d45a1-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="d45a1-112">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="d45a1-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="d45a1-113">Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d45a1-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="d45a1-114">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="d45a1-114">Retire failed</span></span>  <br/> | <span data-ttu-id="d45a1-115">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="d45a1-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="d45a1-116">Wycofaj anulowane</span><span class="sxs-lookup"><span data-stu-id="d45a1-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="d45a1-117">Akcja wycofania została anulowana.</span><span class="sxs-lookup"><span data-stu-id="d45a1-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="d45a1-118">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="d45a1-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="d45a1-119">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="d45a1-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="d45a1-120">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="d45a1-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="d45a1-121">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="d45a1-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="d45a1-122">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="d45a1-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="d45a1-123">Nie można zrobić reset uprzywracania fabrycznego.</span><span class="sxs-lookup"><span data-stu-id="d45a1-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="d45a1-124">Wyczyść anulowane</span><span class="sxs-lookup"><span data-stu-id="d45a1-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="d45a1-125">Wycieranie fabryczne zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="d45a1-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="d45a1-126">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="d45a1-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="d45a1-127">Akcja jest w toku (lub w toku), ale urządzenie nie zaewidencjonowało się przez 30+ dni.</span><span class="sxs-lookup"><span data-stu-id="d45a1-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="d45a1-128">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="d45a1-128">Delete pending</span></span>  <br/> |<span data-ttu-id="d45a1-129">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="d45a1-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="d45a1-130">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="d45a1-130">Discovered</span></span>  <br/> |<span data-ttu-id="d45a1-131">Usługa Microsoft 365 Business wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="d45a1-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
