---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić, czy ustawienia ochrony aplikacji platformy Microsoft 365 dla firm obowiązywały na urządzeniach użytkowników z systemem Windows 10.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912419"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="d4962-103">Sprawdzanie poprawności ustawień ochrony urządzeń na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="d4962-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="d4962-104">Sprawdzanie, czy ustawiono zasady dotyczące urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="d4962-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="d4962-105">Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może upłynieć kilka godzin, aż te zasady zajdą w życie na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="d4962-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="d4962-106">Aby potwierdzić, że zasady te obowiązywały, możesz zobaczyć różne ekrany ustawień systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="d4962-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="d4962-107">Ponieważ użytkownicy nie będą mogli modyfikować ustawień oprogramowania antywirusowego Windows Update i Windows Defender na urządzeniach z systemem Windows 10, wiele opcji zostanie wyszarowanych.</span><span class="sxs-lookup"><span data-stu-id="d4962-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="d4962-108">Przejdź do opcji **Ustawienia** \> **Aktualizacja &amp; zabezpieczeń** \> **Uruchom ponownie usługę Windows Update** i upewnij się, że wszystkie ustawienia są \>  wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="d4962-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Wszystkie opcje Uruchom ponownie są wyszarowane.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="d4962-110">Przejdź do opcji **Ustawienia** Zaktualizuj zabezpieczenia Windows Update Zaawansowane i upewnij się, że wszystkie ustawienia \> **&amp;** \>  \>  są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="d4962-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Opcje aktualizacji zaawansowanych systemu Windows są wyszarowane.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="d4962-112">Przejdź  do ustawień \> **Aktualizacja &amp; zabezpieczeń Opcje** \> **zaawansowane usługi Windows Update** Wybierz sposób dostarczenia \>  \> **aktualizacji.**</span><span class="sxs-lookup"><span data-stu-id="d4962-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="d4962-113">Potwierdź, że widzisz komunikat (kolor czerwony), że niektóre ustawienia są ukryte lub zarządzane przez Twoją organizację, a wszystkie opcje są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="d4962-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Strona Wybieranie sposobu dostarczenia aktualizacji wskazuje, że ustawienia są ukryte lub zarządzane przez Organizację.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="d4962-115">Aby otworzyć usługę Windows Defender Security Center, przejdź do **ustawienia** Zaktualizuj zabezpieczenia Programu Windows Defender, kliknij pozycję Otwórz ochronę wątku wirusów programu \> **&amp;** \>  \> Windows  \> **Defender: &amp;** \> **ustawienia ochrony przed zagrożeniami w &amp; programie Windows Defender.**</span><span class="sxs-lookup"><span data-stu-id="d4962-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="d4962-116">Sprawdź, czy wszystkie opcje są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="d4962-116">Verify that all options are grayed out.</span></span> 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarowane.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="d4962-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="d4962-118">Related Topics</span></span>

[<span data-ttu-id="d4962-119">Dokumentacja i zasoby dotyczące platformy Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="d4962-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="d4962-120">Wprowadzenie do platformy Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="d4962-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="d4962-121">Zarządzanie usługą Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="d4962-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="d4962-122">Konfigurowanie komputerów PC z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="d4962-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
