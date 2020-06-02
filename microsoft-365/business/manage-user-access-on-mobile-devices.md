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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Dowiedz się więcej o zasadach ochrony, które umożliwiają zarządzanie uzyskiwaniem dostępu użytkowników do aplikacji pakietu Office i plików służbowych z urządzeń przenośnych.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471072"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="ec4e5-103">Zarządzanie dostępem użytkowników do dokumentów pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="ec4e5-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="ec4e5-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="ec4e5-105">Ustawienia zasad, które sterują sposobem, w jaki użytkownicy uzyskują dostęp do plików pakietu Office ze swoich urządzeń przenośnych, są domyślnie **Wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="ec4e5-106">Zaleca się akceptowanie wartości domyślnych podczas instalacji w celu utworzenia zasad aplikacji dla systemów Android, iOS i Windows 10, które mają zastosowanie do wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="ec4e5-107">Po zakończeniu instalacji możesz utworzyć więcej zasad.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="ec4e5-108">Ustawienia, które sterują dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="ec4e5-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="ec4e5-109">Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="ec4e5-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ec4e5-110">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="ec4e5-110">Setting</span></span>  <br/> |<span data-ttu-id="ec4e5-111">Opis</span><span class="sxs-lookup"><span data-stu-id="ec4e5-111">Description</span></span>  <br/> |
|<span data-ttu-id="ec4e5-112">Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ec4e5-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="ec4e5-113">Jeśli to ustawienie jest **włączone,** użytkownicy muszą podać inną formę uwierzytelniania, oprócz nazwy użytkownika i hasła, zanim będą mogli korzystać z aplikacji pakietu Office na urządzeniu przenośnym.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="ec4e5-114">Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania</span><span class="sxs-lookup"><span data-stu-id="ec4e5-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="ec4e5-115">Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="ec4e5-116">Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ec4e5-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="ec4e5-117">To ustawienie określa, jak długo użytkownik może być bezczynny, zanim zostanie wyświetlony monit o ponowne zalogowanie się.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="ec4e5-118">Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta</span><span class="sxs-lookup"><span data-stu-id="ec4e5-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="ec4e5-119">Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="ec4e5-120">Oznacza to, że użytkownik może zmodyfikować system operacyjny, co może sprawić, że urządzenie będzie bardziej podatne na złośliwe oprogramowanie.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="ec4e5-121">Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="ec4e5-122">Nie zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do aplikacji osobistych</span><span class="sxs-lookup"><span data-stu-id="ec4e5-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="ec4e5-123">Gdy ustawienie to **Włączone,** użytkownik nie może skopiować informacji w pliku służbowym do pliku osobistego.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="ec4e5-124">Jeśli ustawienie jest **wyłączone,** użytkownik może skopiować informacje z pliku służbowego do aplikacji osobistej lub konta osobistego.</span><span class="sxs-lookup"><span data-stu-id="ec4e5-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

