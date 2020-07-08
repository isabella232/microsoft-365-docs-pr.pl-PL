---
title: Wprowadzenie do usługi Microsoft 365 dla firm
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Dowiedz się więcej o usłudze Microsoft 365 dla firm, o tym, jak ją skonfigurować oraz jak przygotować urządzenia i komputery użytkowników, aby upewnić się, że są one chronione przez usługę Microsoft 365 dla firm.
ms.openlocfilehash: aedcf78f10707dbe6a1d1527effea7d56283dce0
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080048"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Wprowadzenie do usługi Microsoft 365 dla firm

## <a name="what-is-microsoft-365-for-business"></a>Co to jest Microsoft 365 dla firm

Microsoft 365 dla firm to kompleksowy zestaw narzędzi do produktywności i współpracy biznesowej, takich jak Outlook, Word, Excel i inne produkty pakietu Office, które są zawsze aktualne. Pliki robocze można chronić na wszystkich urządzeniach z systemami iOS, Android i Windows 10 za pomocą prostych w zarządzaniu zabezpieczeń klasy korporacyjnej.

Obejrzyj ten klip wideo, aby uzyskać krótki przegląd usługi Microsoft 365 dla firm.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Usługa Microsoft 365 dla firm jest przeznaczona dla maksymalnie 300 licencji. Jeśli potrzebujesz większej liczby licencji, zapoznaj się z dokumentacją usługi [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986), aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-for-business"></a>Uzyskaj usługę Microsoft 365 dla firm

- Jeśli masz partnera, otrzymają microsoft 365 dla firm: [Pobierz microsoft 365 dla firm z Microsoft Partner Center](get-microsoft-365-business.md).
    
- Jeśli nie masz partnera i chcesz uzyskać Microsoft 365 dla biznesu, możesz [go kupić tutaj](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurowanie usługi Microsoft 365 dla firm

 **Omówienie konfiguracji pakietu Microsoft 365 dla firm**
  
Na poniższym diagramie opisano, jak administratorzy skonfigurować usługę Microsoft 365 dla firm. Opisano w nim również kroki przygotowania komputerów z systemem Windows dla usługi Microsoft 365 dla firm. Za pomocą [programu Windows AutoPilot](add-autopilot-devices-and-profile.md)można również dodawać nowe urządzenia w centrum administracyjnym usługi Microsoft 365. Za pomocą programu AutoPilot można skonfigurować i wstępnie skonfigurować nowe urządzenia, tak aby były one gotowe do wydajnego użytku, gdy tylko użytkownik zaloguje się przy użyciu swoich poświadczeń usługi Microsoft 365 dla firm.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Obejrzyj ten klip wideo, aby zapoznać się z omówieniem konfiguracji usługi Microsoft 365 dla firm.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Konfigurowanie usługi Microsoft 365 dla firm (administrator)

Zaloguj się do [centrum administracyjnego usługi Microsoft 365](https://portal.office.com/adminportal/home) przy użyciu poświadczeń administratora globalnego i wykonaj następujące czynności, aby skonfigurować usługę Microsoft 365 dla firm. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach za pomocą usługi Microsoft 365 dla firm](pre-requisites-for-data-protection.md)
    
    Najpierw przeczytaj wymagania wstępne, aby upewnić się, że urządzenia są gotowe do pracy w usłudze Microsoft 365 dla firm.
    
2. [Konfigurowanie usługi Microsoft 365 dla firm za pomocą kreatora instalacji](set-up.md)
    
    Jeśli **trwale przenosisz się z lokalnej usługi Active Directory do chmury,** możesz przejść do centrum administracyjnego usługi Microsoft 365 i użyć kreatora konfiguracji, aby ręcznie dodać użytkowników lub przeprowadzić jednorazową synchronizację z usługą Azure AD Connect. Istnieją dwa sposoby wykonywania tej czynności: 
    
    - Jeśli masz również serwer Exchange 2010, Exchange 2013 lub Exchange 2016, możesz [użyć minimalnej hybrydy, aby szybko przeprowadzić migrację skrzynek pocztowych programu Exchange do usługi Microsoft 365](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). Minimalne kroki hybrydowe obejmują jednorazową synchronizację użytkowników z usługą Azure AD i migrację poczty e-mail z lokalnego do chmury. Po zakończeniu migracji wiadomości e-mail synchronizacja katalogów jest automatycznie wyłączana podczas korzystania z tej metody.
    
    - Użyj kreatora synchronizacji katalogów, aby zsynchronizować użytkowników z chmurą. Wykonaj kroki opisane w [obszarze Konfigurowanie synchronizacji katalogów dla usługi Microsoft 365,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) aby ukończyć ten proces. Po zsynchronizowaniu użytkowników z chmurą należy [wyłączyć synchronizację katalogów dla usługi Microsoft 365](https://docs.microsoft.com/office365/enterprise/turn-off-directory-synchronization).
    
    Musisz również dać każdemu użytkownikowi, który został dodany w ten sposób licencję do usługi Microsoft 365 dla firm. Można to zrobić w [kreatorze instalacji](set-up.md) lub można [przypisać licencje do użytkowników](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: Przygotowanie urządzeń mobilnych

Wykonaj czynności opisane w obszarze [Konfigurowanie urządzeń przenośnych dla usługi Microsoft 365 dla użytkowników biznesowych](set-up-mobile-devices.md) w celu instalowania aplikacji pakietu Office na urządzeniach i upewnienia się, że są one chronione przez usługę Microsoft 365 dla firm. 
  
### <a name="3-prepare-pcs"></a>3: Przygotowanie komputerów

Administratorzy mogą wstępnie wybrać ustawienia dla nowych komputerów z systemem Windows 10 za pomocą [programu Windows AutoPilot](add-autopilot-devices-and-profile.md). Użytkownicy mogą skonfigurować istniejące lub nowe urządzenia z systemem Windows 10, wykonując kroki opisane w tym temacie: [Konfigurowanie komputerów z systemem Windows dla usługi Microsoft 365 dla użytkowników biznesowych.](set-up-windows-devices.md) W przypadku istniejących urządzeń użytkownicy mogą **opcjonalnie** [przenosić pliki do usługi OneDrive dla Firm](move-files-to-onedrive.md). Mogą również używać narzędzi innych firm do przenoszenia plików skojarzonych z profilem systemu Windows do usługi OneDrive.
  
Jeśli twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, można skonfigurować usługę Microsoft 365 dla firm w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego. Wykonaj kroki opisane w [obszarze Włączanie urządzeń z systemem Windows 10 przyłączonych do domeny, które mają być zarządzane przez usługę Microsoft 365 dla firm,](manage-windows-devices.md) aby to skonfigurować. Ta metoda jest preferowana, a urządzenia w tym stanie są nazywane **urządzeniami przyłączanym do usługi Hybrid Azure AD.** 
  
Jeśli zachowasz lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz przyznać **urządzeniom korzystającym z usługi Azure AD** dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: Dostęp do zasobów lokalnych z urządzenia [przyłączanego do usługi Azure AD w usłudze Microsoft 365 dla firm.](access-resources.md)
  
  
## <a name="contact-support"></a>Kontakt z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator usługi Microsoft 365 dla firm masz dostęp do naszego zespołu obsługi klienta: ** [Skontaktuj się z pomocą techniczną dla produktów biznesowych - Pomoc dla administratorów](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Zobacz też

[Microsoft 365 dla dokumentacji biznesowej i zasobów](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Zarządzanie programem Microsoft 365 dla firm](manage.md)[Migruj do usługi Microsoft 365 dla firm](migrate-to-microsoft-365-business.md)

[Wideo dotyczące szkoleń dotyczących usługi Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
