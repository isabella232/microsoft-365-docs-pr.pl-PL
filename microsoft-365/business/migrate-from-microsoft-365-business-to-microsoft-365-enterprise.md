---
title: Migracja z usługi Microsoft 365 Business do usługi Microsoft 365 E3
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
description: Dowiedz się, jak przenieść firmę z usługi Microsoft 365 Business Premium na usługę Microsoft 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081870"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migracja z usługi Microsoft 365 Business Premium do usługi Microsoft 365 E3

Usługa Microsoft 365 Business Premium ma wszystko, czego potrzebujesz dla małej firmy, łącząc najlepsze w swojej klasie aplikacje zwiększające produktywność w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają pracownikom najlepszą pracę. W niektórych przypadkach może być jednak konieczne migracja subskrypcji usługi Microsoft 365 Business Premium do usługi Microsoft 365 E3. 

Na przykład Twoja firma rozrosła się i potrzebuje ponad 300 licencji (gratulacje, nawiasem mówiąc).

Twoja firma potrzebuje też funkcji korporacyjnych, takich jak Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3 lub Enterprise Client Access Licenses (CAL).

Uaktualnienie jest łatwe: uaktualnienie można rozpocząć [w centrum administracyjnym](../commerce/subscriptions/upgrade-to-different-plan.md). Wszystkie dane i konfiguracja w bieżącej subskrypcji są obsługiwane. Nie ma nic do zrobienia, aby przygotować się do migracji i nic do zrobienia później, z wyjątkiem skorzystać z nowych funkcji.

>[!Note]
>Możesz również użyć subskrypcji Usługi Microsoft 365 Business Premium dla maksymalnie 300 miejsc i uzyskać subskrypcję usługi Microsoft 365 E3 na ponad 300 miejsc. Jednak usługa Office 365 ATP nie jest dołączona do usługi Microsoft 365 E3. Aby zapewnić ciągłą ochronę przed zagrożeniami, należy dodać dodatkowe licencje usługi Office 365 ATP, aby wszyscy użytkownicy w zakresie twoich policyjnych pakietów Office 365 ATP podlegali licencji.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Różnice między microsoft 365 Business Premium i Microsoft 365 Enterprise

W tej tabeli przedstawiono różnice między usłudze Microsoft 365 Business Premium a microsoftem 365 E3.

| Funkcja    | Pomoc techniczna w usłudze Microsoft 365 Business Premium    | Pomoc techniczna w usłudze Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Windows 10    | Windows 10 Biznes  |     Windows 10 Enterprise E3| 
| Aplikacje pakietu Office*    | [Aplikacje usługi Microsoft 365 dla firm](#office-365-business)    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje zwiększające produktywność w chmurze**        | | | 
| Usługa Exchange Online i Outlook    | Limit miejsca 50 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online    | Limit miejsca 100 GB na skrzynkę pocztową i nieograniczona archiwizacja usługi Exchange Online | 
| Zespołów    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | Limit pojemności 1 TB na użytkownika    | Nieograniczony | 
| Yammer, SharePoint Online, Planner, Strumień    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Menedżer klienta programu Outlook, MileIQ    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrona przed zagrożeniami**        | | | 
| Możliwości redukcji powierzchni ataku    | [Zobacz tę listę](#threat-protection) | Zarządzanie izolacją sprzętową w przedsiębiorstwie dla przeglądarki Microsoft Edge | 
| Plan 1 zaawansowanej ochrony przed zagrożeniami usługi Office 365 | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | Nie jest dołączony, ale można go dodać na | 
| **Zarządzanie tożsamościami**        | | | 
| Samoobsługowe resetowanie hasła dla hybrydowych kont usługi Azure Active Directory (Azure AD), uwierzytelniania wieloskładnikowego platformy Azure (MFA), dostępu warunkowego, zapisywania haseł dla tożsamości lokalnych|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Odnajdowanie aplikacji w chmurze, kondycja usługi Azure AD Connect    |     | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Aplikacje usługi Azure AD Office 365 Logowanie jednokrotne (logowanie jednokrotne): 10 aplikacji na użytkownika (aplikacje SaaS galerii, takie jak Salesforce)* | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Samoustawne samouszczenia usługi Azure AD Premium 1: bez limitu (aplikacje lokalne za pośrednictwem serwera proxy aplikacji usługi Azure AD i aplikacji innych niż galeria przy użyciu szablonów integracji aplikacji samoobsługowych)    |     | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| **Zarządzanie urządzeniami i aplikacjami**        | | | 
| Microsoft Intune, Windows Autopilot|     ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
|Dostęp do pulpitu wirtualnego (VDA)    |  |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
|Pulpit wirtualny systemu Windows (WVD)    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png) |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
|Aktywacja komputera udostępnionego (SCA)    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png) |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Pakiet optymalizacji pulpitu firmy Microsoft    | |     ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrona informacji**        | | | 
| Zapobieganie utracie danych w usłudze Office 365, plan ochrony informacji platformy Azure 1    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Ochrona informacji o oknie dla punktu końcowego DLP    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| **Licencja dostępu klienta (prawa CAL)**    | | |     
| Pakiet CAL dla przedsiębiorstw (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Zarządzanie prawami systemu Windows)| |         ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| **Zgodności**        | | | 
| Nieograniczona archiwizacja poczty e-mail    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Menedżer wyników/zgodności zgodności    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Zbierania elektronicznych materiałów dowodowych    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Wstrzymanie i zawieszenie w postępowaniu sądowym    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
| Tagi przechowywania i zasady przechowywania usługi Zarządzanie rekordami wiadomości (MRM)    | ![W zestawie z programem Microsoft 365 Business Premium](../media/check-mark.png)    | ![W zestawie z programem Microsoft 365 E3](../media/check-mark.png) | 
||||

\*Użytkownicy, którym przypisano dostęp do aplikacji SaaS, mogą uzyskać dostęp do aplikacji SSO do maksymalnie 10 aplikacji. Administratorzy mogą konfigurować jednokrotne i zmieniać dostęp użytkownika do różnych aplikacji SaaS, ale dostęp do jednokrotnego dostępu jest dozwolony tylko dla 10 aplikacji na użytkownika naraz. Wszystkie aplikacje usługi Office 365 są liczone jako pojedyncza aplikacja.

## <a name="migration"></a>Migracji

Aby przeprowadzić migrację, skontaktuj się z partnerem, aby przenieść subskrypcję i licencje usługi Microsoft 365 Business Premium do odpowiedniej subskrypcji Usługi Microsoft 365 E3 z licencjami.

W poniższych sekcjach opisano, jakie zmiany należy wprowadzić, jeśli istnieją, i co można zrobić po migracji.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfiguracja i dane subskrypcji usługi Microsoft 365

Przed migracją nie trzeba wprowadzać żadnych zmian w bieżącej subskrypcji ani danych, co obejmuje:

- Konfiguracja subskrypcji, na przykład nazwy domen DNS.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usług zwiększających produktywność i ich dane, takie jak usługi Teams, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla Firm i notesy programu OneNote.

Użytkownicy mogą teraz korzystać z nieograniczonej przestrzeni dyskowej w skrzynkach pocztowych usługi Exchange Online i w folderach usługi OneDrive dla Firm.

Możesz rozpocząć korzystanie z odnajdowania aplikacji w chmurze, usługi Azure AD Connect Health i aplikacji SSO dla ponad 10 aplikacji.

>[!Note]
>Użytkownicy migrowani do usługi Microsoft 365 E3 nie mogą już korzystać z programu Outlook Customer Manager i MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrona przed zagrożeniami

System Windows 10 Business zawiera następujące zabezpieczenia:

- Wymuszanie integralności procesu rozruchu systemu operacyjnego
- Egzekwowanie integralności wrażliwych komponentów operacyjnych
- Zaawansowane środki zmniejszające podatność na zagrożenia i luki w zabezpieczeniach typu zero-day
- Ochrona sieciowa oparta na reputacji dla przeglądarki Microsoft Edge, Internet Explorer i Chrome
- Zapora oparta na hoście
- Środki zaradcze związane z oprogramowaniem wymuszającym okup
- Izolacja sprzętowa dla przeglądarki Microsoft Edge
- Sterowanie aplikacjami obsługiwane przez inteligentny wykres zabezpieczeń
- Sterowanie urządzeniem (USB)
- Ochrona sieci w przypadku zagrożeń internetowych
- Zasady zapobiegania włamaniom hosta

System Windows 10 Enterprise E3 obejmuje również zarządzanie izolacją sprzętową dla przeglądarki Microsoft Edge w przedsiębiorstwie.

>[!Note]
>Użytkownicy migrowani do usługi Microsoft 365 E3 będą wymagać licencji usługi Office 365 ATP w celu ciągłej ochrony przed zagrożeniami. Pamiętaj, aby zakupić dodatkowe licencje usługi Office 365 ATP, aby wszyscy użytkownicy w zakresie twoich policyjnych usługi Office 365 ATP były licencjonowane. 
>

### <a name="device-management-with-intune"></a>Zarządzanie urządzeniami za pomocą usługi Intune

Przed migracją nie trzeba wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, która obejmuje zarejestrowane urządzenia oraz ustawienia urządzeń i aplikacji.

### <a name="windows-10"></a>Windows 10

Usługa Microsoft 365 Business Premium zawiera system Windows 10 Business, który można zainstalować za pomocą programu Windows AutoPilot. Podczas migracji do usługi Microsoft 365 E3 każda licencja użytkownika zawiera system Windows 10 Enterprise E3, który można również zainstalować za pomocą programu Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikacje usługi Microsoft 365 dla firm

Klient usługi Microsoft 365 Apps dla firm zainstalowany na twoich urządzeniach automatycznie zacznie korzystać z funkcji aplikacji usługi Microsoft 365 dla przedsiębiorstw. Po migracji można teraz użyć:

 - Aktywacja zbiorcza za pośrednictwem zasad grupy
 - Telemetria aplikacji
 - Kontrolki aktualizacji
 - Porównywanie arkuszy kalkulacyjnych i uzyskiwanie pytań
 - Analityka biznesowa

