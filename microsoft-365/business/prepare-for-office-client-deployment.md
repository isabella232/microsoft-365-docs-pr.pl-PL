---
title: Przygotowywanie do Office klienta przez Microsoft 365 dla firm
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
description: Dowiedz się, jak automatycznie instalować 32-bitowe Office na Windows 10 komputerach i aktualizować je.
ms.openlocfilehash: 134d5f2918e3f28c2025b282b9ae0325b64fe0474ae8123d0637bb43c4730c55
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803571"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Przygotowywanie do Office klienta przez Microsoft 365 dla firm

Ten artykuł dotyczy Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich

Za pomocą tego Microsoft 365 Business Premium automatycznie zainstalować 32-bitowe aplikacje pakietu Office na Windows 10 komputerach i być na bieżąco z aktualizacjami.
  
Automatyczna instalacja działa najlepiej, jeśli na komputerze użytkownika końcowego jest Windows 10 Business i:
  
- nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).
    
    lub
    
- jest zainstalowana wersja Szybka instalacja pakietu Office.
    
Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook). Jeśli zobaczysz **Office, jak** pokazano na poniższej ilustracji, instalacja została wykonana przy użyciu technologii Click-to-Run. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **KtoTo korzyści wynikających z posiadania tej funkcji**
  
Użytkownik końcowy, którego komputer spełnia następujące kryteria:
  
- **Ma** licencję Windows 10 Business użytkownika, aktywną licencję usługi Microsoft 365 dla firm, licencję Aktualizacja systemu Windows 10 dla twórców i jest dołączany do Azure Active Directory. 
    
- **Nie zawiera** 64-bitowych Office (na przykład: Word, Excel, PowerPoint). Jeśli wymagane są 64-bitowe wersje aplikacji pakietu Office, ta funkcja nie jest dobrym rozwiązaniem, ponieważ wyzwalanie 64-bitowej wersji programu Office w wersji 2016 w wersji Click-to-Run z konsoli administracyjnej programu Microsoft 365 dla firm nie jest dostępne. 
    
- **Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project). Microsoft 365 dla firm Office wersji Click-to-Run programu Office 2016, która nie działa z aplikacjami autonomicznymi MSI programu Office 2016. 
    
W poniższej tabeli pokazano, jakie działania, w zależności od stanu rozpoczęcia, muszą zostać uruchomione przez użytkowników końcowych w celu pomyślnego, 32-bitowego wdrożenia programu Office w wersji Click-to-Run z konsoli administracyjnej programu Microsoft 365 dla firm.<br/>


|Stan początkowy instalacji pakietu Office|Czynności do podjęcia przed Microsoft 365 dla firm Office instalacji|Stan końcowy|
|:-----|:-----|:-----|
|Brak zainstalowanego pakietu Office  <br/> |Brak  <br/> |Office 32-bitowej aktualizacji 2016 jest instalowana przy użyciu technologii Click-to-Run  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych  <br/> |Brak  <br/> |Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\*** <br/> |
|Istniejąca 32-bitowa wersja Office i 32-bitowa lub 64-bitowa wersja 32- lub 64-bitowa wersja Click-to-Run Office (na przykład Visio, Project)  <br/> |Brak  <br/> |Nie wpływa to na aplikacje autonomiczne. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)  <br/> |Brak  <br/> |Nie wpływa to na aplikacje autonomiczne. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016  <br/> |
|Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office  <br/> |Odinstaluj 64-bitowe Office, jeśli możesz zamienić je na 32-bitowe Office aplikacje  <br/> |Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016  <br/> |
|Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich  <br/> |Odinstalowanie pakietu Office 2016 w wersji MSI.  <br/> |Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych  <br/> |
|Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office  <br/> |Brak  <br/> |32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle  <br/> |
||||
   
 **(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu. Trwa prace nad poprawą. 
  
