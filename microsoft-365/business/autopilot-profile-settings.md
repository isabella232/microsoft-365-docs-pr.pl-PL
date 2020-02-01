---
title: "Ustawienia profilu rozwiązania AutoPilot \x97 informacje"
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile programu AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkownika. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pominięcie instalacji Cortany.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593338"
---
# <a name="about-autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot  informacje

## <a name="autopilot-profile-settings"></a>Ustawienia profilu Programu AutoPilot

Za pomocą profilów programu AutoPilot można kontrolować sposób instalowania systemu Windows na urządzeniach użytkownika. Profile zawierają następujące ustawienia.
  
 **Domyślne funkcje AutoPilota (wymagane), które są ustawiane automatycznie:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń cortanę, onedrive i rejestrację oem  <br/> |Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobista usługa OneDrive. Użytkownik urządzenia może zainstalować je później, o ile użytkownik jest administratorem lokalnym na urządzeniu. Oryginalna rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez firmę Microsoft 365 Business.  <br/> |
|Zaloguj się do marki swojej firmy  <br/> |Jeśli twoja firma ma [markę Dodaj firmę do strony logowania do usługi Office 365,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)użytkownik urządzenia otrzyma to środowisko podczas logowania.  <br/> |
|Automatyczna rejestracja usługi MDM przy skonfigurowanych kontach add.  <br/> |Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemów Windows i usługi Office 365 przy użyciu poświadczeń usługi Microsoft 365 Business.  <br/> |
   
 **Ustawienia opcjonalne:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomijanie ustawień prywatności (domyślnie wyłączone)  <br/> |Jeśli ta opcja jest ustawiona na **Włączone,** użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy po raz pierwszy się zaloguje.  <br/> |
|Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym  <br/> |Jeśli ta opcja jest ustawiona na **Włączone,** użytkownik urządzenia nie będzie mógł zainstalować żadnych osobistych aplikacji, takich jak Cortana.<br/> |
   
