---
title: Synchronizowanie użytkowników domeny z platformą Microsoft 365
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
description: Synchronizuj użytkowników kontrolowanych przez domenę z platformą Microsoft 365 dla firm.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081908"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synchronizowanie użytkowników domeny z platformą Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotowanie do synchronizacji katalogów 

Przed zsynchronizowanie użytkowników i komputerów z lokalnej domeny usługi Active Directory należy zapoznać się z recenzją [Prepare for directory synchronizacji do usługi Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie istnieją duplikaty dla następujących atrybutów: **poczta,** **proxyAddresses**i **userPrincipalName**. Wartości te muszą być unikatowe i wszystkie duplikaty muszą zostać usunięte.
   
   - Zaleca się skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego w taki sposób, aby odpowiadał podstawowemu adresowi e-mail odpowiadającemu licencjonowanemu użytkownikowi usługi Microsoft 365. Na przykład: *mary.shelley@contoso.com,* a nie *mary@contoso.local*
   
   - Jeśli domena usługi Active Directory kończy się sufiksem niesygnawalnym, takim jak *.local* lub *.lan,* zamiast sufiksu z routingiem internetowym, takim jak *.com* lub *.org,* dostosuj sufiks nazwy UPN kont użytkowników lokalnych, zgodnie z opisem w [polu Przygotuj domenę nie rutowalną do synchronizacji katalogów.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

**Uruchom IdFix** w kroku czwartym (4) poniżej, upewnij się również, że lokalna usługa Active Directory jest gotowa do synchronizacji dir.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i konfigurowanie usługi Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory w usłudze Azure Active Directory, zainstaluj usługę Azure Active Directory Connect i skonfiguruj synchronizację katalogów. 

 1. W centrum administracyjnym przy <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> wyborze **Instalatora** w lewej konsoli.

 2. W obszarze **Logowanie i zabezpieczenia**wybierz pozycję **Wyświetl** w obszarze **Synchronizuj użytkowników z katalogu organizacji**.

 3. Na stronie **Synchronizuj użytkowników z katalogu organizacji** wybierz pozycję **Wprowadzenie**.

 4. W pierwszym kroku uruchom narzędzie IdFix, aby przygotować się do synchronizacji katalogu.

 5. Wykonaj kroki kreatora, aby pobrać usługę Azure AD Connect i użyj jej do zsynchronizowania użytkowników kontrolowanych przez domenę z usługą Microsoft 365.


Aby dowiedzieć się więcej, zobacz [Konfigurowanie synchronizacji katalogów dla usługi Microsoft 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

Podczas konfigurowania opcji usługi Azure AD Connect zaleca się włączenie **synchronizacji haseł,** **bezproblemowego logowania jednokrotnego**i funkcji **zapisywania zwrotnego hasła,** która jest również obsługiwana w usłudze Microsoft 365 dla firm.

> [!NOTE]
> Istnieje kilka dodatkowych kroków dotyczących zapisywania zwrotnego hasła poza polem wyboru w usłudze Azure AD Connect. Aby uzyskać więcej informacji, zobacz [Instrukcje: konfigurowanie storamentu hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Jeśli chcesz również zarządzać urządzeniami z systemem Windows 10 przyłączonych do domeny, zobacz [Włączanie urządzeń z systemem Windows 10 przyłączonych do domeny, którymi ma zarządzać usługa Microsoft 365 Business Premium](manage-windows-devices.md) w celu skonfigurowania hybrydowego dołączania do usługi Azure AD Join. 