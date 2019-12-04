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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dowiedz się, jak skonfigurować firmę Microsoft 365 Business.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831308"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="2cf8b-103">Konfigurowanie Microsoft 365 Business w Kreatorze instalacji</span><span class="sxs-lookup"><span data-stu-id="2cf8b-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="2cf8b-104">Obejrzyj ten film, aby uzyskać omówienie konfiguracji firmy Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="2cf8b-105">Jeśli znalazłeś ten film pomocne, sprawdź [kompletny cykl szkoleń dla małych firm i tych nowych Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="2cf8b-106">Dodawanie domeny, użytkowników i Konfigurowanie zasad</span><span class="sxs-lookup"><span data-stu-id="2cf8b-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="2cf8b-107">[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="2cf8b-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="2cf8b-108">Podczas zakupu Microsoft 365 Business, masz możliwość korzystania z domeny, którą posiadasz, lub kupując go podczas [rejestracji](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="2cf8b-109">Jeśli po zalogowaniu się zarejestrowano nową domenę, domena jest ustawiona i można ją przenieść, aby [dodać użytkowników i przypisać licencje](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="2cf8b-110">Dodawanie domeny w celu personalizacji logowania</span><span class="sxs-lookup"><span data-stu-id="2cf8b-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="2cf8b-111">Zaloguj się do [Centrum administracyjnego Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="2cf8b-112">Wybierz **Przejdź do konfiguracji** , aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Wybierz pozycję Przejdź do konfiguracji.](media/gotosetupinadmincenter.png)

3. <span data-ttu-id="2cf8b-114">Na stronie **Instalowanie aplikacji pakietu Office** można opcjonalnie instalować aplikacje na własnym komputerze.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="2cf8b-115">W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (np. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="2cf8b-116">Jeśli domena została kupiona podczas rejestracji, nie zobaczysz tutaj kroku **Dodaj domenę** .</span><span class="sxs-lookup"><span data-stu-id="2cf8b-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="2cf8b-117">Idź do [Dodaj użytkowników](#add-users-and-assign-licenses) zamiast.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Zrzut ekranu Personalizuj swoją stronę logowania.](media/adddomain.png)

    
4. <span data-ttu-id="2cf8b-119">Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS w dowolnym dostawcy hostingu DNS dla pakietu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , który weryfikuje właścicielem domeny.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="2cf8b-120">Jeśli znasz swojego hosta domeny, zobacz także instrukcje dotyczące [hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="2cf8b-121">Jeśli dostawcą hostingu jest firma GoDaddy lub inny host z włączoną funkcją [Połącz z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces jest łatwy i automatycznie zostanie wyświetlony monit o zalogowanie się i pozwolić firmie Microsoft na uwierzytelnienie w Twoim imieniu.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stronie Potwierdzanie dostępu GoDaddy wybierz Autoryzuj.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="2cf8b-123">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="2cf8b-123">Add users and assign licenses</span></span>

<span data-ttu-id="2cf8b-124">Można dodać użytkowników w kreatorze, ale można również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="2cf8b-125">Ponadto jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="2cf8b-126">Dodawanie użytkowników w Kreatorze</span><span class="sxs-lookup"><span data-stu-id="2cf8b-126">Add users in the wizard</span></span>

<span data-ttu-id="2cf8b-127">Wszyscy użytkownicy dodawani w Kreatorze otrzymują automatycznie przypisaną licencję Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Zrzut ekranu Dodaj nowych użytkowników strony w Kreatorze](media/addnewuserspage.png)

1. <span data-ttu-id="2cf8b-129">Jeśli Twoja subskrypcja Microsoft 365 Business ma istniejących użytkowników (na przykład, jeśli używasz programu Azure AD Connect), masz możliwość przypisania licencji do nich teraz.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="2cf8b-130">Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="2cf8b-131">Po dodaniu użytkowników otrzymasz również opcję udostępnienia poświadczeń nowym użytkownikom, które dodałeś.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="2cf8b-132">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="2cf8b-133">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="2cf8b-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="2cf8b-134">Jeśli zdecydujesz się użyć domeny. onmicrosoft lub użyć usługi Azure AD Connect do konfigurowania użytkowników, nie zobaczysz tego kroku.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="2cf8b-135">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="2cf8b-136">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="2cf8b-137">Jeśli tak się nie [stanie, Zmień serwery nazw, aby skonfigurować pakiet Office 365 z dowolnym rejestratorem domeny](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="2cf8b-138">Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale Twój host DNS jest włączony dla [połączenia z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), wybierz opcję **Dodaj rekordy dla mnie**.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="2cf8b-139">Na stronie **Wybieranie usług online** Zaakceptuj wszystkie ustawienia domyślne i wybierz pozycję **dalej**, a następnie wybierz pozycję **AUTORYZUJ** na stronie hosta DNS.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="2cf8b-140">Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie jest włączona dla połączenia z domeną), będziesz chciał zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostać w kontakcie.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="2cf8b-141">Więcej informacji znajdziesz w artykule [podstawy domeny](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="2cf8b-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktywuj rekordy strony.](media/activaterecords.png)

2. <span data-ttu-id="2cf8b-143">Postępuj zgodnie z instrukcjami kreatora, a poczta e-mail i inne usługi zostaną skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="2cf8b-144">Chroń swoją organizację</span><span class="sxs-lookup"><span data-stu-id="2cf8b-144">Protect your organization</span></span> 

<span data-ttu-id="2cf8b-145">Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grupy zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="2cf8b-146">Można również utworzyć dodatkowe grupy, aby przypisać zasady w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="2cf8b-147">W sprawie **zwiększenia ochrony przed zaawansowanymi zagrożeniami cybernetycznymi**zaleca się zaakceptowanie wartości domyślnych, aby pozwolić, aby pliki skanowania [pakietu Office 365 z wyprzedzeniem ochrony przed zagrożeniami](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) i łącza w aplikacjach pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Zrzut ekranu strony Zwiększ ochronę.](media/increasetreatprotection.png)


2. <span data-ttu-id="2cf8b-149">Na **zapobieganie przeciekom poufnych danych** strony, zaakceptuj ustawienia domyślne, aby włączyć Office 365 ochrony przed utratą danych (DLP) do śledzenia poufnych danych w aplikacjach pakietu Office i zapobiec przypadkowemu udostępnieniu tych poza organizacją.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="2cf8b-150">Na stronie **Chroń dane w pakiecie Office dla urządzeń przenośnych** pozostaw Zarządzanie aplikacjami mobilnymi, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję **Utwórz zasady zarządzania aplikacjami mobilnymi**.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Zrzut ekranu z Chroń dane w pakiecie Office dla urządzeń przenośnych strony.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="2cf8b-152">Bezpieczne komputery z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="2cf8b-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="2cf8b-153">Na lewej NAV wybierz **Ustawienia** , a następnie w obszarze **Sing-in i zabezpieczeń**, wybierz opcję **Zabezpiecz komputery z systemem Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="2cf8b-154">Wybierz **Widok** aby rozpocząć.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-154">Choose **View** to get started.</span></span> <span data-ttu-id="2cf8b-155">Aby uzyskać pełne instrukcje, zobacz [Zabezpieczanie komputerów z systemem Windows 10](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="2cf8b-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="2cf8b-156">Wdrażanie aplikacji klienckich pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="2cf8b-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="2cf8b-157">Jeśli wybrano opcję automatycznego instalowania aplikacji pakietu Office podczas instalacji, aplikacje zostaną zainstalowane na urządzeniach z systemem Windows 10, gdy użytkownicy zalogują się do usługi Azure AD z ich urządzeń z systemem Windows przy użyciu poświadczeń pracy.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="2cf8b-158">Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="2cf8b-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="2cf8b-159">Pakiet Office można również zainstalować osobno.</span><span class="sxs-lookup"><span data-stu-id="2cf8b-159">You can also install Office individually.</span></span> <span data-ttu-id="2cf8b-160">Instrukcje znajdziesz [w artykule Instalowanie pakietu Office na komputerze PC lub Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="2cf8b-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="2cf8b-161">See also</span><span class="sxs-lookup"><span data-stu-id="2cf8b-161">See also</span></span>

[<span data-ttu-id="2cf8b-162">Filmy szkoleniowe Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="2cf8b-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
