---
title: Stany urządzeń
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
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
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Informacje o stanach urządzeń w usłudze Microsoft 365 Business.
ms.openlocfilehash: 26b218cb7b6a14f17e33d34a2e712b06ac814c0c
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065776"
---
# <a name="device-states"></a>Stany urządzeń

Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|**Stan**|**Opis**|
|:-----|:-----|
|Zarządzane przez usługę Intune  <br/> |Zarządzane przez usługę Microsoft 365 Business.  <br/> |
|Oczekiwanie na wycofanie  <br/> |Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.  <br/> |
|Wycofywanie w toku  <br/> |Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.  <br/> |
|Wycofywanie nie powiodło się  <br/> | Akcja usuwania danych firmy nie powiodła się.  <br/> |
|Wycofana anulowana  <br/> |Wycofaj akcję została anulowana.  <br/> |
|Oczekiwanie na wyczyszczenie  <br/> |Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.  <br/> |
|Czyszczenie w toku  <br/> |Wywołano polecenie przywracania ustawień fabrycznych.  <br/> |
|Czyszczenie nie powiodło się  <br/> |Nie można zrobić reset fabryczny.  <br/> |
|Wytrzeć anulowane  <br/> |Fabryczna chusteczka została anulowana.  <br/> |
|Zła kondycja  <br/> |Akcja jest w toku (lub w toku), ale urządzenie nie zaewidencjonowało się przez ponad 30 dni.  <br/> |
|Oczekiwanie na usunięcie  <br/> |Trwa oczekiwanie na akcję usuwania.  <br/> |
|Odnaleziono  <br/> |Usługa Microsoft 365 Business wykryła urządzenie.  <br/> |
   
