---
title: Omówienie konfiguracji
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Przegląd ustaw kroki dla Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086368"
---
# <a name="overview-of-setup"></a>Przegląd ustawień

Większość ustawień czynności może odbywać się w Kreatorze instalacji, ale inne opcje są również wyświetlane.


## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Dodawanie użytkownika domeny i użytkownicy

   - **[Dodawanie domeny](set-up.md#add-your-domain-to-personalize-sign-in)** (jeśli kupiłeś domeny podczas [zarejestrować się](sign-up.md), ten krok jest już zrobione.)

    - **Dodaj użytkowników**. Możesz to zrobić na jeden z trzech sposobów:
        - W oknie [Kreatora](set-up.md#add-users-in-the-wizard).
        - Użyj synchronizacji katalogów, aby [dodać użytkowników za pomocą Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jeśli masz lokalnej usługi Active directory.
        - Można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Ustawianie zasad zabezpieczeń i konfigurowania urządzeń 

  - [Kreator konfiguracji](set-up.md#set-up-security-policies-and-device-configurations) umożliwia skonfigurowanie urządzenia i zabezpieczeń. 
  - Można również dodać więcej lub edytować je później w [Centrum administracyjnego](view-policies-and-devices.md) i [portal Windows Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Oprócz ustawień zabezpieczeń w Kreatorze instalacji ze względów bezpieczeństwa można zwiększyć przez dodanie następujących ustawień:

      - **E-mail, ochrona przed złośliwym oprogramowaniem**
      - **Zaawansowane zagrożenia ochrony (ATP) bezpiecznego łącza**
      - **Załączników bezpieczne ATP**
      - **ATP anti-phishing**
      - **Exchange Online  archiwum**
      - **Zapobieganie utracie danych (DLP)**
      - **Ochrony informacji azure (Plan1**)

          Aby rozpocząć, zobacz [Konfigurowanie zasad zabezpieczeń zaawansowanych](set-up-advanced-security.md).

        Zobacz też [top 10 sposobów zabezpieczenia firmy Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) do utworzenia planu działań najważniejsze wskazówki dotyczące zabezpieczeń.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Konfigurowanie urządzeń i zarządzanie nimi 10 systemu Windows

   Po dołączeniu urządzenia Windows 10 do Azure AD, zasady ustawione w [kroku 2](#step-2-set-up-security-policies-and-configure-devices) będzie stosowane do niego.

   - Windows 10 Pro jest [wstępnie wymagane](pre-requisites-for-data-protection.md) dla Microsoft 365 Business, ale jeśli masz system Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro subskrypcji uprawnia do [uaktualnienia do systemu Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - [Kreator konfiguracji](set-up.md#set-up-security-policies-and-device-configurations) umożliwia konfigurowanie zasad dla urządzeń Windows 10.

## <a name="stes-4-install-office-365-business"></a>Wprowadzają 4: Zainstalować Business Office 365
- Można automatycznie zainstalować pakiet Office w urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](set-up.md#deploy-office-365-client-apps).
- Automatycznie [zainstalować pakiet Office](auto-install-or-uninstall-office.md) z Centrum administracyjnego.
- Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.
     
## <a name="advanced"></a>Zaawansowane
- **Służy do definiowania nowych urządzeń autopilota**
            
     Można użyć [Windows Autopilot](add-autopilot-devices-and-profile.md) automatycznie wstępnie skonfigurować **Nowe** urządzenia Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może zrobić to dla Ciebie. Można także przejść do [Magazyn Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) i zapytać specjalisty w zakresie technologii cloud Ustawianie nowych urządzeń, które kupić dla Ciebie.

- **Dostęp do zasobów lokalnych**

     - Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych. Postępuj zgodnie z instrukcjami [włączyć przyłączonych do domeny Windows 10 urządzenia mają być zarządzane przez Microsoft 365 Business](manage-windows-devices.md) można wybrać tę opcję. Jest to preferowana metoda i urządzeń, w tym stanie są nazywane hybrydowy Azure AD dołączył do urządzenia.

    - Jeśli Twoja firma ma lokalnej usługi Active Directory, który zawiera niektóre zasobów lokalnych (takich jak udziały plików i drukarek), może dać Azure AD przyłączony urządzeniom dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostępu do zasobów lokalnych z Azure AD dołączył do urządzenia w Microsoft 365 Business](access-resources.md).

  