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
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068110"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10

Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego. Można to skonfigurować, najpierw synchronizowanie usługi Active Directory z usługą Azure Active Directory, a następnie rejestrowanie urządzeń z systemem Windows 10 z usługą Azure AD i rejestrowanie ich do zarządzania urządzeniami przenośnymi przez firmę Microsoft 365 Business.
Następujące wideo szczegóły kroki dotyczące sposobu ustawiania tego w najbardziej typowym scenariuszu.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Konfigurowanie urządzeń przyłączonych do domeny, które mają być zarządzane przez firmę Microsoft 365 Business

Aby skonfigurować urządzenia przyłączone do domeny w organizacji, aby korzystać z możliwości oferowanych przez usługę Azure Active Directory oprócz lokalnej usługi Active Directory, można zaimplementować **urządzeń przyłączonych do usługi Azure AD hybrydowy**. Są to urządzenia, które są przyłączone do lokalnej usługi Active Directory i Azure Active Directory. Hybrydowe urządzenia przyłączone do usługi Azure AD mogą być chronione i zarządzane przez firmę Microsoft 365 Business. 
  
Wykonaj poniższe kroki, aby urządzenia z systemem Windows 10 Hybrid Azure AD dołączył i zarządzane przez firmę Microsoft 365 Business.
  
1. **Przygotuj się do synchronizacji katalogów**: przed zsynchronizowaniem użytkowników i komputerów z lokalnej domeny usługi Active Directory, przejrzyj [przygotowanie do synchronizacji katalogów z pakietem Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie istnieją duplikaty dla następujących atrybutów: **mail**, **proxyAddresses**i **userPrincipalName**. Wartości te powinny być unikatowe i wszelkie duplikaty powinny zostać usunięte..
   
   - Zaleca się, że atrybut **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego jest skonfigurowany do dopasowania podstawowy adres e-mail, który odpowiada licencjonowanemu użytkownikowi Microsoft 365. Na przykład **Mary.Shelley@contoso.com** zamiast **Mary @ contoso. Local**
   
   - Jeśli domena usługi Active Directory kończy się sufiksem bez routingu, takim jak **. Local** lub **. LAN**, zamiast sufiksu routingu internetowego, takiego jak **. com** lub **. org**, należy najpierw dostosować sufiks nazwy UPN kont użytkowników lokalnych zgodnie z opisem w [Przygotuj domenę nieroutowalny do synchronizacji katalogów](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

2. **Instalowanie i Konfigurowanie programu Azure AD Connect**: Aby zsynchronizować użytkowników, grup i kontaktów z lokalnej usługi Active Directory w usłudze Azure Active Directory, uruchom Kreatora synchronizacji katalogów z Azure Active Directory Connect. Zobacz [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) , aby dowiedzieć się więcej.
    
    > [!NOTE]
    > Kroki są dokładnie takie same dla Microsoft 365 Business. 
    
Podczas konfigurowania opcji programu Azure AD Connect, zaleca się włączenie **synchronizacji haseł** i bezproblemowe logowanie **jednokrotne**, a także funkcji **zapisywania zwrotnego haseł** , który jest również obsługiwany w Microsoft 365 Business.

> [!NOTE]
> Istnieje kilka dodatkowych kroków do zapisywania zwrotnego haseł poza pole wyboru w programie Azure AD Connect. Odnoszą się do [How-to: Konfigurowanie zapisywania zwrotnego haseł](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **Konfigurowanie hybrydowego Azure AD Join**: przed włączeniem urządzeń systemu Windows 10 do hybrydowego usługi Azure AD, należy upewnić się, że spełniają następujące wymagania wstępne:

   - Używasz najnowszej wersji programu Azure AD Connect.

   - Azure AD Connect zsynchronizował wszystkie obiekty komputerów urządzeń, które mają być hybrydowego usługi Azure AD dołączył. Jeśli obiekty komputera należą do określonych jednostek organizacyjnych (OU), upewnij się, że te jednostki organizacyjne są ustawione do synchronizacji w usłudze Azure AD Connect, jak również.

Aby zarejestrować istniejące urządzenia przyłączone do domeny systemu Windows 10 jako hybrydowy usługi Azure AD przyłączony, wykonaj kroki opisane w [samouczku: Konfigurowanie hybrydowego usługi Azure Active Directory Join dla domen zarządzanych](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Umożliwi to hybrydowe istniejących lokalnych Active Directory przyłączonych komputerów z systemem Windows 10 i uczynić je gotowe do chmury.
    
4. **Włącz automatyczną rejestrację dla systemu Windows 10**: aby automatycznie rejestrować urządzenia z systemem Windows 10 do zarządzania urządzeniami przenośnymi w usłudze Intune, zobacz [Rejestrowanie urządzenia z systemem Windows 10 automatycznie przy użyciu zasad grupy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Można ustawić zasady grupy na poziomie komputera lokalnego lub dla operacji zbiorczych, można utworzyć to ustawienie zasad grupy na kontrolerze domeny przy użyciu konsoli zarządzania zasady grupy i ADMX szablonów.

5. **Skonfiguruj bezproblemowe**Logowanie jednokrotne: bezproblemowe logowanie jednokrotne automatycznie zaloguje użytkowników do swoich zasobów w chmurze Microsoft 365, gdy korzystają z komputerów firmowych. Wystarczy wdrożyć jedną z dwóch opcji zasad grupy opisanych w [usłudze Azure Active Directory bezproblemowe logowanie jednokrotne: Szybki Start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Opcja **zasady grupy** nie zezwala użytkownikom na zmienianie ich ustawień, podczas gdy opcja **preferencji zasady grupy** ustawia wartości, ale również pozostawia je konfigurowalne przez użytkownika.

6. **Konfigurowanie funkcji Windows Hello dla firm**: Windows Hello dla firm zastępuje hasła z silnego uwierzytelniania dwuskładnikowego (2FA) do logowania się do komputera lokalnego. Jednym z czynników jest para kluczy asymetrycznych, a druga to kod PIN lub inny gest lokalny, taki jak odcisk palca lub rozpoznawanie twarzy, jeśli urządzenie je obsługuje. Zaleca się, aby zastąpić hasła z 2FA i Windows Hello dla firm, gdzie to możliwe.

Aby skonfigurować hybrydowy Windows Hello dla firm, przejrzyj [klucz hybrydowy zaufania Windows Hello dla wymagań wstępnych biznesowych](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Następnie postępuj zgodnie z instrukcjami, aby [skonfigurować ustawienia zaufania klucza hybrydowego Windows Hello dla firm](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
