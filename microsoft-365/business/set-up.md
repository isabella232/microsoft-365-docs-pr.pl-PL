---
title: Konfigurowanie usługi Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zapoznaj się z czynnościami konfiguracji usługi Microsoft 365 Business Premium, w tym dodawaniem domeny i użytkowników, konfigurowaniem zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044735"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="0fa19-103">Konfigurowanie usługi Microsoft 365 Business Premium w kreatorze konfiguracji</span><span class="sxs-lookup"><span data-stu-id="0fa19-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="0fa19-104">Obejrzyj ten klip wideo, aby uzyskać omówienie konfiguracji usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0fa19-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="0fa19-105">Dodawanie domeny, użytkowników i konfigurowanie zasad</span><span class="sxs-lookup"><span data-stu-id="0fa19-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="0fa19-106">Przy zakupie usługi Microsoft 365 Business Premium masz możliwość korzystania z domeny, która należy do Ciebie, lub zakupu jej podczas [rejestracji.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="0fa19-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="0fa19-107">Jeśli podczas rejestracji kupiono nową domenę, to domena jest już wszystko ustawiona. Możesz przejść do dodawania użytkowników [i przypisywania licencji.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="0fa19-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="0fa19-108">Dodaj domenę, aby spersonalizować logowanie</span><span class="sxs-lookup"><span data-stu-id="0fa19-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="0fa19-109">Zaloguj się do [centrum administracyjnego platformy Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="0fa19-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="0fa19-110">Wybierz **pozycję Przejdź do konfiguracji,** aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="0fa19-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="0fa19-112">Na stronie **Instalowanie aplikacji pakietu Office** możesz opcjonalnie zainstalować aplikacje na własnym komputerze.</span><span class="sxs-lookup"><span data-stu-id="0fa19-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="0fa19-113">W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).</span><span class="sxs-lookup"><span data-stu-id="0fa19-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0fa19-114">Jeśli domena została kupiona podczas procesu rejestracji, nie zobaczysz tutaj kroku **Dodaj** domenę.</span><span class="sxs-lookup"><span data-stu-id="0fa19-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="0fa19-115">Zamiast tego [przejdź do przycisku Dodaj użytkowników.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="0fa19-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Zrzut ekranu przedstawiający stronę Personalizowanie logowania.](../media/adddomain.png)

    
4. <span data-ttu-id="0fa19-117">Postępuj zgodnie z instrukcjami kreatora, aby utworzyć rekordy DNS u dowolnego dostawcy hostingu DNS dla platformy [Microsoft 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) który potwierdza, że jesteś właścicielem domeny.</span><span class="sxs-lookup"><span data-stu-id="0fa19-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="0fa19-118">Jeśli znasz swojego hosta domeny, zobacz też [szczegółowe instrukcje dotyczące tego hosta.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="0fa19-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="0fa19-119">Jeśli Twój dostawca hostingu ma usługę GoDaddy lub innego hosta z włączoną obsługą połączenia [domeny,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)ten proces jest łatwy i zostanie automatycznie poproszony o zalogowanie się i uwierzytelnienie przez firmę Microsoft w Twoim imieniu.</span><span class="sxs-lookup"><span data-stu-id="0fa19-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stronie Potwierdzanie dostępu w daddy wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="0fa19-121">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="0fa19-121">Add users and assign licenses</span></span>

<span data-ttu-id="0fa19-122">Użytkowników możesz dodać w kreatorze, ale możesz również dodać użytkowników [później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="0fa19-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="0fa19-123">Ponadto, jeśli masz lokalny kontroler domeny, możesz dodawać użytkowników za pomocą [programu Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="0fa19-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="0fa19-124">Dodawanie użytkowników w kreatorze</span><span class="sxs-lookup"><span data-stu-id="0fa19-124">Add users in the wizard</span></span>

<span data-ttu-id="0fa19-125">Każdy użytkownik, który dodasz w kreatorze, automatycznie otrzyma licencję na usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0fa19-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w kreatorze](../media/addnewuserspage.png)

1. <span data-ttu-id="0fa19-127">Jeśli Twoja subskrypcja usługi Microsoft 365 Business Premium ma już użytkowników (na przykład używaliśmy programu Azure AD Connect), możesz teraz przypisać im licencje.</span><span class="sxs-lookup"><span data-stu-id="0fa19-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="0fa19-128">Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="0fa19-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="0fa19-129">Po dodaniu użytkowników zostanie również dodana opcja udostępnienia poświadczeń nowym użytkownikom.</span><span class="sxs-lookup"><span data-stu-id="0fa19-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="0fa19-130">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="0fa19-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="0fa19-131">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="0fa19-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="0fa19-132">Jeśli wybrano domenę .onmicrosoft lub do skonfigurowania użytkowników używaliśmy programu Azure AD Connect, ten krok nie zostanie wyświetlony.</span><span class="sxs-lookup"><span data-stu-id="0fa19-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="0fa19-133">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="0fa19-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="0fa19-134">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="0fa19-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="0fa19-135">Jeśli tak się nie stanie, zmień serwery nazw, aby skonfigurować usługę [Microsoft 365 u dowolnego rejestratora domen.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="0fa19-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="0fa19-136">Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale dla Twojego hosta DNS włączono funkcję łączenia [domen,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)wybierz pozycję **Dodaj rekordy.**</span><span class="sxs-lookup"><span data-stu-id="0fa19-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="0fa19-137">Na stronie **Wybieranie usług online** zaakceptuj wszystkie ustawienia domyślne, wybierz pozycję Dalej, a następnie wybierz pozycję **Autoryzuj** na stronie swojego hosta DNS. </span><span class="sxs-lookup"><span data-stu-id="0fa19-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="0fa19-138">Jeśli masz istniejące rekordy DNS z innymi hostami DNS (bez włączonego łączenia domen), musisz zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostają połączone.</span><span class="sxs-lookup"><span data-stu-id="0fa19-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="0fa19-139">Aby [uzyskać więcej informacji,](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) zobacz podstawowe informacje o domenie.</span><span class="sxs-lookup"><span data-stu-id="0fa19-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Strona aktywowania rekordów.](../media/activaterecords.png)

2. <span data-ttu-id="0fa19-141">Postępuj zgodnie z instrukcjami kreatora, aby skonfigurować pocztę e-mail i inne usługi.</span><span class="sxs-lookup"><span data-stu-id="0fa19-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="0fa19-142">Ochrona organizacji</span><span class="sxs-lookup"><span data-stu-id="0fa19-142">Protect your organization</span></span> 

<span data-ttu-id="0fa19-143">Zasady ustawione w kreatorze są automatycznie [](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) stosowane do grupy zabezpieczeń o *nazwie Wszyscy użytkownicy.*</span><span class="sxs-lookup"><span data-stu-id="0fa19-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="0fa19-144">W centrum administracyjnym możesz również utworzyć dodatkowe grupy, do których będą przypisywane zasady.</span><span class="sxs-lookup"><span data-stu-id="0fa19-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="0fa19-145">W przypadku opcji Zwiększanie ochrony przed **zaawansowanymi zagrożeniami** cyberzagrożeniami zalecane jest zaakceptowanie ustawień domyślnych, aby pliki i linki w aplikacjach pakietu Office można było skanować za pomocą zaawansowanej ochrony przed zagrożeniami w usłudze [Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="0fa19-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Zrzut ekranu przedstawiający stronę Zwiększanie ochrony.](../media/increasetreatprotection.png)


2. <span data-ttu-id="0fa19-147">Na **stronie Zapobiegaj** wyciekom poufnych danych zaakceptuj ustawienia domyślne, aby włączyć zapobieganie utracie danych (DLP, Data Loss Prevention) usługi Office 365 w celu śledzenia poufnych danych w aplikacjach pakietu Office i zapobiegania przypadkowemu udostępnieniu ich poza twoją organizacją.</span><span class="sxs-lookup"><span data-stu-id="0fa19-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="0fa19-148">Na stronie **Ochrona danych w psłudze Office** dla urządzeń przenośnych pozostaw opcję Zarządzania aplikacją mobilną, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję Utwórz zasady zarządzania aplikacją **mobilną.**</span><span class="sxs-lookup"><span data-stu-id="0fa19-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Zrzut ekranu przedstawiający stronę Ochrona danych w psłudze Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="0fa19-150">Zabezpieczanie komputerów z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="0fa19-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="0fa19-151">W lewym obszarze narracji wybierz pozycję Konfiguracja, a następnie w obszarze Logowanie i zabezpieczenia wybierz pozycję Zabezpiecz swoje komputery z systemem **Windows 10.** </span><span class="sxs-lookup"><span data-stu-id="0fa19-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="0fa19-152">Wybierz **pozycję Widok,** aby rozpocząć.</span><span class="sxs-lookup"><span data-stu-id="0fa19-152">Choose **View** to get started.</span></span> <span data-ttu-id="0fa19-153">Zapoznaj się z bezpiecznymi komputerami z systemem [Windows 10,](secure-win-10-pcs.md) aby uzyskać pełne instrukcje.</span><span class="sxs-lookup"><span data-stu-id="0fa19-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="0fa19-154">Wdrażanie aplikacji klienckich usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="0fa19-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="0fa19-155">Jeśli wybierzesz automatyczne instalowanie aplikacji pakietu Office podczas instalacji, zostaną one zainstalowane na urządzeniach z systemem Windows 10 po zalogowaniu się użytkowników do usługi Azure AD na swoich urządzeniach z systemem Windows przy użyciu poświadczeń służbowych.</span><span class="sxs-lookup"><span data-stu-id="0fa19-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="0fa19-156">Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz Konfigurowanie urządzeń przenośnych dla użytkowników usługi [Microsoft 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="0fa19-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="0fa19-157">Możesz również zainstalować pakiet Office pojedynczo.</span><span class="sxs-lookup"><span data-stu-id="0fa19-157">You can also install Office individually.</span></span> <span data-ttu-id="0fa19-158">Aby [uzyskać instrukcje,](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) zobacz instalowanie pakietu Office na komputerze PC lub Mac.</span><span class="sxs-lookup"><span data-stu-id="0fa19-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="0fa19-159">Zobacz też</span><span class="sxs-lookup"><span data-stu-id="0fa19-159">See also</span></span>

[<span data-ttu-id="0fa19-160">Szkolenia dotyczące platformy Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="0fa19-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
