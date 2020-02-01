---
title: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business
f1.keywords:
- NOCSH
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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki z usługi Azure Active Directory przyłączonej do urządzenia z systemem Windows 10.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593238"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business

Każde urządzenie z systemem Windows 10, przyłączone do usługi Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje usługi Office 365, i może być chronione przez firmę Microsoft 365 Business. Można również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje biznesowe (LOB), udziały plików i drukarki. Aby zezwolić na dostęp, użyj [usługi Azure AD Connect,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) aby zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory. 

Aby dowiedzieć się więcej, zobacz [Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Kroki są również podsumowane w poniższych sekcjach.

> [!IMPORTANT]
> Ta procedura ma zastosowanie tylko do OAuth i NTLM. Protokół Kerberos nie jest obsługiwany.
 
## <a name="run-azure-ad-connect"></a>Uruchamianie usługi Azure AD Connect

Wykonaj następujące kroki, aby umożliwić urządzeniom przyłączonym do usługi Azure AD dostęp do zasobów lokalnych w organizacji.
  
1. Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom kreatora synchronizacji katalogu i usługę Azure AD Connect zgodnie z opisem w [obszarze Konfigurowanie synchronizacji katalogów dla usługi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są połączone z usługą Azure AD. Ten krok odbywa się indywidualnie na każdym urządzeniu z systemem Windows 10. Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business.](set-up-windows-devices.md) 
    
3. Po przyłączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń usługi Microsoft 365 Business. Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych.
    
Nie są wymagane żadne dodatkowe kroki, aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączonych do usługi Azure AD. Ta funkcja jest wbudowana w system Windows 10. 

Jeśli masz plany, aby zalogować się do urządzenia AADJ innych niż metoda hasła Jak PIN / Bio-metryki za pośrednictwem logowania poświadczeń WHFB, a następnie uzyskać dostęp do zasobów lokalnych (udziały, drukarki.. itp.), należy postępować zgodnie zhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jeśli twoja organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia połączonego z usługą Azure AD opisanej powyżej, rozważ skonfigurowanie [konfiguracji urządzenia przyłączonego do usługi Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Zagadnienia podczas łączenia urządzeń z systemem Windows do usługi Azure AD

Jeśli urządzenie z systemem Windows przyłączone do usługi Azure-AD było wcześniej przyłączone do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:
  
- Gdy urządzenie usługi Azure AD dołącza, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Profile muszą być ręcznie migrowane. Profil użytkownika zawiera informacje, takie jak ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień na nowy profil.

- Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty zasad grupy mogą nie mieć porównywalnego [dostawcy usług konfiguracji](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune. Uruchom [narzędzie MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) aby znaleźć porównywalne usługi CSP dla istniejących obiektów zasad grupy.

- Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnej auth, jeśli to możliwe.

- Odnajdowanie drukarki usługi Active Directory nie będzie działać. Można udostępnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [funkcji Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
