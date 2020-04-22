---
title: Przygotowanie do wdrożenia klienta pakietu Office przez usługę Microsoft 365 dla firm
f1.keywords:
- CSH
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
ms.openlocfilehash: b5f01bc9bb10765929f3c6bdd5908e8b48a51a11
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633104"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Przygotowanie do wdrożenia klienta pakietu Office przez usługę Microsoft 365 dla firm

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich

Za pomocą usługi Microsoft 365 dla firm można automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i utrzymywać je na bieżąco z aktualizacjami.
  
Automatyczna instalacja działa najlepiej, jeśli komputer użytkownika końcowego jest w systemie Windows 10 Business i:
  
- nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).
    
    lub
    
- jest zainstalowana wersja Szybka instalacja pakietu Office.
    
Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook). Jeśli widzisz **aktualizacje pakietu Office,** jak pokazano na poniższym rysunku, instalacja została wykonana przy użyciu funkcji Szybka instalacja. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kto korzysta z posiadania tej funkcji**
  
Użytkownik końcowy, którego komputer spełnia następujące kryteria:
  
- **Ma** licencję użytkownika systemu Windows 10 Business, aktywną licencję microsoft 365 dla firm, windows 10 Creators Update i jest przyłączony do usługi Azure Active Directory. 
    
- **Nie ma** 64-bitowych aplikacji pakietu Office (np. Jeśli wymagane są 64-bitowe aplikacje pakietu Office, ta funkcja nie jest dobrym rozwiązaniem, ponieważ nie ma obsługi wyzwalania 64-bitowej wersji pakietu Office typu Szybka, aby uruchomić pakiet Office z konsoli administracyjnej usługi Microsoft 365 dla firm. 
    
- **Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project). Usługa Microsoft 365 dla firm uaktualnia pakiet Office do wersji szybka obsługa pakietu Office 2016 i nie działa z autonomicznymi aplikacjami MSI pakietu Office 2016. 
    
W poniższej tabeli przedstawiono, jakie działania użytkownicy końcowi/administratorzy mogą wymagać, w zależności od stanu początkowego, aby mieć pomyślną 32-bitową wersję szybka wdrożenia pakietu Office z konsoli administracyjnej usługi Microsoft 365 dla firm.
  
|**Stan początkowy instalacji pakietu Office**|**Działania, które należy podjąć przed zainstalowaniem pakietu Microsoft 365 dla firm Office**|**Stan końcowy**|
|:-----|:-----|:-----|
|Brak zainstalowanego pakietu Office  <br/> |Brak  <br/> |32-bitowy pakiet Office 2016 jest instalowany przy użyciu funkcji Szybka instalacja  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych  <br/> |Brak  <br/> |Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\*** <br/> |
|Istniejąca 32-bitowa wersja pakietu Click-to-Run pakietu Office i 32-bitowe lub 64-bitowe autonomiczne aplikacje pakietu Office (na przykład Visio, Project)  <br/> |Brak  <br/> |Nie ma to wpływu na aplikacje autonomiczne. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)  <br/> |Brak  <br/> |Nie ma to wpływu na aplikacje autonomiczne. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> ||||
|Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office  <br/> |Odinstalowywanie 64-bitowych aplikacji pakietu Office, jeśli można je zastąpić 32-bitowymi aplikacjami pakietu Office  <br/> |Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich  <br/> |Odinstalowanie pakietu Office 2016 w wersji MSI.  <br/> |Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych  <br/> |
|Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office  <br/> |Brak  <br/> |32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle  <br/> |
||||
   
 **(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu. Poprawka jest w toku. 
  
