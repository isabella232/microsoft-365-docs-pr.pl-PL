---
title: Tworzenie i edytowanie profilów rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983137"
---
# <a name="create-and-edit-autopilot-profiles"></a>Tworzenie i edytowanie profilów rozwiązania AutoPilot

## <a name="create-a-profile"></a>Tworzenie profilu

Profil dotyczy urządzenia lub grupy urządzeń.
  
1. W centrum administracyjnym usług Microsoft 365 Business wybierz pozycję **Wdróż system Windows za pomocą rozwiązania Autopilot** na karcie **Akcje urządzenia**. 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. Na stronie **Przygotowanie systemu Windows** wybierz kartę **Profile** \> **Utwórz profil**.
    
3. Na stronie **Tworzenie profilu** wprowadź opisową nazwę profilu, na przykład Marketing, włącz odpowiednie ustawienia (więcej informacji można znaleźć w temacie [Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md)) i wybierz pozycję **Zapisz**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Stosowanie profilu do urządzenia

Utworzony profil można zastosować do urządzenia lub grupy urządzeń. W [przewodniku krok po kroku](add-autopilot-devices-and-profile.md) można wybrać istniejący profil i zastosować go do nowych urządzeń lub zamienić istniejący profil dla urządzenia lub grupy urządzeń. 
  
1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**. 
    
2. Kliknij pole wyboru obok nazwy urządzenia, jak i w panelu **urządzenia** , wybierz profil z listy rozwijanej **przypisany profil** \> **zapisać**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Edytowanie, usuwanie lub czyszczenie profilu

Profil przypisany do urządzenia można zaktualizować, nawet jeśli już przekazano urządzenie użytkownikowi. Gdy urządzenie łączy się z Internetem, pobiera najnowszą wersję profilu w procesie konfiguracji. Jeśli użytkownik przywróci domyślne ustawienia fabryczne na urządzeniu, ponownie pobierze ono najnowsze aktualizacje profilu. 
  
### <a name="edit-a-profile"></a>Edytowanie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**. 
    
2. Kliknij pole wyboru obok nazwy urządzenia i w **profilu** panelu zaktualizować dowolne dostępne ustawienia \> **zapisać**.
    
    Jeśli zrobisz to, zanim urządzenie użytkownika połączy się z Internetem, profil zostanie zastosowany w procesie konfiguracji.
    
### <a name="delete-a-profile"></a>Usuwanie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**. 
    
2. Kliknij pole wyboru obok nazwy urządzenia, a w panelu **profilu** kliknij przycisk **Usuń profil** \> **zapisać**.
    
    Usunięty profil zostaje odłączony od urządzenia lub grupy urządzeń, do których go przypisano.
    
### <a name="remove-a-profile"></a>Czyszczenie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**. 
    
2. Kliknij pole wyboru obok nazwy urządzenia, jak i w panelu **urządzenia** , wybierz opcję **Brak** z listy rozwijanej **przypisany profil** \> **zapisać**.
    
