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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Dowiedz się, jak skonfigurować ustawienia domyślnych zasad urządzeń, które zostaną odebrane przez dowolne urządzenie z systemem Windows 10 po zalogowaniu się do swojego konta służbowego.
ms.openlocfilehash: b586e687d6b61873b77fac8586396ab51fd90b9b
ms.sourcegitcommit: 90efec455336b4cecc06a8cbf0ce287740433523
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/26/2020
ms.locfileid: "46898073"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="bb7b5-103">Zabezpieczanie urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="bb7b5-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="bb7b5-104">Ten artykuł dotyczy programu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="bb7b5-105">Konfigurowane w tym miejscu ustawienia są częścią domyślnych zasad dotyczących urządzeń dla systemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="bb7b5-106">Wszyscy użytkownicy łączący urządzenie z systemem Windows 10, w tym urządzenia przenośne i komputery PC, logując się przy użyciu swojego konta służbowego, będą automatycznie otrzymywały te ustawienia.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="bb7b5-107">Zalecane jest zaakceptowanie domyślnych zasad podczas instalacji i dodanie w późniejszym terminie zasad dotyczących konkretnych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="bb7b5-108">Ustawienia zabezpieczające urządzenia z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="bb7b5-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="bb7b5-p102">Domyślnie wszystkie ustawienia są **Włączone**. Dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="bb7b5-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="bb7b5-111">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="bb7b5-111">Setting</span></span>  <br/> |<span data-ttu-id="bb7b5-112">Opis</span><span class="sxs-lookup"><span data-stu-id="bb7b5-112">Description</span></span>  <br/> |
|<span data-ttu-id="bb7b5-113">Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="bb7b5-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="bb7b5-114">Wymaga włączenia programu antywirusowego Windows Defender w celu ochrony komputerów przed zagrożeniami związanymi z połączeniem z Internetem.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="bb7b5-115">Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="bb7b5-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="bb7b5-116">Włącza w programie Microsoft Edge ustawienia ułatwiające ochronę użytkowników przed złośliwymi witrynami i złośliwą zawartością do pobrania.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="bb7b5-117">Wyłącz ekran urządzenia po takim czasie bezczynności</span><span class="sxs-lookup"><span data-stu-id="bb7b5-117">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="bb7b5-p103">Zapewnia bezpieczeństwo danych firmowych podczas bezczynności użytkownika. Jeśli użytkownik pracuje w miejscu publicznym, na przykład kawiarni, i odejdzie na chwilę od urządzenia lub skupi uwagę na czymś innym, przypadkowe osoby mogą obejrzeć zawartość ekranu. To ustawienie pozwala kontrolować czas bezczynności użytkownika, po którym ekran zostanie wyłączony.</span><span class="sxs-lookup"><span data-stu-id="bb7b5-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="bb7b5-121">Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="bb7b5-121">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="bb7b5-p104">Pozwala użytkownikom pobierać i instalować aplikacje z witryny Microsoft Store. Do aplikacji tych należą zarówno gry, jak i narzędzia biurowe, więc zostawiamy to ustawienie **włączone**, ale możesz je wyłączyć w celu dodatkowego zwiększenia bezpieczeństwa.  </span><span class="sxs-lookup"><span data-stu-id="bb7b5-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|