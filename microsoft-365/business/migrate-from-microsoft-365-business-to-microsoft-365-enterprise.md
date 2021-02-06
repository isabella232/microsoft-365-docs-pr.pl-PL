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
description: Dowiedz się, jak przenieść swoją firmę z usługi Microsoft 365 Business Premium do platformy Microsoft 365 E3.
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126206"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrowanie z usługi Microsoft 365 Business Premium do platformy Microsoft 365 E3

Usługa Microsoft 365 Business Premium oferuje wszystko, czego potrzebujesz dla Twojej małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają Twoim pracownikom wydajną pracę. Jednak w niektórych przypadkach może być konieczne przeprowadzenie migracji subskrypcji platformy Microsoft 365 Business Premium do platformy Microsoft 365 E3. 

Na przykład Twoja firma rozrosła się i potrzebuje ponad 300 licencji (gratulacje, przy okazji).

Albo Twoja firma potrzebuje funkcji dla przedsiębiorstw, takich jak aplikacje Microsoft 365 dla przedsiębiorstw, licencje CALs (Enterprise Client Access License) dla systemu Windows 10 Enterprise lub Enterprise Client Access License.

Uaktualnienie jest łatwe: możesz rozpocząć uaktualnienie [z centrum administracyjnego.](../commerce/subscriptions/upgrade-to-different-plan.md) Wszystkie dane i konfiguracja w bieżącej subskrypcji są zachowywane. Nie musisz nic robić, aby przygotować się do migracji i nie musisz później nic robić, poza skorzystaniem z nowych funkcji.

>[!Note]
>Możesz również użyć subskrypcji usługi Microsoft 365 Business Premium dla maksymalnie 300 stanowisk i uzyskać subskrypcję Microsoft 365 E3 dla ponad 300 stanowisk. Program Microsoft Defender dla Office 365 nie jest jednak dołączony do platformy Microsoft 365 E3. W celu dalszej ochrony przed zagrożeniami należy dodać kolejne licencje usługi Defender dla usługi Office 365, aby wszyscy użytkownicy w zakresie działań w ramach działań w ramach programu Defender dla usługi Office 365 posiadali licencje.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Różnice między usługami Microsoft 365 Business Premium i Microsoft 365 Enterprise

W poniższej tabeli przedstawiono różnice między usługami Microsoft 365 Business Premium i Microsoft 365 E3.

| Funkcja    | Pomoc techniczna w uwitrynie Microsoft 365 Business Premium    | Pomoc techniczna na microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikacje pakietu Office*    | [Aplikacje Microsoft 365 dla firm](#office-365-business)    | Aplikacje Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje zwiększające produktywność w chmurze**        | | | 
| Exchange Online i Outlook    | Limit miejsca do magazynowania 50 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online    | Limit przestrzeni dyskowej 100 GB na skrzynkę pocztową i nieograniczona archiwizacja w u usługi Exchange Online | 
| Teams    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | Limit przestrzeni dyskowej do 1 TB na użytkownika    | Bez ograniczeń | 
| Yammer, SharePoint Online, Planner, Stream    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| MileIQ    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrona przed zagrożeniami**        | | | 
| Funkcje zmniejszania powierzchni ataków    | [Zobacz tę listę](#threat-protection) | Zarządzanie przedsiębiorstwem izolacji na podstawie sprzętu dla programu Microsoft Edge | 
| Defender dla Office 365 (plan 1) | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | Nie są uwzględniane, ale można dodać do | 
| **Zarządzanie tożsamościami**        | | | 
| Samodzielne resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego usługi Azure AD, dostępu warunkowego, zapisu zwrotnego haseł dla tożsamości lokalnych|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Odnajdowanie aplikacji w chmurze, usługa Azure AD Connect Health    |     | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Aplikacje usługi Azure AD usługi Office 365 single Sign-On (SSO): 10 aplikacji na użytkownika (aplikacje Galerii SaaS, takie jak Salesforce)* | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Logowanie jednokrotne usługi Azure AD Premium 1: bez ograniczeń (aplikacje lokalne za pośrednictwem serwera proxy aplikacji usługi Azure AD i aplikacje nieu galerii przy użyciu szablonów integracji aplikacji usługi Self-Service)    |     | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Zarządzanie urządzeniami i aplikacją**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|Virtual Desktop Access (VDA)    |  |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|Pulpit wirtualny systemu Windows (WVD)    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
|Aktywacja na komputerze udostępnionym (SCA, Shared Computer Activation)    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Pakiet optymalizacji pulpitu firmy Microsoft    | |     ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrona informacji**        | | | 
| Ochrona przed utratą danych w usłudze Office 365, Azure Information Protection Plan 1    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Ochrona informacji o oknie dla ochrony przed DLP punktu końcowego    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Licencja dostępu klienta (prawa cal)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Menedżer konfiguracji, Windows Rights Management)| |         ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| **Zgodność**        | | | 
| Nieograniczona archiwizacja wiadomości e-mail    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Menedżer zgodności    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| zbierania elektronicznych materiałów dowodowych    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Zawieszenie w miejscu i postępowanie sądowe    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do platformy Microsoft 365 E3](../media/check-mark.png) | 
| Tagi przechowywania i zasady przechowywania zarządzania rekordami wiadomości (MRM)    | ![Dołączone do usługi Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączona do platformy Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Użytkownicy, którym przypisano dostęp do aplikacji SaaS, mogą uzyskać dostęp do logowania jednokrotnego do maksymalnie 10 aplikacji. Administratorzy mogą konfigurować logowanie jednokrotne i zmieniać dostęp użytkowników do różnych aplikacji SaaS, ale dostęp do logowania jednokrotnego jest dozwolony tylko dla 10 aplikacji na użytkownika jednocześnie. Wszystkie aplikacje usługi Office 365 są liczone jako jedna aplikacja.

## <a name="migration"></a>Migracja

Aby przeprowadzić migrację, we współpracy z partnerem przenieś subskrypcję i licencje Microsoft 365 Business Premium do odpowiedniej subskrypcji Microsoft 365 E3 wraz z jej licencjami.

W poniższych sekcjach opisano, jakie zmiany należy wprowadzić, jeśli są, oraz co można zrobić po migracji.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Dane i konfiguracja subskrypcji platformy Microsoft 365

Nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych przed migracją, co obejmuje:

- Konfiguracja subskrypcji, taka jak nazwy domen DNS.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usługi zwiększającej produktywność i ich dane, takie jak zespoły, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.

Użytkownicy mogą teraz korzystać z nieograniczonej przestrzeni dyskowej w skrzynkach pocztowych usługi Exchange Online i folderach usługi OneDrive dla Firm.

Możesz zacząć korzystać z funkcji odnajdowania aplikacji w chmurze, usługi Azure AD Connect Health i logowania jednokrotnego dla ponad 10 aplikacji.

>[!Note]
>Użytkownicy zmigrowany do platformy Microsoft 365 E3 nie mogą już korzystać z usługi MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrona przed zagrożeniami

System Windows 10 Business zapewnia następujące zabezpieczenia:

- Wymuszanie integralności procesu rozruchu systemu operacyjnego
- Wymuszanie integralności poufnych składników operacyjnych
- Zaawansowana luki w zabezpieczeniach i środki zaradcze wykorzystujące luki w zabezpieczeniach typu "zero-day"
- Ochrona sieci oparta na reputacji dla przeglądarek Microsoft Edge, Internet Explorer i Chrome
- Zapora oparta na hoście
- Środki zaradcze oprogramowania wymuszającego okup
- Izolowanie oparte na sprzęcie dla programu Microsoft Edge
- Sterowanie aplikacją obsługiwane przez funkcja Intelligent Security Graph
- Sterowanie urządzeniem (USB)
- Ochrona sieci przed zagrożeniami internetowymi
- Reguły zapobiegania intruzom hostów

System Windows 10 Enterprise E3 obejmuje również zarządzanie przedsiębiorstwem izolacji na podstawie sprzętu dla programu Microsoft Edge.

>[!Note]
>Użytkownicy migrowany do platformy Microsoft 365 E3 będą wymagali licencji programu Microsoft Defender dla usługi Office 365 na kontynuowanie ochrony przed zagrożeniami. Pamiętaj o zakupie dodatkowych licencji usługi Defender dla usługi Office 365, tak aby wszyscy użytkownicy korzystający z usług Defender dla office 365 posiadali licencje. 
>

### <a name="device-management-with-intune"></a>Zarządzanie urządzeniami za pomocą usługi Intune

Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, która obejmuje zarejestrowane urządzenia oraz ustawienia urządzeń i aplikacji.

### <a name="windows-10"></a>Windows 10

Usługa Microsoft 365 Business Premium zawiera system Windows 10 Business, który można zainstalować za pomocą rozwiązania Windows AutoPilot. Podczas migracji do platformy Microsoft 365 E3 każda licencja użytkownika obejmuje system Windows 10 Enterprise E3, który można również zainstalować za pomocą rozwiązania Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikacje Microsoft 365 dla firm

Klient aplikacji Microsoft 365 dla firm zainstalowany na Twoich urządzeniach automatycznie zacznie korzystać z funkcji aplikacji platformy Microsoft 365 dla przedsiębiorstw. Po migracji możesz teraz użyć:

 - zasady grupy pomocy technicznej
 - Porównywanie arkuszy kalkulacyjnych i inquire
 - Funkcje analizy biznesowej

