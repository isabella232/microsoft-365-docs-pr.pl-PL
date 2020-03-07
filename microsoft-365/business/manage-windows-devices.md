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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dowiedz się, jak włączyć usługę Microsoft 365 do ochrony lokalnych urządzeń z systemem Windows 10 połączonych z usługą Active Directory w zaledwie kilku krokach.
ms.openlocfilehash: 625eb7ac344b060409101d650ff30044d073f5bf
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561465"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10

Jeśli organizacja korzysta z lokalnego usługi Windows Server Active Directory, można skonfigurować usługę Microsoft 365 Business do ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, można zaimplementować **hybrydowe urządzenia usługi Azure AD przyłączone**. Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i z usługą Azure Active Directory.

W tym klipie wideo opisano kroki, jak skonfigurować ten scenariusz dla najbardziej typowego scenariusza, który jest również wyszczególniony w kolejnych krokach.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotowanie do synchronizacji katalogów 

Przed synchronizacją użytkowników i komputerów z lokalnej domeny usługi Active Directory należy przejrzeć pozycję [Przygotuj do synchronizacji katalogów z usługą Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie istnieją duplikaty dla następujących atrybutów: **mail**, **proxyAddresses**i **userPrincipalName**. Wartości te muszą być unikatowe i wszelkie duplikaty muszą zostać usunięte.
   
   - Zaleca się skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego w celu dopasowania do podstawowego adresu e-mail odpowiadającego licencjonowanemu użytkownikowi usługi Microsoft 365. Na przykład: *mary.shelley@contoso.com,* a nie *mary@contoso.local*
   
   - Jeśli domena usługi Active Directory kończy się sufiksem nierutownym, takim jak *.local* lub *.lan,* zamiast sufiksu routingu internetowego, takiego jak *.com* lub *.org,* dostosuj sufiks nazwy UPN kont użytkowników lokalnych, zgodnie z opisem w [polu Przygotowywanie domeny nieroutingowej do synchronizacji katalogów](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i konfigurowanie usługi Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, należy zainstalować usługę Azure Active Directory Connect i skonfigurować synchronizację katalogów. Aby dowiedzieć się więcej, zobacz [Konfigurowanie synchronizacji katalogów dla usługi Office 365.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> Kroki są dokładnie takie same dla usługi Microsoft 365 Business. 

Podczas konfigurowania opcji usługi Azure AD Connect zaleca się włączenie **synchronizacji haseł**, **bezproblemowego logowania jednoosobowego**i funkcji **zapisywania spod kontroli hasła,** która jest również obsługiwana w usłudze Microsoft 365 Business.

> [!NOTE]
> Istnieje kilka dodatkowych kroków dotyczących zapisywania hasła poza polem wyboru w usłudze Azure AD Connect. Aby uzyskać więcej informacji, zobacz [Instrukcje: konfigurowanie zapisywania spisu haseł](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurowanie hybrydowego sprzężenia z usługą Azure AD

Przed włączeniu urządzeń z systemem Windows 10, które mają być hybrydowe usługi Azure AD przyłączony, upewnij się, że spełnia następujące wymagania wstępne:

   - Używasz najnowszej wersji usługi Azure AD Connect.

   - Usługa Azure AD connect zsynchronizowała wszystkie obiekty komputera urządzeń, do których chcesz dołączyć do hybrydowej usługi Azure AD. Jeśli obiekty komputera należą do określonych jednostek organizacyjnych (OU), upewnij się, że te jednostki organizacyjne są również ustawione do synchronizacji w usłudze Azure AD connect.

Aby zarejestrować istniejące urządzenia systemu Windows 10 przyłączone do usługi Hybrid Azure AD, wykonaj czynności opisane w [samouczku: Konfigurowanie hybrydowego sprzężenia usługi Azure Active Directory dla domen zarządzanych](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Ta hybrydowa włącza istniejące lokalne komputery usługi Active Directory dołączyła do komputerów z systemem Windows 10 i przygotujje je do pracy w chmurze.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Włącz automatyczną rejestrację dla systemu Windows 10

 Aby automatycznie zarejestrować urządzenia z systemem Windows 10 do zarządzania urządzeniami przenośnymi w usłudze Intune, zobacz [Automatyczne rejestrowanie urządzenia z systemem Windows 10 przy użyciu zasad grupy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Zasady grupy można ustawić na poziomie komputera lokalnego lub w przypadku operacji zbiorczych, można utworzyć to ustawienie zasad grupy na kontrolerze domeny za pomocą konsoli zarządzania zasadami grupy i szablonów ADMX.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurowanie bezproblemowego logowania jednoosobowego

  Bezproblemowa logowanie jednoosobowe automatycznie loguje użytkowników do zasobów chmury usługi Microsoft 365 podczas korzystania z komputerów firmowych. Wystarczy wdrożyć jedną z dwóch opcji zasad grupy opisanych w [usłudze Azure Active Directory Bezproblemowe logowanie jednoosobowe: Szybkie uruchamianie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Opcja **Zasady grupy** nie zezwala użytkownikom na zmienianie ustawień, a opcja **Preferencja zasad grupy** ustawia wartości, ale także umożliwia ich konfigurowanie przez użytkownika.

## <a name="6-set-up-windows-hello-for-business"></a>6. Konfigurowanie funkcji Windows Hello dla firm

 Funkcja Windows Hello dla firm zastępuje hasła silnym uwierzytelnianiem dwuskładnikowym (2FA) w celu logowania się do komputera lokalnego. Jednym z czynników jest asymetryczna para kluczy, a drugim jest kod PIN lub inny gest lokalny, taki jak odcisk palca lub rozpoznawanie twarzy, jeśli urządzenie je obsługuje. Zaleca się zastąpienie haseł 2FA i Windows Hello dla firm, jeśli to możliwe.

Aby skonfigurować hybrydowy program Windows Hello dla firm, przejrzyj [wymagania wstępne dotyczące zaufania klucza hybrydowego dla systemu Windows Hello dla firm](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Następnie postępuj zgodnie z instrukcjami w [konfigurowaniu hybrydowych ustawień zaufania kluczy windows hello dla firm](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
