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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dowiedz się, jak włączyć funkcję Microsoft 365 w celu ochrony lokalnych urządzeń z systemem Windows 10 połączonych z usługą Active Directory.
ms.openlocfilehash: 93e3364fc94f3878bec13d0a87b17a7d3678a4cc
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633274"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10

Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego.
Aby skonfigurować tę ochronę, można zaimplementować **urządzeń przyłączonych do hybrydowego usługi Azure AD**. Te urządzenia są przyłączone do lokalnej usługi Active Directory i Azure Active Directory.

Ten film wideo opisuje kroki, jak ustawić to dla najbardziej typowych scenariusz, który jest również szczegółowo w krokach, które należy wykonać.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotuj się do synchronizacji katalogów 

Przed zsynchronizowaniem użytkowników i komputerów z lokalnej domeny usługi Active Directory, przejrzyj [przygotowanie do synchronizacji katalogów z pakietem Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie istnieją duplikaty dla następujących atrybutów: **mail**, **proxyAddresses**i **userPrincipalName**. Te wartości muszą być unikatowe, a wszelkie duplikaty muszą zostać usunięte.
   
   - Zaleca się skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego, aby dopasować podstawowy adres e-mail odpowiadający licencjonowanemu użytkownikowi Microsoft 365. Na przykład: *Mary.Shelley@contoso.com* zamiast *Mary@contoso. Local*
   
   - Jeśli domena usługi Active Directory kończy się sufiksem bez routingu, takim jak *. Local* lub *. LAN*, zamiast sufiksu routingu internetowego, takiego jak *. com* lub *. org*, Dostosuj sufiks UPN kont użytkowników lokalnych najpierw zgodnie z opisem w [przygotowanie domeny innej niż routowalny do synchronizacji katalogów](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i Konfigurowanie usługi Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory w usłudze Azure Active Directory, należy zainstalować usługę Azure Active Directory Connect i skonfigurować synchronizację katalogów. Zobacz [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) , aby dowiedzieć się więcej.

> [!NOTE]
> Kroki są dokładnie takie same dla Microsoft 365 Business. 

Podczas konfigurowania opcji programu Azure AD Connect, zaleca się włączenie **synchronizacji haseł**, **bezproblemowe logowanie jednokrotne**i funkcji **zapisywania zwrotnego haseł** , która jest również obsługiwana w Microsoft 365 Business.

> [!NOTE]
> Istnieje kilka dodatkowych kroków do zapisywania zwrotnego haseł poza pole wyboru w programie Azure AD Connect. Aby uzyskać więcej informacji, zobacz [instrukcje: Konfigurowanie zapisywania zwrotnego haseł](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Skonfiguruj dołączenie do hybrydowej usługi Azure AD

Przed włączeniem urządzeń systemu Windows 10 do hybrydowego usługi Azure AD dołączył, upewnij się, że spełniają następujące wymagania wstępne:

   - Korzystasz z najnowszej wersji programu Azure AD Connect.

   - Azure AD Connect zsynchronizował wszystkie obiekty komputerów urządzeń, które mają być hybrydowego usługi Azure AD dołączył. Jeśli obiekty komputera należą do określonych jednostek organizacyjnych (OU), upewnij się, że te jednostki organizacyjne są ustawione do synchronizacji w usłudze Azure AD Connect, jak również.

Aby zarejestrować istniejące urządzenia przyłączone do domeny systemu Windows 10 jako hybrydowy usługi Azure AD przyłączony, wykonaj kroki opisane w [samouczku: Konfigurowanie hybrydowego usługi Azure Active Directory Join dla domen zarządzanych](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Ta hybrydowa — umożliwia istniejącej lokalnej usługi Active Directory przyłączonych komputerów z systemem Windows 10 i uczynić je gotowe do chmury.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Włącz automatyczną rejestrację w systemie Windows 10

 Aby automatycznie rejestrować urządzenia z systemem Windows 10 do zarządzania urządzeniami przenośnymi w usłudze Intune, zobacz [Rejestrowanie urządzenia z systemem Windows 10 automatycznie przy użyciu zasad grupy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Można ustawić zasady grupy na poziomie komputera lokalnego lub dla operacji zbiorczych, można użyć konsoli zarządzania zasady grupy i ADMX szablony do tworzenia tego ustawienia zasady grupy na kontrolerze domeny.

## <a name="5-configure-seamless-single-sign-on"></a>5. Skonfiguruj bezproblemowe logowanie jednokrotne

  Bezproblemowe logowanie jednokrotne automatycznie podpisuje użytkowników do swoich zasobów w chmurze Microsoft 365, gdy korzystają z komputerów firmowych. Wystarczy wdrożyć jedną z dwóch opcji zasad grupy opisanych w [usłudze Azure Active Directory bezproblemowe logowanie jednokrotne: Szybki Start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Opcja **zasady grupy** nie zezwala użytkownikom na zmienianie ich ustawień, podczas gdy opcja **preferencji zasady grupy** ustawia wartości, ale również pozostawia je konfigurowalne przez użytkownika.

## <a name="6-set-up-windows-hello-for-business"></a>6. Konfigurowanie systemu Windows Hello dla firm

 Windows Hello dla firm zastępuje hasła z silnego uwierzytelniania dwuskładnikowego (2FA) do logowania się do komputera lokalnego. Jednym z czynników jest para kluczy asymetrycznych, a druga to kod PIN lub inny gest lokalny, taki jak odcisk palca lub rozpoznawanie twarzy, jeśli urządzenie je obsługuje. Zalecamy zastąpienie haseł 2FA i Windows Hello dla firm, jeśli to możliwe.

Aby skonfigurować hybrydowy Windows Hello dla firm, przejrzyj [klucz hybrydowy zaufania Windows Hello dla wymagań wstępnych biznesowych](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Następnie postępuj zgodnie z instrukcjami w [Konfigurowanie hybrydowy Windows Hello dla firmy ustawienia zaufania kluczy](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
