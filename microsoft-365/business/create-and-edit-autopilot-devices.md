---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzeń za pomocą autopilota w Microsoft 365 Business. Można przypisać profil do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660441"
---
# <a name="create-and-edit-autopilot-devices"></a>Tworzenie i edytowanie urządzeń rozwiązania AutoPilot

## <a name="upload-a-list-of-devices"></a>Przekazywanie listy urządzeń

Aby przekazać urządzenia, możesz skorzystać z [przewodnika krok po kroku](add-autopilot-devices-and-profile.md), ale możesz to również zrobić przy użyciu karty **Urządzenia**. 
  
Urządzenia muszą spełniać następujące wymagania:
  
- System Windows 10 w wersji 1703 lub nowszej.
    
- Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.

1. W Centrum administrator firmy Microsoft 365, wybierz **urządzenia** \> **autopilota**.
  
2. Na stronie **autopilota** , wybierz kartę **urządzenia** \> **Dodaj urządzenia**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Dodaj urządzenia** , przejdź do [pliku CSV lista urządzeń](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , przygotowanego \> **zapisać** \> **Zamknij**.
    
    Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik csv. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Przypisywanie profilu do urządzenia lub grupy urządzeń

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pola wyboru obok odpowiednich urządzeń. 
    
2. W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**. 
    
    Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md). 
    
