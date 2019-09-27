---
title: Zabezpieczanie urządzeń z systemem Windows 10
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Dowiedz się więcej o domyślnych i innych ustawieniach, aby zabezpieczyć urządzenia z systemem Windows 10. '
ms.openlocfilehash: c2607b026bca582afcea76d4c0b3e8088c00252d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288650"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="04e75-103">Zabezpieczanie urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="04e75-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="04e75-p101">Konfigurowane w tym miejscu ustawienia są częścią domyślnych zasad dotyczących urządzeń dla systemu Windows 10. Wszyscy użytkownicy, którzy łączą się z urządzeniami z systemem Windows 10 (w tym z urządzeniami przenośnymi i komputerami), logując się przy użyciu swojego konta służbowego, automatycznie otrzymają te ustawienia. Zalecane jest zaakceptowanie domyślnych zasad podczas instalacji i dodanie w późniejszym terminie zasad dotyczących konkretnych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="04e75-p101">The settings that you configure here are part of the default device policy for Windows 10. All users that connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account, will automatically receive these settings. We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="04e75-107">Ustawienia zabezpieczające urządzenia z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="04e75-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="04e75-p102">Domyślnie wszystkie ustawienia są **Włączone**. Dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="04e75-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="04e75-110">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="04e75-110">Setting</span></span>  <br/> |<span data-ttu-id="04e75-111">Opis</span><span class="sxs-lookup"><span data-stu-id="04e75-111">Description</span></span>  <br/> |
|<span data-ttu-id="04e75-112">Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="04e75-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="04e75-113">Wymaga włączenia programu antywirusowego Windows Defender w celu ochrony komputerów przed zagrożeniami związanymi z połączeniem z Internetem.</span><span class="sxs-lookup"><span data-stu-id="04e75-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="04e75-114">Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="04e75-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="04e75-115">Włącza w programie Microsoft Edge ustawienia ułatwiające ochronę użytkowników przed złośliwymi witrynami i złośliwą zawartością do pobrania.</span><span class="sxs-lookup"><span data-stu-id="04e75-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="04e75-116">Wyłącz ekran urządzenia po takim czasie bezczynności</span><span class="sxs-lookup"><span data-stu-id="04e75-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="04e75-p103">Zapewnia bezpieczeństwo danych firmowych podczas bezczynności użytkownika. Jeśli użytkownik pracuje w miejscu publicznym, na przykład kawiarni, i odejdzie na chwilę od urządzenia lub skupi uwagę na czymś innym, przypadkowe osoby mogą obejrzeć zawartość ekranu. To ustawienie pozwala kontrolować czas bezczynności użytkownika, po którym ekran zostanie wyłączony.</span><span class="sxs-lookup"><span data-stu-id="04e75-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="04e75-120">Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="04e75-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="04e75-p104">Pozwala użytkownikom pobierać i instalować aplikacje z witryny Microsoft Store. Do aplikacji tych należą zarówno gry, jak i narzędzia biurowe, więc zostawiamy to ustawienie **włączone**, ale możesz je wyłączyć w celu dodatkowego zwiększenia bezpieczeństwa.  </span><span class="sxs-lookup"><span data-stu-id="04e75-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="04e75-123">Zezwalaj użytkownikom na korzystanie z Cortany</span><span class="sxs-lookup"><span data-stu-id="04e75-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="04e75-p105">Cortana może być bardzo pomocna. Może włączać lub wyłączać ustawienia, udzielać wskazówek i przypominać o spotkaniach, więc to ustawienie domyślnie jest **włączone**.  </span><span class="sxs-lookup"><span data-stu-id="04e75-p105">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="04e75-126">Zezwalaj użytkownikom na otrzymywanie porad i reklam dotyczących systemu Windows od firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="04e75-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="04e75-127">Porady dotyczące systemu Windows mogą być przydatne i ułatwiać użytkownikom zapoznawanie się nowymi funkcjami.</span><span class="sxs-lookup"><span data-stu-id="04e75-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="04e75-128">Automatycznie aktualizuj urządzenia z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="04e75-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="04e75-129">Zapewnia, że urządzenia z systemem Windows 10 automatycznie otrzymują najnowsze aktualizacje.</span><span class="sxs-lookup"><span data-stu-id="04e75-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

