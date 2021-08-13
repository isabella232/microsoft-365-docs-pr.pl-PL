---
title: Omówienie konfiguracji
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z krokami konfiguracji Microsoft 365 Business Premium, od subskrybowania, dodawania domeny i użytkowników po konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 7c09dca354781bf92f6bbecca0f3fb9875fb654515fe35c2f96cc780a894a764
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803227"
---
# <a name="overview-of-setup"></a>Omówienie konfiguracji

Obejrzyj krótki klip wideo na temat Microsoft 365 Business Premium konfiguracji.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](../business-video/index.yml).

Większość kroków konfiguracji można wykonać przy instalacji ze przewodnikiem, ale wymienione są również inne opcje.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1. Dodawanie domeny i użytkowników

   - **[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji](sign-up.md), ten krok jest już wykonane).

   - **Dodaj użytkowników.** Użytkowników możesz dodać na jeden z trzech sposobów:
        - W konfiguracji [z przewodnikiem](set-up.md#add-users-in-the-wizard).
        - Użyj synchronizacji [katalogów, aby dodać użytkowników przy użyciu usługi Azure AD Połączenie,](../enterprise/set-up-directory-synchronization.md) jeśli masz lokalną usługę Active Directory.
        - Użytkowników możesz [również dodać w dalszej](../admin/add-users/add-users.md) części centrum administracyjnego.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2. Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń 

  - Skonfiguruj zasady dotyczące urządzeń [przy](set-up.md#protect-your-organization) użyciu konfiguracji ze przewodnikiem. 
  - Możesz również dodać więcej lub edytować je później w centrum administracyjnym i w [portalu Intune.](/intune/tutorial-walkthrough-intune-portal) [](view-policies-and-devices.md)
  - Kreator konfiguracji skonfiguruje również podstawowe ustawienia ochrony przed zagrożeniami i utratą danych.
  
  Oprócz ustawień zabezpieczeń w kreatorze konfiguracji możesz zwiększyć poziom zabezpieczeń, dodając następujące ustawienia:

- **Ochrona przed złośliwym oprogramowaniem w wiadomościach e-mail**
- **Ochrona przed wyłudzaniem informacji w programie Defender dla Office 365**
- **Exchange Online  archiwum**
- **Azure Information Protection (plan1)**

Aby rozpocząć, zobacz [Zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) [i konfigurowanie funkcji zgodności.](set-up-compliance.md)

Zobacz [również 10 najlepszych](/office365/admin/security-and-compliance/secure-your-business-data) sposobów zabezpieczania konta Microsoft 365 Business Premium, aby uzyskać plan najlepszych rozwiązań w zakresie zabezpieczeń.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3. Konfigurowanie urządzeń przenośnych i Windows 10 zarządzanie nimi

Po zakończeniu konfiguracji ze przewodnikiem należy chronić wszystkie Windows 10 w organizacji.
  
- Windows 10 Pro wymaga wstępnie [](pre-requisites-for-data-protection.md) wersji Microsoft 365 Business Premium, ale jeśli masz subskrypcję usługi Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja uprawnia do uaktualnienia do systemu [Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).
- Postępuj zgodnie z instrukcjami w [zabezpieczaniu Windows 10 PC,](secure-win-10-pcs.md) aby skonfigurować zasady dotyczące Windows 10 komputerach.

Po dołączeniu urządzenia Windows 10 do usługi Azure AD są do niej stosowane zasady ustawione dla Windows 10 komputerów. Aby uzyskać więcej informacji, [zobacz Konfigurowanie Windows dla Microsoft 365 użytkowników.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4. Instalowanie Aplikacje Microsoft 365 dla firm
- Możesz automatycznie zainstalować Office urządzeniach Windows urządzeniach przy użyciu [kreatora konfiguracji.](set-up.md#deploy-office-365-client-apps)
- Umożliwianie [użytkownikom Office aplikacji dla](/office365/admin/setup/install-applications) Windows i urządzeń.
     
## <a name="advanced"></a>Advanced
- **Konfigurowanie nowych urządzeń za pomocą rozwiązania Autopilot**
            
     Możesz użyć rozwiązania [Windows Autopilot,](add-autopilot-devices-and-profile.md) aby  automatycznie wstępnie skonfigurować nowe urządzenia Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie. Możesz również przejść do [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), a następnie poprosić eksperta z technologii w chmurze o skonfigurowanie nowych kupowanych urządzeń.

- **Zasoby lokalne programu Access**

     - Jeśli Twoja organizacja Windows Server Active Directory korzysta z lokalnego systemu, możesz skonfigurować usługę Microsoft 365 Business Premium do ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego. Postępuj zgodnie z instrukcjami w włączanie zarządzania przez Windows 10 [przyłączone](manage-windows-devices.md) do domeny przez Microsoft 365 Business Premium, aby to skonfigurować. Jest to preferowana metoda, a urządzenia w tym stanie mają nazwę Urządzenia sprzężenia hybrydowego usługi Azure AD.

    - Jeśli Twoja firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udzielić swoim urządzeniu przyłączony do usługi Azure AD dostępu do tych zasobów, korzystając z procedury opisanej tutaj: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie [Microsoft 365 Business Premium.](access-resources.md)

## <a name="related-content"></a>Zawartość pokrewna

[Microsoft 365 szkoleniowe klipy wideo dla firm](../business-video/index.yml) (strona linku)