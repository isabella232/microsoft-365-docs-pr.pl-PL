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
description: Dowiedz się, jak włączyć Microsoft 365 do ochrony lokalnych urządzeń z systemem Windows 10 przyłączonych do usługi AD.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992234"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10

Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego. Można to skonfigurować, najpierw synchronizowanie usługi Active Directory z usługą Azure Active Directory, a następnie rejestrowanie urządzeń z systemem Windows 10 z usługą Azure AD i rejestrowanie ich do zarządzania urządzeniami przenośnymi przez firmę Microsoft 365 Business.
Następujące wideo szczegóły kroki dotyczące sposobu ustawiania tego w najbardziej typowym scenariuszu.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Konfigurowanie urządzeń przyłączonych do domeny, które mają być zarządzane przez firmę Microsoft 365 Business

Aby skonfigurować urządzenia przyłączone do domeny w organizacji, aby korzystać z możliwości oferowanych przez usługę Azure Active Directory oprócz lokalnej usługi Active Directory, można zaimplementować **urządzeń przyłączonych do usługi Azure AD hybrydowy**. Są to urządzenia, które są przyłączone do lokalnej usługi Active Directory i Azure Active Directory. Hybrydowe urządzenia przyłączone do usługi Azure AD mogą być chronione i zarządzane przez firmę Microsoft 365 Business. 
  
Wykonaj poniższe kroki, aby urządzenia z systemem Windows 10 Hybrid Azure AD dołączył i zarządzane przez firmę Microsoft 365 Business.
  
1. Aby zsynchronizować użytkowników, grup i kontaktów z lokalnej usługi Active Directory w usłudze Azure Active Directory, uruchom Kreatora synchronizacji katalogów i Azure Active Directory Connect zgodnie z opisem w [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Kroki są dokładnie takie same dla Microsoft 365 Business. 
  
2. Przed wykonaniem kroku 3, aby włączyć urządzenia systemu Windows 10 do hybrydowego usługi Azure AD dołączył, należy upewnić się, że spełniają następujące wymagania wstępne:

   - Używasz najnowszej wersji programu Azure AD Connect.

   - Azure AD Connect zsynchronizował wszystkie obiekty komputerów urządzeń, które mają być hybrydowego usługi Azure AD dołączył. Jeśli obiekty komputera należą do określonych jednostek organizacyjnych (OU), upewnij się, że te jednostki organizacyjne są ustawione do synchronizacji w usłudze Azure AD Connect, jak również.
    
3. Zarejestruj istniejące urządzenia przyłączone do domeny systemu Windows 10 do hybrydowego usługi Azure AD dołączył i zarejestrować je do zarządzania urządzeniami przenośnymi przez usługę Intune (Microsoft 365 Business):
    
4. Postępuj zgodnie z instrukcjami krok po kroku w [sposobie konfigurowania hybrydowego usługi Azure Active Directory przyłączonych urządzeń](https://go.microsoft.com/fwlink/p/?linkid=872870). Umożliwi to synchronizację lokalnej usługi Active Directory przyłączonych komputerów z systemem Windows 10 i sprawi, że będą gotowe do chmury.
    
5. Aby zarejestrować urządzenie z systemem Windows 10 do zarządzania urządzeniami przenośnymi, zobacz [Rejestrowanie urządzenia z systemem Windows 10 przy użyciu usługi Intune za pomocą zasad grupy](https://go.microsoft.com/fwlink/p/?linkid=872871) , aby uzyskać instrukcje. Można ustawić zasady grupy na poziomie komputera lokalnego lub dla operacji zbiorczych, można utworzyć to ustawienie zasad grupy na serwerze kontrolera domeny.