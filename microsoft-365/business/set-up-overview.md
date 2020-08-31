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
description: Zapoznaj się z instrukcjami dotyczącymi konfigurowania programu Microsoft 365 Business Premium, od abonamentu, aby dodać domenę i użytkowników, skonfigurować zasady zabezpieczeń i nie tylko.
ms.openlocfilehash: fa9c02fa9546437c83b9cc6c1f1e6e0d723ec868
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306474"
---
# <a name="overview-of-setup"></a>Omówienie konfiguracji

Obejrzyj krótki klip wideo o konfiguracji programu Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Większość kroków konfiguracji można wykonać w Kreatorze konfiguracji, ale inne opcje są również wyświetlane.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Dodawanie domeny i użytkowników

   - **[Dodaj swoją domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (Jeśli podczas [tworzenia konta](sign-up.md)zakupiono domenę, ten krok jest już wykonywany).

   - **Dodaj użytkowników**. Użytkowników możesz dodać na jeden z trzech sposobów:
        - W [Kreatorze](set-up.md#add-users-in-the-wizard).
        - Za pomocą funkcji synchronizacji katalogów [Dodaj użytkowników przy użyciu usługi Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) , jeśli masz lokalną usługę Active Directory.
        - Możesz również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Konfigurowanie zasad zabezpieczeń i Konfigurowanie urządzeń 

  - Skonfiguruj zasady urządzenia za pomocą [Kreatora konfiguracji](set-up.md#protect-your-organization) . 
  - Możesz również dodać je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Kreator instalacji również skonfiguruje podstawowe ustawienia ochrony przed zagrożeniami i ochrona przed utratą danych.
  
  Oprócz ustawień zabezpieczeń w Kreatorze konfiguracji możesz zwiększyć bezpieczeństwo, dodając następujące ustawienia:

- **Ochrona przed złośliwym oprogramowaniem e-mail**
- **Ochrona ATP — wyłudzanie informacji**
- **Exchange Online  archiwum**
- **Usługa Azure Information Protection (Plan1**)

Aby rozpocząć, zobacz [zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) i [Konfigurowanie funkcji zgodności](set-up-compliance.md).

Zobacz też [10 najważniejszych sposobów zabezpieczenia usługi Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) , aby uzyskać plan najważniejszych wskazówek dotyczących bezpieczeństwa.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi

Po uruchomieniu Kreatora konfiguracji będziesz proctect wszystkie komputery Windows 10 w organizacji.
  
- System Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) produktu Microsoft 365 Business Premium, ale jeśli masz system Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, abonament uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Postępuj zgodnie z instrukcjami w artykule [Zabezpieczanie komputerów z systemem Windows 10](secure-win-10-pcs.md) , aby skonfigurować zasady dla urządzeń z systemem Windows 10.

Po dołączeniu do urządzenia z systemem Windows 10 do usługi Azure AD zostaną zastosowane zasady skonfigurowane dla komputerów z systemem Windows 10. Aby uzyskać więcej informacji, zobacz [Konfigurowanie urządzeń z systemem Windows dla systemu Microsoft 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4: Instalowanie aplikacji Microsoft 365 dla firm
- Możesz automatycznie zainstalować pakiet Office na urządzeniach z systemem Windows za pomocą [Kreatora konfiguracji](set-up.md#deploy-office-365-client-apps).
- Zezwól użytkownikom na [Instalowanie aplikacji pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
## <a name="advanced"></a>Advanced
- **Konfigurowanie nowych urządzeń za pomocą autopilota**
            
     Za pomocą [autopilota systemu Windows](add-autopilot-devices-and-profile.md) można automatycznie skonfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale łatwiej można uzyskać od niego [partnera](https://www.microsoft.com/solution-providers/search) . Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta o technologii chmury o skonfigurowanie nowych urządzeń do zakupu.

- **Uzyskiwanie dostępu do zasobów lokalnych**

     - Jeśli Twoja organizacja korzysta z usługi Active Directory w systemie Windows Server, możesz skonfigurować aplikację Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelnienia lokalnego. Postępuj zgodnie z instrukcjami zawartymi w artykule [Włączanie obsługi urządzeń z systemem Windows 10 dołączonymi do domeny](manage-windows-devices.md) w celu skonfigurowania usługi Microsoft 365 Business Premium. Jest to preferowana metoda, a urządzenia w tym stanie są nazywane urządzeniami hybrydowymi usługi Azure AD.

    - Jeśli Twoja firma korzysta z lokalnej usługi Active Directory, która zawiera zasoby lokalne (takie jak udziały plików i drukarki), możesz udostępnić urządzeniom z systemem Azure AD, aby uzyskać dostęp do tych zasobów, wykonując czynności opisane tutaj: [Uzyskiwanie dostępu do zasobów lokalnych z urządzenia z przyłączeniem usługi Azure AD w programie Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>Zobacz też

[Szkolenia wideo dotyczące programu Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
