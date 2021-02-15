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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki, z urządzenia z systemem Windows 10, do których dołączyć do usługi Azure Active Directory.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233845"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business Premium

Ten artykuł dotyczy usługi Microsoft 365 Business Premium.

Każde urządzenie z systemem Windows 10, do których dołączyć usługa Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje platformy Microsoft 365, i może być chronione przez usługę Microsoft 365 Business Premium. Możesz również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje biznesowe (LOB), udziały plików i drukarki. Aby zezwolić na dostęp, użyj programu [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) w celu zsynchronizowania lokalnej usługi Active Directory z usługą Azure Active Directory. 

Aby dowiedzieć się więcej, [zobacz Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
Kroki podsumowywane są również w poniższych sekcjach.
 
## <a name="run-azure-ad-connect"></a>Uruchamianie programu Azure AD Connect

Wykonaj poniższe czynności, aby umożliwić urządzeniu przyłączone do usługi Azure AD Twojej organizacji dostęp do zasobów lokalnych.
  
1. Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom kreatora synchronizacji katalogów i narzędzie Azure AD Connect zgodnie z opisem w tece Konfigurowanie synchronizacji katalogów dla usługi [Office 365.](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia organizacji z systemem Windows 10 są połączone z usługą Azure AD. Ten krok jest wykonywane osobno na każdym urządzeniu z systemem Windows 10. Aby uzyskać szczegółowe informacje, zobacz "Konfigurowanie urządzeń [z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium".](set-up-windows-devices.md) 
    
3. Po dołączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń usługi Microsoft 365 Business Premium. Wszystkie urządzenia mają teraz również dostęp do zasobów lokalnych.
    
Aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłącznych do usługi Azure AD, nie są wymagane żadne dodatkowe kroki. Ta funkcja jest wbudowana w system Windows 10. 

Jeśli planujesz zalogowanie się do urządzenia AADJ inną niż metoda hasła, na przykład numer PIN/metryka biometrycznych za pośrednictwem logowania poświadczeń WHFB, a następnie dostęp do zasobów lokalnych (udziałów,drukarek). itp.), postępuj zgodnie z https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jeśli Twoja organizacja nie jest jeszcze gotowa do wdrożenia w opisanej powyżej konfiguracji urządzenia połączonego z usługą Azure AD, rozważ skonfigurowanie konfiguracji urządzenia połączonego z usługą [Azure AD.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD

Jeśli urządzenie z systemem Windows, do których dołączyła usługa Azure-AD, było wcześniej przyłączone do domeny lub w grupie roboczej, rozważ następujące ograniczenia:
  
- Po dołączeniu urządzenia do usługi Azure AD tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Profile należy migrować ręcznie. Profil użytkownika zawiera informacje, takie jak ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień na nowy profil.

- Jeśli urządzenie korzysta z obiektów zasady grupy (GPO), niektóre obiekty GPO mogą nie mieć w usłudze Intune [porównywalnego](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) dostawcy usług konfiguracji (CSP). Uruchom narzędzie [MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) aby znaleźć porównywalną csP dla istniejących zasad GPO.

- Użytkownicy mogą nie być w stanie uwierzytelnić się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Oceń starszą aplikację i rozważ aktualizację do aplikacji, która korzysta z nowoczesnego uwierzytelniania, jeśli to możliwe.

- Odnajdowanie drukarek usługi Active Directory nie będzie działać. Możesz udostępnić bezpośrednie ścieżki drukarek wszystkim użytkownikom lub użyć [drukowania uniwersalnego.](https://aka.ms/UPDocs)
