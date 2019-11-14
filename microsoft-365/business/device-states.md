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
description: Dowiedz się więcej o Stanach urządzeń w Microsoft 365 Business.
ms.openlocfilehash: b55e6a5d538ec28d195225e93797cea27afd2e8b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320213"
---
# <a name="device-states"></a><span data-ttu-id="49c29-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="49c29-103">Device states</span></span>

<span data-ttu-id="49c29-104">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="49c29-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="49c29-106">**Stan**</span><span class="sxs-lookup"><span data-stu-id="49c29-106">**Status**</span></span>|<span data-ttu-id="49c29-107">**Opis**</span><span class="sxs-lookup"><span data-stu-id="49c29-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49c29-108">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="49c29-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="49c29-109">Zarządzane przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="49c29-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="49c29-110">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="49c29-110">Retire pending</span></span>  <br/> |<span data-ttu-id="49c29-111">Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="49c29-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="49c29-112">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="49c29-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="49c29-113">Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="49c29-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="49c29-114">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="49c29-114">Retire failed</span></span>  <br/> | <span data-ttu-id="49c29-115">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="49c29-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="49c29-116">Wycofanie anulowane</span><span class="sxs-lookup"><span data-stu-id="49c29-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="49c29-117">Wycofanie akcji zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="49c29-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="49c29-118">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="49c29-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="49c29-119">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="49c29-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="49c29-120">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="49c29-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="49c29-121">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="49c29-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="49c29-122">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="49c29-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="49c29-123">Nie można przywrócić ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="49c29-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="49c29-124">Przetrzeć anulowane</span><span class="sxs-lookup"><span data-stu-id="49c29-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="49c29-125">Czyszczenie fabryczne zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="49c29-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="49c29-126">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="49c29-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="49c29-127">Akcja jest oczekująca (lub w toku), ale urządzenie nie zostało zaewidencjonowane przez 30 + dni.</span><span class="sxs-lookup"><span data-stu-id="49c29-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="49c29-128">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="49c29-128">Delete pending</span></span>  <br/> |<span data-ttu-id="49c29-129">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="49c29-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="49c29-130">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="49c29-130">Discovered</span></span>  <br/> |<span data-ttu-id="49c29-131">Usługa Microsoft 365 Business wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="49c29-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
