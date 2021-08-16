---
title: Edytowanie lub ustawianie ustawień ochrony aplikacji dla Windows 10 urządzeniach
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Dowiedz się, jak tworzyć lub edytować zasady zarządzania aplikacją i chronić pliki służbowe na osobistych Windows 10 urządzeniach.
ms.openlocfilehash: 6d38d1765e0a331516b2261870112d530ab4ee50f24c6defba95964ea4d9dcfa
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852668"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Konfigurowanie lub edytowanie ustawień ochrony aplikacji dla Windows 10 urządzeniach

Ten artykuł dotyczy Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Edytowanie zasad zarządzania aplikacją dla Windows 10

1. Przejdź do centrum administracyjnego w stronie <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. W lewym okienku narracji wybierz pozycję **Zasady** \> **dotyczące urządzeń.**
1. Wybierz istniejącą Windows aplikacji, a następnie pozycję **Edytuj**.
1. Wybierz **pozycję Edytuj** obok ustawienia, które chcesz zmienić, a następnie wybierz pozycję **Zapisz**.

## <a name="create-an-app-management-policy-for-windows-10"></a>Tworzenie zasad zarządzania aplikacjami dla systemu Windows 10

Jeśli użytkownicy mają urządzenia osobiste z systemem Windows 10, na których wykonują zadania służbowe, możesz również chronić dane na tych urządzeniach.
  
1. Przejdź do centrum administracyjnego w stronie <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. W lewym okienku narracji wybierz pozycję **Urządzenia Zasady** \>  \> **Dodaj**.
3. W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad. 
4. W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Windows 10**.
5. W **obszarze Typ urządzenia** wybierz pozycję **Osobiste** lub **Własność firmy**.
6. Opcja **Szyfruj pliki służbowe** zostanie włączona automatycznie. 
7. Jeśli nie chcesz, aby użytkownicy mogli zapisywać pliki służbowe na swoich komputerach, **włącz** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm**. 
9. Rozwiń **rozwijanie odzyskaj dane Windows urządzeniach.** Zalecamy jej włączenie **.**
    Aby móc przejść do lokalizacji certyfikatu agenta odzyskiwania danych, musisz najpierw go utworzyć. Aby uzyskać instrukcje, zobacz Tworzenie i weryfikowanie certyfikatu agenta odzyskiwania danych systemu szyfrowania plików [(EFS).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)
    
    Domyślnie pliki robocze są szyfrowane przy użyciu klucza tajnego, który jest przechowywany na urządzeniu i skojarzony z profilem użytkownika. Tylko użytkownik może otwierać i odszyfrowywać plik. Jednak w razie utraty urządzenia lub usunięcia użytkownika plik może utknąć w stanie zaszyfrowania. Administrator może odszyfrować plik za pomocą certyfikatu agenta odzyskiwania danych (DRA).
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Rozwiń **pozycję Chroń dodatkowe** lokalizacje sieciowe i w chmurze, jeśli chcesz dodać dodatkowe domeny lub SharePoint lokalizacji online, aby mieć pewność, że pliki we wszystkich wymienionych aplikacjach są chronione. Jeśli dla każdego pola trzeba wprowadzić więcej niż jeden element, użyj średnika (;) między elementami.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
12. Na koniec wybierz przycisk **Dodaj**, aby zapisać zasady i zastosować je na urządzeniach.