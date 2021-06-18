---
title: Przygotowywanie klienta pakietu Office do wdrożenia za pomocą platformy Microsoft 365 dla firm
f1.keywords:
- CSH
ms.author: efrene
author: efrene
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Dowiedz się, jak automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i aktualizować je.
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924232"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Przygotowywanie klienta pakietu Office do wdrożenia za pomocą platformy Microsoft 365 dla firm

Ten artykuł dotyczy usługi Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich

Za pomocą usługi Microsoft 365 Business Premium możesz automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i być na bieżąco z ich aktualizacjami.
  
Automatyczna instalacja działa najlepiej, jeśli komputer użytkownika końcowego znajduje się w systemie Windows 10 Business i:
  
- nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).
    
    lub
    
- jest zainstalowana wersja Szybka instalacja pakietu Office.
    
Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook). Jeśli widzisz aktualizacje **pakietu Office,** jak pokazano na poniższej ilustracji, instalacja została wykonana przy użyciu technologii Click-to-Run. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kto korzysta z tej funkcji**
  
Użytkownik końcowy, którego komputer spełnia następujące kryteria:
  
- **Ma**  licencję użytkownika systemu Windows 10 Business, aktywną licencję platformy Microsoft 365 dla firm i aktualizację systemu Windows 10 dla twórców oraz jest dołączany do usługi Azure Active Directory. 
    
- **Nie zawiera** 64-bitowych aplikacji pakietu Office (przykład: Word, Excel, PowerPoint). Jeśli 64-bitowe wersje aplikacji pakietu Office są wymagane, ta funkcja nie jest dobrym rozwiązaniem, ponieważ wyzwalanie 64-bitowej wersji 2016 pakietu Office w wersji Click-to-Run z konsoli administracyjnej platformy Microsoft 365 dla firm nie jest dostępne. 
    
- **Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project). Usługa Microsoft 365 dla firm uaktualnia pakiet Office do wersji Click-to-Run pakietu Office 2016, która nie działa z aplikacjami autonomicznymi MSI pakietu Office 2016. 
    
W poniższej tabeli przedstawiono działania, jakie mogą zostać podjąć użytkownicy końcowi/administratorzy w zależności od stanu ich rozpoczęcia, aby pomyślnie uruchomić 32-bitową wersję Technologii Kliknij, aby uruchomić wdrożenie pakietu Office z konsoli administracyjnej platformy Microsoft 365 dla firm.<br/>


|Stan początkowy instalacji pakietu Office|Akcja do podjęcia przed zainstalowaniem pakietu Office na platformie Microsoft 365 dla firm|Stan końcowy|
|:-----|:-----|:-----|
|Brak zainstalowanego pakietu Office  <br/> |Brak  <br/> |32-bitowy pakiet Office 2016 jest instalowany przy użyciu technologii Click-to-Run  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych  <br/> |Brak  <br/> |Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\*** <br/> |
|Istniejąca 32-bitowa wersja Click-to-Run pakietu Office i 32-bitowe lub 64-bitowe aplikacje autonomiczne pakietu Office w wersji Click-to-Run (na przykład Visio lub Project)  <br/> |Brak  <br/> |Nie wpływa to na aplikacje autonomiczne. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)  <br/> |Brak  <br/> |Nie wpływa to na aplikacje autonomiczne. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office  <br/> |Odinstaluj 64-bitowe aplikacje pakietu Office, jeśli można je zamienić na 32-bitowe aplikacje pakietu Office  <br/> |Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich  <br/> |Odinstalowanie pakietu Office 2016 w wersji MSI.  <br/> |Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych  <br/> |
|Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office  <br/> |Brak  <br/> |32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle  <br/> |
||||
   
 **(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu. Trwa prace nad poprawą. 
  
