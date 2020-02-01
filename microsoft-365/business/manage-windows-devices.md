---
title: Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dowiedz się, jak włączyć usługę Microsoft 365 do ochrony lokalnych urządzeń z systemem Windows 10 przyłączonych do usługi Active Directory.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593806"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10

Jeśli organizacja korzysta z usługi Windows Server Active Directory w środowisku lokalnym, można skonfigurować usługę Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych wymagających uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, można zaimplementować **hybrydowe urządzenia połączone z usługi Azure AD.** Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i z usługą Azure Active Directory.

W tym klipie wideo opisano kroki konfigurowania tego dla najbardziej typowego scenariusza, który jest również szczegółowo opisany w kolejnych krokach.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotuj się do synchronizacji katalogów 

Przed synchronizacją użytkowników i komputerów z lokalnej domeny usługi Active Directory przejrzyj [pozycję Przygotuj synchronizację katalogów z usługą Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie ma duplikatów dla następujących atrybutów: **poczta,** **proxyAddresses**i **userPrincipalName**. Wartości te muszą być unikatowe i wszelkie duplikaty muszą zostać usunięte.
   
   - Zaleca się skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego lokalnego konta użytkownika tak, aby odpowiadał podstawowemu adresowi e-mail odpowiadającemu licencjonowanemu użytkownikowi usługi Microsoft 365. Na przykład: *mary.shelley@contoso.com,* a nie *mary@contoso.local*
   
   - Jeśli domena usługi Active Directory kończy się sufiksem nieroutingowym, takim jak *.local* lub *.lan,* zamiast internetowego sufiksu routingu, takiego jak *.com* lub *.org,* należy najpierw dostosować sufiks nazwy UPN lokalnych kont użytkowników zgodnie z opisem w [obszarze Przygotowanie domeny nieroutingu do synchronizacji katalogów.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i konfigurowanie usługi Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, zainstaluj usługę Azure Active Directory Connect i skonfiguruj synchronizację katalogów. Zobacz [Konfigurowanie synchronizacji katalogów usługi Office 365,](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) aby dowiedzieć się więcej.

> [!NOTE]
> Kroki są dokładnie takie same dla usługi Microsoft 365 Business. 

Podczas konfigurowania opcji usługi Azure AD Connect zaleca się włączenie **synchronizacji haseł,** **bezproblemowego logowania jednolitego**i funkcji **zapisywania danych przy użyciu hasła,** która jest również obsługiwana w programie Microsoft 365 Business.

> [!NOTE]
> Istnieje kilka dodatkowych kroków dotyczących zapisywania danych spisu haseł poza polewyboru w usłudze Azure AD Connect. Aby uzyskać więcej informacji, zobacz [Instrukcje: konfigurowanie zapisywania danych spisu hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurowanie hybrydowego dołączania do usługi Azure AD

Przed włączeniu urządzeń z systemem Windows 10 do łączenia z pomocą hybrydową usługi Azure AD upewnij się, że spełniasz następujące wymagania wstępne:

   - Używasz najnowszej wersji usługi Azure AD Connect.

   - Usługa Azure AD connect zsynchronizowała wszystkie obiekty komputera urządzeń, do których chcesz dołączyć hybrydowe usługi Azure AD. Jeśli obiekty komputera należą do określonych jednostek organizacyjnych, upewnij się, że te jednostki organizacyjne są ustawione do synchronizacji w usłudze Azure AD connect, jak również.

Aby zarejestrować istniejące urządzenia z systemem Windows 10 przyłączone do domeny w obszarze hybrydowa usługa Azure AD, wykonaj czynności opisane w [samouczku: Konfigurowanie hybrydowego dołączenia do usługi Azure Active Directory dla domen zarządzanych.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Ta hybryda umożliwia istniejące lokalne usługi Active Directory połączone z systemem Windows 10 komputery i uczynić je w chmurze gotowy.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Włącz automatyczną rejestrację dla systemu Windows 10

 Aby automatycznie zarejestrować urządzenia z systemem Windows 10 do zarządzania urządzeniami przenośnymi w usłudze Intune, zobacz Automatyczne rejestrowanie urządzenia z [systemem Windows 10 przy użyciu zasad grupy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Zasady grupy można ustawić na poziomie komputera lokalnego lub dla operacji zbiorczych, aby utworzyć to ustawienie Zasad grupy na kontrolerze domeny za pomocą konsoli zarządzania zasadami grupy i szablonów ADMX.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurowanie bezproblemowego logowania jednolitego

  Bezproblemowe logowanie jednoosłowe automatycznie podpisuje użytkowników w zasobach w chmurze usługi Microsoft 365, gdy korzystają z komputerów firmowych. Wystarczy wdrożyć jedną z dwóch opcji zasad grupy opisanych w [usłudze Azure Active Directory Bezproblemowe logowanie jednoliwe: Szybkie uruchamianie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Opcja **Zasady grupy** nie zezwala użytkownikom na zmianę ustawień, podczas gdy opcja **Preferencja zasad grupy** ustawia wartości, ale pozostawia je konfigurowalne przez użytkownika.

## <a name="6-set-up-windows-hello-for-business"></a>6. Konfigurowanie funkcji Windows Hello dla firm

 Funkcja Windows Hello dla firm zastępuje hasła silnym uwierzytelnianiem dwuskładnikowym (2FA) do logowania się na komputerze lokalnym. Jednym z czynników jest asymetryczna para kluczy, a drugi to kod PIN lub inny gest lokalny, taki jak odcisk palca lub rozpoznawanie twarzy, jeśli urządzenie je obsługuje. W miarę możliwości zaleca się zastąpienie haseł funkcjami 2FA i Windows Hello dla firm.

Aby skonfigurować hybrydowe funkcje funkcji Windows Hello dla firm, zapoznaj się z wymaganiami wstępnych programu Windows Hello dla firm — zaufanie [klucza hybrydowego](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Następnie postępuj zgodnie z instrukcjami w [konfiguracji hybrydowych ustawień zaufania klucza systemu Windows Hello dla firm](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
