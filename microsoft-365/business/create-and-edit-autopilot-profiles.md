---
title: Tworzenie i edytowanie profilów rozwiązania AutoPilot
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Dowiedz się, jak tworzyć, edytować, usuwać lub usuwać profile programu AutoPilot.
ms.openlocfilehash: 35967cb1f6e2cdeea9d7c42a529526410fa8b586
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593996"
---
# <a name="create-and-edit-autopilot-profiles"></a>Tworzenie i edytowanie profilów rozwiązania AutoPilot

## <a name="create-a-profile"></a>Tworzenie profilu

Profil dotyczy urządzenia lub grupy urządzeń.
  
1. W centrum administracyjnym programu Microsoft 365 Business wybierz pozycję **Autopilot** **urządzeń** \> .
  
2. Na stronie **Autopilot** wybierz kartę **Profile** \> **stwórz profil**.
    
3. Na stronie **Tworzenie profilu** wprowadź nazwę profilu, który pomaga go zidentyfikować, na przykład Marketing. Włącz żądane ustawienie, a następnie wybierz pozycję **Zapisz**. Aby uzyskać więcej informacji na temat ustawień profilu AutoPilot, zobacz [Ustawienia profilu AutoPilota](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Stosowanie profilu do urządzenia

Po utworzeniu profilu można go zastosować do urządzenia lub grupy urządzeń. Możesz wybrać istniejący profil w [przewodniku krok po kroku](add-autopilot-devices-and-profile.md) i zastosować go do nowych urządzeń lub zastąpić istniejący profil dla urządzenia lub grupy urządzeń. 
  
1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**. 
    
2. Zaznacz pole wyboru obok nazwy urządzenia, a następnie w panelu **Urządzenie** wybierz profil \> z listy rozwijanej **Przypisany profil** **Zapisz**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Edytowanie, usuwanie lub czyszczenie profilu

Profil przypisany do urządzenia można zaktualizować, nawet jeśli już przekazano urządzenie użytkownikowi. Gdy urządzenie łączy się z Internetem, pobiera najnowszą wersję profilu w procesie konfiguracji. Jeśli użytkownik przywróci domyślne ustawienia fabryczne na urządzeniu, ponownie pobierze ono najnowsze aktualizacje profilu. 
  
### <a name="edit-a-profile"></a>Edytowanie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**. 
    
2. Zaznacz pole wyboru obok nazwy urządzenia, **** a następnie w panelu \> Profil zaktualizuj dowolne z dostępnych ustawień **Zapisz**.
    
    Jeśli zrobisz to, zanim urządzenie użytkownika połączy się z Internetem, profil zostanie zastosowany w procesie konfiguracji.
    
### <a name="delete-a-profile"></a>Usuwanie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**. 
    
2. Zaznacz pole wyboru obok nazwy urządzenia, a następnie w panelu **Profil** wybierz polecenie **Usuń zapisywanie** **profilu** \> .
    
    Usunięty profil zostaje odłączony od urządzenia lub grupy urządzeń, do których go przypisano.
    
### <a name="remove-a-profile"></a>Czyszczenie profilu

1. Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**. 
    
2. Zaznacz pole wyboru obok nazwy urządzenia, a następnie w panelu **Urządzenie** wybierz pozycję \> **Brak** z listy rozwijanej **Przypisany profil** **Zapisz**.
    
