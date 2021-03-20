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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile rozwiązania AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pominięcie instalacji Cortany.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913383"
---
# <a name="about-autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot  informacje

## <a name="autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot

Profile rozwiązania AutoPilot mogą pomóc w kontrolowaniu sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają następujące ustawienia.
  
 **Funkcje domyślne rozwiązania AutoPilot ustawiane automatycznie (wymagane):**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń rejestrację Cortany, usługi OneDrive i OEM  <br/> |Pomija instalację aplikacji dla klientów konsumenckich, takich jak Cortana i osobista aplikacja OneDrive. Użytkownik urządzenia może je zainstalować później, o ile użytkownik jest administratorem lokalnym na urządzeniu. Rejestracja oryginalnego producenta zostanie pominięta, ponieważ urządzeniem będzie zarządzana usługa Microsoft 365 Business Premium.  <br/> |
|Logowanie się za pomocą marki firmowej  <br/> |Jeśli twoja firma ma znakowanie Dodaj markę twojej firmy do strony logowania na platformie [Microsoft 365,](../admin/setup/customize-sign-in-page.md)użytkownik urządzenia będzie miał to doświadczenie podczas logowania.  <br/> |
|Automatyczne rejestrowanie w uścisku usługi MDM ze skonfigurowanymi kontami AAD.  <br/> |Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy logują się do systemu Windows i platformy Microsoft 365 za pomocą poświadczeń platformy Microsoft 365 Business Premium.  <br/> |
   
 **Ustawienia opcjonalne:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń ustawienia prywatności (domyślnie wyłączone)  <br/> |Jeśli ta opcja jest ustawiona **na** Wł., użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy tylko się wcześniej pojawi.  <br/> |
|Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym  <br/> |Jeśli ta opcja jest ustawiona na Wł., użytkownik urządzenia nie będzie mógł zainstalować żadnych aplikacji osobistych, takich jak Cortana.<br/> |
