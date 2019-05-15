---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązać problemy z błędami pliku urządzenia autopilota.
ms.openlocfilehash: 88b59ec20ddda401c1dac45ff729ac38497a767e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074365"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="45c6b-103">Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="45c6b-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="45c6b-104">Komunikaty o błędach pliku urządzenia</span><span class="sxs-lookup"><span data-stu-id="45c6b-104">Device file error messages</span></span>

<span data-ttu-id="45c6b-105">Oto informacje na niektóre błędy mogą pojawić się podczas pracy z plikami urządzenia autopilota w Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="45c6b-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="45c6b-106">**Kod błędu**</span><span class="sxs-lookup"><span data-stu-id="45c6b-106">**Error code**</span></span>|<span data-ttu-id="45c6b-107">**Aby spróbować naprawić**</span><span class="sxs-lookup"><span data-stu-id="45c6b-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45c6b-108">Nieprawidłowe żądanie ciała</span><span class="sxs-lookup"><span data-stu-id="45c6b-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="45c6b-109">Ten błąd powinno mieć miejsce rzadko, jeśli widzisz ten błąd, spróbuj ponowić operację.</span><span class="sxs-lookup"><span data-stu-id="45c6b-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="45c6b-110">Wartość mieszania sprzętu dla urządzenia nie są poprawne.</span><span class="sxs-lookup"><span data-stu-id="45c6b-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="45c6b-111">Wystąpienie tego błędu oznacza, że wartości podane w pliku CSV dla hash hardwaru jednym z urządzeń nie jest prawidłowe.</span><span class="sxs-lookup"><span data-stu-id="45c6b-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="45c6b-112">Najpierw upewnij się, że wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="45c6b-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="45c6b-113">Jeśli uważasz, że wartość jest poprawna, ale nadal dzieje się ten błąd, należy poprosić o pomoc z dostawcą sprzętu.</span><span class="sxs-lookup"><span data-stu-id="45c6b-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="45c6b-114">Urządzenia przypisane do innego lokatora</span><span class="sxs-lookup"><span data-stu-id="45c6b-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="45c6b-115">Wystąpienie tego błędu oznacza, że wartości podane w pliku CSV dla numeru seryjnego lub klucz produktu dla jednego lub więcej urządzeń nie jest prawidłowe.</span><span class="sxs-lookup"><span data-stu-id="45c6b-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="45c6b-116">Najpierw upewnij się, że wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="45c6b-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="45c6b-117">Jeśli uważasz, że wartość jest poprawna, ale nadal dzieje się ten błąd, należy poprosić o pomoc z dostawcą sprzętu.</span><span class="sxs-lookup"><span data-stu-id="45c6b-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="45c6b-118">Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu</span><span class="sxs-lookup"><span data-stu-id="45c6b-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="45c6b-119">Wystąpienie tego błędu oznacza, że urządzenie, które są podczas rejestracji jest już zarejestrowana przez innych organizacji.</span><span class="sxs-lookup"><span data-stu-id="45c6b-119">If you see this error it means that the device you are tyring to register is already registered by an other organization.</span></span> <span data-ttu-id="45c6b-120">Aby rozwiązać ten problem, poproś o pomoc z dostawcą sprzętu.</span><span class="sxs-lookup"><span data-stu-id="45c6b-120">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="45c6b-121">To urządzenie nie jest obsługiwana dla instalacji za pomocą autopilota</span><span class="sxs-lookup"><span data-stu-id="45c6b-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="45c6b-122">Ten błąd oznacza, że urządzenie nie spełnia wymagania dotyczące wdrażania autopilota.</span><span class="sxs-lookup"><span data-stu-id="45c6b-122">This error means the device does not meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="45c6b-123">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="45c6b-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="45c6b-124">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="45c6b-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="45c6b-125">Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="45c6b-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="45c6b-126">Nie znaleziono urządzenia</span><span class="sxs-lookup"><span data-stu-id="45c6b-126">Device not found</span></span>  <br/> |<span data-ttu-id="45c6b-127">Ten błąd oznacza, że jedno lub więcej urządzeń w pliku CSV nie jest zarejestrowany dla danej organizacji.</span><span class="sxs-lookup"><span data-stu-id="45c6b-127">This error means that one or more devices in your CSV file is not registered to your organization.</span></span> <span data-ttu-id="45c6b-128">Aby rozwiązać ten problem, poproś o pomoc z dostawcą sprzętu.</span><span class="sxs-lookup"><span data-stu-id="45c6b-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
