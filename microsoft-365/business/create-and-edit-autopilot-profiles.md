---
title: Tworzenie i edytowanie profilów rozwiązania AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Dowiedz się, tworzenie, edytowanie, usuwanie lub Usuń profile autopilota. '
ms.openlocfilehash: 7987cafb3ea234d81be72c79aee8e584a3770875
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073495"
---
# <a name="create-and-edit-autopilot-profiles"></a>Tworzenie i edytowanie profilów rozwiązania AutoPilot

## <a name="create-a-profile"></a>Tworzenie profilu

Profil dotyczy urządzenia lub grupy urządzeń.
  
1. W Centrum administrator firmy Microsoft 365, wybierz **urządzenia** \> **autopilota**.
  
2. Na stronie **autopilota** , wybierz kartę **Profile** \> **Utwórz profil**.
    
3. Na stronie **Tworzenie profilu** wprowadź opisową nazwę profilu, na przykład Marketing, włącz odpowiednie ustawienia (więcej informacji można znaleźć w temacie [Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md)) i wybierz pozycję **Zapisz**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Stosowanie profilu do urządzenia

Utworzony profil można zastosować do urządzenia lub grupy urządzeń. W [przewodniku krok po kroku](add-autopilot-devices-and-profile.md) można wybrać istniejący profil i zastosować go do nowych urządzeń lub zamienić istniejący profil dla urządzenia lub grupy urządzeń. 
  
1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Edytowanie, usuwanie lub czyszczenie profilu

Profil przypisany do urządzenia można zaktualizować, nawet jeśli już przekazano urządzenie użytkownikowi. Gdy urządzenie łączy się z Internetem, pobiera najnowszą wersję profilu w procesie konfiguracji. Jeśli użytkownik przywróci domyślne ustawienia fabryczne na urządzeniu, ponownie pobierze ono najnowsze aktualizacje profilu. 
  
### <a name="edit-a-profile"></a>Edytowanie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**. 
    
2. Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.
    
    Jeśli zrobisz to, zanim urządzenie użytkownika połączy się z Internetem, profil zostanie zastosowany w procesie konfiguracji.
    
### <a name="delete-a-profile"></a>Usuwanie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**. 
    
2. Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.
    
    Usunięty profil zostaje odłączony od urządzenia lub grupy urządzeń, do których go przypisano.
    
### <a name="remove-a-profile"></a>Czyszczenie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.
    
