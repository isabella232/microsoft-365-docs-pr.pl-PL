---
title: Zarządzanie dostępem użytkowników do dokumentów pakietu Office na urządzeniach przenośnych
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Dowiedz się więcej o zasadach ochrony, które mogą pomóc bezpiecznego dostępu do aplikacji pakietu Office z urządzeń przenośnych.
ms.openlocfilehash: cade979635dd5d4a618537d544a7a76ef64a2963
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071535"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="57bb6-103">Zarządzanie dostępem użytkowników do dokumentów pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="57bb6-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="57bb6-p101">Ustawienia zasad, które sterują sposobem, w jaki użytkownicy uzyskują dostęp do plików pakietu Office ze swoich urządzeń przenośnych, są domyślnie **Wyłączone**. Zalecane jest zaakceptowanie domyślnych wartości podczas instalacji w celu utworzenia zasad aplikacji dla systemów Android, iOS i Windows 10 dotyczących wszystkich użytkowników. Po zakończeniu instalacji możesz utworzyć więcej zasad.</span><span class="sxs-lookup"><span data-stu-id="57bb6-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="57bb6-107">Ustawienia, które sterują dostępem użytkowników do plików pakietu Office na urządzeniach przenośnych</span><span class="sxs-lookup"><span data-stu-id="57bb6-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="57bb6-108">Na potrzeby zarządzania dostępem użytkowników do plików służbowych w pakiecie Office dostępne są następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="57bb6-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="57bb6-109">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="57bb6-109">Setting</span></span>  <br/> |<span data-ttu-id="57bb6-110">Opis</span><span class="sxs-lookup"><span data-stu-id="57bb6-110">Description</span></span>  <br/> |
|<span data-ttu-id="57bb6-111">Wymagaj numeru PIN lub odcisku palca w celu uzyskania dostępu do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="57bb6-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="57bb6-112">Gdy to ustawienie jest **włączone**, użytkownicy muszą się dodatkowo uwierzytelnić, korzystając z innej metody (oprócz podania nazwy użytkownika i hasła), aby uzyskać dostęp do aplikacji pakietu Office na urządzeniach przenośnych.</span><span class="sxs-lookup"><span data-stu-id="57bb6-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="57bb6-113">Resetuj numer PIN w przypadku wielokrotnego niepowodzenia logowania</span><span class="sxs-lookup"><span data-stu-id="57bb6-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="57bb6-114">Aby uniemożliwić nieautoryzowanym użytkownikom odgadywanie kodu PIN, ten kod jest resetowany po określonej liczbie nieudanych prób jego podania.</span><span class="sxs-lookup"><span data-stu-id="57bb6-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="57bb6-115">Wymagaj ponownego logowania użytkowników po czasie bezczynności aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="57bb6-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="57bb6-116">To ustawienie określa, jak długo użytkownik może nie korzystać z aplikacji, zanim będzie wymagane ponowne zalogowanie się.</span><span class="sxs-lookup"><span data-stu-id="57bb6-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="57bb6-117">Odmów dostępu do plików służbowych na urządzeniach z usuniętymi natywnymi ograniczeniami producenta</span><span class="sxs-lookup"><span data-stu-id="57bb6-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="57bb6-p102">Sprytni użytkownicy mogą mieć urządzenie z usuniętymi natywnymi ograniczeniami producenta. Umożliwia to użytkownikowi modyfikowanie systemu operacyjnego, co może uczynić urządzenie bardziej podatnym na złośliwe oprogramowanie. Te urządzenia zostaną zablokowane, jeśli to ustawienie będzie **Włączone**.  </span><span class="sxs-lookup"><span data-stu-id="57bb6-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="57bb6-121">Nie zezwalaj użytkownikom na kopiowanie zawartości z aplikacji pakietu Office do osobistych aplikacji</span><span class="sxs-lookup"><span data-stu-id="57bb6-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="57bb6-122">Gdy to ustawienie jest **włączone**, użytkownik nie może skopiować informacje w pliku roboczego pliku osobistego.</span><span class="sxs-lookup"><span data-stu-id="57bb6-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="57bb6-123">Jeśli to ustawienie jest **wyłączone**, użytkownik może skopiować informacje z pliku roboczego do osobistych aplikacji lub konto osobiste.</span><span class="sxs-lookup"><span data-stu-id="57bb6-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

