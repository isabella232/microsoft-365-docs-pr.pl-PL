---
title: Synchronizowanie użytkowników domeny z programem Microsoft 365
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
description: Synchronizowanie użytkowników kontrolowanych przez domeny z aplikacją Microsoft 365 dla firm.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306454"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synchronizowanie użytkowników domeny z programem Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Przygotowywanie do synchronizacji katalogów 

Przed zsynchronizowaniem użytkowników i komputerów z lokalnej domeny usługi Active Directory Przejrzyj [przygotowanie do synchronizacji katalogów z systemem Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization). W szczególności:

   - Upewnij się, że w katalogu nie ma żadnych duplikatów dla następujących atrybutów: **mail**, **proxyAddresses**i **userPrincipalName**. Te wartości muszą być unikatowe i muszą być usunięte wszystkie duplikaty.
   
   - Zalecamy skonfigurowanie atrybutu **userPrincipalName** (UPN) dla każdego konta użytkownika lokalnego, aby odpowiadał pierwotnemu adresowi e-mail, który odpowiada licencjonowanemu użytkownikowi usługi Microsoft 365. Na przykład: *Mary.Shelley@contoso.com* , a nie *Mary@contoso. Local*
   
   - Jeśli domena usługi Active Directory kończy się na takim samym sufiksie, jak *. Local* lub. *LAN*, zamiast sufiksu internetowej obsługi routingu, takiego jak *com* lub *org*, należy dostosować sufiks głównej nazwy użytkownika konta użytkowników lokalnych zgodnie z opisem w części [Przygotowywanie do synchronizacji katalogów](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

**Uruchomienie narzędzia IdFix** w kroku cztery (4) poniżej spowoduje również upewnienie się, że lokalna usługa Active Directory jest gotowa do synchronizacji katalogu.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalowanie i Konfigurowanie usługi Azure AD Connect

Aby zsynchronizować użytkowników, grupy i kontakty z lokalnej usługi Active Directory z usługą Azure Active Directory, zainstaluj usługę Azure Active Directory Connect i skonfiguruj synchronizację katalogów. 

 1. W centrum administracyjnym po <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> wybraniu **Ustawienia** w lewym obszarze nawigacji.

 2. W obszarze **Logowanie i zabezpieczenia**wybierz pozycję **Wyświetl**  w obszarze **Użytkownicy synchronizacji w katalogu**organizacji.

 3. Na stronie **Synchronizuj użytkowników ze swojego katalogu w organizacji** **Wybierz pozycję wprowadzenie.**

 4. W pierwszym kroku Uruchom narzędzie narzędzia IdFix, aby przygotować się do synchronizacji katalogów.

 5. Postępuj zgodnie z instrukcjami kreatora, aby pobrać usługę Azure AD Connect, i użyć jej do zsynchronizowania użytkowników kontrolowanych przez domeny z systemem Microsoft 365.


Aby dowiedzieć się więcej, zobacz [Konfigurowanie synchronizacji katalogów dla programu Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .

Po skonfigurowaniu opcji usługi Azure AD Connect zalecamy włączenie **synchronizacji haseł**, **jednolite logowanie**jednokrotne oraz funkcji **zapisywania zwrotnego haseł** , która jest również obsługiwana w programie Microsoft 365 dla firm.

> [!NOTE]
> Istnieje kilka dodatkowych kroków dotyczących stornowania haseł poza polem wyboru w usłudze Azure AD Connect. Aby uzyskać więcej informacji, zobacz [instrukcje: Konfigurowanie zapisywania zwrotnego hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Jeśli chcesz zarządzać urządzeniami z systemem Windows 10 dołączonymi do domeny, zobacz [Włączanie zarządzania za pomocą programu Microsoft 365 Business Premium na urządzeniach z systemem Windows 10 przyłączonych do domeny](manage-windows-devices.md) . 