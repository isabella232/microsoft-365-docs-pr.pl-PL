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
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966983"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="71b7a-103">Konfigurowanie Microsoft 365 Business w Kreatorze instalacji</span><span class="sxs-lookup"><span data-stu-id="71b7a-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="71b7a-104">Domeny, użytkownicy, dodawanie i konfigurowanie zasad</span><span class="sxs-lookup"><span data-stu-id="71b7a-104">Add your domain, users, and set up policies</span></span>

![Transparent odsyłających do https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="71b7a-106">Kupując Microsoft 365 Business, istnieje możliwość korzystania z własnej domeny lub kupić jeden podczas [zapisywania się](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="71b7a-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="71b7a-107">Jeśli zakupiono nową domenę podczas rejestracji, domeny jest ustawiona w górę i można przenieść do [dodawania użytkowników i przypisywanie licencji](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="71b7a-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="71b7a-108">Dodawanie domeny do spersonalizowania logowanie</span><span class="sxs-lookup"><span data-stu-id="71b7a-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="71b7a-109">Zaloguj się do [Centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="71b7a-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="71b7a-110">Wybierz polecenie **Dodaj domenę** lub **Dodawanie użytkowników** , aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="71b7a-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="71b7a-111">Jeśli zakupiono domeny podczas rejestracji, będzie nie się **dodać domenę** krok tutaj.</span><span class="sxs-lookup"><span data-stu-id="71b7a-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="71b7a-112">Przejdź do [Dodawanie użytkowników](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="71b7a-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Wybierz Dodaj domenę.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="71b7a-114">W Kreatorze wprowadź nazwę domeny, którą chcesz użyć (np. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="71b7a-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Zrzut ekranu Personalizuj stronę logowania.](media/personalizesignin.png)

    
4. <span data-ttu-id="71b7a-116">Postępuj zgodnie z instrukcjami w kreatorze [Tworzenie rekordów DNS u dowolnego dostawcy usług hosta DNS dla usługi Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sprawdza, czy użytkownik jest właścicielem domeny.</span><span class="sxs-lookup"><span data-stu-id="71b7a-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="71b7a-117">Jeśli znasz hostem domeny, zobacz też [host konkretne instrukcje](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="71b7a-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="71b7a-118">Jeśli dostawcą hostingu jest GoDaddy, proces jest łatwe i automatycznie uzyskasz zalogować się i powiadomić firmę Microsoft uwierzytelniania w Twoim imieniu:</span><span class="sxs-lookup"><span data-stu-id="71b7a-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na stronie Potwierdzenie dostępu GoDaddy wybierz opcję Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="71b7a-120">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="71b7a-120">Add users and assign licenses</span></span>

<span data-ttu-id="71b7a-121">W kreatorze można dodawać użytkowników, ale można również [dodać później użytkowników](add-users-m365b.md) w Centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="71b7a-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="71b7a-122">Dodatkowo Jeśli w komputerze znajduje się kontroler domeny lokalnej, można dodać użytkowników z [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="71b7a-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="71b7a-123">Dodaj użytkowników w Kreatorze</span><span class="sxs-lookup"><span data-stu-id="71b7a-123">Add users in the wizard</span></span>

<span data-ttu-id="71b7a-124">Wszyscy użytkownicy, które można dodać w Kreatorze uzyskać automatycznie przypisywany licencji Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="71b7a-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Zrzut ekranu strony Dodaj nowych użytkowników w Kreatorze](media/addnewuserspage.png)

1. <span data-ttu-id="71b7a-126">Jeśli subskrypcja Microsoft 365 Business istniejących użytkowników (na przykład, jeśli użyto Azure Połącz AD), masz możliwość przypisania licencji do nich teraz.</span><span class="sxs-lookup"><span data-stu-id="71b7a-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="71b7a-127">Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="71b7a-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="71b7a-128">Po dodaniu użytkowników otrzymają również opcję udostępniania poświadczeń z nowych użytkowników, które zostały dodane.</span><span class="sxs-lookup"><span data-stu-id="71b7a-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="71b7a-129">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="71b7a-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="71b7a-130">Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**.</span><span class="sxs-lookup"><span data-stu-id="71b7a-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="71b7a-131">Jeśli jest przesuwana od innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [migracji wiadomości e-mail i kontaktów do usługi Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="71b7a-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="71b7a-132">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="71b7a-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="71b7a-133">Jeśli wybrany do korzystania z domeny .onmicrosoft lub Azure AD Connect umożliwia konfigurowanie użytkowników, nie zobaczysz ten krok.</span><span class="sxs-lookup"><span data-stu-id="71b7a-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="71b7a-134">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="71b7a-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="71b7a-135">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="71b7a-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="71b7a-136">Jeśli tak nie jest, [Zmień serwery nazw do skonfigurowania usługi Office 365 z dowolnym domen](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="71b7a-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="71b7a-137">Jeśli masz istniejące rekordy DNS, na przykład istniejącej witryny sieci web, można zarządzać własne rekordy DNS, aby upewnić się, że łączność istniejących usług.</span><span class="sxs-lookup"><span data-stu-id="71b7a-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="71b7a-138">Zobacz [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="71b7a-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Domeny połączyć stronę z I zarządzać własną rekordów DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="71b7a-140">Postępuj zgodnie z instrukcjami w kreatorze i poczty e-mail i innych usług ustala się dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="71b7a-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="71b7a-141">Konfigurowanie zasad zabezpieczeń i konfiguracji urządzeń</span><span class="sxs-lookup"><span data-stu-id="71b7a-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="71b7a-142">Zasady, które można skonfigurować w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*.</span><span class="sxs-lookup"><span data-stu-id="71b7a-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="71b7a-143">Można również utworzyć dodatkowe grupy do przypisywania zasad do w Centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="71b7a-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="71b7a-144">Na **chronić pliki praca na urządzeniach przenośnych** opcję **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** jest zaznaczone domyślnie.</span><span class="sxs-lookup"><span data-stu-id="71b7a-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="71b7a-145">Masz możliwość włączyć **Zarządzanie dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych**i jest to zalecane.</span><span class="sxs-lookup"><span data-stu-id="71b7a-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Zrzut ekranu chronić pliki pracy na stronie dla urządzeń przenośnych.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="71b7a-147">Rozwiń **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** , aby wyświetlić [wartości domyślnych](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="71b7a-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Zrzut ekranu z wartości domyślne dla ochrony plików na urządzeniach utracone.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="71b7a-149">Wybierz polecenie **Zarządzaj dostęp użytkowników do plików pakietu Office na urządzeniach przenośnych** i rozwinąć, aby wyświetlić [wartości domyślne](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="71b7a-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="71b7a-150">Firma Microsoft zaleca, aby zaakceptować wartości domyślne podczas instalacji do tworzenia zasad aplikacji dla Androida, iOS i 10 systemu Windows, które dotyczą wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="71b7a-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="71b7a-151">Po zakończeniu instalacji możesz utworzyć więcej zasad.</span><span class="sxs-lookup"><span data-stu-id="71b7a-151">You can create more policies after setup completes.</span></span>

        ![Zrzut ekranu ustawienia ochrony dla plików pakietu Office na telefon komórkowy.](media/useraccessonmobile.png)

2. <span data-ttu-id="71b7a-153">Ostatni krok na ochronę danych i urządzeń umożliwia konfigurowanie zasad w celu zabezpieczenia systemu Windows 10 urządzeń.</span><span class="sxs-lookup"><span data-stu-id="71b7a-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="71b7a-154">Te ustawienia są stosowane automatycznie, gdy użytkownik systemu Windows 10 łączy się z organizacji.</span><span class="sxs-lookup"><span data-stu-id="71b7a-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="71b7a-155">Po rozwinięciu **Secure Windows 10 urządzenia** , aby wyświetlić i zmodyfikować [wartości domyślne](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="71b7a-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="71b7a-156">Można także [automatycznie zainstalować pakiet Office](install-office-on-windows-10-during-setup.md) na urządzeniach Windows 10.</span><span class="sxs-lookup"><span data-stu-id="71b7a-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Zrzut ekranu przedstawiający Ustaw stronę konfiguracji urządzenia Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="71b7a-158">Wdrażanie aplikacji klienckich pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="71b7a-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="71b7a-159">Jeśli wybrano opcję automatycznie zainstalować aplikacje pakietu Office w trakcie zestaw się, aplikacje zainstaluje na urządzeniach Windows 10 po użytkowników jest zarejestrowany w programie Azure AD z ich urządzeń systemu Windows przy użyciu poświadczeń pracy.</span><span class="sxs-lookup"><span data-stu-id="71b7a-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="71b7a-160">Aby zainstalować pakiet Office na przenośnym lub tabletu, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników biznesowych 365 firmy Microsoft](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="71b7a-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="71b7a-161">Można także zainstalować Office indywidualnie.</span><span class="sxs-lookup"><span data-stu-id="71b7a-161">You can also install Office individually.</span></span> <span data-ttu-id="71b7a-162">Zobacz [instalacji pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) , aby uzyskać instrukcje.</span><span class="sxs-lookup"><span data-stu-id="71b7a-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>
