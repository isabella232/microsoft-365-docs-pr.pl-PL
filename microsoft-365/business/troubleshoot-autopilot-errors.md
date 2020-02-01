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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązywać problemy z błędami plików urządzenia AutoPilot.
ms.openlocfilehash: 8390f695a3e11386ae2617da4061bed1d8214375
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594213"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="88e1a-103">Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="88e1a-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="88e1a-104">Komunikaty o błędach plików urządzenia</span><span class="sxs-lookup"><span data-stu-id="88e1a-104">Device file error messages</span></span>

<span data-ttu-id="88e1a-105">Oto informacje na temat niektórych błędów, które mogą pojawić się podczas pracy z plikami urządzeń AutoPilot w usłudze Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="88e1a-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="88e1a-106">**Kod błędu**</span><span class="sxs-lookup"><span data-stu-id="88e1a-106">**Error code**</span></span>|<span data-ttu-id="88e1a-107">**Napraw, aby spróbować**</span><span class="sxs-lookup"><span data-stu-id="88e1a-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88e1a-108">Nieprawidłowy organ żądania</span><span class="sxs-lookup"><span data-stu-id="88e1a-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="88e1a-109">Ten błąd powinien wystąpić rzadko, jeśli widzisz ten błąd, spróbuj ponownie wykonać operację.</span><span class="sxs-lookup"><span data-stu-id="88e1a-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="88e1a-110">Wartość skrótu sprzętowego dla urządzenia jest niepoprawna.</span><span class="sxs-lookup"><span data-stu-id="88e1a-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="88e1a-111">Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla skrótu sprzętowego jednego urządzenia jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="88e1a-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="88e1a-112">Najpierw sprawdź, czy wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="88e1a-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="88e1a-113">Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="88e1a-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="88e1a-114">Urządzenie przypisane do innej dzierżawy</span><span class="sxs-lookup"><span data-stu-id="88e1a-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="88e1a-115">Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub więcej urządzeń jest niepoprawna.</span><span class="sxs-lookup"><span data-stu-id="88e1a-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="88e1a-116">Najpierw sprawdź, czy wartość została wpisana poprawnie.</span><span class="sxs-lookup"><span data-stu-id="88e1a-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="88e1a-117">Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="88e1a-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="88e1a-118">Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu</span><span class="sxs-lookup"><span data-stu-id="88e1a-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="88e1a-119">Jeśli widzisz ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację.</span><span class="sxs-lookup"><span data-stu-id="88e1a-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="88e1a-120">Aby naprawić ten błąd, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="88e1a-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="88e1a-121">To urządzenie nie jest obsługiwane do konfiguracji przy użyciu programu AutoPilot</span><span class="sxs-lookup"><span data-stu-id="88e1a-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="88e1a-122">Ten błąd oznacza, że urządzenie nie spełnia wymagań wdrażania programu AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="88e1a-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="88e1a-123">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="88e1a-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="88e1a-124">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="88e1a-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="88e1a-125">Nowe urządzenia, które nie przeszły przez system Windows out-of-box środowiska.</span><span class="sxs-lookup"><span data-stu-id="88e1a-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="88e1a-126">Nie znaleziono urządzenia</span><span class="sxs-lookup"><span data-stu-id="88e1a-126">Device not found</span></span>  <br/> |<span data-ttu-id="88e1a-127">Ten błąd oznacza, że co najmniej jedno urządzenie w pliku CSV nie jest zarejestrowane w organizacji.</span><span class="sxs-lookup"><span data-stu-id="88e1a-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="88e1a-128">Aby rozwiązać ten problem, poproś o pomoc dostawcę sprzętu.</span><span class="sxs-lookup"><span data-stu-id="88e1a-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
