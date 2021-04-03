---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przekazywać urządzenia za pomocą rozwiązania AutoPilot w uwitrynie Microsoft 365 Business Premium. Profil możesz przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 506ff44e3cb6656b19174e82688b5af141ea2b79
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578492"
---
# <a name="create-and-edit-autopilot-devices"></a>Tworzenie i edytowanie urządzeń rozwiązania AutoPilot

## <a name="upload-a-list-of-devices"></a>Przekazywanie listy urządzeń

Aby przekazać [urządzenia,](add-autopilot-devices-and-profile.md) możesz skorzystać z przewodnika krok po kroku, ale możesz również przekazać urządzenia na **karcie** Urządzenia. 
  
Urządzenia muszą spełniać następujące wymagania:
  
- Windows 10 w wersji 1703 lub nowszej
    
- Nowe urządzenia, które nie są już w stanie obsługi klienta systemu Windows

1. W centrum administracyjnym platformy Microsoft 365 wybierz pozycję **Devices** \> **AutoPilot (Rozwiązania rozwiązania Devices AutoPilot).**
  
2. Na stronie **AutoPilot** wybierz kartę **Urządzenia** Dodaj \> **urządzenia.**
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. W **panelu Dodaj urządzenia** przejdź do przygotowanego przez Ciebie pliku [CSV](../admin/misc/device-list.md) z listą urządzeń i zapisz \>  \> **zamknij.**
    
    Możesz uzyskać te informacje od producenta sprzętu lub wygenerować plik CSV za pomocą skryptu programu [PowerShell Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Przypisywanie profilu do urządzenia lub grupy urządzeń

1. Na stronie **Przygotowywanie systemu Windows** wybierz **kartę** Urządzenia, a następnie zaznacz pole wyboru obok jednego lub większej liczby urządzeń. 
    
2. W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**. 
    
    Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md). 
