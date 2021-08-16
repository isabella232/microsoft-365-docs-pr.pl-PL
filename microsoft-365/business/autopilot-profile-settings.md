---
title: "Ustawienia profilu rozwiązania AutoPilot \x97 informacje"
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Profile rozwiązania AutoPilot ułatwiają kontrolowanie sposobu Windows instalacji na urządzeniach użytkowników. Profile zawierają ustawienia domyślne i opcjonalne, takie jak pomijanie Cortana instalacji.
ms.openlocfilehash: 67ad6e92583d71207e2807657a7ad00261e1249291e2e6a7546f544ea924b394
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896328"
---
# <a name="about-autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot  informacje

## <a name="autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot

Profile rozwiązania AutoPilot mogą pomóc w kontrolowaniu sposobu Windows na urządzeniach użytkowników. Profile zawierają następujące ustawienia.
  
 **Funkcje domyślne rozwiązania AutoPilot ustawiane automatycznie (wymagane):**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń Cortana, OneDrive i OEM  <br/> |Pomija instalowanie aplikacji dla klientów osobistych, takich Cortana i aplikacji OneDrive. Użytkownik urządzenia może je zainstalować później, o ile użytkownik jest administratorem lokalnym na urządzeniu. Rejestracja oryginalnego producenta zostanie pominięta, ponieważ urządzeniem będzie zarządzać Microsoft 365 Business Premium.  <br/> |
|Logowanie się za pomocą marki firmowej  <br/> |Jeśli twoja firma ma znakowanie Dodaj markę twojej firmy do [strony Microsoft 365](../admin/setup/customize-sign-in-page.md)logowania, użytkownik urządzenia otrzyma to środowisko podczas logowania.  <br/> |
|Automatyczne rejestrowanie w uścisku usługi MDM ze skonfigurowanymi kontami AAD.  <br/> |Tożsamość użytkownika będzie zarządzana przez firmę Azure Active Directory, a użytkownicy będą logować się Windows i Microsoft 365 przy użyciu swoich poświadczeń logowania Microsoft 365 Business Premium konta.  <br/> |
   
 **Ustawienia opcjonalne:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń ustawienia prywatności (domyślnie wyłączone)  <br/> |Jeśli ta opcja jest **ustawiona** na Wł., użytkownik urządzenia nie zobaczy umowy licencyjnej urządzenia i nie zobaczy Windows po pierwszym się do urządzenia.  <br/> |
|Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym  <br/> |Jeśli ta opcja jest ustawiona na Wł., użytkownik urządzenia nie będzie mógł zainstalować żadnych aplikacji osobistych, takich jak Cortana.<br/> |
