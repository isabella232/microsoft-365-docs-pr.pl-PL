---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
f1.keywords:
- NOCSH
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązywać problemy, które mogą pojawić się podczas pracy z plikami urządzeń AutoPilot w usłudze Microsoft 365 Business.
ms.openlocfilehash: dc1abd508156c8525859f6ca7e291ab38fc8859c
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560705"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="4f804-103">Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="4f804-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="4f804-104">Komunikaty o błędach pliku urządzenia</span><span class="sxs-lookup"><span data-stu-id="4f804-104">Device file error messages</span></span>

<span data-ttu-id="4f804-105">Oto informacje o niektórych błędach, które mogą pojawić się podczas pracy z plikami urządzeń AutoPilot w usłudze Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4f804-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="4f804-106">**Kod błędu**</span><span class="sxs-lookup"><span data-stu-id="4f804-106">**Error code**</span></span>|<span data-ttu-id="4f804-107">**Poprawka, aby spróbować**</span><span class="sxs-lookup"><span data-stu-id="4f804-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f804-108">Nieprawidłowy organ żądania</span><span class="sxs-lookup"><span data-stu-id="4f804-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="4f804-109">Ten błąd powinien się zdarzyć rzadko, jeśli widzisz ten błąd, spróbuj ponownie wykonać operację.</span><span class="sxs-lookup"><span data-stu-id="4f804-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="4f804-110">Wartość skrótu sprzętowego dla urządzenia jest nieprawidłowa.</span><span class="sxs-lookup"><span data-stu-id="4f804-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="4f804-111">Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla skrótu sprzętowego jednego urządzenia jest niepoprawna.</span><span class="sxs-lookup"><span data-stu-id="4f804-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="4f804-112">Najpierw sprawdź, czy wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="4f804-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="4f804-113">Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="4f804-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="4f804-114">Urządzenie przypisane do innej dzierżawy</span><span class="sxs-lookup"><span data-stu-id="4f804-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="4f804-115">Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub większej liczby urządzeń jest niepoprawna.</span><span class="sxs-lookup"><span data-stu-id="4f804-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="4f804-116">Najpierw sprawdź, czy wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="4f804-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="4f804-117">Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="4f804-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="4f804-118">Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu</span><span class="sxs-lookup"><span data-stu-id="4f804-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="4f804-119">Jeśli widzisz ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację.</span><span class="sxs-lookup"><span data-stu-id="4f804-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="4f804-120">Aby naprawić ten błąd, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="4f804-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="4f804-121">To urządzenie nie jest obsługiwane do konfiguracji przy użyciu programu AutoPilot</span><span class="sxs-lookup"><span data-stu-id="4f804-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="4f804-122">Ten błąd oznacza, że urządzenie nie spełnia wymagań dotyczących wdrażania programu AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="4f804-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="4f804-123">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="4f804-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="4f804-124">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="4f804-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="4f804-125">Nowe urządzenia, które nie zostały za pośrednictwem systemu Windows out-of-box środowiska.</span><span class="sxs-lookup"><span data-stu-id="4f804-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="4f804-126">Nie znaleziono urządzenia</span><span class="sxs-lookup"><span data-stu-id="4f804-126">Device not found</span></span>  <br/> |<span data-ttu-id="4f804-127">Ten błąd oznacza, że co najmniej jedno urządzenie w pliku CSV nie jest zarejestrowane w organizacji.</span><span class="sxs-lookup"><span data-stu-id="4f804-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="4f804-128">Aby rozwiązać ten problem, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="4f804-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
