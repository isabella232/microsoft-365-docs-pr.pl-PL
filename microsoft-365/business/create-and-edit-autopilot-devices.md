---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
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
description: Dowiedz się, jak przesyłać urządzenia za pomocą funkcji AutoPilot w Microsoft 365 Business. Profil można przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 4eadaa800aa174bcd9cac50375f68c8471e1684e
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575413"
---
# <a name="create-and-edit-autopilot-devices"></a>Tworzenie i edytowanie urządzeń rozwiązania AutoPilot

## <a name="upload-a-list-of-devices"></a>Przekazywanie listy urządzeń

Aby przekazać urządzenia, możesz skorzystać z [przewodnika krok po kroku](add-autopilot-devices-and-profile.md), ale możesz to również zrobić przy użyciu karty **Urządzenia**. 
  
Urządzenia muszą spełniać następujące wymagania:
  
- System Windows 10 w wersji 1703 lub nowszej.
    
- Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.

1. W centrum administracyjnym Microsoft 365 dla firm wybierz opcję **urządzenia** \> **autopilot**.
  
2. Na stronie **autopilot** wybierz kartę \> **urządzenia** , a następnie **Dodaj urządzenia**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na **Dodaj urządzenia** panelu, przejdź do [listy urządzeń CSV-plik](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , który został przygotowany \> **Zapisz** \> **Zamknij**.
    
    Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik csv. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Przypisywanie profilu do urządzenia lub grupy urządzeń

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pola wyboru obok odpowiednich urządzeń. 
    
2. W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**. 
    
    Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md). 
    
