---
title: Rozpoczynanie pracy z aplikacją Microsoft 365 dla firm
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
description: Informacje o programie Microsoft 365 dla firm, sposobie jego konfigurowania i przygotowywaniu urządzeń i komputerów użytkowników w celu zapewnienia ich ochrony firmie Microsoft 365 dla firm.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306494"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Rozpoczynanie pracy z aplikacją Microsoft 365 dla firm

## <a name="what-is-microsoft-365-for-business"></a>Co to jest Microsoft 365 dla firm

Microsoft 365 dla firm to kompleksowy zestaw narzędzi do pracy i współpracy, takich jak program Outlook, Word, Excel i inne produkty pakietu Office, które są zawsze aktualne. Pliki służbowe można chronić na wszystkich urządzeniach z systemem iOS, Android i Windows 10, korzystając z zabezpieczeń innych firm, które są łatwe w zarządzaniu.

Obejrzyj ten klip wideo, aby zapoznać się z krótkim omówieniem programu Microsoft 365 dla firm.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Pakiet Microsoft 365 dla firm jest przeznaczony do 300 licencji. Jeśli potrzebujesz większej liczby licencji, zapoznaj się z dokumentacją usługi [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986), aby uzyskać więcej informacji. 
  
## <a name="get-microsoft-365-for-business"></a>Pobierz aplikację Microsoft 365 dla firm

- Jeśli masz partnera, otrzymasz aplikację Microsoft 365 dla firm: [Uzyskaj aplikację microsoft 365 dla firm z Centrum partnerskiego firmy Microsoft](get-microsoft-365-business.md).
    
- Jeśli nie masz partnera i chcesz uzyskać oprogramowanie Microsoft 365 dla firm, możesz [go kupić tutaj](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurowanie usługi Microsoft 365 dla firm

 **Omówienie konfiguracji programu Microsoft 365 dla firm Suite**
  
Na poniższym diagramie opisano, jak administratorzy konfigurują aplikację Microsoft 365 dla firm. Opisano tu również procedurę przygotowywania komputerów z systemem Windows dla systemu Microsoft 365 dla firm. Możesz również dodać nowe urządzenia w centrum administracyjnym usługi Microsoft 365 z programem [Windows dla pilota](add-autopilot-devices-and-profile.md). Możesz użyć autopilota, aby skonfigurować i wstępnie skonfigurować nowe urządzenia, tak aby były gotowe do użycia, gdy tylko użytkownik zaloguje się przy użyciu poświadczeń programu Microsoft 365 dla firm.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Obejrzyj ten klip wideo, aby zapoznać się z omówieniem konfiguracji programu Microsoft 365 dla firm.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Konfigurowanie usługi Microsoft 365 dla firm (Administrator)

Zaloguj się do [Centrum administracyjnego programu Microsoft 365](https://portal.office.com/adminportal/home) z poświadczeniami administratora globalnego i wykonaj poniższe czynności, aby skonfigurować aplikację Microsoft 365 dla firm. 
  
1. [Wymagania wstępne dotyczące ochrony danych na urządzeniach z programem Microsoft 365 dla firm](pre-requisites-for-data-protection.md)
    
    Najpierw przeczytaj wymagania wstępne, aby upewnić się, że Twoje urządzenia są gotowe do obsługi programu Microsoft 365 dla firm.
    
2. [Konfigurowanie programu Microsoft 365 dla firm przy użyciu Kreatora konfiguracji](set-up.md)
    
    Jeśli **stale przenosisz się z lokalnej usługi Active Directory do chmury**, możesz przejść do centrum administracyjnego usługi Microsoft 365 i użyć Kreatora konfiguracji w celu ręcznego dodania użytkowników lub można przeprowadzić jednorazową synchronizację z usługą Azure AD Connect. Istnieją dwa sposoby wykonywania tej czynności: 
    
    - Jeśli masz także serwer programu Exchange 2010, Exchange 2013 lub Exchange 2016, możesz [szybko przeprowadzić migrację skrzynek pocztowych programu Exchange do usługi Microsoft 365 za pomocą minimalnego środowiska hybrydowego](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). Minimalne czynności hybrydowe zawierają jednorazową synchronizację użytkowników z usługą Azure AD oraz migrację poczty e-mail z lokalnego do chmury. Po zakończeniu migracji poczty e-mail Synchronizacja katalogów jest automatycznie wyłączana po zastosowaniu tej metody.
    
    - Zsynchronizuj użytkowników z chmurą za pomocą Kreatora synchronizacji katalogów. Postępuj zgodnie z instrukcjami [podanymi w artykule Konfigurowanie synchronizacji katalogów dla Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) , aby ukończyć ten proces. Po zsynchronizowaniu użytkowników z chmurą konieczne będzie [wyłączenie synchronizacji katalogów dla programu Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization).
    
    Trzeba także nadać każdemu użytkownikowi w ten sposób licencję na aplikację Microsoft 365 dla firm. Możesz to zrobić w [Kreatorze konfiguracji](set-up.md) lub [przypisać licencje użytkownikom](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: Przygotowywanie urządzeń przenośnych

Postępuj zgodnie z instrukcjami w artykule [Konfigurowanie urządzeń przenośnych dla aplikacji Microsoft 365 dla firm](set-up-mobile-devices.md) , aby zainstalować aplikacje pakietu Office na urządzeniach i upewnić się, że są one chronione przez firmę Microsoft 365 dla firm. 
  
### <a name="3-prepare-pcs"></a>3: przygotowywanie komputerów

Administratorzy mogą wstępnie wybierać ustawienia nowych komputerów z systemem Windows 10 przy użyciu [autopilota systemu Windows](add-autopilot-devices-and-profile.md). Użytkownicy mogą skonfigurować istniejące lub nowe urządzenia z systemem Windows 10, wykonując czynności opisane w tym temacie: [Konfigurowanie komputerów z systemem Windows dla systemu Microsoft 365 dla firm](set-up-windows-devices.md). W przypadku istniejących urządzeń użytkownicy mogą **Opcjonalnie** [przenosić pliki do usługi OneDrive dla firm](move-files-to-onedrive.md). Mogą także korzystać z narzędzi innych firm do przenoszenia plików skojarzonych z profilem systemu Windows do usługi OneDrive.
  
Jeśli w organizacji jest używana usługa Active Directory w systemie Windows Server, możesz skonfigurować aplikację Microsoft 365 dla firm w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelnienia lokalnego. Postępuj zgodnie z instrukcjami w artykule [Włącz zarządzanie urządzeniami z systemem Windows 10 dołączonymi do domeny przez aplikację Microsoft 365 dla firm,](manage-windows-devices.md) aby ją skonfigurować. Ta metoda jest preferowana, a urządzenia w tym stanie są nazywane **urządzeniami hybrydowymi usługi Azure AD**. 
  
Jeśli zatrzymasz lokalną usługę Active Directory zawierającą niektóre zasoby lokalne (takie jak udziały plików i drukarki), możesz udostępnić **urządzeniom z systemem Azure AD** , aby uzyskać dostęp do tych zasobów, wykonując czynności opisane tutaj: [Uzyskiwanie dostępu do zasobów lokalnych z urządzenia opartego na usłudze Azure AD w programie Microsoft 365 dla firm](access-resources.md).
  
  
## <a name="contact-support"></a>Kontakt z pomocą techniczną

 **Jeśli potrzebujesz pomocy technicznej:**
  
- Skontaktuj się ze swoim partnerem.
    
- Jako administrator programu Microsoft 365 dla firm możesz uzyskać dostęp do naszego zespołu obsługi klienta: ** [kontaktowanie się z pomocą techniczną dla produktów biznesowych — pomoc dla administratorów](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Zobacz też

[Dokumentacja i zasoby dotyczące programu Microsoft 365 dla firm](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Zarządzanie programem microsoft 365 dla firm](manage.md)po[migracji do programu Microsoft 365 dla firm](migrate-to-microsoft-365-business.md)

[Szkolenia wideo dotyczące programu Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
