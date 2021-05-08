---
title: Konfigurowanie Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z krokami konfiguracji Microsoft 365 Business Premium, w tym dodawanie domeny i użytkowników, konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: 37607b483686fc12ac6253ae9f693ec86c073c4e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245049"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="5e446-103">Konfigurowanie Microsoft 365 Business Premium kreatora konfiguracji</span><span class="sxs-lookup"><span data-stu-id="5e446-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="5e446-104">Obejrzyj ten klip wideo, aby uzyskać omówienie Microsoft 365 Business Premium konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="5e446-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="5e446-105">Dodawanie domeny, użytkowników i konfigurowanie zasad</span><span class="sxs-lookup"><span data-stu-id="5e446-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="5e446-106">Podczas zakupu Microsoft 365 Business Premium masz możliwość używania domeny, która należy do Ciebie, lub kupowania jej podczas [rejestracji](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="5e446-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="5e446-107">Jeśli podczas rejestracji w domenie kupiono nową domenę, to jest ona w ogóle ustawiona. Możesz przejść do dodawania użytkowników [i przypisywania licencji.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="5e446-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="5e446-108">Dodawanie domeny w celu spersonalizowania logowania</span><span class="sxs-lookup"><span data-stu-id="5e446-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="5e446-109">Zaloguj się do [Microsoft 365 administracyjnego](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="5e446-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="5e446-110">Wybierz **pozycję Przejdź do konfiguracji,** aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="5e446-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="5e446-112">Na **stronie Instalowanie Office aplikacji** możesz opcjonalnie zainstalować te aplikacje na swoim komputerze.</span><span class="sxs-lookup"><span data-stu-id="5e446-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="5e446-113">W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5e446-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="5e446-114">Jeśli podczas rejestracji zakupiono domenę, nie zobaczysz tutaj kroku **Dodaj** domenę.</span><span class="sxs-lookup"><span data-stu-id="5e446-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="5e446-115">Zamiast tego [przejdź do przycisku Dodaj](#add-users-and-assign-licenses) użytkowników.</span><span class="sxs-lookup"><span data-stu-id="5e446-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Zrzut ekranu przedstawiający stronę Personalizowanie logowania.](../media/adddomain.png)

    
4. <span data-ttu-id="5e446-117">Postępuj zgodnie z instrukcjami kreatora, aby utworzyć rekordy DNS u dowolnego dostawcy [hostingu DNS](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) dla Microsoft 365 weryfikację prawa do domeny.</span><span class="sxs-lookup"><span data-stu-id="5e446-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="5e446-118">Jeśli znasz hosta domeny, zobacz też szczegółowe [instrukcje dla danego hosta.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="5e446-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="5e446-119">Jeśli Twój dostawca hostingu to Firma [](/office365/admin/get-help-with-domains/domain-connect)GoDaddy lub inny host z włączonym nawiązywaniem połączenia z domeną, ten proces jest łatwy i zostanie automatycznie poproszony o zalogowanie się i uwierzytelnienie przez firmę Microsoft w Twoim imieniu.</span><span class="sxs-lookup"><span data-stu-id="5e446-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stronie Potwierdzanie dostępu w daddy wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="5e446-121">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="5e446-121">Add users and assign licenses</span></span>

<span data-ttu-id="5e446-122">Użytkowników można dodać w kreatorze, ale można też [dodać](../admin/add-users/add-users.md) ich później w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="5e446-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="5e446-123">Ponadto, jeśli masz lokalny kontroler domeny, możesz dodawać użytkowników z [usługą Azure AD Połączenie.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="5e446-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="5e446-124">Dodawanie użytkowników w kreatorze</span><span class="sxs-lookup"><span data-stu-id="5e446-124">Add users in the wizard</span></span>

<span data-ttu-id="5e446-125">Użytkownicy, których dodasz w kreatorze, zostaną automatycznie przypisani do Microsoft 365 Business Premium licencji.</span><span class="sxs-lookup"><span data-stu-id="5e446-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w kreatorze](../media/addnewuserspage.png)

1. <span data-ttu-id="5e446-127">Jeśli Twoja Microsoft 365 Business Premium ma już użytkowników (na przykład jeśli używasz usługi Azure AD Połączenie), możesz teraz przypisać im licencje.</span><span class="sxs-lookup"><span data-stu-id="5e446-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="5e446-128">Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="5e446-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="5e446-129">Po dodaniu użytkowników zostanie również dodana opcja udostępnienia poświadczeń nowym użytkownikom.</span><span class="sxs-lookup"><span data-stu-id="5e446-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="5e446-130">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="5e446-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="5e446-131">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="5e446-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="5e446-132">Jeśli do skonfigurowania użytkowników wybrano domenę .onmicrosoft lub do skonfigurowania użytkowników była używana usługa Azure AD Połączenie, ten krok nie zostanie wyświetlony.</span><span class="sxs-lookup"><span data-stu-id="5e446-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="5e446-133">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="5e446-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="5e446-134">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="5e446-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="5e446-135">Jeśli tak się nie stanie, zmień serwery nazw, aby Microsoft 365 [u dowolnego rejestratora domen.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="5e446-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="5e446-136">Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę internetową, ale dla Twojego hosta DNS włączono łączenie [domen,](/office365/admin/get-help-with-domains/domain-connect)wybierz pozycję **Dodaj rekordy.**</span><span class="sxs-lookup"><span data-stu-id="5e446-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="5e446-137">Na stronie **Wybierz usługi online** zaakceptuj wszystkie ustawienia domyślne, wybierz pozycję **Dalej,** a następnie wybierz pozycję **Autoryzuj** na stronie swojego hosta DNS.</span><span class="sxs-lookup"><span data-stu-id="5e446-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="5e446-138">Jeśli masz istniejące rekordy DNS z innymi hostami DNS (bez włączonego łączenia domen), musisz zarządzać swoimi rekordami DNS, aby upewnić się, że istniejące usługi pozostają połączone.</span><span class="sxs-lookup"><span data-stu-id="5e446-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="5e446-139">Aby [uzyskać więcej informacji, zobacz](/office365/admin/get-help-with-domains/dns-basics) Podstawowe informacje o domenie.</span><span class="sxs-lookup"><span data-stu-id="5e446-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktywowanie strony rekordów.](../media/activaterecords.png)

2. <span data-ttu-id="5e446-141">Postępuj zgodnie z instrukcjami kreatora, aby skonfigurować pocztę e-mail i inne usługi.</span><span class="sxs-lookup"><span data-stu-id="5e446-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="5e446-142">Ochrona organizacji</span><span class="sxs-lookup"><span data-stu-id="5e446-142">Protect your organization</span></span> 

<span data-ttu-id="5e446-143">Zasady ustawione w kreatorze są automatycznie stosowane do [grupy](/office365/admin/create-groups/compare-groups#security-groups) zabezpieczeń o nazwie *Wszyscy użytkownicy.*</span><span class="sxs-lookup"><span data-stu-id="5e446-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="5e446-144">Możesz również utworzyć dodatkowe grupy, do których będą przypisywane zasady w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="5e446-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="5e446-145">Na stronie Zwiększanie ochrony przed **zaawansowanymi zagrożeniami** cyberzagrożeniami zalecane jest zaakceptowanie ustawień domyślnych w celu Office 365 zaawansowanej ochrony przed zagrożeniami w plikach i linkach w Office aplikacjach. [](../security/office-365-security/defender-for-office-365.md)</span><span class="sxs-lookup"><span data-stu-id="5e446-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Zrzut ekranu przedstawiający stronę Zwiększanie ochrony.](../media/increasetreatprotection.png)


2. <span data-ttu-id="5e446-147">Na stronie **Zapobiegaj wyciekom poufnych** danych zaakceptuj wartości domyślne Office 365, aby włączyć zapobieganie utracie danych (DLP, Data Loss Prevention) w celu śledzenia poufnych danych w aplikacjach Office i zapobiegania przypadkowemu udostępnianiu tych danych poza Twoją organizacją.</span><span class="sxs-lookup"><span data-stu-id="5e446-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="5e446-148">Na stronie **Ochrona danych w aplikacji Office** dla urządzeń przenośnych pozostaw opcję zarządzanie aplikacją mobilną wł., rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję Utwórz zasady zarządzania aplikacją **mobilną.**</span><span class="sxs-lookup"><span data-stu-id="5e446-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Zrzut ekranu przedstawiający stronę Ochrona danych Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="5e446-150">Zabezpieczanie Windows 10 komputerach</span><span class="sxs-lookup"><span data-stu-id="5e446-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="5e446-151">W okienku po lewej stronie wybierz pozycję **Konfiguracja,** a następnie w obszarze Logowanie się i zabezpieczenia wybierz pozycję Zabezpiecz swoje **Windows 10 komputerach**.</span><span class="sxs-lookup"><span data-stu-id="5e446-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="5e446-152">Wybierz **pozycję Widok,** aby rozpocząć.</span><span class="sxs-lookup"><span data-stu-id="5e446-152">Choose **View** to get started.</span></span> <span data-ttu-id="5e446-153">Zobacz [Zabezpieczanie komputera Windows 10, aby](secure-win-10-pcs.md) uzyskać pełne instrukcje.</span><span class="sxs-lookup"><span data-stu-id="5e446-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="5e446-154">Wdrażanie Office 365 klienckich</span><span class="sxs-lookup"><span data-stu-id="5e446-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="5e446-155">Jeśli podczas instalacji wybierzesz automatyczne instalowanie aplikacji Office, zostaną one zainstalowane na urządzeniach z systemem Windows 10 po zalogowaniu się użytkowników do usługi Azure AD na ich urządzeniach z systemem Windows przy użyciu poświadczeń służbowych.</span><span class="sxs-lookup"><span data-stu-id="5e446-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="5e446-156">Aby zainstalować Office urządzeniach przenośnych z systemem iOS lub Android, zobacz Konfigurowanie urządzeń przenośnych [Microsoft 365 Business Premium użytkowników.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="5e446-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="5e446-157">Możesz również zainstalować pakiet Office instalacji pojedynczo.</span><span class="sxs-lookup"><span data-stu-id="5e446-157">You can also install Office individually.</span></span> <span data-ttu-id="5e446-158">Aby [uzyskać instrukcje,](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) Office zainstalować pakiet na komputerze PC lub Mac.</span><span class="sxs-lookup"><span data-stu-id="5e446-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="5e446-159">Zobacz też</span><span class="sxs-lookup"><span data-stu-id="5e446-159">See also</span></span>

[<span data-ttu-id="5e446-160">Microsoft 365 szkoleniowe klipy wideo dla firm</span><span class="sxs-lookup"><span data-stu-id="5e446-160">Microsoft 365 for business training videos</span></span>](../business-video/index.yml)
