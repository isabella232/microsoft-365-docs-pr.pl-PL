---
title: Konfigurowanie programu Microsoft 365 Business Premium
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
description: Odkryj kroki konfiguracji programu Microsoft 365 Business Premium, w tym dodawanie domeny i użytkowników, Konfigurowanie zasad zabezpieczeń i nie tylko.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324501"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="8ae47-103">Konfigurowanie usługi Microsoft 365 Business Premium w Kreatorze konfiguracji</span><span class="sxs-lookup"><span data-stu-id="8ae47-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="8ae47-104">Obejrzyj ten klip wideo, aby zapoznać się z omówieniem konfiguracji programu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8ae47-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="8ae47-105">Dodawanie domeny, użytkowników i Konfigurowanie zasad</span><span class="sxs-lookup"><span data-stu-id="8ae47-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="8ae47-106">Po zakupie produktu Microsoft 365 Business Premium możesz korzystać z domeny, którą posiadasz, lub kupić ją podczas [tworzenia konta](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="8ae47-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="8ae47-107">Jeśli nowa domena została zakupiona podczas tworzenia konta, Twoja domena jest skonfigurowana i możesz ją przenieść, aby [dodać użytkowników i przypisać licencje](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="8ae47-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="8ae47-108">Dodawanie domeny w celu personalizacji logowania</span><span class="sxs-lookup"><span data-stu-id="8ae47-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="8ae47-109">Zaloguj się do [Centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com) przy użyciu poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="8ae47-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="8ae47-110">Wybierz pozycję **Przejdź do konfiguracji** , aby uruchomić kreatora.</span><span class="sxs-lookup"><span data-stu-id="8ae47-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Wybierz pozycję Przejdź do konfiguracji.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="8ae47-112">Na stronie **Instalowanie aplikacji pakietu Office** możesz opcjonalnie zainstalować aplikacje na własnym komputerze.</span><span class="sxs-lookup"><span data-stu-id="8ae47-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="8ae47-113">W kroku **Dodaj domenę** wprowadź nazwę domeny, której chcesz użyć (na przykład contoso.com).</span><span class="sxs-lookup"><span data-stu-id="8ae47-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="8ae47-114">Jeśli w trakcie tworzenia konta została kupiona domena, w tym miejscu nie będzie widoczny krok **Dodaj domenę** .</span><span class="sxs-lookup"><span data-stu-id="8ae47-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="8ae47-115">Zamiast tego przejdź do obszaru [Dodaj użytkowników](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="8ae47-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Zrzut ekranu przedstawiający stronę logowania.](../media/adddomain.png)

    
4. <span data-ttu-id="8ae47-117">Postępuj zgodnie z instrukcjami kreatora, aby [utworzyć rekordy DNS u dowolnego dostawcy hostingu DNS dla systemu Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , który weryfikuje, że jesteś właścicielem domeny.</span><span class="sxs-lookup"><span data-stu-id="8ae47-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="8ae47-118">Jeśli znasz hosta domeny, zobacz też [instrukcje dotyczące hosta](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="8ae47-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="8ae47-119">Jeśli Twój dostawca hostingu jest GoDaddy lub inny host jest włączony z funkcją [łączenia się z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces jest prosty i automatycznie zostanie wyświetlony monit o zalogowanie się i umożliwienie firmie Microsoft uwierzytelniania w Twoim imieniu.</span><span class="sxs-lookup"><span data-stu-id="8ae47-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stronie GoDaddy Potwierdź dostęp wybierz pozycję Autoryzuj.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="8ae47-121">Dodawanie użytkowników i przypisywanie licencji</span><span class="sxs-lookup"><span data-stu-id="8ae47-121">Add users and assign licenses</span></span>

<span data-ttu-id="8ae47-122">Możesz dodać użytkowników w kreatorze, ale możesz również [dodać użytkowników później](add-users-m365b.md) w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="8ae47-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="8ae47-123">Ponadto, jeśli masz lokalny kontroler domeny, możesz dodać użytkowników za pomocą funkcji [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="8ae47-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="8ae47-124">Dodawanie użytkowników w Kreatorze</span><span class="sxs-lookup"><span data-stu-id="8ae47-124">Add users in the wizard</span></span>

<span data-ttu-id="8ae47-125">Wszyscy użytkownicy dodaniu w Kreatorze uzyskają automatycznie przypisaną licencję Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8ae47-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Zrzut ekranu przedstawiający stronę Dodawanie nowych użytkowników w Kreatorze](../media/addnewuserspage.png)

1. <span data-ttu-id="8ae47-127">Jeśli Twoja subskrypcja programu Microsoft 365 Business Premium ma istniejących użytkowników (na przykład w przypadku korzystania z usługi Azure AD Connect), uzyskasz możliwość przydzielenia im licencji.</span><span class="sxs-lookup"><span data-stu-id="8ae47-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="8ae47-128">Możesz dodać licencje dla tych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="8ae47-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="8ae47-129">Po dodaniu użytkowników możesz także skorzystać z opcji udostępniania poświadczeń nowym użytkownikom, które dodali.</span><span class="sxs-lookup"><span data-stu-id="8ae47-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="8ae47-130">Możesz wydrukować te informacje, wysłać je pocztą e-mail lub pobrać.</span><span class="sxs-lookup"><span data-stu-id="8ae47-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="8ae47-131">Łączenie domeny</span><span class="sxs-lookup"><span data-stu-id="8ae47-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="8ae47-132">Jeśli w celu skonfigurowania użytkowników użyto domeny. onmicrosoft lub usługi Azure AD Connect, ten krok nie będzie widoczny.</span><span class="sxs-lookup"><span data-stu-id="8ae47-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="8ae47-133">Aby skonfigurować usługi, musisz zaktualizować niektóre rekordy na swoim hoście DNS lub u rejestratora domen.</span><span class="sxs-lookup"><span data-stu-id="8ae47-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="8ae47-134">Kreator konfiguracji zwykle wykrywa rejestratora i udostępnia linki do instrukcji krok po kroku dotyczących aktualizowania rekordów serwera nazw w witrynie internetowej rejestratora.</span><span class="sxs-lookup"><span data-stu-id="8ae47-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="8ae47-135">Jeśli nie, [Zmień serwery nazw, aby skonfigurować aplikację Microsoft 365 z dowolnym rejestratorem domen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="8ae47-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="8ae47-136">Jeśli masz istniejące rekordy DNS, na przykład istniejącą witrynę sieci Web, ale Twój host DNS jest włączony dla [połączenia z domeną](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), wybierz pozycję **Dodaj rekordy dla mnie**.</span><span class="sxs-lookup"><span data-stu-id="8ae47-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="8ae47-137">Na stronie **Wybieranie usług online** Zaakceptuj wszystkie ustawienia domyślne i wybierz pozycję **dalej**, a następnie wybierz pozycję **AUTORYZUJ** na stronie swojego hosta DNS.</span><span class="sxs-lookup"><span data-stu-id="8ae47-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="8ae47-138">Jeśli masz istniejące rekordy DNS z innymi hostami DNS (nie włączono dla połączenia z domeną), możesz zarządzać własnymi rekordami DNS, aby upewnić się, że istniejące usługi pozostają połączone.</span><span class="sxs-lookup"><span data-stu-id="8ae47-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="8ae47-139">Aby uzyskać więcej informacji, zobacz podstawowe informacje o [domenie](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="8ae47-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Strona aktywowania rekordów.](../media/activaterecords.png)

2. <span data-ttu-id="8ae47-141">Postępuj zgodnie z instrukcjami w kreatorze, a poczta e-mail i inne usługi zostaną skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="8ae47-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="8ae47-142">Ochrona organizacji</span><span class="sxs-lookup"><span data-stu-id="8ae47-142">Protect your organization</span></span> 

<span data-ttu-id="8ae47-143">Zasady skonfigurowane w kreatorze są automatycznie stosowane do [grup zabezpieczeń](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) o nazwie *Wszyscy użytkownicy*.</span><span class="sxs-lookup"><span data-stu-id="8ae47-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="8ae47-144">Możesz również utworzyć dodatkowe grupy, aby przypisać zasady w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="8ae47-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="8ae47-145">W przypadku **zaawansowanych zagrożeń cyber**zaleca się zaakceptowanie ustawień domyślnych, aby umożliwić [ochronę przed zagrożeniami pakietu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanowanie plików i linków w aplikacjach pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="8ae47-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Zrzut ekranu przedstawiający stronę zwiększania ochrony.](../media/increasetreatprotection.png)


2. <span data-ttu-id="8ae47-147">Na stronie **zapobieganie przeciekom wrażliwych danych** zaakceptuj ustawienia domyślne, aby włączyć ochronę przed utratą danych pakietu Office 365 (DLP) w celu śledzenia wrażliwych danych w aplikacjach pakietu Office i zapobiegania przypadkowemu udostępnianiu tych informacji poza organizacją.</span><span class="sxs-lookup"><span data-stu-id="8ae47-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="8ae47-148">Na stronie **Ochrona danych w pakiecie Office dla urządzeń przenośnych** pozostaw pozycję Zarządzanie aplikacjami mobilnymi, rozwiń ustawienia i przejrzyj je, a następnie wybierz pozycję **Utwórz zasady zarządzania aplikacjami mobilnymi**.</span><span class="sxs-lookup"><span data-stu-id="8ae47-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Zrzut ekranu przedstawiający ochronę danych w pakiecie Office dla urządzeń przenośnych.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="8ae47-150">Bezpieczne komputery z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="8ae47-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="8ae47-151">W lewym okienku nawigacji wybierz pozycję **Konfiguracja** , a następnie w obszarze **Logowanie i zabezpieczenia**wybierz pozycję **Zabezpiecz komputery z systemem Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="8ae47-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="8ae47-152">Wybierz pozycję **Wyświetl** , aby rozpocząć.</span><span class="sxs-lookup"><span data-stu-id="8ae47-152">Choose **View** to get started.</span></span> <span data-ttu-id="8ae47-153">Zobacz [Zabezpieczanie komputerów z systemem Windows 10](secure-win-10-pcs.md) , aby uzyskać pełne instrukcje.</span><span class="sxs-lookup"><span data-stu-id="8ae47-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="8ae47-154">Wdrażanie aplikacji klienckich pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="8ae47-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="8ae47-155">Jeśli podczas instalacji wybrano opcję automatycznego instalowania aplikacji pakietu Office, aplikacje te zostaną zainstalowane na urządzeniach z systemem Windows 10, gdy użytkownicy zalogują się do usługi Azure AD z urządzeń z systemem Windows za pomocą poświadczeń służbowych.</span><span class="sxs-lookup"><span data-stu-id="8ae47-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="8ae47-156">Aby zainstalować pakiet Office na urządzeniach przenośnych z systemem iOS lub Android, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business Premium](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="8ae47-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="8ae47-157">Możesz również zainstalować pakiet Office osobno.</span><span class="sxs-lookup"><span data-stu-id="8ae47-157">You can also install Office individually.</span></span> <span data-ttu-id="8ae47-158">Aby uzyskać instrukcje, zobacz [Instalowanie pakietu Office na komputerze PC lub Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="8ae47-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="8ae47-159">Zobacz też</span><span class="sxs-lookup"><span data-stu-id="8ae47-159">See also</span></span>

[<span data-ttu-id="8ae47-160">Szkolenia wideo dotyczące programu Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="8ae47-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
