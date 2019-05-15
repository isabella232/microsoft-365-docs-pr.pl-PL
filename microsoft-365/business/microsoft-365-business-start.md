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
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Dowiedz się skonfigurować Microsoft 365 Business.
ms.openlocfilehash: d309700761ee48ef66a8cd3886fd416c79463ed5
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074305"
---
# <a name="get-started-with-microsoft-365-business"></a>Rozpoczynanie pracy z usługą Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co to jest usługa Microsoft 365 Business

Usługa Microsoft 365 Business to kompleksowy zestaw rozwiązań biurowych i narzędzi do współpracy, takich jak Outlook, Word, Excel i inne aplikacje pakietu Office, które są zawsze aktualne. Możesz chronić swoje pliki na wszystkich urządzeniach z systemami iOS, Android i Windows 10, korzystając z łatwych w zarządzaniu zabezpieczeń klasy biznesowej.
  
Usługa Microsoft 365 Business może obsługiwać do 300 licencji. Jeśli potrzebujesz większej liczby licencji, zapoznaj się z dokumentacją usługi [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986), aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-business"></a>Uzyskiwanie usługi Microsoft 365 Business

- Partnerzy otrzymają usługę Microsoft 365 Business: [Uzyskiwanie usługi Microsoft 365 Business w Centrum partnerskim firmy Microsoft](get-microsoft-365-business.md).
    
- Jeśli nie masz partnera i chcesz uzyskać usługę Microsoft 365 Business, możesz [kupić ją tutaj](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Konfigurowanie usługi Microsoft 365 Business

 **Omówienie Konfigurowanie pakietu Business 365 Microsoft**
  
Poniższy diagram przedstawia, jak Administratorzy konfigurowania Microsoft 365 Business. Zawiera on także instrukcje dotyczące przygotowania komputerów z systemem Windows do współdziałania z usługą Microsoft 365 Business. Nowe urządzenia możesz również dodać za pomocą rozwiązania [Windows AutoPilot](add-autopilot-devices-and-profile.md) w centrum administracyjnym usługi Microsoft 365 Business. Gdy nowe urządzenia zostaną dodane i wstępnie skonfigurowane przy użyciu rozwiązania AutoPilot, będą gotowe do użycia w środowisku produkcyjnym od razu po zalogowaniu się użytkowników za pomocą poświadczeń usługi Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Konfigurowanie 365 Microsoft Business (Administrator)

Zaloguj się do [centrum administracyjnego usługi Microsoft 365 Business](https://portal.office.com/adminportal/home) za pomocą poświadczeń administratora globalnego i wykonaj poniższe czynności, aby skonfigurować usługę Microsoft 365 Business. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach przy użyciu usługi Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    W pierwszej kolejności przeczytaj wymagania wstępne, aby upewnić się, że urządzenia obsługują usługę Microsoft 365 Business.
    
2. [Konfigurowanie usługi Microsoft 365 Business przy użyciu kreatora konfiguracji](set-up.md)
    
    Jeśli **stałe przeniesienie z lokalnego Active Directory do chmury**, można dodać użytkowników ręcznie w Centrum administracyjnym Microsoft 365 Business przy użyciu Kreatora instalacji lub można zrobić jednorazowa synchronizacja z Azure AD Connect. Istnieją dwa sposoby wykonywania tej czynności: 
    
  - Jeśli masz również Exchange 2010, Exchange 2013 lub 2016 programu Exchange server, możesz [Użycia minimalne hybrydowe szybko migracji skrzynek pocztowych programu Exchange do usługi Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Czynności związane z tą metodą obejmują jednorazową synchronizację kont użytkowników do narzędzia Azure AD oraz migrację wiadomości e-mail z magazynu lokalnego do chmury. W przypadku użycia tej metody synchronizacja katalogu zostaje automatycznie wyłączona, gdy migracja poczty e-mail dobiegnie końca.
    
  - Za pomocą kreatora synchronizacji katalogu usługi Office 365 zsynchronizuj konta użytkowników z chmurą. Aby przeprowadzić tę operację, wykonaj czynności opisane w artykule [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po zsynchronizowaniu kont użytkowników z chmurą musisz [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Ponadto musisz przypisać licencję usługi Microsoft 365 Business każdemu użytkownikowi, który został dodany w ten sposób. Można to zrobić w oknie [Kreatora instalacji](set-up.md)lub w [Przypisywanie licencji do użytkowników w usłudze Office 365 dla firm](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: przygotowanie urządzeń przenośnych

Postępuj zgodnie z instrukcjami[Konfigurowanie urządzeń przenośnych dla użytkowników biznesowych 365 firmy Microsoft,](set-up-mobile-devices.md) Aby zainstalować aplikacje pakietu Office na urządzeniach i upewniając się, że są one chronione przez Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: przygotować komputery PC

Administratorzy mogą wstępnie wybrać ustawień dla nowych urządzeń 10 komputerów z systemem Windows za pomocą [Autopilota systemu Windows](add-autopilot-devices-and-profile.md). Użytkownicy mogą konfigurować swoich istniejących lub nowych urządzeń 10 systemu Windows, wykonując kroki opisane w tym temacie: [Konfigurowanie komputerów z systemem Windows dla użytkowników biznesowych 365 firmy Microsoft](set-up-windows-devices.md). Dla istniejących urządzeń użytkownicy są mogą również **Opcjonalnie można**[przenieść pliki do OneDrive dla firmy](move-files-to-onedrive.md). Można również użyć narzędzi innych firm do przenoszenia plików skojarzonych z profilem systemu Windows do OneDrive.
  
Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych. Postępuj zgodnie z instrukcjami [włączyć przyłączonych do domeny Windows 10 urządzenia mają być zarządzane przez Microsoft 365 Business](manage-windows-devices.md) można wybrać tę opcję. Jest to preferowana metoda i urządzeń, w tym stanie są nazywane **hybrydowy Azure AD dołączył do urządzenia**. 
  
Aby zachować lokalnej usługi Active Directory, który zawiera niektóre zasobów lokalnych (takich jak udziały plików i drukarek), może dać **Azure AD przyłączony urządzeniom** dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostępu do zasobów lokalnych z Azure AD dołączył do urządzenia w Microsoft 365 Business](access-resources.md).
  
Po zdefiniowaniu 10 komputerów z systemem Windows można [automatycznie zainstalować pakietu Office](auto-install-or-uninstall-office.md) do urządzeń. 
  
## <a name="contact-support"></a>Skontaktuj się z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator Microsoft 365 Business użytkownik ma dostęp do działu obsługi klienta, ** [kontakt z pomocą techniczną dla produktów biznesowych - Pomoc administracyjna](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Tematy pokrewne
[Dokumentacja i zasoby dotyczące platformy Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Zarządzanie platformą Microsoft 365 Business](manage.md)[Migrowanie do platformy Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

