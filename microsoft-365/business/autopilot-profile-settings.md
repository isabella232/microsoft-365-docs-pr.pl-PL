---
title: "Ustawienia profilu rozwiązania AutoPilot \x97 informacje"
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile AutoPilot ułatwiają kontrolowanie sposobu instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają domyślne i opcjonalne ustawienia, takie jak Pomiń instalację Cortany.
ms.openlocfilehash: cd66627943301f4a4f2410bafeff6074919ec29d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287480"
---
# <a name="about-autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot  informacje

## <a name="autopilot-profile-settings"></a>Ustawienia profilu AutoPilot

Za pomocą profilów AutoPilot można kontrolować sposób instalowania systemu Windows na urządzeniach użytkowników. Profile zawierają następujące ustawienia.
  
 **Domyślne funkcje autopilota (wymagane), które są ustawiane automatycznie:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń rejestrację Cortany, OneDrive i OEM  <br/> |Pomija instalację aplikacji konsumenckich, takich jak Cortana i osobisty OneDrive. Użytkownik urządzenia można zainstalować te później tak długo, jak on lub ona jest administratorem lokalnym na urządzeniu. Oryginalna Rejestracja producenta jest pomijana, ponieważ urządzenie będzie zarządzane przez firmę Microsoft 365 Business.  <br/> |
|Zaloguj się w swojej firmie  <br/> |Jeśli Twoja firma ma [dodać marki firmy do pakietu Office 365 Zaloguj się na stronie](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), użytkownik urządzenia będzie uzyskać to doświadczenie podczas logowania.  <br/> |
|Automatyczna rejestracja MDM z skonfigurowanymi kontami usługi AAD.  <br/> |Tożsamość użytkownika będzie zarządzana przez usługę Azure Active Directory, a użytkownicy będą logować się do systemu Windows i pakietu Office 365 za pomocą poświadczeń firmy Microsoft 365 Business.  <br/> |
   
 **Ustawienia opcjonalne:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń ustawienia prywatności (domyślnie wyłączone)  <br/> |Jeśli ta opcja jest **włączona**, użytkownik urządzenia nie zobaczy umowy licencyjnej dla urządzenia i systemu Windows, gdy on lub ona po raz pierwszy loguje się.  <br/> |
|Nie Zezwalaj, aby użytkownik stał się administratorem lokalnym  <br/> |Jeśli ta opcja jest **włączona**, użytkownik urządzenia nie będzie mógł instalować żadnych osobistych aplikacji, takich jak Cortana.  <br/> |
   
