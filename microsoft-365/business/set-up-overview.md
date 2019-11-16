---
title: Omówienie konfigurowania
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Omówienie konfigurowania kroków dla Microsoft 365 Business.
ms.openlocfilehash: 3e1cf240db673a7b961ec8aa574f3e09efee476b
ms.sourcegitcommit: 8ca97fa879ae4ea44468be629d6c32b429efeeec
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/16/2019
ms.locfileid: "38676033"
---
# <a name="overview-of-setup"></a>Przegląd ustawień

Większość kroków konfiguracji można wykonać w Kreatorze instalacji, ale inne opcje są również wymienione.


## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Dodaj domenę i użytkowników

   - **[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (Jeśli Twoja domena została [kupiona podczas rejestracji](sign-up.md), ten krok jest już zrobione).

    - **Dodawanie użytkowników**. Można to zrobić na trzy sposoby:
        - W [Kreatorze](set-up.md#add-users-in-the-wizard).
        - Użyj synchronizacji katalogów, aby [dodać użytkowników przy użyciu programu Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jeśli masz lokalną usługę Active Directory.
        - Możesz także [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Konfigurowanie zasad zabezpieczeń i Konfigurowanie urządzeń 

  - Skonfiguruj zasady dotyczące urządzeń i zabezpieczeń za pomocą [Kreatora instalacji](set-up.md#protect-data-and-devices) . 
  - Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Oprócz ustawień zabezpieczeń w Kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:

      - **Ochrona przed złośliwym oprogramowaniem poczty e-mail**
      - **Zaawansowane zabezpieczenia przed zagrożeniami (ATP) bezpieczne łącza**
      - **Bezpieczne załączniki ATP**
      - **ATP anty-phishing**
      - **Exchange Online  archiwum**
      - **Zapobieganie utracie danych (DLP)**
      - **Ochrona informacji Azure (Plan1**)

          Aby rozpocząć, zobacz [Konfigurowanie zaawansowanych zasad zabezpieczeń](set-up-advanced-security.md).

        Zobacz także [10 najlepszych sposobów zabezpieczania Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) dla planu najlepszych praktyk w zakresie bezpieczeństwa.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi

   Po przyłączeniu urządzenia systemu Windows 10 do usługi Azure AD, zasady skonfigurowane w [kroku 2](#step-2-set-up-security-policies-and-configure-devices) Get stosowane do niego.

   - Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla Microsoft 365 Business, ale jeśli masz Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Użyj [Kreatora konfiguracji](set-up.md#protect-data-and-devices) , aby skonfigurować zasady dla urządzeń z systemem Windows 10.

## <a name="stes-4-install-office-365-business"></a>Stes 4: instalacja pakietu Office 365 Business
- Pakiet Office można automatycznie zainstalować na urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](set-up.md#deploy-office-365-client-apps).
- Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
## <a name="advanced"></a>Zaawansowane
- **Konfigurowanie nowych urządzeń za pomocą autopilota**
            
     Za pomocą programu [Windows autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie konfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może to zrobić dla Ciebie. Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) i poprosić eksperta w zakresie technologii chmurowej o ustawienie nowych urządzeń, które zakupisz.

- **Dostęp do zasobów lokalnych**

     - Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego. Wykonaj kroki opisane w [Włączanie przyłączonych do domeny urządzeń z systemem Windows 10, które mają być zarządzane przez firmę Microsoft 365 Business](manage-windows-devices.md) , aby to skonfigurować. Jest to preferowana metoda i urządzenia w tym stanie są nazywane hybrydowych urządzeń przyłączonych do usługi Azure AD.

    - Jeśli firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (na przykład udziały plików i drukarki), możesz nadać urządzeniom przyłączonym do usługi Azure AD dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: dostęp do [zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business](access-resources.md).

  