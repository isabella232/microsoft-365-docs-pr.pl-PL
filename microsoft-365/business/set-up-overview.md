---
title: Omówienie konfiguracji
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Zapoznaj się z czynnościami konfiguracyjną usługi Microsoft 365 Business Premium, od subskrybowania, dodawania domeny i użytkowników po konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 9d92aefb3b5666bb7c2fd2e13c9a00f074f107a7
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912495"
---
# <a name="overview-of-setup"></a>Omówienie konfiguracji

Obejrzyj krótki klip wideo o konfiguracji usługi Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Większość kroków konfiguracji można wykonać przy instalacji ze przewodnikiem, ale wymienione są również inne opcje.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1. Dodawanie domeny i użytkowników

   - **[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji](sign-up.md), ten krok jest już wykonane).

   - **Dodaj użytkowników.** Użytkowników możesz dodać na jeden z trzech sposobów:
        - W konfiguracji [z przewodnikiem](set-up.md#add-users-in-the-wizard).
        - Użyj synchronizacji [katalogów, aby dodać użytkowników za pomocą programu Azure AD Connect,](../enterprise/set-up-directory-synchronization.md) jeśli masz lokalną usługę Active Directory.
        - Użytkowników możesz [również dodać w dalszej](../admin/add-users/add-users.md) części centrum administracyjnego.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2. Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń 

  - Skonfiguruj zasady dotyczące urządzeń [przy](set-up.md#protect-your-organization) użyciu konfiguracji ze przewodnikiem. 
  - Możesz również dodać więcej lub edytować je później w centrum administracyjnym i w [portalu Intune.](/intune/tutorial-walkthrough-intune-portal) [](view-policies-and-devices.md)
  - Kreator konfiguracji skonfiguruje również podstawowe ustawienia ochrony przed zagrożeniami i utratą danych.
  
  Oprócz ustawień zabezpieczeń w kreatorze konfiguracji możesz zwiększyć poziom zabezpieczeń, dodając następujące ustawienia:

- **Ochrona przed złośliwym oprogramowaniem w wiadomościach e-mail**
- **Ochrona przed wyłudzaniem informacji w usłudze Defender dla usługi Office 365**
- **Exchange Online  archiwum**
- **Azure Information Protection (plan1)**

Aby rozpocząć, zobacz [Zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) [i konfigurowanie funkcji zgodności.](set-up-compliance.md)

Zapoznaj się również z 10 najlepszymi sposobami zabezpieczania usługi [Microsoft 365 Business Premium,](/office365/admin/security-and-compliance/secure-your-business-data) aby uzyskać drogową mapę z najlepszymi rozwiązaniami w zakresie zabezpieczeń.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3. Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi

Po zakończeniu konfiguracji ze przewodnikiem należy chronić wszystkie komputery z systemem Windows 10 w organizacji.
  
- System Windows 10 [](pre-requisites-for-data-protection.md) Pro stanowi wymaganie wstępne dla usługi Microsoft 365 Business Premium, ale jeśli masz system Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja uprawnia do uaktualnienia do systemu [Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)
- Postępuj zgodnie z instrukcjami w zabezpieczaniu komputerów z systemem [Windows 10,](secure-win-10-pcs.md) aby skonfigurować zasady dla urządzeń z systemem Windows 10.

Po dołączeniu urządzenia z systemem Windows 10 do usługi Azure AD są do niej stosowane zasady ustawione dla komputerów z systemem Windows 10. Aby uzyskać więcej informacji, [zobacz Konfigurowanie urządzeń z systemem Windows dla użytkowników platformy Microsoft 365.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4. Instalowanie aplikacji platformy Microsoft 365 dla firm
- Pakiet Office na urządzeniach z systemem Windows można zainstalować automatycznie za pomocą [kreatora konfiguracji.](set-up.md#deploy-office-365-client-apps)
- Umożliwianie [użytkownikom instalowania aplikacji pakietu Office](/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
## <a name="advanced"></a>Advanced
- **Konfigurowanie nowych urządzeń za pomocą rozwiązania Autopilot**
            
     Rozwiązania [Windows Autopilot](add-autopilot-devices-and-profile.md) można użyć do automatycznego wstępnego skonfigurowania nowych urządzeń z systemem **Windows** 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie. Możesz również przejść do [Sklepu Microsoft](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta z technologii w chmurze o skonfigurowanie nowych, kupowanych urządzeń.

- **Zasoby lokalne programu Access**

     - Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego. Aby skonfigurować to ustawienie, wykonaj czynności opisane w tece Włączanie zarządzania przez usługę [Microsoft 365 Business Premium](manage-windows-devices.md) dla urządzeń przyłączanych do domeny systemu Windows 10. Jest to preferowana metoda, a urządzenia w tym stanie mają nazwę Urządzenia sprzężenia hybrydowego usługi Azure AD.

    - Jeśli Twoja firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udzielić swoim urządzeniu przyłączony do usługi Azure AD dostępu do tych zasobów, korzystając z procedury opisanej w tym miejscu: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze [Microsoft 365 Business Premium.](access-resources.md)

## <a name="see-also"></a>Zobacz też

[Szkoleniowe klipy wideo dotyczące platformy Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)