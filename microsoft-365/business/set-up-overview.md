---
title: Przegląd ustawień
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
description: Omówienie kroków konfiguracji dla Microsoft 365 Business.
ms.openlocfilehash: cab999493bf86ed0adf32521eaf6b3943f107f79
ms.sourcegitcommit: cf7b0fd80ecfb7a216111a801269c5322794795e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/09/2020
ms.locfileid: "40995255"
---
# <a name="overview-of-setup"></a>Przegląd ustawień

Obejrzyj krótki film o instalacji Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Większość czynności konfiguracyjnych można wykonać w Kreatorze instalacji, ale wyświetlane są również inne opcje.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Dodaj domenę i użytkowników

   - **[Dodaj domenę](set-up.md#add-your-domain-to-personalize-sign-in)** (Jeśli Twoja domena została [kupiona podczas rejestracji](sign-up.md), ten krok jest już zrobione).

    - **Dodawanie użytkowników**. Możesz dodać użytkowników na trzy sposoby:
        - W [Kreatorze](set-up.md#add-users-in-the-wizard).
        - Użyj synchronizacji katalogów, aby [dodać użytkowników przy użyciu programu Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jeśli masz lokalną usługę Active Directory.
        - Możesz także [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Konfigurowanie zasad zabezpieczeń i Konfigurowanie urządzeń 

  - Skonfiguruj zasady urządzeń za pomocą [Kreatora instalacji](set-up.md#protect-your-organization) . 
  - Można również dodać więcej lub edytować je później w [centrum administracyjnym](view-policies-and-devices.md) i w [portalu usługi Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Kreator konfiguracji ustawi również podstawowe ustawienia ochrony przed zagrożeniami i zapobiegania utracie danych.
  
  Oprócz ustawień zabezpieczeń w Kreatorze konfiguracji można zwiększyć bezpieczeństwo, dodając następujące ustawienia:

- **Ochrona przed złośliwym oprogramowaniem poczty e-mail**
- **ATP anty-phishing**
- **Exchange Online  archiwum**
- **Ochrona informacji Azure (Plan1**)

Aby rozpocząć, zobacz [zwiększanie ochrony przed zagrożeniami](increase-threat-protection.md) i [Konfigurowanie funkcji zgodności](set-up-compliance.md).

Zobacz także [10 najlepszych sposobów zabezpieczania Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) dla planu najlepszych praktyk w zakresie bezpieczeństwa.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Konfigurowanie urządzeń z systemem Windows 10 i zarządzanie nimi

Po uruchomieniu Kreatora konfiguracji, będziemy chcieli, aby samoobrony wszystkie komputery Windwos 10 w organizacji.
  
- Windows 10 Pro jest [warunkiem wstępnym](pre-requisites-for-data-protection.md) dla Microsoft 365 Business, ale jeśli masz Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, subskrypcja uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Wykonaj kroki opisane w [bezpiecznych komputerach z systemem Windows 10](secure-win-10-pcs.md) , aby skonfigurować zasady dla urządzeń z systemem Windows 10.

Po przyłączeniu urządzenia systemu Windows 10 do usługi Azure AD, zasady ustawione dla komputerów z systemem Windows 10 zostanie zastosowany do niego. Aby uzyskać więcej informacji, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników Microsoft 365 Business](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Krok 4: instalacja pakietu Office 365 Business
- Pakiet Office można automatycznie zainstalować na urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](set-up.md#deploy-office-365-client-apps).
- Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
## <a name="advanced"></a>Zaawansowane
- **Konfigurowanie nowych urządzeń za pomocą autopilota**
            
     Za pomocą programu [Windows autopilot](add-autopilot-devices-and-profile.md) można automatycznie wstępnie konfigurować **nowe** urządzenia z systemem Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może to zrobić dla Ciebie. Możesz również przejść do [sklepu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)i poprosić eksperta w zakresie technologii chmurowej o konfigurowanie nowych urządzeń, które kupujesz.

- **Dostęp do zasobów lokalnych**

     - Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego. Wykonaj kroki opisane w [Włączanie przyłączonych do domeny urządzeń z systemem Windows 10, które mają być zarządzane przez firmę Microsoft 365 Business](manage-windows-devices.md) , aby to skonfigurować. Jest to preferowana metoda, a urządzenia w tym stanie nazywane są urządzeniami przyłączone do hybrydowej usługi Azure AD.

    - Jeśli firma ma lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (na przykład udziały plików i drukarki), możesz nadać urządzeniom przyłączonym do usługi Azure AD dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: dostęp do [zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>Zobacz też

[Szkoleniowe klipy wideo dotyczące rozwiązania Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
