---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzenia za pomocą programu AutoPilot w usłudze Microsoft 365 Business. Profil można przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 640e4af7cccde83c87d90a875c1d44dead7255ca
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065992"
---
# <a name="create-and-edit-autopilot-devices"></a>Tworzenie i edytowanie urządzeń rozwiązania AutoPilot

## <a name="upload-a-list-of-devices"></a>Przekazywanie listy urządzeń

Aby przekazać urządzenia, możesz też użyć [przewodnika krok po kroku,](add-autopilot-devices-and-profile.md) ale możesz też przekazać urządzenia na karcie **Urządzenia.** 
  
Urządzenia muszą spełniać następujące wymagania:
  
- Windows 10, wersja 1703 lub nowsza
    
- Nowe urządzenia, które nie przeszły przez system Windows gotowe do obsługi

1. W centrum administracyjnym programu Microsoft 365 Business wybierz pozycję **Autopilot** **urządzeń** \> .
  
2. Na stronie **Autopilot** wybierz kartę **Urządzenia** , \> **dodaj urządzenia**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Dodawanie urządzeń** przejdź do [pliku CSV listy urządzeń](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) przygotowanego \> **zapisz** \> **zamknij**.
    
    Te informacje można uzyskać od dostawcy sprzętu lub użyć [skryptu Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) do wygenerowania pliku CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Przypisywanie profilu do urządzenia lub grupy urządzeń

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pole wyboru obok jednego lub większej liczby urządzeń. 
    
2. W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**. 
    
    Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md). 
    
