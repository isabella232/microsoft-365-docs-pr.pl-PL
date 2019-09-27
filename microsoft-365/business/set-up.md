---
title: Konfigurowanie usługi Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować firmę Microsoft 365 Business.
ms.openlocfilehash: d33839693001f36fbb56541775015f739300b043
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288500"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="3baf2-103">Konfigurowanie Microsoft 365 Business w Kreatorze instalacji</span><span class="sxs-lookup"><span data-stu-id="3baf2-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="3baf2-104">Dodawanie domeny, użytkowników i Konfigurowanie zasad</span><span class="sxs-lookup"><span data-stu-id="3baf2-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="3baf2-105">[![Etykieta, aby poinformować, że centrum admin zmienia się i można znaleźć więcej szczegółów na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="3baf2-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="3baf2-106">Podczas zakupu Microsoft 365 Business, masz możliwość korzystania z domeny, którą posiadasz, lub kupując go podczas [rejestracji](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="3baf2-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="3baf2-107">Jeśli po zalogowaniu się zarejestrowano nową domenę, domena jest ustawiona i można ją przenieść, aby [dodać użytkowników i przypisać licencje](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="3baf2-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="3baf2-108">Dodawanie domeny w celu personalizacji logowania</span><span class="sxs-lookup"><span data-stu-id="3baf2-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="3baf2-109">Zaloguj się do [Centrum administracyjnego Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="3baf2-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="3baf2-110">Wybierz pozycję **Dodaj domenę** lub **Dodaj użytkowników** , aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="3baf2-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="3baf2-111">Jeśli domena została kupiona podczas rejestracji, nie zobaczysz tutaj kroku **Dodaj domenę** .</span><span class="sxs-lookup"><span data-stu-id="3baf2-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="3baf2-112">Idź do [Dodaj użytkowników](#add-users-and-assign-licenses) zamiast.</span><span class="sxs-lookup"><span data-stu-id="3baf2-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Wybierz pozycję Dodaj domenę.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="3baf2-114">W Kreatorze wprowadź nazwę domeny, której chcesz użyć (np. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="3baf2-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Zrzut ekranu Personalizuj swoją stronę logowania.](media/personalizesignin.png)

    
4. <span data-ttu-id="3baf2-116">Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS w dowolnym dostawcy hostingu DNS dla pakietu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , który weryfikuje właścicielem domeny.</span><span class="sxs-lookup"><span data-stu-id="3baf2-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="3baf2-117">Jeśli znasz swojego hosta domeny, zobacz także instrukcje dotyczące [hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="3baf2-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="3baf2-118">Jeśli dostawcą hostingu jest firma GoDaddy lub inny host z włączoną funkcją [Domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces jest łatwy, a użytkownik zostanie automatycznie poproszony o zalogowanie się i niech Microsoft uwierzytelni się w Twoim imieniu:</span><span class="sxs-lookup"><span data-stu-id="3baf2-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect),the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na stronie Potwierdzanie dostępu GoDaddy wybierz Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="3baf2-120">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="3baf2-120">Add users and assign licenses</span></span>

<span data-ttu-id="3baf2-121">Można dodać użytkowników w kreatorze, ale można również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="3baf2-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="3baf2-122">Ponadto jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="3baf2-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="3baf2-123">Dodawanie użytkowników w Kreatorze</span><span class="sxs-lookup"><span data-stu-id="3baf2-123">Add users in the wizard</span></span>

<span data-ttu-id="3baf2-124">Wszyscy użytkownicy dodawani w Kreatorze otrzymują automatycznie przypisaną licencję Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3baf2-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Zrzut ekranu Dodaj nowych użytkowników strony w Kreatorze](media/addnewuserspage.png)

1. <span data-ttu-id="3baf2-126">Jeśli Twoja subskrypcja Microsoft 365 Business ma istniejących użytkowników (na przykład, jeśli używasz programu Azure AD Connect), masz możliwość przypisania licencji do nich teraz.</span><span class="sxs-lookup"><span data-stu-id="3baf2-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="3baf2-127">Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3baf2-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="3baf2-128">Po dodaniu użytkowników otrzymasz również opcję udostępnienia poświadczeń nowym użytkownikom, które dodałeś.</span><span class="sxs-lookup"><span data-stu-id="3baf2-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="3baf2-129">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="3baf2-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="3baf2-130">Pomiń migrację wiadomości e-mail i wybierz przycisk **Dalej** na stronie **Migracja wiadomości e-mail**.</span><span class="sxs-lookup"><span data-stu-id="3baf2-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="3baf2-131">Jeśli przenoś się z innego dostawcy poczty e-mail i chcesz skopiować dane później, możesz [przenieść pocztę e-mail i kontakty do pakietu Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="3baf2-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="3baf2-132">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="3baf2-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="3baf2-133">Jeśli zdecydujesz się użyć domeny. onmicrosoft lub użyć usługi Azure AD Connect do konfigurowania użytkowników, nie zobaczysz tego kroku.</span><span class="sxs-lookup"><span data-stu-id="3baf2-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="3baf2-134">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="3baf2-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="3baf2-135">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="3baf2-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="3baf2-136">Jeśli tak się nie [stanie, Zmień serwery nazw, aby skonfigurować pakiet Office 365 z dowolnym rejestratorem domeny](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="3baf2-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="3baf2-137">Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale Twój host DNS jest włączony dla [połączenia z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), wybierz opcję **Dodaj rekordy dla mnie**.</span><span class="sxs-lookup"><span data-stu-id="3baf2-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> 
    - <span data-ttu-id="3baf2-138">Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie jest włączona dla połączenia z domeną), będziesz chciał zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostać w kontakcie.</span><span class="sxs-lookup"><span data-stu-id="3baf2-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="3baf2-139">Więcej informacji znajdziesz w artykule [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="3baf2-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Połącz stronę domeny z zarządzam własnymi rekordami DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="3baf2-141">Postępuj zgodnie z instrukcjami kreatora, a poczta e-mail i inne usługi zostaną skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="3baf2-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="3baf2-142">Konfigurowanie zasad zabezpieczeń i konfiguracji urządzeń</span><span class="sxs-lookup"><span data-stu-id="3baf2-142">Set up security policies and device configurations</span></span> 

<span data-ttu-id="3baf2-143">Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*.</span><span class="sxs-lookup"><span data-stu-id="3baf2-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="3baf2-144">Można również utworzyć dodatkowe grupy, aby przypisać zasady w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="3baf2-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="3baf2-145">Na stronie **Chroń pliki robocze na urządzeniach przenośnych** opcja **Chroń pliki robocze, gdy urządzenia są zagubione lub skradzione** , jest domyślnie zaznaczona.</span><span class="sxs-lookup"><span data-stu-id="3baf2-145">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="3baf2-146">Masz opcję, aby włączyć zarządzanie, **jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych**, a to jest zalecane.</span><span class="sxs-lookup"><span data-stu-id="3baf2-146">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Zrzut ekranu z Chroń pliki robocze na urządzeniach przenośnych strony.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="3baf2-148">Rozwiń pozycję **Chroń pliki robocze, gdy urządzenia zostaną zgubione lub skradzione** , aby wyświetlić [wartości domyślne](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="3baf2-148">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Zrzut ekranu z wartościami domyślnymi chroniącymi pliki na utraconych urządzeniach.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="3baf2-150">Wybierz **Zarządzaj, jak użytkownicy uzyskują dostęp do plików pakietu Office na urządzeniach przenośnych** i rozwiń go, aby wyświetlić [wartości domyślne](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="3baf2-150">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="3baf2-151">Zaleca się zaakceptowanie wartości domyślnych podczas instalacji, aby utworzyć zasady aplikacji dla systemu Android, iOS i Windows 10, które mają zastosowanie do wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3baf2-151">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="3baf2-152">Po zakończeniu instalacji możesz utworzyć więcej zasad.</span><span class="sxs-lookup"><span data-stu-id="3baf2-152">You can create more policies after setup completes.</span></span>

        ![Zrzut ekranu ustawień ochrony dla plików pakietu Office na urządzeniach przenośnych.](media/useraccessonmobile.png)

2. <span data-ttu-id="3baf2-154">Ostatni krok na temat ochrony danych i urządzeń umożliwia konfigurowanie zasad zabezpieczania urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3baf2-154">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="3baf2-155">Te ustawienia są stosowane automatycznie, gdy użytkownik Windows 10 łączy się z organizacją.</span><span class="sxs-lookup"><span data-stu-id="3baf2-155">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="3baf2-156">Można rozwinąć **bezpieczne urządzenia z systemem Windows 10** , aby zobaczyć i zmodyfikować [wartości domyślne](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="3baf2-156">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="3baf2-157">Można również wybrać opcję [automatycznej instalacji pakietu Office](install-office-on-windows-10-during-setup.md) na urządzeniach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3baf2-157">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Zrzut ekranu zestawu Windows 10 konfiguracji urządzenia strony.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="3baf2-159">Wdrażanie aplikacji klienckich pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="3baf2-159">Deploy Office 365 client apps</span></span>

<span data-ttu-id="3baf2-160">Jeśli wybrano automatyczne instalowanie aplikacji pakietu Office w trakcie konfigurowania, aplikacje zostaną zainstalowane na urządzeniach z systemem Windows 10, gdy użytkownicy zalogują się do usługi Azure AD z ich urządzeń z systemem Windows przy użyciu poświadczeń pracy.</span><span class="sxs-lookup"><span data-stu-id="3baf2-160">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="3baf2-161">Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="3baf2-161">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="3baf2-162">Pakiet Office można również zainstalować osobno.</span><span class="sxs-lookup"><span data-stu-id="3baf2-162">You can also install Office individually.</span></span> <span data-ttu-id="3baf2-163">Instrukcje znajdziesz [w artykule Instalowanie pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="3baf2-163">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
