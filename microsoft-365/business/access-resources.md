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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje biznesowe, udziały plików i drukarki, z urządzenia z systemem Windows 10, do których dołączyć usługa Azure Active Directory.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445353"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w usłudze Microsoft 365 Business Premium

Ten artykuł dotyczy usługi Microsoft 365 Business Premium.

Każde urządzenie z systemem Windows 10, do których dołączyć jest usługa Azure Active Directory, ma dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje platformy Microsoft 365, i może być chronione przez usługę Microsoft 365 Business Premium. Możesz również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje firmowe (LOB), udziały plików i drukarki. Aby zezwolić na dostęp, użyj programu [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) do zsynchronizowania lokalnej usługi Active Directory z usługą Azure Active Directory. 

Aby dowiedzieć się więcej, [zobacz Wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory.](/azure/active-directory/device-management-introduction)
Kroki te zostały również podsumowane w poniższych sekcjach.
 
## <a name="run-azure-ad-connect"></a>Uruchamianie programu Azure AD Connect

Wykonaj poniższe czynności, aby umożliwić organizacji urządzenia przyłączone do usługi Azure AD w celu uzyskiwania dostępu do zasobów lokalnych.
  
1. Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom kreatora synchronizacji katalogów i programu Azure AD Connect zgodnie z opisem w tesłudze Konfigurowanie synchronizacji katalogów dla usługi [Office 365.](../enterprise/set-up-directory-synchronization.md)
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia Organizacji z systemem Windows 10 są przyłączone do usługi Azure AD. Ten krok jest wykonywane pojedynczo na każdym urządzeniu z systemem Windows 10. Aby uzyskać szczegółowe informacje, zobacz Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi [Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
3. Gdy urządzenia z systemem Windows 10 dołączą do usługi Azure AD, każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń platformy Microsoft 365 Business Premium. Wszystkie urządzenia mają teraz również dostęp do zasobów lokalnych.
    
Aby uzyskać dostęp do zasobów lokalnych dla urządzeń przyłączony do usługi Azure AD, nie są wymagane żadne dodatkowe czynności. Ta funkcja jest wbudowana w system Windows 10. 

Jeśli planujesz zalogować się do urządzenia AADJ inną niż metoda haseł Like PIN/Bio-metric za pośrednictwem logowania poświadczeń WHFB, a następnie uzyskać dostęp do zasobów lokalnych (udziałów,drukarek). itp.), postępuj zgodnie z https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jeśli Twoja organizacja nie jest jeszcze gotowa do wdrożenia w opisanej powyżej konfiguracji urządzenia połączonego z usługą Azure AD, rozważ skonfigurowanie hybrydowej konfiguracji urządzenia przyłączonego do usługi [Azure AD.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD

Jeśli urządzenie z systemem Windows, do których dodano usługę Azure-AD, było wcześniej przyłączone do domeny lub w grupie roboczej, rozważ następujące ograniczenia:
  
- Gdy urządzenie dołącza do usługi Azure AD, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Profile należy migrować ręcznie. Profil użytkownika zawiera informacje, takie jak ulubione, pliki lokalne, ustawienia przeglądarki i ustawienia menu Start. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień na nowy profil.

- Jeśli urządzenie używa obiektów zasady grupy (GPO), niektóre obiekty GPOs [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) mogą nie mieć porównywalnego dostawcy usług konfiguracji (CSP) w usłudze Intune. Uruchom narzędzie [MMAT, aby](https://www.microsoft.com/download/details.aspx?id=45520) znaleźć porównywalne pliki CSP dla istniejących gpOs.

- Użytkownicy mogą nie być w stanie uwierzytelnić się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Oceń starszą aplikację i rozważ aktualizację do aplikacji, która używa nowoczesnego uwierzytelniania, jeśli to możliwe.

- Odnajdowanie drukarek usługi Active Directory nie będzie działać. Możesz udostępnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub użyć [drukowania uniwersalnego.](/universal-print/)

### <a name="related-articles"></a>Artykuły pokrewne

[Wymagania wstępne programu Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
