---
title: Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączonych do domeny przez usługę Microsoft 365 dla firm
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dowiedz się, jak w kilku krokach umożliwić programowi Microsoft 365 ochronę lokalnych urządzeń z systemem Windows 10 połączonych z usługą Active Directory.
ms.openlocfilehash: e7f83e620fbb43a478dba98f78d5f471a541aea7
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403063"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-for-business"></a>Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączonych do domeny przez usługę Microsoft 365 dla firm

Jeśli twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, można skonfigurować usługę Microsoft 365 dla firm w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, można zaimplementować **urządzenia przyłączone do usługi Azure AD.** Te urządzenia są przyłączane zarówno do lokalnej usługi Active Directory, jak i usługi Azure Active Directory.

W tym klipie wideo opisano kroki dotyczące konfigurowania tego dla najbardziej typowych scenariuszy, który jest również szczegółowo opisany w kolejnych krokach.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotowanie do synchronizacji katalogów 

Przed zsynchronizowanie użytkowników i komputerów z lokalnej domeny usługi Active Directory należy zapoznać się z recenzją [Prepare for directory synchronizacji do usługi Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie istnieją duplikaty dla następujących atrybutów: **poczta,** **proxyAddresses**i **userPrincipalName**. Wartości te muszą być unikatowe i wszystkie duplikaty muszą zostać usunięte.
   
   - Zaleca się skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego w taki sposób, aby odpowiadał podstawowemu adresowi e-mail odpowiadającemu licencjonowanemu użytkownikowi usługi Microsoft 365. Na przykład: *mary.shelley@contoso.com,* a nie *mary@contoso.local*
   
   - Jeśli domena usługi Active Directory kończy się sufiksem niesygnawalnym, takim jak *.local* lub *.lan,* zamiast sufiksu z routingiem internetowym, takim jak *.com* lub *.org,* dostosuj sufiks nazwy UPN kont użytkowników lokalnych, zgodnie z opisem w [polu Przygotuj domenę nie rutowalną do synchronizacji katalogów.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i konfigurowanie usługi Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory w usłudze Azure Active Directory, zainstaluj usługę Azure Active Directory Connect i skonfiguruj synchronizację katalogów. Aby dowiedzieć się więcej, zobacz [Konfigurowanie synchronizacji katalogów dla usługi Office 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

> [!NOTE]
> Kroki są dokładnie takie same dla usługi Microsoft 365 dla firm. 

Podczas konfigurowania opcji usługi Azure AD Connect zaleca się włączenie **synchronizacji haseł,** **bezproblemowego logowania jednokrotnego**i funkcji **zapisywania zwrotnego hasła,** która jest również obsługiwana w usłudze Microsoft 365 dla firm.

> [!NOTE]
> Istnieje kilka dodatkowych kroków dotyczących zapisywania zwrotnego hasła poza polem wyboru w usłudze Azure AD Connect. Aby uzyskać więcej informacji, zobacz [Instrukcje: konfigurowanie storamentu hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurowanie hybrydowego sprzężenia usługi Azure AD

Przed włączeniem urządzeń z systemem Windows 10 do przyłączenia hybrydowej usługi Azure AD upewnij się, że spełniasz następujące wymagania wstępne:

   - Korzystasz z najnowszej wersji usługi Azure AD Connect.

   - Usługa Azure AD connect zsynchronizowała wszystkie obiekty komputera urządzeń, do których ma być przyłączona hybrydowa usługa Azure AD. Jeśli obiekty komputera należą do określonych jednostek organizacyjnych (OU), upewnij się, że te jednostki organizacyjne są ustawione do synchronizacji w usłudze Azure AD connect.

Aby zarejestrować istniejące urządzenia z systemem Windows 10 przyłączone do domeny jako połączone z usługą Hybrid Azure AD, wykonaj czynności opisane w [samouczku: Konfigurowanie hybrydowego sprzężenia usługi Azure Active Directory dla domen zarządzanych](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Ta hybrydowa umożliwia istniejącej lokalnej usłudze Active Directory dołączenie do komputerów z systemem Windows 10 i przygotowanie ich do chmury.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Włącz automatyczną rejestrację dla systemu Windows 10

 Aby automatycznie rejestrować urządzenia z systemem Windows 10 do zarządzania urządzeniami przenośnymi w usłudze Intune, zobacz [Automatyczne rejestrowanie urządzenia z systemem Windows 10 przy użyciu zasad grupy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Zasady grupy można ustawić na poziomie komputera lokalnego lub w przypadku operacji zbiorczych, aby utworzyć to ustawienie zasad grupy na kontrolerze domeny, można ustawić zasady grupy na poziomie komputera lokalnego lub w przypadku operacji zbiorczych.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurowanie bezproblemowego logowania jednokrotnego

  Bezproblemowe logowanie jednokrotne automatycznie loguje użytkowników do zasobów w chmurze usługi Microsoft 365 podczas korzystania z komputerów firmowych. Wystarczy wdrożyć jedną z dwóch opcji zasad grupy opisanych w [usłudze Azure Active Directory Bezproblemowe logowanie jednokrotne: Szybkie uruchamianie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Opcja **Zasady grupy** nie zezwala użytkownikom na zmienianie ustawień, podczas gdy opcja **Preferencje zasad grupy** ustawia wartości, ale także pozostawia je konfigurowalne przez użytkownika.

## <a name="6-set-up-windows-hello-for-business"></a>6. Konfigurowanie funkcji Windows Hello dla firm

 Funkcja Windows Hello dla firm zastępuje hasła silnym uwierzytelnianiem dwuskładnikowym (2FA) w celu zalogowania się na komputerze lokalnym. Jednym z czynników jest asymetryczna para kluczy, a drugim jest kod PIN lub inny gest lokalny, taki jak odcisk palca lub rozpoznawanie twarzy, jeśli urządzenie go obsługuje. W miarę możliwości zaleca się zastąpienie haseł 2FA i Windows Hello for Business.

Aby skonfigurować hybrydowy element Windows Hello dla firm, zapoznaj się z [wymaganiami wstępnymi systemu Windows Hello dla firm dotyczących klucza hybrydowego](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Następnie postępuj zgodnie z instrukcjami w [temacie Konfigurowanie hybrydowych ustawień zaufania kluczy systemu Windows Hello dla firm](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
