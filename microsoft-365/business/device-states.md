---
title: Stany urządzeń
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Dowiedz się więcej o Stany urządzeń w Microsoft 365 Business.
ms.openlocfilehash: 15114835a5014f5bfac600eac79bcdffdaec481a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276991"
---
# <a name="device-states"></a>Stany urządzeń

## <a name="device-states"></a>Stany urządzeń

Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|**Stan**|**Opis**|
|:-----|:-----|
|Zarządzane przez usługę Intune  <br/> |Zarządzane przez usługę Microsoft 365 Business.  <br/> |
|Oczekiwanie na wycofanie  <br/> |Trwa przygotowywanie do usunięcia danych firmy z urządzenia przez usługę Microsoft 365 Business.  <br/> |
|Wycofywanie w toku  <br/> |Trwa usuwanie danych firmy z urządzenia przez usługę Microsoft 365 Business.  <br/> |
|Wycofywanie nie powiodło się  <br/> | Akcja usuwania danych firmy nie powiodła się.  <br/> |
|Anulowano wycofywanie  <br/> |Akcja wycofywania została anulowana.  <br/> |
|Oczekiwanie na wyczyszczenie  <br/> |Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.  <br/> |
|Czyszczenie w toku  <br/> |Wywołano polecenie przywracania ustawień fabrycznych.  <br/> |
|Czyszczenie nie powiodło się  <br/> |Nie można przywrócić ustawień fabrycznych.  <br/> |
|Anulowano czyszczenie  <br/> |Przywracanie ustawień fabrycznych zostało anulowane.  <br/> |
|Zła kondycja  <br/> |Trwa oczekiwanie na rozpoczęcie akcji (lub jest ona w toku), ale urządzenie nie zostało zaewidencjonowane przez ponad 30 dni.  <br/> |
|Oczekiwanie na usunięcie  <br/> |Trwa oczekiwanie na akcję usuwania.  <br/> |
|Odnaleziono  <br/> |Usługa Microsoft 365 Business wykryła urządzenie.  <br/> |
   
