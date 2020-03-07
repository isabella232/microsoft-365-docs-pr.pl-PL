---
title: Zabezpieczanie urządzeń z systemem Windows 10
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Dowiedz się więcej o konfigurowaniu ustawień domyślnych zasad urządzenia, które każde urządzenie z systemem Windows 10 otrzyma po zalogowaniu się na swoje konto służbowe.
ms.openlocfilehash: dfa6aca1f12ab37b8b0926dea4a6a79c934b1250
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561285"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="b49ca-103">Zabezpieczanie urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="b49ca-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="b49ca-104">Konfigurowane w tym miejscu ustawienia są częścią domyślnych zasad dotyczących urządzeń dla systemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b49ca-104">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="b49ca-105">Wszyscy użytkownicy, którzy podłączą urządzenie z systemem Windows 10, w tym urządzenia przenośne i komputery, logując się za pomocą swojego konta służbowego, automatycznie otrzymają te ustawienia.</span><span class="sxs-lookup"><span data-stu-id="b49ca-105">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="b49ca-106">Zalecane jest zaakceptowanie domyślnych zasad podczas instalacji i dodanie w późniejszym terminie zasad dotyczących konkretnych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="b49ca-106">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="b49ca-107">Ustawienia zabezpieczające urządzenia z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="b49ca-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="b49ca-p102">Domyślnie wszystkie ustawienia są **Włączone**. Dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="b49ca-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b49ca-110">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="b49ca-110">Setting</span></span>  <br/> |<span data-ttu-id="b49ca-111">Opis</span><span class="sxs-lookup"><span data-stu-id="b49ca-111">Description</span></span>  <br/> |
|<span data-ttu-id="b49ca-112">Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="b49ca-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="b49ca-113">Wymaga włączenia programu antywirusowego Windows Defender w celu ochrony komputerów przed zagrożeniami związanymi z połączeniem z Internetem.</span><span class="sxs-lookup"><span data-stu-id="b49ca-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="b49ca-114">Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b49ca-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="b49ca-115">Włącza w programie Microsoft Edge ustawienia ułatwiające ochronę użytkowników przed złośliwymi witrynami i złośliwą zawartością do pobrania.</span><span class="sxs-lookup"><span data-stu-id="b49ca-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="b49ca-116">Wyłącz ekran urządzenia po takim czasie bezczynności</span><span class="sxs-lookup"><span data-stu-id="b49ca-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="b49ca-p103">Zapewnia bezpieczeństwo danych firmowych podczas bezczynności użytkownika. Jeśli użytkownik pracuje w miejscu publicznym, na przykład kawiarni, i odejdzie na chwilę od urządzenia lub skupi uwagę na czymś innym, przypadkowe osoby mogą obejrzeć zawartość ekranu. To ustawienie pozwala kontrolować czas bezczynności użytkownika, po którym ekran zostanie wyłączony.</span><span class="sxs-lookup"><span data-stu-id="b49ca-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="b49ca-120">Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="b49ca-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="b49ca-p104">Pozwala użytkownikom pobierać i instalować aplikacje z witryny Microsoft Store. Do aplikacji tych należą zarówno gry, jak i narzędzia biurowe, więc zostawiamy to ustawienie **włączone**, ale możesz je wyłączyć w celu dodatkowego zwiększenia bezpieczeństwa.  </span><span class="sxs-lookup"><span data-stu-id="b49ca-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="b49ca-123">Zezwalaj użytkownikom na korzystanie z Cortany</span><span class="sxs-lookup"><span data-stu-id="b49ca-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="b49ca-124">Cortana może być bardzo pomocna.</span><span class="sxs-lookup"><span data-stu-id="b49ca-124">Cortana can be very helpful!</span></span> <span data-ttu-id="b49ca-125">Cortana może włączać lub wyłączać ustawienia, udzielać wskazówek dojazdu i mieć pewność, że jesteś na czas na terminy, więc domyślnie to ustawienie jest **włączone.**</span><span class="sxs-lookup"><span data-stu-id="b49ca-125">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="b49ca-126">Zezwalaj użytkownikom na otrzymywanie porad i reklam dotyczących systemu Windows od firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="b49ca-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="b49ca-127">Porady dotyczące systemu Windows mogą być przydatne i ułatwiać użytkownikom zapoznawanie się nowymi funkcjami.</span><span class="sxs-lookup"><span data-stu-id="b49ca-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="b49ca-128">Automatycznie aktualizuj urządzenia z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="b49ca-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="b49ca-129">Zapewnia, że urządzenia z systemem Windows 10 automatycznie otrzymują najnowsze aktualizacje.</span><span class="sxs-lookup"><span data-stu-id="b49ca-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

