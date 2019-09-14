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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dowiedz się, jak uzyskać dostęp do zasobów lokalnych, takich jak aplikacje linii biznesowych, udziałów plików i drukarek z usługi Azure Active Directory przyłączony do systemu Windows 10 urządzenia.
ms.openlocfilehash: ab9049e78617372463b8446dc8f8bc0089d8c117
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2019
ms.locfileid: "36981666"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Dostęp do zasobów lokalnych z urządzenia przyłączone do usługi Azure AD w Microsoft 365 Business

Wszystkie urządzenia z systemem Windows 10, które są przyłączone do usługi Azure Active Directory, będą miały dostęp do wszystkich zasobów opartych na chmurze, takich jak aplikacje pakietu Office 365 i mogą być chronione przez firmę Microsoft 365 Business. Aby również zezwolić na dostęp do zasobów lokalnych, takich jak aplikacje linii biznesowych (LOB), udziałów plików i drukarek, należy zsynchronizować lokalną usługę Active Directory z usługą Azure Active Directory przy użyciu programu [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). Następujące wideo szczegóły kroki dotyczące sposobu ustawiania tego w najbardziej typowym scenariuszu.
 
> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]

Zobacz [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) , aby dowiedzieć się więcej.
Kroki są również podsumowane w poniższych sekcjach.

## <a name="run-azure-ad-connect"></a>Uruchom program Azure AD Connect

Wykonaj następujące kroki, aby włączyć urządzenia przyłączone do usługi Azure AD w organizacji dostępu do zasobów lokalnych.
  
1. Aby zsynchronizować użytkowników, grup i kontaktów z lokalnej usługi Active Directory w usłudze Azure Active Directory, uruchom Kreatora synchronizacji katalogów i Azure AD Connect zgodnie z opisem w [Konfigurowanie synchronizacji katalogów dla pakietu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po zakończeniu synchronizacji katalogów upewnij się, że urządzenia z systemem Windows 10 w organizacji są przyłączone do usługi Azure AD. Ten krok jest wykonywana indywidualnie na każdym urządzeniu z systemem Windows 10. Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników Microsoft 365 Business](set-up-windows-devices.md) . 
    
3. Po przyłączeniu urządzeń z systemem Windows 10 do usługi Azure AD każdy użytkownik powinien ponownie uruchomić swoje urządzenia i zalogować się przy użyciu poświadczeń firmy Microsoft 365 Business. Wszystkie urządzenia będą teraz mieć dostęp do zasobów lokalnych, jak również.
    
Nie dodatkowe kroki są wymagane, aby uzyskać dostęp do zasobów lokalnych dla usługi Azure AD przyłączonych urządzeń. Jest to wbudowana funkcja dostępna w systemie Windows 10. 
  
Jeśli organizacja nie jest gotowa do wdrożenia w konfiguracji urządzenia przyłączone do usługi Azure AD opisanych powyżej, należy rozważyć skonfigurowanie [konfiguracji urządzenia przyłączone do hybrydowej usługi Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Zagadnienia dotyczące dołączania urządzeń z systemem Windows do usługi Azure AD

Jeśli usługi Azure AD przyłączanie urządzenia systemu Windows, który wcześniej został przyłączony do domeny lub w grupie roboczej, należy wziąć pod uwagę następujące ograniczenia:
  
- Gdy urządzenie dołącza do usługi Azure AD, tworzy nowego użytkownika bez odwoływania się do istniejącego profilu. Aby rozwiązać ten problem, profile muszą być migrowane ręcznie. Profil użytkownika zawiera takie informacje, jak Ulubione, pliki lokalne, ustawienia przeglądarki, ustawienia menu Start itp. Najlepszym rozwiązaniem jest znalezienie narzędzia innej firmy do mapowania istniejących plików i ustawień do nowego profilu

- Jeśli urządzenie korzysta z obiektów zasad grupy (GPO), niektóre obiekty GPO mogą nie mieć porównywalnego [dostawcy usług konfiguracji (CSP, Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) ) w usłudze Intune. Uruchom [Narzędzie MMat](https://www.microsoft.com/download/details.aspx?id=45520) , aby znaleźć porównywalne dostawcy CSP dla istniejących obiektów zasad grupy.

- Użytkownicy nie będą mogli uwierzytelniać się w aplikacjach zależnych od uwierzytelniania usługi Active Directory. Aby poradzić sobie z tym ocenić za pomocą starszej wersji aplikacji i rozważyć aktualizację do aplikacji, która korzysta z nowoczesnych auth, jeśli to możliwe.

- Odnajdowanie drukarek usługi Active Directory nie będzie działać. Aby rozwiązać ten problem, należy zapewnić bezpośrednie ścieżki drukarki dla wszystkich użytkowników lub wykorzystać [hybrydowy Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
