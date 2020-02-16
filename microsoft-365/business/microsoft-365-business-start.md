---
title: Rozpoczynanie pracy z usługą Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Dowiedz się, jak skonfigurować usługę Microsoft 365 Business.
ms.openlocfilehash: 5491486c2bf8da1ee38fcd986d5ecd682d57c82e
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065621"
---
# <a name="get-started-with-microsoft-365-business"></a>Rozpoczynanie pracy z usługą Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co to jest usługa Microsoft 365 Business

Microsoft 365 Business to kompleksowy zestaw narzędzi do pracy i współpracy, takich jak Outlook, Word, Excel i inne produkty pakietu Office, które są zawsze aktualne. Pliki robocze można chronić na wszystkich urządzeniach z systemami iOS, Android i Windows 10 za pomocą zabezpieczeń klasy korporacyjnej, które są łatwe w zarządzaniu.

Ten klip wideo zawiera krótki przegląd usługi Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Usługa Microsoft 365 Business jest przeznaczona dla maksymalnie 300 licencji. Jeśli potrzebujesz więcej licencji, zobacz dokumentację [programu Microsoft 365 Enterprise,](https://go.microsoft.com/fwlink/p/?linkid=860986) aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-business"></a>Uzyskiwanie usługi Microsoft 365 Business

- Jeśli masz partnera, otrzymają oni usługę Microsoft 365 Business: [Pobierz usługę Microsoft 365 Business z Centrum partnerów firmy Microsoft](get-microsoft-365-business.md).
    
- Jeśli nie masz partnera i chcesz uzyskać usługę Microsoft 365 Business, możesz [kupić ją tutaj](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Konfigurowanie usługi Microsoft 365 Business

 **Omówienie konfiguracji pakietu Microsoft 365 Business Suite**
  
Na poniższym diagramie opisano sposób konfigurowania przez administratorów usługi Microsoft 365 Business. Zawiera on także instrukcje dotyczące przygotowania komputerów z systemem Windows do współdziałania z usługą Microsoft 365 Business. Możesz również dodać nowe urządzenia w centrum administracyjnym programu Microsoft 365 Business za pomocą [programu Windows AutoPilot](add-autopilot-devices-and-profile.md). Za pomocą programu AutoPilot można skonfigurować i wstępnie skonfigurować nowe urządzenia, tak aby były gotowe do produktywnego użytku, gdy tylko użytkownik zaloguje się przy użyciu swoich poświadczeń microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ten klip wideo zawiera omówienie konfiguracji usługi Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Konfigurowanie usługi Microsoft 365 Business (administrator)

Zaloguj się do [centrum administracyjnego firmy Microsoft 365 Business](https://portal.office.com/adminportal/home) przy użyciu globalnych poświadczeń administratora i wykonaj następujące kroki, aby skonfigurować usługę Microsoft 365 Business. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach z programem Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Najpierw przeczytaj wymagania wstępne, aby upewnić się, że urządzenia są gotowe do pracy w usłudze Microsoft 365 Business.
    
2. [Konfigurowanie programu Microsoft 365 Business za pomocą kreatora konfiguracji](set-up.md)
    
    Jeśli na **stałe przechodzisz z lokalnej usługi Active Directory do chmury,** możesz przejść do centrum administracyjnego usługi Microsoft 365 Business i użyć kreatora konfiguracji, aby ręcznie dodać użytkowników lub przeprowadzić jednorazową synchronizację z usługą Azure AD Connect. Istnieją dwa sposoby wykonywania tej czynności: 
    
    - Jeśli masz również serwer programu Exchange 2010, Exchange 2013 lub Exchange 2016, możesz [użyć minimum hybrydowego, aby szybko przeprowadzić migrację skrzynek pocztowych programu Exchange do usługi Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Minimalne kroki hybrydowe obejmują jednorazową synchronizację użytkowników z usługą Azure AD i migrację poczty e-mail z lokalnego do chmury. Po zakończeniu migracji poczty e-mail synchronizacja katalogów jest automatycznie wyłączana podczas korzystania z tej metody.
    
    - Użyj kreatora synchronizacji katalogów usługi Office 365, aby zsynchronizować użytkowników z chmurą. Aby przeprowadzić tę operację, wykonaj czynności opisane w artykule [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po zsynchronizowaniu użytkowników z chmurą musisz [wyłączyć synchronizację katalogów usługi Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Musisz również dać każdemu użytkownikowi, który został dodany w ten sposób licencję do usługi Microsoft 365 Business. Można to zrobić w [kreatorze konfiguracji](set-up.md) lub [przypisać licencje do użytkowników w usłudze Office 365 dla firm](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Przygotowanie urządzeń mobilnych

Wykonaj czynności opisane w artykule [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business](set-up-mobile-devices.md) w celu instalowania aplikacji pakietu Office na urządzeniach i upewnienia się, że są chronione przez usługę Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Przygotowanie komputerów

Administratorzy mogą wstępnie wybrać ustawienia dla nowych komputerów z systemem Windows 10 za pomocą [programu Windows AutoPilot](add-autopilot-devices-and-profile.md). Użytkownicy mogą skonfigurować istniejące lub nowe urządzenia z systemem Windows 10, wykonując czynności opisane w tym temacie: [Konfigurowanie komputerów z systemem Windows dla użytkowników microsoft 365 Business](set-up-windows-devices.md). W przypadku istniejących urządzeń użytkownicy mogą **opcjonalnie** przenosić pliki do usługi [OneDrive dla Firm](move-files-to-onedrive.md). Mogą również używać narzędzi innych firm do przenoszenia plików skojarzonych z profilem systemu Windows do usługi OneDrive.
  
Jeśli organizacja korzysta z usługi Windows Server Active Directory w środowisku lokalnym, można skonfigurować usługę Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych wymagających uwierzytelniania lokalnego. Wykonaj czynności opisane w artykule Włącz urządzenia z [systemem Windows 10 przyłączone do domeny, które mają być zarządzane przez firmę Microsoft 365 Business,](manage-windows-devices.md) aby skonfigurować tę konfigurację. Ta metoda jest preferowana, a urządzenia w tym stanie są nazywane **hybrydowymi urządzeniami sprzęgłymi z usługi Azure AD.** 
  
Jeśli zachowasz lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz przyznać **tym zasobom przyłączonym do** usługi Azure AD dostęp do tych zasobów, wykonując następujące kroki: Dostęp do zasobów lokalnych z urządzenia [połączonego z usługą Azure AD w usłudze Microsoft 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Skontaktuj się z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator firmy Microsoft 365 Business masz dostęp do naszego zespołu obsługi klienta: ** [Skontaktuj się z pomocą techniczną dla produktów biznesowych — Pomoc dla administratorów](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Zobacz też

[Dokumentacja i zasoby dotyczące platformy Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Zarządzanie platformą Microsoft 365 Business](manage.md)[Migrowanie do platformy Microsoft 365 Business](migrate-to-microsoft-365-business.md)

[Szkoleniowe klipy wideo dotyczące rozwiązania Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
