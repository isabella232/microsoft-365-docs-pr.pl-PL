---
title: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 Business
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
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak linia aplikacji biznesowych, udziały plików i drukarki z urządzenia usługi Azure Active Directory połączonego z systemem Windows 10.
ms.openlocfilehash: 22edf0c23d6318e1f70bcb21b2cd697ea0a75da4
ms.sourcegitcommit: 849b365bd3eaa9f3c3a9ef9f5973ef81af9156fa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/16/2020
ms.locfileid: "49688238"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 Business Premium

Ten artykuł dotyczy programu Microsoft 365 Business Premium.

Wszystkie urządzenia z systemem Windows 10, które są połączone z usługą Azure Active Directory, mają dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje Microsoft 365, i mogą być chronione przez firmę Microsoft 365 Business Premium. Możesz również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje LOB, udziały plików i drukarki. Aby zezwolić na dostęp, użyj funkcji [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) w celu zsynchronizowania lokalnej usługi Active Directory z usługą Azure Active Directory. 

Aby dowiedzieć się więcej, zobacz [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Instrukcje te zostały również podsumowane w poniższych sekcjach.
 
## <a name="run-azure-ad-connect"></a>Uruchamianie usługi Azure AD Connect

Wykonaj poniższe czynności, aby włączyć dostęp do zasobów lokalnych w Twojej organizacji z dołączonymi urządzeniami usługi Azure AD.
  
1. Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, uruchom Kreatora synchronizacji katalogów i usługi Azure AD Connect zgodnie z opisem w obszarze [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że na urządzeniach z systemem Windows 10 organizacji jest przyłączony system Azure AD. Ten krok należy przeprowadzić indywidualnie na każdym urządzeniu z systemem Windows 10. Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla programu Microsoft 365 Business Premium](set-up-windows-devices.md) . 
    
3. Po przełączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik musi ponownie uruchomić urządzenia i zalogować się przy użyciu poświadczeń programu Microsoft 365 Business Premium. Wszystkie urządzenia mają teraz dostęp do zasobów lokalnych.
    
Aby uzyskać dostęp do zasobów lokalnych dla przyłączonych urządzeń Azure AD, nie są wymagane żadne dodatkowe czynności. Ta funkcja jest wbudowana w systemie Windows 10. 

Jeśli masz plan logowania na urządzeniu AADJ innym niż Metoda Password, taką jak PIN/Bio-Metric za pomocą WHFB poświadczenia logowania, a następnie uzyskujesz dostęp do zasobów lokalnymi (udziałów, drukarek. itd.), wykonaj https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jeśli Twoja organizacja nie jest gotowa do wdrożenia w opisanej powyżej konfiguracji urządzenia połączonego z usługą Azure AD, spróbuj skonfigurować [konfigurację hybrydowego urządzenia z usługą Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD

Jeśli urządzenie z systemem Windows, na którym znajduje się usługa Azure-AD, była już przyłączone do domeny lub w grupie roboczej, należy uwzględnić następujące ograniczenia:
  
- Po dołączeniu do usługi Azure AD program tworzy nowego użytkownika bez odwołania do istniejącego profilu. Profile należy poddać ręcznej migracji. Profil użytkownika zawiera informacje, takie jak Ulubione, lokalne pliki, ustawienia przeglądarki i ustawienia menu Start. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy służącego do mapowania istniejących plików i ustawień na nowy profil.

- Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty GPO mogą nie mieć porównywalnego [dostawcy usług konfiguracji](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) w usłudze Intune. Uruchom [Narzędzie MMAT](https://www.microsoft.com/download/details.aspx?id=45520) , aby znaleźć porównywalnych dostawców CSP dla istniejących obiektów zasad grupy.

- Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Oceń starszą aplikację i spróbuj zaktualizować aplikację, która korzysta z nowoczesnego uwierzytelniania, jeśli to możliwe.

- Odnajdowanie drukarek w usłudze Active Directory nie będzie działać. Możesz udostępnić bezpośrednie ścieżki drukarki wszystkim użytkownikom lub użyć [uniwersalnego wydruku](https://aka.ms/UPDocs).
