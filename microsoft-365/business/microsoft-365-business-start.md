---
title: Wprowadzenie do platformy Microsoft 365 dla firm
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Poznaj platformę Microsoft 365 dla firm, dowiedz się, jak ją skonfigurować i jak przygotować urządzenia i komputery użytkowników do zapewnienia ich ochrony za pomocą platformy Microsoft 365 dla firm.
ms.openlocfilehash: 83bd2ff87683c1ad810d20658ba20f3229408968
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580099"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Wprowadzenie do platformy Microsoft 365 dla firm

## <a name="what-is-microsoft-365-for-business"></a>Co to jest usługa Microsoft 365 dla firm

Usługa Microsoft 365 dla firm to kompleksowy zestaw zawsze aktualnych produktów pakietu Office, takich jak Outlook, Word, Excel i inne narzędzia do współpracy biznesowej, takie jak Outlook, Word i Excel. Możesz chronić swoje pliki na wszystkich urządzeniach z systemami iOS, Android i Windows 10, dzięki łatwym w zarządzaniu zabezpieczeniam klasy korporacyjnej.

Ten klip wideo zawiera krótkie omówienie platformy Microsoft 365 dla firm.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Usługa Microsoft 365 dla firm jest przeznaczona dla maksymalnie 300 licencji. Jeśli potrzebujesz większej liczby licencji, zapoznaj się z dokumentacją usługi [Microsoft 365 Enterprise](../enterprise/index.yml), aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-for-business"></a>Uzyskaj platformę Microsoft 365 dla firm

- Partner otrzyma platformę Microsoft 365 dla firm: Uzyskaj platformę [Microsoft 365 dla](get-microsoft-365-business.md)firm z Centrum partnerskiego firmy Microsoft.
    
- Jeśli nie masz partnera i chcesz uzyskać platformę Microsoft 365 dla firm, możesz [kupić ją tutaj.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurowanie platformy Microsoft 365 dla firm

 **Omówienie usługi Microsoft 365 dla firm — konfigurowanie pakietu**
  
Na poniższym diagramie opisano sposób skonfigurowania platformy Microsoft 365 dla firm przez administratorów. Opisano w nim również czynności, jakie należy wykonać w celu przygotowania komputerów z systemem Windows do platformy Microsoft 365 dla firm. Nowe urządzenia możesz również dodać za pomocą rozwiązania [Windows AutoPilot](add-autopilot-devices-and-profile.md)w centrum administracyjnym platformy Microsoft 365. Rozwiązania AutoPilot możesz użyć do skonfigurowania i wstępnego skonfigurowania nowych urządzeń, aby były gotowe do użycia w produktywnej pracy od razu po kilku logowaniach się użytkowników przy użyciu poświadczeń platformy Microsoft 365 dla firm.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ten klip wideo zawiera omówienie konfigurowania platformy Microsoft 365 dla firm.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1. Konfigurowanie platformy Microsoft 365 dla firm (administrator)

Zaloguj się do [centrum administracyjnego platformy Microsoft 365](https://portal.office.com/adminportal/home) za pomocą poświadczeń administratora globalnego i wykonaj poniższe czynności, aby skonfigurować platformę Microsoft 365 dla firm. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach przy użyciu platformy Microsoft 365 dla firm](pre-requisites-for-data-protection.md)
    
    Przeczytaj wymagania wstępne, aby upewnić się, że Twoje urządzenia są gotowe do użycia platformy Microsoft 365 dla firm.
    
2. [Konfigurowanie platformy Microsoft 365 dla firm przy użyciu kreatora konfiguracji](set-up.md)
    
    Jeśli na stałe przenosisz się z lokalnej usługi **Active Directory** do chmury, możesz przejść do centrum administracyjnego platformy Microsoft 365 i ręcznie dodać użytkowników za pomocą kreatora konfiguracji lub wykonać synchronizację ręczną za pomocą programu Azure AD Connect. Istnieją dwa sposoby wykonywania tej czynności: 
    
    - Jeśli masz również serwer programu Exchange 2010, Exchange 2013 lub Exchange 2016, możesz użyć minimalnej konfiguracji hybrydowej, aby szybko przeprowadzić migrację skrzynek pocztowych programu Exchange do platformy [Microsoft 365.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Czynności w ramach minimalnej synchronizacji hybrydowej obejmują synchronizuj razową synchronizację użytkowników z usługą Azure AD oraz migrację poczty e-mail ze środowiska lokalnego do chmury. W przypadku użycia tej metody synchronizacja katalogów zostanie automatycznie wyłączona po zakończeniu migracji poczty e-mail.
    
    - Za pomocą kreatora synchronizacji katalogów zsynchronizuj konta użytkowników z chmurą. Aby ukończyć ten proces, wykonaj czynności opisane w tece Konfigurowanie synchronizacji katalogów dla platformy [Microsoft 365.](../enterprise/set-up-directory-synchronization.md) Po zsynchronizowaniu użytkowników z chmurą musisz wyłączyć synchronizację katalogów na platformie [Microsoft 365.](../enterprise/turn-off-directory-synchronization.md)
    
    Ponadto musisz nadać każdemu użytkownikowi, który został dodany w ten sposób, licencję na platformę Microsoft 365 dla firm. Możesz to zrobić za pomocą kreatora [konfiguracji](set-up.md) lub możesz przypisać [licencje użytkownikom.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2. Przygotowanie urządzeń przenośnych

Postępuj zgodnie z instrukcjami w tece Konfigurowanie urządzeń przenośnych dla użytkowników platformy [Microsoft 365](set-up-mobile-devices.md) dla firm, aby zainstalować aplikacje pakietu Office na urządzeniach i upewnić się, że są chronione przez usługę Microsoft 365 dla firm. 
  
### <a name="3-prepare-pcs"></a>3. Przygotowywanie komputerów

Administratorzy mogą wstępnie wybrać ustawienia nowych komputerów z systemem Windows 10 za pomocą rozwiązania [Windows AutoPilot.](add-autopilot-devices-and-profile.md) Użytkownicy mogą skonfigurować swoje istniejące lub nowe urządzenia z systemem Windows 10, korzystając z procedury opisanej w tym temacie: Konfigurowanie komputerów PC z systemem Windows dla użytkowników usługi [Microsoft 365 dla firm.](set-up-windows-devices.md) W przypadku istniejących urządzeń użytkownicy **mogą** [opcjonalnie przenosić pliki do usługi OneDrive dla Firm.](move-files-to-onedrive.md) Mogą oni również używać narzędzi innych firm, aby przenosić pliki skojarzone z profilem systemu Windows do usługi OneDrive.
  
Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 dla firm w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego. Wykonaj czynności opisane w tece Włączanie zarządzania przez platformę [Microsoft 365](manage-windows-devices.md) dla firm dla urządzeń przyłączanych do domeny systemu Windows 10 w celu skonfigurowania tej funkcji. Ta metoda jest preferowana, a urządzenia w tym stanie mają nazwę Urządzenia sprzężenia **hybrydowego usługi Azure AD.** 
  
Jeśli zachowasz lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udzielić swoim urządzeniu przyłączanych do usługi **Azure AD** dostępu do tych zasobów, korzystając z procedury opisanej tutaj: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD na platformie [Microsoft 365 dla firm.](access-resources.md)
  
  
## <a name="contact-support"></a>Kontakt z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator platformy Microsoft 365 dla firm masz dostęp do naszego zespołu obsługi klienta: Kontaktowanie się z pomocą techniczną dla produktów biznesowych **[— Pomoc dla administratorów](../admin/contact-support-for-business-products.md)**
    
## <a name="see-also"></a>Zobacz też

[Dokumentacja i zasoby dotyczące platformy Microsoft 365 dla firm](./index.yml)
  
[Zarządzanie usługą Microsoft 365 dla firm](manage.md)[Migrowanie do platformy Microsoft 365 dla firm](migrate-to-microsoft-365-business.md)

[Szkoleniowe klipy wideo dotyczące platformy Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)