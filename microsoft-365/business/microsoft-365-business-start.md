---
title: Rozpoczynanie pracy z usługą Microsoft 365 Business
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Dowiedz się, jak skonfigurować Microsoft 365 Business.
ms.openlocfilehash: 5986e3fb7786ebb3fa7bcf42b34345be98af44a2
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633434"
---
# <a name="get-started-with-microsoft-365-business"></a>Rozpoczynanie pracy z usługą Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co to jest usługa Microsoft 365 Business

Microsoft 365 Business to kompleksowy zestaw narzędzi do pracy w biznesie i współpracy, takich jak Outlook, Word, Excel i inne produkty biurowe, które są zawsze aktualne. Możesz chronić swoje pliki robocze na wszystkich urządzeniach z systemami iOS, Android i Windows 10, dzięki czemu można łatwo zarządzać zabezpieczeniami klasy korporacyjnej.
  
Microsoft 365 Business jest przeznaczona dla maksymalnie 300 licencji. Jeśli potrzebujesz więcej licencji, zobacz dokumentację [firmy Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) , aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-business"></a>Uzyskiwanie usługi Microsoft 365 Business

- Jeśli masz partnera, otrzymasz Microsoft 365 Business: [Pobierz microsoft 365 Business z Microsoft Partner Center](get-microsoft-365-business.md).
    
- Jeśli nie masz partnera i chcesz uzyskać usługę Microsoft 365 Business, możesz [kupić ją tutaj](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Konfigurowanie usługi Microsoft 365 Business

 **Omówienie zestawu Microsoft 365 Business Suite**
  
Na poniższym diagramie opisano, jak Administratorzy skonfigurować Microsoft 365 Business. Zawiera on także instrukcje dotyczące przygotowania komputerów z systemem Windows do współdziałania z usługą Microsoft 365 Business. Można również dodać nowe urządzenia w centrum administracyjnym Microsoft 365 Business z [systemem Windows AutoPilot](add-autopilot-devices-and-profile.md). Za pomocą AutoPilot można skonfigurować i wstępnie skonfigurować nowe urządzenia, tak aby były gotowe do użytku produkcyjnego, gdy tylko użytkownik zaloguje się przy użyciu poświadczeń firmy Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: konfiguracja Microsoft 365 Business (admin)

Zaloguj się w [witrynie microsoft 365 Business Admin Center](https://portal.office.com/adminportal/home) przy użyciu poświadczeń administratora globalnego i wykonaj następujące kroki, aby skonfigurować Microsoft 365 Business. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach z Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Najpierw przeczytaj wymagania wstępne, aby upewnić się, że urządzenia są gotowe do firmy Microsoft 365 Business.
    
2. [Użyj Kreatora konfiguracji, aby skonfigurować Microsoft 365 Business](set-up.md)
    
    Jeśli **trwale przemieszczasz się z lokalnej usługi Active Directory do chmury**, możesz przejść do centrum administracyjnego Microsoft 365 Business i użyć Kreatora instalacji, aby ręcznie dodać użytkowników, lub możesz wykonać jednorazową synchronizację z usługą Azure AD Connect. Istnieją dwa sposoby wykonywania tej czynności: 
    
    - Jeśli masz również Exchange 2010, Exchange 2013 lub serwera Exchange 2016, można [użyć minimalnego hybrydowego do szybkiej migracji skrzynek pocztowych programu Exchange do pakietu Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Minimalne kroki hybrydowe obejmują jednorazową synchronizację użytkowników z usługą Azure AD i migrację poczty e-mail ze środowiska lokalnego do chmury. Po zakończeniu migracji wiadomości e-mail Synchronizacja katalogów jest automatycznie wyłączany podczas korzystania z tej metody.
    
    - Użyj Kreatora synchronizacji katalogów 365 pakietu Office, aby zsynchronizować użytkowników z chmurą. Aby przeprowadzić tę operację, wykonaj czynności opisane w artykule [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po zsynchronizowaniu użytkowników z chmurą musisz [wyłączyć synchronizację katalogów dla pakietu Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Musisz również dać każdemu użytkownikowi, który został dodany w ten sposób licencję na Microsoft 365 Business. Można to zrobić w [Kreatorze instalacji](set-up.md) lub można [przypisać licencje użytkownikom w pakiecie Office 365 dla firm](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Przygotuj urządzenia mobilne

Wykonaj kroki opisane w [Konfigurowanie urządzeń przenośnych dla użytkowników microsoft 365 Business](set-up-mobile-devices.md) do zainstalowania aplikacji pakietu Office na urządzeniach i upewnij się, że są one chronione przez firmę Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Przygotuj komputery

Administratorzy mogą wstępnie wybrać ustawienia dla nowych komputerów z systemem Windows 10 przy użyciu programu [Windows AutoPilot](add-autopilot-devices-and-profile.md). Użytkownicy mogą skonfigurować istniejące lub nowe urządzenia z systemem Windows 10, wykonując kroki opisane w tym temacie: [Konfigurowanie komputerów z systemem Windows dla użytkowników Microsoft 365 Business](set-up-windows-devices.md). W przypadku istniejących urządzeń użytkownicy mogą **Opcjonalnie** [przenosić pliki do usługi OneDrive dla firm](move-files-to-onedrive.md). Mogą również korzystać z narzędzi innych firm do przenoszenia plików skojarzonych z profilem systemu Windows do usługi OneDrive.
  
Jeśli organizacja korzysta z lokalnego systemu Windows Server Active Directory, można skonfigurować Microsoft 365 Business w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego. Wykonaj kroki opisane w [Włączanie przyłączonych do domeny urządzeń z systemem Windows 10, które mają być zarządzane przez firmę Microsoft 365 Business](manage-windows-devices.md) , aby to skonfigurować. Ta metoda jest preferowana, a urządzenia w tym stanie są nazywane **hybrydowych urządzeń przyłączonych do usługi Azure AD**. 
  
Jeśli zachowasz lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz nadać **urządzeniom przyłączonym do usługi Azure AD** dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostęp do zasobów lokalnych z urządzenia przyłączone do usługi Azure ad w Microsoft 365 Business](access-resources.md).
  
Po skonfigurowaniu komputerów z systemem Windows 10 można [automatycznie zainstalować pakiet Office](auto-install-or-uninstall-office.md) na urządzeniach. 
  
## <a name="contact-support"></a>Skontaktuj się z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator Microsoft 365 Business, masz dostęp do naszego zespołu obsługi klienta: ** [skontaktuj się z działem pomocy technicznej dla produktów biznesowych-admin-pomoc](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Tematy pokrewne
[Dokumentacja i zasoby dotyczące platformy Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Zarządzanie platformą Microsoft 365 Business](manage.md)[Migrowanie do platformy Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

