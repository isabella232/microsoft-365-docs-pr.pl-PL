---
title: Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Dowiedz się, jak automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i aktualizować je.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640774"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich

Można użyć Microsoft 365 Business, aby automatycznie zainstalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i zachować je aktualne aktualizacje.
  
Automatyczna instalacja działa najlepiej, jeśli komputer użytkownika końcowego jest w systemie Windows 10 Business i:
  
- nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).
    
    lub
    
- jest zainstalowana wersja Szybka instalacja pakietu Office.
    
Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook). Jeśli widzisz **aktualizacje pakietu Office** , jak pokazano na poniższej ilustracji, a następnie instalacja została wykonana za pomocą kliknij, aby uruchomić. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kto korzysta z tej funkcji**
  
Użytkownik końcowy, którego komputer spełnia następujące kryteria:
  
- **Zawiera** licencję użytkownika systemu Windows 10 Business i aktywną licencję usług Microsoft 365 Business oraz aktualizację dla twórców systemu Windows 10, a także jest dołączony do usługi Azure Active Directory. 
    
- **Nie ma** 64-bitowych aplikacji pakietu Office (przykład: Word, Excel, PowerPoint). Jeśli wymagane są 64-bitowe aplikacje pakietu Office, ta funkcja nie jest dobrym dopasowaniem, ponieważ nie ma żadnego wsparcia dla wyzwalania 64-bitowego 2016-szybka wersja pakietu Office z konsoli administracyjnej Microsoft 365 Business. 
    
- **Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project). Mikroskop 365 sprawa ulepsza Wydział wobec ten trzaskać-wobec-biegać wersja od Wydział 2016 i ów nie robi ' praca rezygnować Wydział 2016 MSI autonomiczny Apps. 
    
W poniższej tabeli przedstawiono akcję, jaką użytkownicy/Administratorzy końcowi mogą potrzebować w zależności od stanu początkowego, aby mieć pomyślny 32-bitowej wersji pakietu Office z systemem Szybka instalacja z konsoli administracyjnej Microsoft 365 Business.
  
|**Stan początkowy instalacji pakietu Office**|**Działanie do wykonania przed rozpoczęciem instalacji pakietu Office przy użyciu usług Microsoft 365 Business**|**Stan końcowy**|
|:-----|:-----|:-----|
|Brak zainstalowanego pakietu Office  <br/> |Brak  <br/> |Pakiet Office 2016 32-bit jest instalowany przy użyciu funkcji Szybka instalacja  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych  <br/> |Brak  <br/> |Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\*** <br/> |
|Istniejąca szybka i szybka wersja 32-bitowej wersji pakietu Office i szybka aplikacja pakietu Office 32-bitowego lub 64-bitowego (na przykład Visio, Project)  <br/> |Brak  <br/> |Nie ma to wpływu na samodzielne aplikacje. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)  <br/> |Brak  <br/> |Nie ma to wpływu na samodzielne aplikacje. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> ||||
|Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office  <br/> |Odinstaluj 64-bitowe aplikacje pakietu Office, jeśli jest to OK, aby zastąpić je z 32-bitowe aplikacje pakietu Office  <br/> |Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich  <br/> |Odinstalowanie pakietu Office 2016 w wersji MSI.  <br/> |Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych  <br/> |
|Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office  <br/> |Brak  <br/> |32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle  <br/> |
||||
   
 **(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu. Poprawka jest w toku. 
  