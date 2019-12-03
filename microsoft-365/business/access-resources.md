---
title: Dostęp do zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do lokalnych zasobów, takich jak aplikacje biznesowe, udziały plików i drukarki z urządzenia z systemem Windows 10 przyłączonych do usługi Azure Active Directory.
ms.openlocfilehash: 4a2ff28107c6e2ec4473859c75bf720df7662747
ms.sourcegitcommit: 58a7bd70a4bcf52530baf5f82507fd5dc4455fd9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/03/2019
ms.locfileid: "39668793"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Dostęp do zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business

Wszystkie urządzenia z systemem Windows 10, które są przyłączone do usługi Azure Active Directory, mają dostęp do wszystkich zasobów w chmurze, takich jak aplikacje pakietu Office 365 i mogą być chronione przez firmę Microsoft 365 Business. Można również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje biznesowe (LOB), udziałów plików i drukarek. Aby zezwolić na dostęp, użyj [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) , aby zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory. 

Aby dowiedzieć się więcej, zobacz [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Kroki są również podsumowane w poniższych sekcjach.

> [!IMPORTANT]
> Ta procedura ma zastosowanie tylko do uwierzytelniania OAuth i NTLM. Protokół Kerberos nie jest obsługiwany.
 
## <a name="run-azure-ad-connect"></a>Uruchom program Azure AD Connect

Wykonaj następujące kroki, aby włączyć urządzenia przyłączone do usługi Azure AD w organizacji dostępu do zasobów lokalnych.
  
1. Aby zsynchronizować użytkowników, grup i kontaktów z lokalnej usługi Active Directory w usłudze Azure Active Directory, uruchom Kreatora synchronizacji katalogów i Azure AD Connect zgodnie z opisem w [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są przyłączone do usługi Azure AD. Ten krok jest wykonywana indywidualnie na każdym urządzeniu z systemem Windows 10. Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników Microsoft 365 Business](set-up-windows-devices.md) . 
    
3. Po przyłączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik musi ponownie uruchomić swoje urządzenia i zalogować się przy użyciu poświadczeń firmy Microsoft 365 Business. Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych, jak również.
    
Nie dodatkowe kroki są wymagane, aby uzyskać dostęp do zasobów lokalnych dla usługi Azure AD przyłączonych urządzeń. Ta funkcja jest wbudowana w system Windows 10. 

Jeśli masz plany, aby zalogować się do urządzenia AADJ inne niż Metoda Password jak PIN/Bio-Metric poprzez WHFB poświadczeń logowania, a następnie dostęp do zasobów lokalnych (akcje, drukarki.. itp.), należy przestrzegaćhttps://docs.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jeśli organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia przyłączone do usługi Azure AD opisanych powyżej, należy rozważyć skonfigurowanie [konfiguracji urządzenia przyłączone do hybrydowej usługi Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD

Jeśli urządzenie systemu Windows, które dołączyła do usługi Azure AD został wcześniej przyłączony do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:
  
- Gdy urządzenie dołącza do usługi Azure AD, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Profile muszą być migrowane ręcznie. Profil użytkownika zawiera takie informacje, jak Ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień do nowego profilu.

- Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty GPO mogą nie mieć porównywalnego [dostawcy usług konfiguracji (CSP, Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) ) w usłudze Intune. Uruchom [Narzędzie MMat](https://www.microsoft.com/download/details.aspx?id=45520) , aby znaleźć porównywalne dostawcy CSP dla istniejących obiektów zasad grupy.

- Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Oceń starszej wersji aplikacji i rozważ aktualizację do aplikacji, która używa nowoczesnych auth, jeśli to możliwe.

- Odnajdowanie drukarek usługi Active Directory nie będzie działać. Można zapewnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [chmury hybrydowej](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
