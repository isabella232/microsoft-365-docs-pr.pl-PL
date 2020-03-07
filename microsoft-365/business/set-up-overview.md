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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z instrukcjami konfiguracji usługi Microsoft 365 Business, od subskrypcji po dodawanie domeny i użytkowników, po konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 9bb536b52981966f6c4c487f8400577b896261e0
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561207"
---
# <a name="overview-of-setup"></a>Omówienie konfiguracji

Obejrzyj krótki film o konfiguracji usługi Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników platformy Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Większość kroków konfiguracji można wykonać w kreatorze konfiguracji, ale inne opcje są również wymienione.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Dodaj domenę i użytkowników

   - **[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli domena została kupiona podczas [rejestracji,](sign-up.md)ten krok jest już wykonany).

    - **Dodaj użytkowników**. Możesz dodać użytkowników na jeden z trzech sposobów:
        - W [kreatorze](set-up.md#add-users-in-the-wizard).
        - Synchronizacja katalogów umożliwia [dodawanie użytkowników przy użyciu usługi Azure AD Connect,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) jeśli masz lokalny katalog Active.
        - Możesz również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Konfigurowanie zasad zabezpieczeń i konfigurowanie urządzeń 

  - Użyj [Kreatora instalacji,](set-up.md#protect-your-organization) aby skonfigurować zasady dotyczące urządzeń. 
  - Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Kreator konfiguracji skonfiguruj również podstawowe ustawienia ochrony przed zagrożeniami i zapobiegania utracie danych.
  
  Oprócz ustawień zabezpieczeń w kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:

- **Ochrona przed złośliwym oprogramowaniem poczty e-mail**
- **Ochrona przed phishingiem atp**
- **Exchange Online  archiwum**
- **Usługa Azure Information Protection (Plan1)**

Aby rozpocząć, zobacz [zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) i [konfigurowanie funkcji zgodności](set-up-compliance.md).

Zobacz też [10 najważniejszych sposobów zabezpieczenia usługi Microsoft 365 Business,](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) aby zapoznać się z planem najlepszych rozwiązań w zakresie zabezpieczeń.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi

Po uruchomieniu kreatora konfiguracji należy zwiększyć wszystkie komputery Windwos 10 w organizacji.
  
- Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla microsoft 365 Business, ale jeśli masz Windows 7 Pro, Windows 8 Pro, lub Windows 8.1 Pro, subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Wykonaj kroki opisane w [bezpiecznych komputerach z systemem Windows 10,](secure-win-10-pcs.md) aby skonfigurować zasady dla urządzeń z systemem Windows 10.

Po dołączeniu urządzenia z systemem Windows 10 do usługi Azure AD zasady ustawione dla komputerów z systemem Windows 10 są do niego stosowane. Aby uzyskać więcej informacji, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Krok 4: Instalowanie usługi Office 365 Business
- Pakiet Office można zainstalować automatycznie na urządzeniach z systemem Windows za pomocą [kreatora instalacji](set-up.md#deploy-office-365-client-apps).
- Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
## <a name="advanced"></a>Zaawansowane
- **Konfigurowanie nowych urządzeń za pomocą programu Autopilot**
            
     Za pomocą [programu Windows Autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie skonfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera,](https://www.microsoft.com/solution-providers/search) który może to zrobić za Ciebie. Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta w dziedzinie technologii w chmurze o skonfigurowanie nowych kupowanego urządzeń.

- **Dostęp do zasobów lokalnych**

     - Jeśli organizacja korzysta z lokalnego usługi Windows Server Active Directory, można skonfigurować usługę Microsoft 365 Business do ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego. Wykonaj kroki opisane w [artykule Włącz urządzenia z systemem Windows 10 przyłączone do domeny, które mają być zarządzane przez firmę Microsoft 365 Business,](manage-windows-devices.md) aby to skonfigurować. Jest to preferowana metoda, a urządzenia w tym stanie są nazywane hybrydowymi urządzeniami usługi Azure AD przyłączonymi.

    - Jeśli twoja firma ma lokalną usługę Active Directory zawierającą pewne zasoby lokalne (takie jak udziały plików i drukarki), można przyznać urządzeniom przyłączonym do usługi Azure AD dostęp do tych zasobów, wykonując następujące kroki w tym miejscu: [Dostęp do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>Zobacz też

[Szkoleniowe klipy wideo dotyczące rozwiązania Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
