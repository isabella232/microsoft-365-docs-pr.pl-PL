---
title: Migrowanie z platformy Microsoft 365 Business do platformy Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Dowiedz się, jak przenieść firmę z usługi Microsoft 365 Business Premium do platformy Microsoft 365 E3.
ms.openlocfilehash: 10630671f3deb7eff0ad0f601d301b90743ee35f
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164518"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrowanie z platformy Microsoft 365 Business Premium do platformy Microsoft 365 E3

Usługa Microsoft 365 Business Premium oferuje wszystko, czego potrzebujesz dla Twojej małej firmy, i łączy najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają Twoim pracownikom wydajną pracę. W niektórych przypadkach może być jednak konieczne przeprowadzenie migracji subskrypcji platformy Microsoft 365 Business Premium do platformy Microsoft 365 E3. 

Na przykład Twoja firma wyrosła i potrzebuje ponad 300 licencji (gratulacje, przy okazji).

Twoja firma również potrzebuje funkcji dla przedsiębiorstw, takich jak aplikacje platformy Microsoft 365 dla przedsiębiorstw, licencje CALs (Enterprise Client Access License) dla systemu Windows 10 Enterprise.

Uaktualnienie jest łatwe: możesz rozpocząć uaktualnienie [z centrum administracyjnego.](../commerce/subscriptions/upgrade-to-different-plan.md) Wszystkie Dane i konfiguracja w bieżącej subskrypcji są zachowywane. Nie musisz nic robić, aby przygotować się do migracji i po jej zakończeniu nic nie robić, z wyjątkiem skorzystania z nowych funkcji.

>[!Note]
>Możesz również użyć subskrypcji usługi Microsoft 365 Business Premium na maksymalnie 300 stanowisk i uzyskać subskrypcję Microsoft 365 E3 dla ponad 300 stanowisk. Usługa Microsoft Defender dla usługi Office 365 nie jest jednak dołączona do platformy Microsoft 365 E3. W celu dalszej ochrony przed zagrożeniami należy dodać kolejne licencje usługi Defender dla usługi Office 365, tak aby wszyscy użytkownicy, którzy są dostępni do programu Defender w ramach firmy Usługi Office 365, posiadali licencje.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Różnice między usługami Microsoft 365 Business Premium i Microsoft 365 Enterprise

W poniższej tabeli przedstawiono różnice między usługą Microsoft 365 Business Premium a usługą Microsoft 365 E3.

| Funkcja    | Pomoc techniczna na platformy Microsoft 365 Business Premium    | Pomoc techniczna na microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikacje pakietu Office*    | [Aplikacje Microsoft 365 dla firm](#office-365-business)    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje zwiększające produktywność w chmurze**        | | | 
| Usługi Exchange Online i Outlook    | Limit miejsca do magazynowania 50 GB na skrzynkę pocztową i nieograniczona archiwizacja w u usługi Exchange Online    | 100 GB miejsca do magazynowania na skrzynkę pocztową i nieograniczona archiwizacja w u usługi Exchange Online | 
| Teams    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | 1 TB miejsca do magazynowania na użytkownika    | Bez ograniczeń | 
| Yammer, SharePoint Online, Planner, Stream    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrona przed zagrożeniami**        | | | 
| Możliwości zmniejszania powierzchni ataków    | [Zobacz tę listę](#threat-protection) | Zarządzanie przedsiębiorstwem izolacji na podstawie sprzętu dla programu Microsoft Edge | 
| Defender dla usługi Office 365 (plan 1) | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | Nie dołączona, ale można ją dodać do | 
| **Zarządzanie tożsamościami**        | | | 
| Samodzielne resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego (MFA), dostępu warunkowego i zapisu haseł tożsamości lokalnych|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Odnajdowanie aplikacji w chmurze, kondycja usługi Azure AD Connect    |     | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Aplikacje usługi Azure AD usługi Office 365 Pojedyncza Sign-On (SSO): 10 aplikacji na użytkownika (aplikacje Galerii SaaS, takie jak Salesforce)* | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Logowanie jednokrotne usługi Azure AD Premium 1: bez ograniczeń (aplikacje lokalne za pośrednictwem serwera proxy aplikacji usługi Azure AD i aplikacje nie gallery przy użyciu szablonów integracji aplikacji usługi Self-Service)    |     | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Zarządzanie urządzeniami i aplikacją**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|Dostęp do pulpitu wirtualnego (VDA)    |  |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|Pulpit wirtualny Windows (WVD)    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|Aktywacja na komputerze udostępnionym (SCA, Shared Computer Activation)    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Pakiet optymalizacji pulpitu firmy Microsoft    | |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrona informacji**        | | | 
| Ochrona przed utratą danych w usłudze Office 365, Azure Information Protection Plan 1    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Ochrona informacji o oknie dla ochrony przed dlp punktu końcowego    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Licencja dostępu klienta (prawa calowe)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Menedżer konfiguracji, Windows Rights Management)| |         ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Zgodność**        | | | 
| Nieograniczona archiwizacja wiadomości e-mail    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Menedżer zgodności    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| zbierania elektronicznych materiałów dowodowych    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Zawieszenie w miejscu i postępowanie sądowe    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Tagi przechowywania rekordów wiadomości (MRM) i zasady przechowywania    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Użytkownicy z przypisanym dostępem do aplikacji SaaS mogą uzyskać dostęp do logowania jednokrotnego do maksymalnie 10 aplikacji. Administratorzy mogą konfigurować logowanie jednokrotne i zmieniać dostęp użytkowników do różnych aplikacji SaaS, ale dostęp do logowania jednokrotnego jest dozwolony tylko dla 10 aplikacji na użytkownika jednocześnie. Wszystkie aplikacje usługi Office 365 są liczone jako jedna aplikacja.

## <a name="migration"></a>Migracja

Aby przeprowadzić migrację, we współpracy z partnerem przenieś subskrypcję i licencje platformy Microsoft 365 Business Premium do odpowiedniej subskrypcji Microsoft 365 E3 wraz z jej licencjami.

W poniższych sekcjach opisano, jakie zmiany należy wprowadzić (o ile są) i co można zrobić po migracji.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Dane i konfiguracja subskrypcji platformy Microsoft 365

Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:

- Konfiguracja subskrypcji, taka jak nazwy domen DNS.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usługi zwiększającej produktywność i ich dane, takie jak usługa Teams, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.

Użytkownicy mogą teraz korzystać z nieograniczonej przestrzeni dyskowej w skrzynkach pocztowych usługi Exchange Online i folderach usługi OneDrive dla Firm.

Możesz rozpocząć korzystanie z odnajdowania aplikacji w chmurze, usługi Azure AD Connect Health i logowania jednokrotnego dla ponad 10 aplikacji.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrona przed zagrożeniami

System Windows 10 Business zapewnia następujące zabezpieczenia:

- Wymuszanie integralności procesu rozruchu systemu operacyjnego
- Wymuszanie integralności wrażliwych składników operacyjnych
- Zaawansowana luki w zabezpieczeniach i środki zaradcze wykorzystujące bezbłędne wykorzystywanie luk
- Ochrona sieci oparta na reputacji dla przeglądarek Microsoft Edge, Internet Explorer i Chrome
- Zapora oparta na hoście
- Środki zaradcze oprogramowania wymuszającego okup
- Izolacji oparte na sprzęcie dla programu Microsoft Edge
- Sterowanie aplikacją obsługiwane przez funkcja Intelligent Security Graph
- Sterowanie urządzeniem (USB)
- Ochrona sieci przed zagrożeniami internetowymi
- Reguły ochrony przed nieuprawnianiem hostów

System Windows 10 Enterprise E3 obejmuje również zarządzanie przedsiębiorstwem izolacji na podstawie sprzętu dla programu Microsoft Edge.

>[!Note]
>Użytkownicy, którzy migrowali do platformy Microsoft 365 E3, będą wymagać licencji programu Microsoft Defender dla usługi Office 365 na kontynuujoną ochronę przed zagrożeniami. Kup dodatkową usługę Defender dla licencji usługi Office 365, aby wszyscy użytkownicy, którzy mają dostęp do twoich przepisów usługi Defender dla usługi Office 365, posiadali licencje. 
>

### <a name="device-management-with-intune"></a>Zarządzanie urządzeniami za pomocą usługi Intune

Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, która obejmuje zarejestrowane urządzenia oraz ustawienia urządzenia i aplikacji.

### <a name="windows-10"></a>Windows 10

Usługa Microsoft 365 Business Premium zawiera system Windows 10 Business, który można zainstalować za pomocą rozwiązania Windows AutoPilot. Podczas migracji do platformy Microsoft 365 E3 każda licencja użytkownika obejmuje system Windows 10 Enterprise E3, który można również zainstalować za pomocą rozwiązania Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikacje Microsoft 365 dla firm

Klient aplikacji Microsoft 365 dla firm zainstalowany na Twoich urządzeniach automatycznie zacznie korzystać z funkcji aplikacji platformy Microsoft 365 dla przedsiębiorstw. Po zakończeniu migracji możesz teraz użyć:

 - zasady grupy pomocy technicznej
 - Porównywanie arkuszy kalkulacyjnych i inquire
 - Analizę biznesową

