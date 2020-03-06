---
title: Zarządzanie dostępem użytkowników do dokumentów pakietu Office na urządzeniach przenośnych
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Dowiedz się więcej o zasadach ochrony, które umożliwiają zarządzanie dostępem użytkowników do aplikacji pakietu Office i plików roboczych z urządzeń przenośnych.
ms.openlocfilehash: 21e83114664d06aaeb27b08d9f4e2153eea02030
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550322"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="af23b-103">Zarządzanie dostępem użytkowników do dokumentów pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="af23b-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="af23b-104">Ustawienia zasad, które sterują sposobem, w jaki użytkownicy uzyskują dostęp do plików pakietu Office ze swoich urządzeń przenośnych, są domyślnie **Wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="af23b-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="af23b-105">Zaleca się zaakceptowanie wartości domyślnych podczas instalacji w celu utworzenia zasad aplikacji dla systemów Android, iOS i Windows 10, które mają zastosowanie do wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="af23b-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="af23b-106">Po zakończeniu instalacji możesz utworzyć więcej zasad.</span><span class="sxs-lookup"><span data-stu-id="af23b-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="af23b-107">Ustawienia, które sterują dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="af23b-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="af23b-108">Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="af23b-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="af23b-109">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="af23b-109">Setting</span></span>  <br/> |<span data-ttu-id="af23b-110">Opis</span><span class="sxs-lookup"><span data-stu-id="af23b-110">Description</span></span>  <br/> |
|<span data-ttu-id="af23b-111">Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="af23b-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="af23b-112">Jeśli to ustawienie jest **włączone,** użytkownicy muszą podać inną formę uwierzytelniania, oprócz nazwy użytkownika i hasła, aby mogli korzystać z aplikacji pakietu Office na swoim urządzeniu przenośnym.</span><span class="sxs-lookup"><span data-stu-id="af23b-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="af23b-113">Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania</span><span class="sxs-lookup"><span data-stu-id="af23b-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="af23b-114">Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.</span><span class="sxs-lookup"><span data-stu-id="af23b-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="af23b-115">Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="af23b-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="af23b-116">To ustawienie określa, jak długo użytkownik może być bezczynny, zanim zostanie wyświetlony monit o ponowne zalogowanie się.</span><span class="sxs-lookup"><span data-stu-id="af23b-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="af23b-117">Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta</span><span class="sxs-lookup"><span data-stu-id="af23b-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="af23b-118">Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta.</span><span class="sxs-lookup"><span data-stu-id="af23b-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="af23b-119">Oznacza to, że użytkownik może zmodyfikować system operacyjny, co może sprawić, że urządzenie będzie bardziej podatne na złośliwe oprogramowanie.</span><span class="sxs-lookup"><span data-stu-id="af23b-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="af23b-120">Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.</span><span class="sxs-lookup"><span data-stu-id="af23b-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="af23b-121">Nie zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych</span><span class="sxs-lookup"><span data-stu-id="af23b-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="af23b-122">Gdy ustawienie jest **włączone,** użytkownik nie może skopiować informacji w pliku roboczym do pliku osobistego.</span><span class="sxs-lookup"><span data-stu-id="af23b-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="af23b-123">Jeśli ustawienie jest **wyłączone,** użytkownik może skopiować informacje z pliku roboczego do aplikacji osobistej lub konta osobistego.</span><span class="sxs-lookup"><span data-stu-id="af23b-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

