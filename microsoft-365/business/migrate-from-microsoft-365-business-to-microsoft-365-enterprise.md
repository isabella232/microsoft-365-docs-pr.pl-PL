---
title: Migrowanie z Microsoft 365 Business do Microsoft 365 E3
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
description: Dowiedz się, jak przenieść firmę z Microsoft 365 Business Premium do Microsoft 365 E3.
ms.openlocfilehash: d3030518f7f4467c7b2e16897dc7b100764d9d5a36c50169b58f1adcd7bef209
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837648"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrowanie z Microsoft 365 Business Premium do Microsoft 365 E3

Microsoft 365 Business Premium wszystko, czego potrzebujesz dla Twojej małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają Twoim pracownikom wydajną pracę. W niektórych przypadkach może być jednak konieczne przeprowadzenie migracji subskrypcji Microsoft 365 Business Premium do Microsoft 365 E3.

Na przykład Twoja firma wyrosła i potrzebuje ponad 300 licencji (gratulacje, przy okazji).

Twoja firma potrzebuje funkcji dla przedsiębiorstw, takich jak licencje Aplikacje Microsoft 365 dla przedsiębiorstw, Windows 10 Enterprise E3 lub licencje dostępu Enterprise klienta.

Uaktualnienie jest łatwe: możesz rozpocząć uaktualnienie [z centrum administracyjnego.](../commerce/subscriptions/upgrade-to-different-plan.md) Wszystkie Dane i konfiguracja w bieżącej subskrypcji są zachowywane. Nie musisz nic robić, aby przygotować się do migracji i po jej zakończeniu nic nie robić, z wyjątkiem skorzystania z nowych funkcji.

> [!NOTE]
> Możesz także użyć subskrypcji Microsoft 365 Business Premium na maksymalnie 300 stanowisk i uzyskać subskrypcję Microsoft 365 E3 na ponad 300 stanowisk. Program Microsoft Defender for Office 365 nie jest jednak dołączony do Microsoft 365 E3. Aby nadal chronić przed zagrożeniami, należy dodać Office 365 Defender dla licencji usługi Office 365, aby wszyscy użytkownicy korzystający z usługi Defender for Office 365 policys posiadali licencje.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Różnice między Microsoft 365 Business Premium a Microsoft 365 Enterprise

W poniższej tabeli przedstawiono różnice między Microsoft 365 Business Premium a Microsoft 365 E3.

| Funkcja    | Pomoc techniczna w Microsoft 365 Business Premium    | Pomoc techniczna w Microsoft 365 E3 |
|:-------|:-----|:-----|
| **Lokalnie**        | | |
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office aplikacji*    | [Aplikacje Microsoft 365 dla firm](#office-365-business)    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw |
| **Aplikacje zwiększające produktywność w chmurze**        | | |
| Exchange Online i Outlook    | Limit miejsca do magazynowania 50 GB na skrzynkę pocztową i nieograniczona Exchange Online archiwizacja    | 100 GB miejsca do magazynowania na skrzynkę pocztową i nieograniczona Exchange Online archiwizacja |
| Teams    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| OneDrive dla Firm    | 1 TB miejsca do magazynowania na użytkownika    | Bez ograniczeń |
| Yammer, SharePoint Online, Planner, Stream    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| **Ochrona przed zagrożeniami**        | | |
| Możliwości zmniejszania powierzchni ataków    | [Zobacz tę listę](#threat-protection) | Enterprise zarządzania izolacji komputera opartego na sprzęcie Microsoft Edge |
| Defender dla Office 365 Plan 1 | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | Nie dołączona, ale można ją dodać do |
| **Zarządzanie tożsamościami**        | | |
| Samodzielne resetowanie hasła dla kont Azure Active Directory hybrydowych (Azure AD), uwierzytelnianie wieloskładnikowe (MFA), dostęp warunkowy, funkcja zapisu hasła dla tożsamości lokalnych|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Odnajdowanie aplikacji w chmurze, usługa Azure AD Połączenie Health    |     | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Aplikacje Azure AD Office 365 logowanie jednokrotne Sign-On jednokrotnego): 10 aplikacji na użytkownika (aplikacje Galerii SaaS, takie jak Salesforce)* | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Azure AD — wersja Premium logowania jednokrotnego 1: brak ograniczenia (aplikacje lokalne za pośrednictwem serwera proxy aplikacji usługi Azure AD i aplikacje nieseksaplikacyjne przy użyciu szablonów integracji aplikacji usługi Self-Service)    |     | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| **Zarządzanie urządzeniami i aplikacją**        | | |
| Microsoft Intune, Windows Autopilot|     ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
|Dostęp do pulpitu wirtualnego (VDA)    |  |     ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
|Windows Pulpit wirtualny (WVD)    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
|Aktywacja na komputerze udostępnionym (SCA, Shared Computer Activation)    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Pakiet optymalizacji pulpitu firmy Microsoft    | |     ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| **Ochrona informacji**        | | |
| Office 365 Ochrona przed utratą danych, Azure Information Protection Plan 1    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Ochrona informacji o oknie dla ochrony przed dlp punktu końcowego    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| **Licencja dostępu klienta (prawa calowe)**    | | |
| Enterprise Pakiet CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows zarządzania prawami dostępu)| |         ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| **Zgodność**        | | |
| Nieograniczona archiwizacja wiadomości e-mail    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Menedżer zgodności    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| zbierania elektronicznych materiałów dowodowych    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Zawieszenie w miejscu i postępowanie sądowe    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
| Tagi przechowywania rekordów wiadomości (MRM) i zasady przechowywania    | ![Dołączone do Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dołączone do Microsoft 365 E3](../media/check-mark.png) |
||||

\* Użytkownicy z przypisanym dostępem do aplikacji SaaS mogą uzyskać dostęp do logowania jednokrotnego do maksymalnie 10 aplikacji. Administratorzy mogą konfigurować logowanie jednokrotne i zmieniać dostęp użytkowników do różnych aplikacji SaaS, ale dostęp do logowania jednokrotnego jest dozwolony tylko dla 10 aplikacji na użytkownika jednocześnie. Wszystkie Office 365 są liczone jako jedna aplikacja.

## <a name="migration"></a>Migracja

Aby przeprowadzić migrację, we współpracy z partnerem przenieś subskrypcję usługi Microsoft 365 Business Premium licencje do odpowiedniej Microsoft 365 E3 subskrypcji wraz z jego licencjami.

W poniższych sekcjach opisano, jakie zmiany należy wprowadzić (o ile są) i co można zrobić po migracji.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 konfiguracji i danych subskrypcji

Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:

- Konfiguracja subskrypcji, taka jak nazwy domen DNS.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usługi zwiększającej produktywność i ich dane, takie Teams, Exchange Online pocztowe, SharePoint online, OneDrive dla Firm foldery i OneNote notesy.

Użytkownicy mogą teraz korzystać z nieograniczonej przestrzeni dyskowej w Exchange Online skrzynek pocztowych i OneDrive dla Firm folderach.

Możesz rozpocząć korzystanie z odnajdowania aplikacji w chmurze, usługi Azure AD Połączenie Health i logowania jednokrotnego dla ponad 10 aplikacji.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrona przed zagrożeniami

Windows 10 Business obejmuje następujące zabezpieczenia:

- Wymuszanie integralności procesu rozruchu systemu operacyjnego
- Wymuszanie integralności wrażliwych składników operacyjnych
- Zaawansowana luki w zabezpieczeniach i środki zaradcze wykorzystujące bezbłędne wykorzystywanie luk
- Ochrona sieci oparta na reputacji dla przeglądarek Microsoft Edge, Internet Explorer i Chrome
- Zapora oparta na hoście
- Środki zaradcze oprogramowania wymuszającego okup
- Izolacja komputera oparta na sprzęcie Microsoft Edge
- Sterowanie aplikacją obsługiwane przez inteligentne zabezpieczenia Graph
- Sterowanie urządzeniem (USB)
- Ochrona sieci przed zagrożeniami internetowymi
- Reguły ochrony przed nieuprawnianiem hostów

Windows 10 Enterprise E3 obejmuje również zarządzanie w przedsiębiorstwie izolacji na podstawie sprzętu Microsoft Edge.

> [!NOTE]
> Użytkownicy, którzy migrowali Microsoft 365 E3 będą wymagać licencji usługi Microsoft Defender Office 365 do dalszej ochrony przed zagrożeniami. Pamiętaj o zakupie dodatkowej usługi Defender Office 365 licencji, aby wszyscy użytkownicy, którzy mają dostęp do usługi Defender for Office 365, posiadali licencje.

### <a name="device-management-with-intune"></a>Zarządzanie urządzeniami za pomocą usługi Intune

Przed rozpoczęciem migracji nie musisz wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, która obejmuje zarejestrowane urządzenia oraz ustawienia urządzenia i aplikacji.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium zawiera Windows 10 Business, którą można zainstalować za pomocą rozwiązania Windows AutoPilot. Podczas migracji do programu Microsoft 365 E3 licencja każdego użytkownika obejmuje Windows 10 Enterprise E3, którą można również zainstalować za pomocą rozwiązania Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikacje Microsoft 365 dla firm

Twój Aplikacje Microsoft 365 dla firm zainstalowany na Twoich urządzeniach automatycznie zacznie korzystać z funkcji aplikacji Aplikacje Microsoft 365 dla przedsiębiorstw. Po zakończeniu migracji możesz teraz użyć:

- zasady grupy pomocy technicznej
- Porównywanie arkuszy kalkulacyjnych i inquire
- Analizę biznesową
