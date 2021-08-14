---
title: Wprowadzenie do usługi Microsoft 365 dla firm
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
description: Dowiedz się Microsoft 365 dla firm, jak ją skonfigurować i jak przygotować urządzenia i komputery, aby zapewnić ich ochronę przez usługę Microsoft 365 dla firm.
ms.openlocfilehash: 3ac8ec3c831d14cfa6d0018340458b2b494b2dd746a7f2bd61d2eba0b4eaf0a1
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837908"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Wprowadzenie do usługi Microsoft 365 dla firm

## <a name="what-is-microsoft-365-for-business"></a>Co to Microsoft 365 dla firm

Program Microsoft 365 dla firm to kompleksowy zestaw zawsze aktualnych produktów firmy i narzędzi do współpracy, takich jak Outlook, Word, Excel i inne produkty firmy Office. Możesz chronić swoje pliki służbowe na wszystkich urządzeniach z systemami iOS, Android Windows 10, dzięki łatwym w zarządzaniu poziomem zabezpieczeń klasy korporacyjnej.

## <a name="watch-what-is-microsoft-365-business-premium"></a>Obejrzyj: Co to jest usługa Microsoft 365 Business Premium

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 dla firm jest przeznaczona dla maksymalnie 300 licencji. Jeśli potrzebujesz większej liczby licencji, zapoznaj się z dokumentacją usługi [Microsoft 365 Enterprise](../enterprise/index.yml), aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-for-business"></a>Pobierz Microsoft 365 dla firm

- Jeśli masz partnera, uzyskają oni usługę Microsoft 365 dla firm: Uzyskiwanie Microsoft 365 dla firm [z Centrum partnerskiego firmy Microsoft.](get-microsoft-365-business.md)
    
- Jeśli nie masz partnera i chcesz uzyskać usługę Microsoft 365 dla firm, możesz [kupić ją tutaj.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurowanie usługi Microsoft 365 dla firm

 **Omówienie Microsoft 365 usługi dla firm**
  
Na poniższym diagramie opisano sposób, w jaki administratorzy Microsoft 365 dla firm. Opisano w nim również czynności, które należy wykonać Windows komputerów PC do Microsoft 365 dla firm. Nowe urządzenia można także dodawać w programie centrum administracyjne platformy Microsoft 365 za pomocą rozwiązania [Windows AutoPilot.](add-autopilot-devices-and-profile.md) Rozwiązania AutoPilot możesz użyć do skonfigurowania i wstępnego skonfigurowania nowych urządzeń, aby były gotowe do użycia w produktywnej pracy od razu po kilku logowaniach się użytkowników przy użyciu poświadczeń Microsoft 365 dla firm.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

## <a name="watch-set-up-microsoft-365-business"></a>Obejrzyj: Konfigurowanie usługi Microsoft 365 Firm

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](../business-video/index.yml).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1. Konfigurowanie usługi Microsoft 365 dla firm (administrator)

Zaloguj się [centrum administracyjne platformy Microsoft 365](https://admin.microsoft.com/adminportal/home) poświadczeniami administratora globalnego i wykonaj poniższe czynności, aby skonfigurować usługę Microsoft 365 dla firm. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach za pomocą Microsoft 365 dla firm](pre-requisites-for-data-protection.md)
    
    Przeczytaj wymagania wstępne, aby upewnić się, że Twoje urządzenia są gotowe do Microsoft 365 dla firm.
    
2. [Konfigurowanie usługi Microsoft 365 dla firm przy użyciu kreatora konfiguracji](set-up.md)
    
    Jeśli na stałe przenosisz się z lokalnej usługi **Active Directory** do chmury, możesz przejść do usługi centrum administracyjne platformy Microsoft 365 i ręcznie dodać użytkowników za pomocą kreatora konfiguracji lub wykonać synchronizację ręczną z usługą Azure AD Połączenie. Istnieją dwa sposoby wykonywania tej czynności: 
    
    - Jeśli masz również serwer programu Exchange 2010, Exchange 2013 lub Exchange 2016, możesz użyć minimalnej konfiguracji hybrydowej, aby szybko przeprowadzić migrację skrzynek pocztowych programu Exchange do programu [Microsoft 365.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Czynności w ramach minimalnej synchronizacji hybrydowej obejmują synchronizuj razową synchronizację użytkowników z usługą Azure AD oraz migrację poczty e-mail ze środowiska lokalnego do chmury. W przypadku użycia tej metody synchronizacja katalogów zostanie automatycznie wyłączona po zakończeniu migracji poczty e-mail.
    
    - Za pomocą kreatora synchronizacji katalogów zsynchronizuj konta użytkowników z chmurą. Aby ukończyć ten [proces,](../enterprise/set-up-directory-synchronization.md) wykonaj Microsoft 365 konfigurowanie synchronizacji katalogów. Po zsynchronizowaniu użytkowników z chmurą musisz wyłączyć synchronizację katalogów dla usługi [Microsoft 365.](../enterprise/turn-off-directory-synchronization.md)
    
    Ponadto musisz nadać każdemu użytkownikowi, który został dodany w ten sposób, licencję na usługę Microsoft 365 dla firm. Możesz to zrobić za pomocą kreatora [konfiguracji](set-up.md) lub możesz przypisać [licencje użytkownikom.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2. Przygotowanie urządzeń przenośnych

Postępuj zgodnie z instrukcjami w tece Konfigurowanie urządzeń przenośnych dla użytkowników usługi [Microsoft 365](set-up-mobile-devices.md) dla firm, aby instalować aplikacje pakietu Office na urządzeniach i upewniać się, że są one chronione przez usługę Microsoft 365 dla firm. 
  
### <a name="3-prepare-pcs"></a>3. Przygotowywanie komputerów

Administratorzy mogą wstępnie wybrać ustawienia dla nowych komputerów Windows 10 PC za pomocą rozwiązania [Windows AutoPilot.](add-autopilot-devices-and-profile.md) Użytkownicy mogą skonfigurować swoje istniejące lub nowe urządzenia Windows 10, korzystając z procedury opisanej w tym temacie: Konfigurowanie komputerów Windows pc dla użytkowników Microsoft 365 [firm.](set-up-windows-devices.md) W przypadku istniejących urządzeń użytkownicy **mogą** [opcjonalnie przenosić pliki do OneDrive dla Firm.](move-files-to-onedrive.md) Mogą oni również używać narzędzi innych firm, aby przenosić pliki skojarzone z profilem Windows, aby OneDrive.
  
Jeśli Twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, możesz skonfigurować usługę Microsoft 365 dla firm do ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego. Postępuj zgodnie z instrukcjami w włączanie zarządzania przez Windows 10 [przyłączone](manage-windows-devices.md) do domeny przez usługę Microsoft 365 dla firm w celu skonfigurowania tej funkcji. Ta metoda jest preferowana, a urządzenia w tym stanie mają nazwę Urządzenia sprzężenia **hybrydowego usługi Azure AD.** 
  
Jeśli zachowasz lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udzielić swoim urządzeniu przyłączony do usługi **Azure AD** dostępu do tych zasobów, korzystając z procedury opisanej tutaj: Uzyskiwanie dostępu do zasobów lokalnych z urządzenia połączonego z usługą Azure AD w programie Microsoft 365 [dla firm.](access-resources.md)
  
  
## <a name="contact-support"></a>Kontakt z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator Microsoft 365 dla firm masz dostęp do naszego zespołu obsługi klienta: Kontaktowanie się z pomocą techniczną dla produktów biznesowych **[— Pomoc dla administratorów](../business-video/get-help-support.md)**
    
## <a name="related-content"></a>Zawartość pokrewna

[Microsoft 365 i zasoby dla firm](./index.yml) (strona linku)\
[Zarządzanie Microsoft 365 dla firm](manage.md) (artykuł)\
[Migrowanie do Microsoft 365 dla firm](migrate-to-microsoft-365-business.md) (artykuł)\
[Microsoft 365 szkoleniowe klipy wideo dla firm](../business-video/index.yml) (strona linku)