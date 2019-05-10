---
title: Konfigurowanie usługi Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować Microsoft 365 Business.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660864"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="daf3b-103">Konfigurowanie usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="daf3b-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="daf3b-104">Przed rozpoczęciem pracy, zobacz [Uzyskiwanie Microsoft Business 365](get-microsoft-365-business.md) szczegółowe zapisywania się.</span><span class="sxs-lookup"><span data-stu-id="daf3b-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="daf3b-105">Obejrzyj [krótki klip wideo o tym, jak skonfigurować Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) przy użyciu zestawu kreatora, a gdy nie ma usługi Active Directory na lokalnym</span><span class="sxs-lookup"><span data-stu-id="daf3b-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="daf3b-106">Omówienie</span><span class="sxs-lookup"><span data-stu-id="daf3b-106">Overview</span></span>

<span data-ttu-id="daf3b-107">Większość ustawień czynności może odbywać się w Kreatorze instalacji, ale inne opcje są również wyświetlane.</span><span class="sxs-lookup"><span data-stu-id="daf3b-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="daf3b-108">[Dodawanie domeny](#add-your-domain-to-personalize-sign-in) (jeśli kupiłeś domeny podczas [zarejestrować się](sign-up.md), ten krok jest już zrobione.)</span><span class="sxs-lookup"><span data-stu-id="daf3b-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="daf3b-109">Dodaj użytkowników.</span><span class="sxs-lookup"><span data-stu-id="daf3b-109">Add users.</span></span> <span data-ttu-id="daf3b-110">Możesz to zrobić na jeden z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="daf3b-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="daf3b-111">W oknie [Kreatora instalacji](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="daf3b-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="daf3b-112">Użyj synchronizacji katalogów, aby [dodać użytkowników za pomocą Azure AD Connect](#add-users-by-using-azure-ad-connect) , jeśli masz lokalnej usługi Active directory.</span><span class="sxs-lookup"><span data-stu-id="daf3b-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="daf3b-113">Można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="daf3b-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="daf3b-114">Konfigurowanie zasad zabezpieczeń i skonfigurować urządzenia.</span><span class="sxs-lookup"><span data-stu-id="daf3b-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="daf3b-115">Możesz to zrobić na jeden z trzech sposobów:</span><span class="sxs-lookup"><span data-stu-id="daf3b-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="daf3b-116">W oknie [Kreatora instalacji](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="daf3b-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="daf3b-117">W [Centrum administracyjnego](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="daf3b-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="daf3b-118">W [Centrum administracyjnego usługi Intune](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="daf3b-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="daf3b-119">Konfigurowanie i zarządzanie urządzeniami Windows 10.</span><span class="sxs-lookup"><span data-stu-id="daf3b-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="daf3b-120">Po dołączeniu urządzenia WIndows 10 do Azure AD wszystkich zasad będzie stosowane do niego.</span><span class="sxs-lookup"><span data-stu-id="daf3b-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="daf3b-121">Ustawianie konfiguracji urządzeń systemu Windows 10 w oknie [Kreatora instalacji](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="daf3b-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="daf3b-122">Dołącz [nowe urządzenie Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="daf3b-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="daf3b-123">Dołącz do [istniejącego urządzenia Windows 10](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="daf3b-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="daf3b-124">Zainstaluj pakiet Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="daf3b-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="daf3b-125">Można automatycznie zainstalować pakiet Office w urządzeniach z systemem Windows przy użyciu [Kreatora instalacji](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="daf3b-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="daf3b-126">Automatycznie [zainstalować pakiet Office](auto-install-or-uninstall-office.md) z Centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="daf3b-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="daf3b-127">Pozwól użytkownikom [instalować aplikacje pakietu Office](https://docs.microsoft.com/office365/admin/setup/install-applications) dla systemu Windows i urządzeń.</span><span class="sxs-lookup"><span data-stu-id="daf3b-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="daf3b-128">Konfigurowanie dodatkowych zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="daf3b-128">Set up additional security.</span></span>
    - <span data-ttu-id="daf3b-129">Kreator instalacji dodaje zasad, aby zabezpieczyć swoje urządzenia, ale można również Państwo skorzystać z funkcji [dodatkowych zabezpieczeń](#additional-security-settings) pomaga chronić dane, kont i wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="daf3b-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="daf3b-130">Dodawanie domeny, użytkowników i ustawianie zasad</span><span class="sxs-lookup"><span data-stu-id="daf3b-130">Add your domain, users and set up policies</span></span>

![Transparent odsyłających do https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="daf3b-132">Kupując Microsoft 365 Business, istnieje możliwość korzystania z własnej domeny lub kupić jeden podczas [zapisywania się](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="daf3b-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="daf3b-133">Jeśli zakupiono nową domenę podczas rejestracji, domeny jest ustawiona w górę i można przenieść do [dodawania użytkowników i przypisywanie licencji](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="daf3b-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="daf3b-134">Dodawanie domeny do spersonalizowania logowanie</span><span class="sxs-lookup"><span data-stu-id="daf3b-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="daf3b-135">Zaloguj się do [Centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="daf3b-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="daf3b-136">Wybierz przycisk **Dodaj domenę** , aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="daf3b-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Wybierz Dodaj domenę.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="daf3b-138">W Kreatorze wprowadź nazwę domeny, którą chcesz użyć (np. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="daf3b-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Zrzut ekranu Personalizuj stronę logowania.](media/personalizesignin.png)

    
4. <span data-ttu-id="daf3b-140">Postępuj zgodnie z instrukcjami w kreatorze [Tworzenie rekordów DNS u dowolnego dostawcy usług hosta DNS dla usługi Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sprawdza, czy użytkownik jest właścicielem domeny.</span><span class="sxs-lookup"><span data-stu-id="daf3b-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="daf3b-141">Jeśli znasz hostem domeny, zobacz też [host konkretne instrukcje](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="daf3b-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="daf3b-142">Jeśli dostawcą hostingu jest GoDaddy, proces jest łatwe i automatycznie uzyskasz zalogować się i powiadomić firmę Microsoft uwierzytelniania w Twoim imieniu:</span><span class="sxs-lookup"><span data-stu-id="daf3b-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na stronie Potwierdzenie dostępu GoDaddy wybierz opcję Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="daf3b-144">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="daf3b-144">Add users and assign licenses</span></span>

<span data-ttu-id="daf3b-145">W kreatorze można dodawać użytkowników, ale można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="daf3b-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="daf3b-146">Dodatkowo Jeśli w komputerze znajduje się kontroler domeny lokalnej, można dodać użytkowników z [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="daf3b-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="daf3b-147">Dodaj użytkowników w Kreatorze</span><span class="sxs-lookup"><span data-stu-id="daf3b-147">Add users in the wizard</span></span>

<span data-ttu-id="daf3b-148">Wszyscy użytkownicy, które można dodać w Kreatorze uzyskać automatycznie przypisywany licencji Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="daf3b-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="daf3b-149">Jeśli jest używany kontroler domeny lokalnej, a jest używana usługa Active Directory, zobacz [jak ddd użytkowników za pomocą Azure AD Connect](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="daf3b-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Zrzut ekranu strony Dodaj nowych użytkowników w Kreatorze](media/addnewuserspage.png)

1. <span data-ttu-id="daf3b-p106">Jeśli Twoja subskrypcja usługi Microsoft 365 Business zawiera już użytkowników (na przykład użyto narzędzia Azure AD Connect), zobaczysz opcję przypisania im licencji. Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="daf3b-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="daf3b-153">Po dodaniu użytkowników otrzymają również opcję udostępniania poświadczeń z nowych użytkowników, które zostały dodane.</span><span class="sxs-lookup"><span data-stu-id="daf3b-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="daf3b-154">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="daf3b-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="daf3b-155">Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**.</span><span class="sxs-lookup"><span data-stu-id="daf3b-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="daf3b-156">Jeśli jest przesuwana od innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [migracji wiadomości e-mail i kontaktów do usługi Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="daf3b-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="daf3b-157">Dodawanie użytkowników za pomocą Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="daf3b-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="daf3b-158">Jeśli masz kontroler domeny lokalnej z usługą Active Directory, synchronizowania użytkowników Microsoft 365 Business przy użyciu [Azure Połącz AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="daf3b-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="daf3b-159">Zakończ to przed uruchomieniem Kreatora instalacji.</span><span class="sxs-lookup"><span data-stu-id="daf3b-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="daf3b-160">Można go pobrać w Centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="daf3b-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="daf3b-161">Przejdź do **użytkowników** \> **aktywnych użytkowników**, wybierz Wielokropek na górze strony, a następnie wybierz **synchronizacji katalogów** do pobrania Azure Połącz AD.</span><span class="sxs-lookup"><span data-stu-id="daf3b-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Na stronie aktywnych użytkowników wybierz elipsy > katalog snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="daf3b-163">Jeśli tworzenie użytkowników w ten sposób będzie jeszcze do przypisywania licencji do nich w Centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="daf3b-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="daf3b-164">Dostęp do domeny aplikacji i urządzeń w dalszym ciągu</span><span class="sxs-lookup"><span data-stu-id="daf3b-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="daf3b-165">Jeśli chcesz w dalszym ciągu dostęp do domeny aplikacji i urządzeń, przeczytanie następujących artykułów dla dwóch różnych rozwiązanie pozwalające który:</span><span class="sxs-lookup"><span data-stu-id="daf3b-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="daf3b-166">Włączanie zarządzania przez usługę Microsoft 365 Business dla urządzeń przyłączonych do domeny systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="daf3b-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="daf3b-167">Jest to zalecany sposób.</span><span class="sxs-lookup"><span data-stu-id="daf3b-167">This is the recommended way.</span></span>

- [<span data-ttu-id="daf3b-168">Dostęp do zasobów lokalnych z Azure urządzenia przyłączonych do AD w Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="daf3b-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="daf3b-169">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="daf3b-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="daf3b-170">Jeśli wybrany do korzystania z domeny .onmicrosoft lub Azure AD Connect umożliwia konfigurowanie użytkowników, nie zobaczysz ten krok.</span><span class="sxs-lookup"><span data-stu-id="daf3b-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="daf3b-171">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="daf3b-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="daf3b-172">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="daf3b-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="daf3b-173">Jeśli tak nie jest, [Zmień serwery nazw do skonfigurowania usługi Office 365 z dowolnym domen](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="daf3b-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="daf3b-174">Jeśli masz istniejące rekordy DNS, na przykład istniejącej witryny sieci web, można zarządzać własne rekordy DNS, aby upewnić się, że łączność istniejących usług.</span><span class="sxs-lookup"><span data-stu-id="daf3b-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="daf3b-175">Zobacz [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="daf3b-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Domeny połączyć stronę z I zarządzać własną rekordów DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="daf3b-177">Postępuj zgodnie z instrukcjami w kreatorze i poczty e-mail i innych usług ustala się dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="daf3b-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="daf3b-178">Konfigurowanie zasad zabezpieczeń i konfiguracji urządzeń</span><span class="sxs-lookup"><span data-stu-id="daf3b-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="daf3b-179">Te zasady są stosowane do każdego użytkownika, jeśli użytkownik chce przypisać różne zasady do zestawu użytkowników dać licencji, lub grupie użytkowników.</span><span class="sxs-lookup"><span data-stu-id="daf3b-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="daf3b-180">Ustawianie zasad w Kreatorze</span><span class="sxs-lookup"><span data-stu-id="daf3b-180">Set up policies in the wizard</span></span>

<span data-ttu-id="daf3b-181">Zasady, które można skonfigurować w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*.</span><span class="sxs-lookup"><span data-stu-id="daf3b-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="daf3b-182">Na **chronić pliki praca na urządzeniach przenośnych** opcję **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** jest zaznaczone domyślnie.</span><span class="sxs-lookup"><span data-stu-id="daf3b-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="daf3b-183">Masz możliwość włączyć **Zarządzanie dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych**i jest to zalecane.</span><span class="sxs-lookup"><span data-stu-id="daf3b-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Zrzut ekranu chronić pliki pracy na stronie dla urządzeń przenośnych.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="daf3b-185">Jeżeli rozwiniesz **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione**, [wartości domyślne](protect-work-files-on-lost-or-stolen-device.md) są wstępnie wybrane:</span><span class="sxs-lookup"><span data-stu-id="daf3b-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Zrzut ekranu z wartości domyślne dla ochrony plików na urządzeniach utracone.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="daf3b-187">Wybierz polecenie **Zarządzaj dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** i rozwiń ją, wyświetlone zostaną [wartości domyślne](manage-user-access-on-mobile-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="daf3b-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="daf3b-188">Zalecane jest zaakceptowanie domyślnych wartości podczas instalacji w celu utworzenia zasad aplikacji dla systemów Android, iOS i Windows 10 dotyczących wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="daf3b-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="daf3b-189">Po zakończeniu instalacji możesz utworzyć więcej zasad.</span><span class="sxs-lookup"><span data-stu-id="daf3b-189">You can create more policies after setup completes.</span></span>

        ![Zrzut ekranu ustawienia ochrony dla plików pakietu Office na telefon komórkowy.](media/useraccessonmobile.png)

2. <span data-ttu-id="daf3b-191">Ostatni krok na ochronę danych i urządzeń umożliwia konfigurowanie zasad w celu zabezpieczenia systemu Windows 10 urządzeń.</span><span class="sxs-lookup"><span data-stu-id="daf3b-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="daf3b-192">Te ustawienia są stosowane automatycznie, gdy użytkownik systemu Windows 10 łączy się z organizacji.</span><span class="sxs-lookup"><span data-stu-id="daf3b-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="daf3b-193">Po rozwinięciu **Secure Windows 10 urządzenia** , aby wyświetlić i zmodyfikować [wartości domyślne](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="daf3b-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="daf3b-194">Można także [automatycznie zainstalować pakiet Office](install-office-on-windows-10-during-setup.md) na urządzeniach Windows 10.</span><span class="sxs-lookup"><span data-stu-id="daf3b-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Zrzut ekranu przedstawiający Ustaw stronę konfiguracji urządzenia Windows 10.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="daf3b-196">Modyfikowanie lub Dodawanie zasady w Centrum administracyjnym</span><span class="sxs-lookup"><span data-stu-id="daf3b-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="daf3b-197">Zobacz [Zarządzanie Microsoft 365 Business](manage.md) dla zasady łącza do tematów dotyczących sposobu wyświetlania i modyfikowania ochrony urządzeń i aplikacji i jak usunąć dane z lub resetowania urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="daf3b-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="daf3b-198">Wdrażanie i zarządzanie systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="daf3b-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="daf3b-199">Zobacz [Konfigurowanie urządzeń systemu Windows dla użytkowników biznesowych 365 firmy Microsoft,](set-up-windows-devices.md) Aby ręcznie połączyć Azure AD, albo w trakcie instalacji dla nowych komputerów lub zmieniając profilu rejestrowania dla istniejących komputerów.</span><span class="sxs-lookup"><span data-stu-id="daf3b-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="daf3b-200">Służy do definiowania nowych urządzeń autopilota</span><span class="sxs-lookup"><span data-stu-id="daf3b-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="daf3b-201">Można użyć [Windows Autopilot](add-autopilot-devices-and-profile.md) automatycznie wstępnie skonfigurować **Nowe** urządzenia Windows 10 dla użytkownika, ale może być łatwiej uzyskać [partnera](https://www.microsoft.com/solution-providers/search) , który może zrobić to dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="daf3b-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="daf3b-202">Można także przejść do [Magazyn Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) i zapytać specjalisty w zakresie technologii cloud Ustawianie nowych urządzeń, które kupić dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="daf3b-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="daf3b-203">Dostęp do zasobów lokalnych</span><span class="sxs-lookup"><span data-stu-id="daf3b-203">Access on-premises resources</span></span>

<span data-ttu-id="daf3b-204">Jeśli organizacja używa lokalnej usługi Active Directory systemu Windows Server, można zdefiniować Microsoft 365 gospodarczych, do ochrony urządzeń Windows 10, przy jednoczesnym zachowaniu dostępu do zasobów lokalnych, które wymagają uwierzytelniania lokalnych.</span><span class="sxs-lookup"><span data-stu-id="daf3b-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="daf3b-205">Postępuj zgodnie z instrukcjami [włączyć przyłączonych do domeny Windows 10 urządzenia mają być zarządzane przez Microsoft 365 Business](manage-windows-devices.md) można wybrać tę opcję.</span><span class="sxs-lookup"><span data-stu-id="daf3b-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="daf3b-206">Jest to preferowana metoda i urządzeń, w tym stanie są nazywane hybrydowy Azure AD dołączył do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="daf3b-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="daf3b-207">Jeśli Twoja firma ma lokalnej usługi Active Directory, który zawiera niektóre zasobów lokalnych (takich jak udziały plików i drukarek), może dać Azure AD przyłączony urządzeniom dostęp do tych zasobów, wykonując kroki opisane w tym miejscu: [dostępu do zasobów lokalnych z Azure AD dołączył do urządzenia w Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="daf3b-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="daf3b-208">Wdrażanie aplikacji klienckich pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="daf3b-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="daf3b-209">Jeśli wybrano opcję automatycznie zainstalować aplikacje pakietu Office w trakcie zestaw się, aplikacje zainstaluje na urządzeniach Windows 10 po użytkowników jest zarejestrowany w programie Azure AD z ich urządzeń systemu Windows przy użyciu poświadczeń pracy.</span><span class="sxs-lookup"><span data-stu-id="daf3b-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="daf3b-210">Aby zainstalować pakiet Office na przenośnym lub tabletu, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników biznesowych 365 firmy Microsoft](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="daf3b-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="daf3b-211">Można także zainstalować Office indywidualnie.</span><span class="sxs-lookup"><span data-stu-id="daf3b-211">You can also install Office individually.</span></span> <span data-ttu-id="daf3b-212">Zobacz [instalacji pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) , aby uzyskać instrukcje.</span><span class="sxs-lookup"><span data-stu-id="daf3b-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="daf3b-213">Dodatkowych ustawień zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="daf3b-213">Additional security settings</span></span>

<span data-ttu-id="daf3b-214">Oprócz zabezpieczeń i ustawienie zgodności w Kreatorze instalacji można skonfigurować następujące dodatkowe ustawienia:</span><span class="sxs-lookup"><span data-stu-id="daf3b-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="daf3b-215">**E-mail, ochrona przed złośliwym oprogramowaniem**</span><span class="sxs-lookup"><span data-stu-id="daf3b-215">**Email malware protection**</span></span>
- <span data-ttu-id="daf3b-216">**Zaawansowane zagrożenia ochrony (ATP) bezpieczne załączniki**</span><span class="sxs-lookup"><span data-stu-id="daf3b-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="daf3b-217">**Łącza bezpieczny ATP**</span><span class="sxs-lookup"><span data-stu-id="daf3b-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="daf3b-218">**ZDOLNY anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="daf3b-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="daf3b-219">**Exchange Online  archiwum**</span><span class="sxs-lookup"><span data-stu-id="daf3b-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="daf3b-220">**Zapobieganie utracie danych (DLP)**</span><span class="sxs-lookup"><span data-stu-id="daf3b-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="daf3b-221">**Ochrona informacji Azure** (Plan 1)</span><span class="sxs-lookup"><span data-stu-id="daf3b-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="daf3b-222">**Dostępność portalu Windows Intune**</span><span class="sxs-lookup"><span data-stu-id="daf3b-222">**Intune portal availability**</span></span>

<span data-ttu-id="daf3b-223">Aby rozpocząć, zobacz [Konfigurowanie zasad zabezpieczeń zaawansowanych](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="daf3b-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="daf3b-224">Zobacz też [top 10 sposobów zabezpieczenia firmy Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) do utworzenia planu działań najważniejsze wskazówki dotyczące zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="daf3b-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>