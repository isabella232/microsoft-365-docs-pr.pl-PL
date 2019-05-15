---
title: Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
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
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dowiedz się, jak włączyć Microsoft 365 do ochrony AD lokalnych połączonych urządzeń Windows 10.
ms.openlocfilehash: af0e78ef6e79bfd612b11a16538e7afcd377ffb0
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071555"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10

Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych. Możesz ustawić to dzięki pierwszej synchronizacji usługi Active Directory z usługą Active Directory, a następnie rejestracji urządzeń 10 systemu Windows Azure AD i zapisywania ich do zarządzania urządzeniami przenośnymi przez Microsoft 365 Business.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Konfigurowanie urządzeń przyłączonych do domeny mają być zarządzane przez Microsoft 365 Business

Aby skonfigurować urządzenia przyłączone do domeny organizacji do korzystania z możliwości oferowane przez usługę Active Directory Azure oprócz lokalnej usługi Active Directory, można zaimplementować **hybrydowy Azure AD dołączył do urządzenia**. Są to urządzenia, które są połączone, zarówno w usłudze Active Directory na lokalnym i usługi Active Directory Azure. Urządzeniach hybrydowych Azure AD dołączył do mogą być chronione i zarządzane przez Microsoft 365 Business. 
  
Należy wykonać poniższe kroki, aby utworzyć urządzeniach 10 systemu Windows Azure AD przyłączony i zarządzany przez Microsoft 365 Business hybrydowy.
  
1. Aby zsynchronizować użytkowników, grup i kontakty z lokalną usługę Active Directory z usługą Active Directory Azure, uruchom Kreatora synchronizacji katalogu i Azure Active Directory połączyć zgodnie z opisem w [Konfigurowanie synchronizacji katalogów usługi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Kroki są dokładnie takie same dla Microsoft 365 Business. 
  
2. Przed wykonaniem kroku 3, aby włączyć w urządzeniach Windows 10 za hybrydowe dołączył do Azure AD, należy upewnić się, że spełniasz następujące wymagania wstępne:

   - Używasz najnowszej wersji programu Azure AD connect.

   - Połączyć Azure AD został zsynchronizowany wszystkie obiekty komputera ma być hybrydowy Azure AD dołączył do urządzeń. Jeśli obiekty komputerów należą do poszczególnych jednostek organizacyjnych (OU), a następnie upewnij się, że te jednostki organizacyjne są ustawione dla synchronizacji w Azure AD również połączyć.
    
3. Zarejestruj istniejących urządzeniach Windows 10 domeny hybrydowy Azure AD połączonych i zapisać je do zarządzania urządzeniami przenośnymi przez Intune (Microsoft 365 Business):
    
4. Postępuj zgodnie z instrukcjami krok po kroku, w [jaki sposób skonfigurować hybrydowy Azure Active Directory dołączył do urządzenia](https://go.microsoft.com/fwlink/p/?linkid=872870). Spowoduje to włączenie synchronizacji usługi Active Directory na lokalnym przyłączony systemie Windows 10 komputerów i ich gotowości w chmurze.
    
5. Aby zarejestrować urządzenie Windows 10 do zarządzania urządzeniami przenośnymi, zobacz [Rejestrowanie urządzeń systemu Windows 10 z Windows Intune za pomocą zasady grupy](https://go.microsoft.com/fwlink/p/?linkid=872871) instrukcje. Poziom można ustawić zasady grupy na komputerze lokalnym lub operacje zbiorcze można utworzyć ustawienie zasad grupy na serwerze kontrolera domeny.