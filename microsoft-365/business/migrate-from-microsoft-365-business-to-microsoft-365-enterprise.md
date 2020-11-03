---
title: Migrowanie z programu Microsoft 365 Business do firmy Microsoft 365 E3
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
description: Dowiedz się, jak przenieść firmę z witryny Microsoft 365 Business Premium do firmy Microsoft 365 E3.
ms.openlocfilehash: 874da0d35759c8af4c3ee2ca4a1bdfa90a91627c
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842205"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrowanie z usługi Microsoft 365 Business Premium do firmy Microsoft 365 E3

Aplikacja Microsoft 365 Business Premium ma wszystko, czego potrzebujesz dla małych firm, łącząc aplikacje biurowe najlepiej obsługujące się w chmurze z prostym zarządzaniem urządzeniami i zabezpieczeniami, które umożliwiają pracownikom wykonywanie ich najlepszej pracy. Jednak w niektórych przypadkach konieczne może być Migrowanie subskrypcji programu Microsoft 365 Business Premium do firmy Microsoft 365 E3. 

Na przykład Twoja firma rozwinęła się i potrzebuje więcej niż 300 licencji (Gratulacje, w drodze).

Ponadto firma potrzebuje funkcji organizacji, takich jak aplikacje Microsoft 365 dla przedsiębiorstw, Windows 10 Enterprise E3 lub licencje dostępu klienta (CAL) dla przedsiębiorstw.

Uaktualnienie jest proste: możesz rozpocząć uaktualnianie [w centrum administracyjnym](../commerce/subscriptions/upgrade-to-different-plan.md). Wszystkie dane i konfiguracja w bieżącej subskrypcji są zachowywane. Nie trzeba nic robić, aby przygotować się do migracji i nic nie robić, z wyjątkiem możliwości skorzystania z nowych funkcji.

>[!Note]
>Możesz również skorzystać z abonamentu Microsoft 365 Business Premium dla maksymalnie 300 stanowisk i uzyskać abonament Microsoft 365 E3 na więcej niż 300 miejsc. Program Microsoft Defender dla Office 365 nie jest jednak dostępny w witrynie Microsoft 365 E3. Aby zapewnić ciągłą ochronę przed zagrożeniami, należy dodać dodatkowe usługi Defender for Office 365, aby uzyskać licencję wszystkich użytkowników w zakresie usługi Defender dla Office 365.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Różnice między programem Microsoft 365 Business Premium a programem Microsoft 365 Enterprise

W poniższej tabeli przedstawiono różnice między programami Microsoft 365 Business Premium i Microsoft 365 E3.

| Funkcja    | Pomoc techniczna w programie Microsoft 365 Business Premium    | Pomoc techniczna w witrynie Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalnie**        | | | 
| Windows 10    | System Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikacje pakietu Office *    | [Aplikacje Microsoft 365 dla firm](#office-365-business)    | Aplikacje usługi Microsoft 365 dla przedsiębiorstw | 
| **Aplikacje do pracy w chmurze**        | | | 
| Exchange Online i Outlook    | 50 GB limitu magazynowania na skrzynkę pocztową i funkcję archiwizacji usługi Exchange Online    | 100 GB limitu magazynowania na skrzynkę pocztową i funkcję archiwizacji usługi Exchange Online | 
| Teams    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive dla Firm    | 1 TB limitu magazynowania na użytkownika    | Czas | 
| Yammer, SharePoint Online, Planner, Stream    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Program Outlook Customer Manager, MileIQ    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrona przed zagrożeniami**        | | | 
| Funkcje ograniczania powierzchni ataku    | [Zobacz tę listę](#threat-protection) | Zarządzanie przedsiębiorstwem izolacji opartej na sprzęcie dla przeglądarki Microsoft Edge | 
| Defender dla Office 365 (plan 1) | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | Nieuwzględniona, ale można ją dodać | 
| **Zarządzanie tożsamościami**        | | | 
| Samoobsługowe resetowanie hasła dla kont hybrydowych usługi Azure Active Directory (MFA), usługi Azure Multi-Factor Authentication (MFA), dostęp warunkowy, Stornowanie hasła dla tożsamości lokalnych|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Odnajdowanie aplikacji w chmurze, usługa Azure AD Connect Health    |     | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Aplikacje usługi Azure AD Office 365 pojedyncza Sign-On (SSO): 10 aplikacji na użytkownika (aplikacje galerii SaaS, takie jak usługi Salesforce) * | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Usługa Azure AD Premium 1 SSO: brak limitu (aplikacje lokalne za pośrednictwem serwera proxy aplikacji Azure AD i aplikacji nienależących do galerii przy użyciu szablonów integracji aplikacji Self-Service)    |     | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| **Zarządzanie urządzeniami i aplikacjami**        | | | 
| Microsoft Intune, Windows dla autopilota|     ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
|Wirtualny dostęp do pulpitu (VDA)    |  |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
|Pulpit wirtualny systemu Windows (WVD)    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
|Aktywacja na komputerze współużytkowanym (BRIDGED)    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png) |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Pakiet optymalizacji Microsoft Desktop    | |     ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrona informacji**        | | | 
| Ochrona przed utratą danych w pakiecie Office 365 i usługa Azure Information Protection Plan 1    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Ochrona informacji o oknach dla punktu końcowego DLP    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| **Licencja dostępu klienta (prawa CAL)**    | | |     
| Pakiet Enterprise CAL (Exchange, SharePoint, Skype, Windows, Menedżer konfiguracji programu Microsoft Endpoint, zarządzanie prawami dostępu w systemie Windows)| |         ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| **Spełnienia**        | | | 
| Archiwizowanie wiadomości e-mail bez ograniczeń    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Menedżer zgodności    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Materiałów    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Przechowywanie w miejscu i w ramach postępowania sądowego    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
| Znaczniki przechowywania i zasady przechowywania rekordów funkcji zarządzania rekordami wiadomości (MRM)    | ![Dostępne w programie Microsoft 365 Business Premium](../media/check-mark.png)    | ![Dostępne w programie Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Użytkownicy, którym przypisano dostęp do aplikacji SaaS, mogą uzyskać dostęp SSO do 10 aplikacji. Administratorzy mogą konfigurować Logowanie jednokrotne i zmieniać dostęp użytkowników do różnych aplikacji SaaS, ale dostęp SSO jest dozwolony tylko dla 10 aplikacji na użytkownika naraz. Wszystkie aplikacje pakietu Office 365 są liczone jako pojedyncza aplikacja.

## <a name="migration"></a>Migracj

Aby przeprowadzić migrację, należy współpracować z partnerem w celu przeniesienia abonamentu i licencji programu Microsoft 365 Business Premium na odpowiednią subskrypcję Microsoft 365 E3 z jej licencjami.

W poniższych sekcjach opisano, jakie zmiany należy wprowadzić, jeśli istnieją, oraz jakie czynności można wykonać po zakończeniu migracji.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfiguracja i dane subskrypcji programu Microsoft 365

Przed przeprowadzeniem migracji nie trzeba wprowadzać żadnych zmian w bieżącym abonamentu ani danych, co obejmuje następujące funkcje:

- Konfiguracja subskrypcji, na przykład nazwy domen DNS.
- Konta użytkowników i grup oraz ustawienia uwierzytelniania, takie jak uwierzytelnianie wieloskładnikowe lub zasady dostępu warunkowego.
- Konfiguracje usług biurowych i ich dane, takie jak zespoły, skrzynki pocztowe usługi Exchange Online, witryny usługi SharePoint Online, foldery usługi OneDrive dla firm i Notesy programu OneNote.

Użytkownicy mogą teraz korzystać z przestrzeni dyskowej bez ograniczeń w folderach skrzynek pocztowych Exchange Online i OneDrive dla firm.

Możesz zacząć korzystać z funkcji Odnajdowanie aplikacji w chmurze, Azure AD Connect Health i SSO na więcej niż 10 aplikacji.

>[!Note]
>Użytkownicy zmigrowani do programu Microsoft 365 E3 nie mogą już używać aplikacji Outlook Customer Manager i MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrona przed zagrożeniami

System Windows 10 Business obejmuje następujące funkcje:

- Proces wdrażania integralności procesu uruchamiania systemu operacyjnego
- Egzekwowanie integralności wrażliwych składników operacyjnych
- Zaawansowana Luka w zabezpieczeniach oraz łagodzenie wykorzystania zer
- Ochrona sieci oparta na reputacji w programie Microsoft Edge, Internet Explorer i w programie Chrome
- Zapora oparta na hoście
- Ograniczenia dotyczące oprogramowania wymuszającego okup
- Izolacja sprzętowa przeglądarki Microsoft Edge
- Sterowanie aplikacjami obsługiwane przez wykres inteligentne zabezpieczenia
- Sterowanie urządzeniem (USB)
- Ochrona sieci na potrzeby zagrożeń opartych na sieci Web
- Reguły zapobiegania włamaniom hosta

System Windows 10 Enterprise E3 obejmuje również zarządzanie przedsiębiorstwem izolacji opartej na sprzęcie dla przeglądarki Microsoft Edge.

>[!Note]
>Użytkownicy zmigrowani do programu Microsoft 365 E3 będą musieli uzyskać licencję usługi Microsoft Defender for Office 365 na kontynuację ochrony przed zagrożeniami. Pamiętaj, aby zakupić dodatkowe usługi Defender dla licencji Office 365, aby uzyskać licencję wszystkich użytkowników w zakresie usługi Defender dla Office 365. 
>

### <a name="device-management-with-intune"></a>Zarządzanie urządzeniami za pomocą usługi Intune

Przed przeprowadzeniem migracji nie trzeba wprowadzać żadnych zmian w bieżącej konfiguracji usługi Intune, obejmującym zarejestrowane urządzenia i ustawienia urządzeń oraz aplikacji.

### <a name="windows-10"></a>Windows 10

Pakiet Microsoft 365 Business Premium obejmuje system Windows 10 Business, który można zainstalować za pomocą autopilota systemu Windows. Podczas migrowania do programu Microsoft 365 E3 każda Licencja użytkownika obejmuje system Windows 10 Enterprise E3, który można też zainstalować za pomocą autopilota systemu Windows.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikacje Microsoft 365 dla firm

Program Microsoft 365 Apps dla firm zainstalowany na urządzeniach automatycznie rozpocznie korzystanie z funkcji aplikacji Microsoft 365 w wersji Enterprise. Po zakończeniu migracji możesz teraz używać następujących czynności:

 - Aktywacja Zbiorcza za pomocą zasad grupy
 - Telemetria aplikacji
 - Aktualizowanie kontrolek
 - Porównywanie arkuszy kalkulacyjnych i zapytanie
 - Analiza biznesowa

