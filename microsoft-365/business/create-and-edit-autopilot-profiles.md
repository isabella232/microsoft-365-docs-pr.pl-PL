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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Dowiedz się, jak tworzyć, edytować, usuwać i usuwać profile AutoPilot. '
ms.openlocfilehash: 8fae8af5e7aa7b866745d0b34a4fe11862de6e9d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287780"
---
# <a name="create-and-edit-autopilot-profiles"></a>Tworzenie i edytowanie profilów rozwiązania AutoPilot

## <a name="create-a-profile"></a>Tworzenie profilu

Profil dotyczy urządzenia lub grupy urządzeń.
  
1. W centrum administracyjnym Microsoft 365 dla firm wybierz opcję **urządzenia** \> **autopilot**.
  
2. Na stronie **autopilot** wybierz zakładkę \> **Profile** **Utwórz profil**.
    
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
    
