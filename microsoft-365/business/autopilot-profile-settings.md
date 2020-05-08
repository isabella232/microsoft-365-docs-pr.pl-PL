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
description: Profile autopilot ułatwią kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pomiń instalację Cortany.
ms.openlocfilehash: 0c706d12ba262856ff40ea3bee57c64234fd77f7
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165846"
---
# <a name="about-autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot  informacje

## <a name="autopilot-profile-settings"></a>Ustawienia profilu autopilot

Za pomocą profilów programu AutoPilot można kontrolować sposób instalowania systemu Windows na urządzeniach użytkownika. Profile zawierają następujące ustawienia.
  
 **Domyślne funkcje autopilot (wymagane), które są ustawiane automatycznie:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń rejestrację Cortany, Usługi OneDrive i OEM  <br/> |Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobista usługa OneDrive. Użytkownik urządzenia może zainstalować je później, o ile użytkownik jest administratorem lokalnym na urządzeniu. Oryginalna rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez usługę Microsoft 365 Business Premium.  <br/> |
|Zaloguj się za pomocą marki firmy  <br/> |Jeśli twoja firma ma [pozycję Dodaj markę firmy do strony logowania do usługi Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page)użytkownik urządzenia otrzyma to doświadczenie podczas logowania.  <br/> |
|Automatyczna rejestracja mdm ze skonfigurowanymi kontami AAD.  <br/> |Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemu Windows i usługi Microsoft 365 przy użyciu poświadczeń usługi Microsoft 365 Business Premium.  <br/> |
   
 **Ustawienia opcjonalne:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń ustawienia prywatności (domyślnie wyłączone)  <br/> |Jeśli ta opcja jest ustawiona **na Włączone,** użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy po raz pierwszy się zaloguje.  <br/> |
|Nie zezwalaj użytkownikowi na stanie się administratorem lokalnym  <br/> |Jeśli ta opcja jest **ustawiona na Włączone,** użytkownik urządzenia nie będzie mógł zainstalować żadnych aplikacji osobistych, takich jak Cortana.<br/> |
   
