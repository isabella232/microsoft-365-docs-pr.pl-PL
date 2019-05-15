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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profile autopilota można kontrolować, jak system Windows zostanie zainstalowany na urządzeniach użytkowników. Profile zawierają domyślne i ustawienia opcjonalne, takie jak pominąć instalację Cortana.
ms.openlocfilehash: adc8112861b67fd96a91ff24dc155aeb0c394532
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071865"
---
# <a name="about-autopilot-profile-settings"></a>Ustawienia profilu rozwiązania AutoPilot  informacje

## <a name="autopilot-profile-settings"></a>Ustawienia profilu autopilota

Można kontrolować, jak system Windows zostanie zainstalowany na urządzenia użytkownika przy użyciu profilów autopilota. Profile zawierają następujące ustawienia.
  
 **Autopilota domyślne funkcje (pole wymagane), które są ustawiane automatycznie:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomijanie rejestracji Cortana, OneDrive i OEM  <br/> |Pomija instalacji aplikacji konsumenta, takich jak Cortana i OneDrive osobistych. Urządzenie użytkownika można zainstalować później, tak długo, jak długo dany użytkownik jest administratorem lokalnym na urządzeniu. Pierwotnej rejestracji producenta jest pomijane, ponieważ urządzenie będzie zarządzany przez Microsoft 365 Business.  <br/> |
|Zaloguj się doświadczenie do marki firmy  <br/> |Jeśli Twoja firma ma, [Dodaj firmę znakowania do Office 365 stronę logowania](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), użytkownik urządzenia otrzyma tego doświadczenia podczas logowania się.  <br/> |
|MDM autorejestrowania z skonfigurowanych kont AAD.  <br/> |Tożsamość użytkownika będą zarządzane przez usługę Azure Active directory, a użytkownicy będą logują się do systemu Windows i Office 365 przy użyciu poświadczeń Microsoft 365 Business.  <br/> |
   
 **Ustawienia opcjonalne:**
  
|**Ustawienie**|**Opis**|
|:-----|:-----|
|Pomiń ustawienia prywatności (domyślnie wyłączone)  <br/> |Jeśli ta opcja jest ustawiona na **On**, urządzenie użytkownika nie zobaczą umowy licencyjnej dla urządzenia i Windows podczas po raz pierwszy zaloguje się.  <br/> |
|Niezezwalanie użytkownikowi stać się administratorem lokalnym  <br/> |Jeśli ta opcja jest ustawiona na **On**, użytkownik urządzenia nie będzie mógł zainstalować wszystkie aplikacje osobistych, takich jak Cortana.  <br/> |
   
