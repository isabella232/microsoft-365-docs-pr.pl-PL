---
title: Dostęp do zasobów lokalnych z urządzenia przyłączanego do usługi Azure AD w usłudze Microsoft 365 Business
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki z usługi Azure Active Directory przyłączone do urządzenia z systemem Windows 10.
ms.openlocfilehash: 9615ecc9469992d3e5a7479f4799c610db11fb41
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471256"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Dostęp do zasobów lokalnych z urządzenia przyłączanego do usługi Azure AD w usłudze Microsoft 365 Business Premium

Ten artykuł dotyczy usługi Microsoft 365 Business Premium.

Każde urządzenie z systemem Windows 10, do którego dołączona jest usługa Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje usługi Microsoft 365, i może być chronione przez usługę Microsoft 365 Business Premium. Można również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje biznesowe (LOB), udziały plików i drukarki. Aby zezwolić na dostęp, użyj [usługi Azure AD Connect,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) aby zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory. 

Aby dowiedzieć się więcej, zobacz [Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Kroki są również podsumowane w poniższych sekcjach.

> [!IMPORTANT]
> Ta procedura ma zastosowanie tylko do OAuth i NTLM. Protokół Kerberos nie jest obsługiwany.
 
## <a name="run-azure-ad-connect"></a>Uruchamianie usługi Azure AD Connect

Wykonaj następujące kroki, aby umożliwić urządzeniom przyłączanym do usługi Azure AD w organizacji dostęp do zasobów lokalnych.
  
1. Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom Kreatora synchronizacji katalogów i usługi Azure AD Connect zgodnie z opisem w [obszarze Konfigurowanie synchronizacji katalogów dla usługi Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są przyłączone do usługi Azure AD. Ten krok jest wykonywany indywidualnie na każdym urządzeniu z systemem Windows 10. Szczegółowe informacje można znaleźć w witrynie [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
3. Gdy urządzenia z systemem Windows 10 są przyłączone do usługi Azure AD, każdy użytkownik musi ponownie uruchomić swoje urządzenia i zalogować się przy użyciu poświadczeń usługi Microsoft 365 Business Premium. Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych, jak również.
    
Żadne dodatkowe kroki nie są wymagane, aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączonych do usługi Azure AD. Ta funkcja jest wbudowana w system Windows 10. 

Jeśli masz plany logowania się do urządzenia AADJ inne niż metoda hasła, takie jak PIN/Bio-metryka za pośrednictwem logowania poświadczeń WHFB, a następnie dostęp do zasobów lokalnych (udziały,drukarki.. itp.), należy postępować zgodnie zhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jeśli twoja organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia przyłączanym do usługi Azure AD, opisana powyżej, należy rozważyć skonfigurowanie [konfiguracji urządzenia przyłączone do usługi Azure AD.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD

Jeśli urządzenie z systemem Windows, do którego przyłączono usługę Azure-AD, było wcześniej przyłączone do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:
  
- Gdy urządzenie usługi Azure AD sprzężenia, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Profile muszą być migrowane ręcznie. Profil użytkownika zawiera informacje, takie jak ulubione pliki, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień do nowego profilu.

- Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty zasad grupy mogą nie mieć porównywalnego [dostawcy usług konfiguracji](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune. Uruchom [narzędzie MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) aby znaleźć porównywalne dostawcy usług internetowych dla istniejących zasad grupy.

- Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnej eru, jeśli to możliwe.

- Odnajdowanie drukarek usługi Active Directory nie będzie działać. Można zapewnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [hybrid cloud print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
