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
ms.openlocfilehash: 5b28c1e62d813c52b41ce8e7619c865cdf7690e2
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575823"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich

Usługi Microsoft 365 Business umożliwiają automatyczne instalowanie 32-bitowych aplikacji pakietu Office i aktualizacji dla tych aplikacji na komputerach z systemem Windows 10.
  
To rozwiązanie działa najlepiej, gdy na komputerze użytkownika końcowego jest zainstalowany system Windows 10 Business oraz:
  
- nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).
    
    lub
    
- jest zainstalowana wersja Szybka instalacja pakietu Office.
    
Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook). Jeśli zostaną wyświetlone aktualizacje pakietu Office, jak pokazano na poniższej ilustracji, oznacza to, że instalację przeprowadzono za pomocą modułu Szybka instalacja. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kto będzie korzystać z tej funkcji**
  
Użytkownik końcowy, którego komputer spełnia następujące kryteria:
  
- **Zawiera** licencję użytkownika systemu Windows 10 Business i aktywną licencję usług Microsoft 365 Business oraz aktualizację dla twórców systemu Windows 10, a także jest dołączony do usługi Azure Active Directory. 
    
- **Nie zawiera** 64-bitowych wersji aplikacji pakietu Office (przykład: Word, Excel, PowerPoint). Jeśli 64-bitowe wersje aplikacji pakietu Office są wymagane, ta funkcja nie jest dobrym rozwiązaniem, ponieważ wyzwalanie 64-bitowego modułu Szybka instalacja pakietu Office w wersji 2016 z poziomu konsoli administracyjnej usług Microsoft 365 Business nie jest obsługiwane. 
    
- **Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project). Usługi Microsoft 365 Business umożliwiają uaktualnienie pakietu Office do wersji Szybka instalacja pakietu Office 2016, która nie współdziała z aplikacjami autonomicznymi MSI pakietu Office 2016. 
    
W poniższej tabeli wyszczególniono możliwe działania, które użytkownicy końcowi lub administratorzy muszą wykonać w zależności od stanu początkowego, aby pomyślnie zainstalować 32-bitową wersję Szybka instalacja wdrożenia pakietu Office z poziomu konsoli administracyjnej usług Microsoft 365 Business.
  
|**Stan początkowy instalacji pakietu Office**|**Działanie do wykonania przed rozpoczęciem instalacji pakietu Office przy użyciu usług Microsoft 365 Business**|**Stan końcowy**|
|:-----|:-----|:-----|
|Brak zainstalowanego pakietu Office  <br/> |Brak  <br/> |Pakiet Office 2016 w wersji 32-bitowej zainstalowany za pomocą modułu Szybka instalacja  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych  <br/> |Brak  <br/> |Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\*** <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i 32- lub 64-bitowe aplikacje autonomiczne pakietu Office w wersji Szybka instalacja (na przykład Visio lub Project)  <br/> |Brak  <br/> |Aplikacje autonomiczne pozostają nienaruszone. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)  <br/> |Brak  <br/> |Aplikacje autonomiczne pozostają nienaruszone. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> ||||
|Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office  <br/> |Odinstalowanie 64-bitowych wersji aplikacji pakietu Office, jeśli można je zamienić na 32-bitowe wersje aplikacji pakietu Office  <br/> |Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich  <br/> |Odinstalowanie pakietu Office 2016 w wersji MSI.  <br/> |Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych  <br/> |
|Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office  <br/> |Brak  <br/> |32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle  <br/> |
||||
   
 **(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu. Trwa opracowywanie rozwiązania. 
  


