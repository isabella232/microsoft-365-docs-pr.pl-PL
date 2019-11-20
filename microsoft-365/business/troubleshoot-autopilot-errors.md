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
description: Dowiedz się, jak rozwiązywać problemy z błędami plików urządzenia AutoPilot.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718704"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="5ab50-103">Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5ab50-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="5ab50-104">Komunikaty o błędach pliku urządzenia</span><span class="sxs-lookup"><span data-stu-id="5ab50-104">Device file error messages</span></span>

<span data-ttu-id="5ab50-105">Oto informacje na temat niektórych błędów, które mogą być widoczne podczas pracy z plikami urządzeń AutoPilot w Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="5ab50-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="5ab50-106">**Kod błędu**</span><span class="sxs-lookup"><span data-stu-id="5ab50-106">**Error code**</span></span>|<span data-ttu-id="5ab50-107">**Napraw, aby spróbować**</span><span class="sxs-lookup"><span data-stu-id="5ab50-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5ab50-108">Nieprawidłowa treść żądania</span><span class="sxs-lookup"><span data-stu-id="5ab50-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="5ab50-109">Ten błąd powinien się zdarzyć rzadko, jeśli widzisz ten błąd, spróbuj ponownie wykonać operację.</span><span class="sxs-lookup"><span data-stu-id="5ab50-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="5ab50-110">Wartość skrótu sprzętowego urządzenia nie jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="5ab50-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="5ab50-111">Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla skrótu sprzętowego jednego urządzenia nie jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="5ab50-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="5ab50-112">Najpierw sprawdź, czy wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="5ab50-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="5ab50-113">Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal się dzieje, Poproś dostawcę sprzętu o pomoc.</span><span class="sxs-lookup"><span data-stu-id="5ab50-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="5ab50-114">Urządzenie przypisane do innego dzierżawcy</span><span class="sxs-lookup"><span data-stu-id="5ab50-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="5ab50-115">Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub większej liczby urządzeń nie jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="5ab50-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="5ab50-116">Najpierw sprawdź, czy wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="5ab50-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="5ab50-117">Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal się dzieje, Poproś dostawcę sprzętu o pomoc.</span><span class="sxs-lookup"><span data-stu-id="5ab50-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="5ab50-118">Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu</span><span class="sxs-lookup"><span data-stu-id="5ab50-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="5ab50-119">Jeśli widzisz ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację.</span><span class="sxs-lookup"><span data-stu-id="5ab50-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="5ab50-120">Aby naprawić ten błąd, Poproś dostawcę sprzętu o pomoc.</span><span class="sxs-lookup"><span data-stu-id="5ab50-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="5ab50-121">To urządzenie nie jest obsługiwane w przypadku instalacji przy użyciu funkcji AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5ab50-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="5ab50-122">Ten błąd oznacza, że urządzenie nie spełnia wymagań dotyczących wdrażania AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ab50-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="5ab50-123">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="5ab50-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="5ab50-124">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="5ab50-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="5ab50-125">Nowe urządzenia, które nie zostały przez Windows out-of-Box doświadczenia.</span><span class="sxs-lookup"><span data-stu-id="5ab50-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="5ab50-126">Nie znaleziono urządzenia</span><span class="sxs-lookup"><span data-stu-id="5ab50-126">Device not found</span></span>  <br/> |<span data-ttu-id="5ab50-127">Ten błąd oznacza, że jeden lub więcej urządzeń w pliku CSV nie jest zarejestrowany w organizacji.</span><span class="sxs-lookup"><span data-stu-id="5ab50-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="5ab50-128">Aby rozwiązać ten problem, Poproś dostawcę sprzętu o pomoc.</span><span class="sxs-lookup"><span data-stu-id="5ab50-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
