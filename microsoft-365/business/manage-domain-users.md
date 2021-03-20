---
title: Synchronizowanie użytkowników domeny z usługą Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
- MOE150
description: Synchronizowanie użytkowników kontrolowanych domeną z platformą Microsoft 365 dla firm.
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913259"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synchronizowanie użytkowników domeny z usługą Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotowywanie do synchronizacji katalogów 

Przed zsynchronizowaniem użytkowników i komputerów z lokalnej domeny usługi Active Directory zapoznaj się z tematem Przygotowanie do synchronizacji katalogów [z platformą Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md) W szczególności:

   - Upewnij się, że w katalogu nie występują duplikaty następujących atrybutów: **mail,** **proxyAddresses** i **userPrincipalName.** Te wartości muszą być unikatowe, a wszelkie duplikaty muszą zostać usunięte.
   
   - Zalecamy skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego tak, aby był on taki, jak podstawowy adres e-mail odpowiadający licencjonowanemu użytkownikowi platformy Microsoft 365. Na przykład: *mary.shelley@contoso.com* zamiast *mary@contoso.local*
   
   - Jeśli domena usługi Active Directory kończy się sufiksem nie routowalnym, takim jak *.local* lub *lan,* zamiast sufiksu routowalnego przez Internet, takiego jak *.com* lub *.org,* najpierw dostosuj sufiks upn kont użytkowników lokalnych zgodnie z opisem w tesłudze Przygotowywanie domeny nie routowalnej do synchronizacji [katalogów.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

Uruchomienie **programu IdFix** w kroku 4 (4) poniżej spowoduje również upewninie się, że lokalna usługa Active Directory jest gotowa do synchronizacji katalogów.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i konfigurowanie programu Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, zainstaluj narzędzie Azure Active Directory Connect i skonfiguruj synchronizację katalogów. 

 1. W centrum [administracyjnym wybierz](https://go.microsoft.com/fwlink/p/?linkid=2024339) **pozycję Konfiguracja w** lewym okienku narracji.

 2. W **obszarze Logowanie i zabezpieczenia wybierz** pozycję **Wyświetl** w obszarze Synchronizowanie użytkowników z **katalogu organizacji.**

 3. Na stronie **Synchronizuj użytkowników** z katalogu organizacji wybierz pozycję **Wprowadzenie.**

 4. W pierwszym kroku uruchom narzędzie IdFix, aby przygotować się do synchronizacji katalogów.

 5. Postępuj zgodnie z instrukcjami kreatora, aby pobrać program Azure AD Connect i za jego pomocą zsynchronizować użytkowników kontrolowanych domeną z platformą Microsoft 365.


Aby dowiedzieć się więcej, zobacz Konfigurowanie synchronizacji katalogów na platformie [Microsoft 365.](../enterprise/set-up-directory-synchronization.md)

Podczas konfigurowania opcji dla programu Azure AD Connect zalecamy włączenie synchronizacji **haseł,**  bezproblemowego logowania pojedynczego i funkcji zapisu hasła, która jest również obsługiwana na platformie Microsoft 365 dla firm.

> [!NOTE]
> Istnieje kilka dodatkowych kroków zapisu hasła poza polem wyboru w programie Azure AD Connect. Aby uzyskać więcej informacji, zobacz [Jak skonfigurować pisanie hasła.](/azure/active-directory/authentication/howto-sspr-writeback) 

Jeśli chcesz również zarządzać urządzeniami z systemem Windows 10 przyłączanych do domeny, zobacz Włączanie zarządzania przez platformę [Microsoft 365 Business Premium](manage-windows-devices.md) dla urządzeń przyłącznych do domeny w celu skonfigurowania hybrydowego dołączenia do usługi Azure AD.