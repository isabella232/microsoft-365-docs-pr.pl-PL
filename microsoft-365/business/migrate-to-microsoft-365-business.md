---
title: Uaktualnienie do wersji Microsoft 365 Business z pakietu Office 365 Business Premium
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Kroki, które uaktualnią firmę z pakietu Office 365 Business Premium do firmy Microsoft 365 Business.
ms.openlocfilehash: f3a25746cf123fa471c29084a62a6fcfc1542a02
ms.sourcegitcommit: f0a4290793e296474ecd3c6eb0ca96eae7faa434
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/11/2019
ms.locfileid: "38231416"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a><span data-ttu-id="a97df-103">Uaktualnienie do wersji Microsoft 365 Business z pakietu Office 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="a97df-103">Upgrade to Microsoft 365 Business from Office 365 Business Premium</span></span>

<span data-ttu-id="a97df-104">Jeśli masz [office 365 dla subskrypcji biznesowych](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), na przykład Office 365 Business Premium, można łatwo uaktualnić do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="a97df-104">If you have an [Office 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Office 365 Business Premium, you can easily upgrade to Microsoft 365 Business.</span></span> <span data-ttu-id="a97df-105">Uaktualnienie do firmy Microsoft 365 Business, jeśli chcesz dodać:</span><span class="sxs-lookup"><span data-stu-id="a97df-105">Upgrade to Microsoft 365 Business if you want to add:</span></span> 
- <span data-ttu-id="a97df-106">Windows 10 Pro (na komputerach z systemem Windows 8 lub nowszym)</span><span class="sxs-lookup"><span data-stu-id="a97df-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>
- <span data-ttu-id="a97df-107">Proste elementy sterujące, które zarządzają danymi biznesowymi na urządzeniach</span><span class="sxs-lookup"><span data-stu-id="a97df-107">Simple controls that manage business data on devices</span></span>
- <span data-ttu-id="a97df-108">Zaawansowane funkcje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="a97df-108">Advanced security capabilities.</span></span>
<span data-ttu-id="a97df-109">Dowiedz się więcej o Microsoft 365 Business w [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="a97df-109">Find out more about Microsoft 365 Business at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a><span data-ttu-id="a97df-110">Jaka jest różnica między pakietem Office 365 Business Premium a Microsoft 365 Business?</span><span class="sxs-lookup"><span data-stu-id="a97df-110">What's the difference between Office 365 Business Premium and Microsoft 365 Business?</span></span>
<span data-ttu-id="a97df-111">Dodaliśmy porównanie Side-by-Side tych dwóch planów do [opisu usługi Microsoft 365 Business](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="a97df-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business service description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="a97df-112">Zanim zaczniesz</span><span class="sxs-lookup"><span data-stu-id="a97df-112">Before you get started</span></span>

- <span data-ttu-id="a97df-113">**Kiedy należy wybrać uaktualnienie?**</span><span class="sxs-lookup"><span data-stu-id="a97df-113">**When should I choose upgrade?**</span></span> <span data-ttu-id="a97df-114">Uaktualnienie jest właściwym wyborem, gdy chcesz uaktualnić **wszystkich użytkowników** przypisanych do jednego planu.</span><span class="sxs-lookup"><span data-stu-id="a97df-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="a97df-115">Po wybraniu uaktualnienia wszyscy użytkownicy planu zostaną przełączone na inny plan w tym samym czasie.</span><span class="sxs-lookup"><span data-stu-id="a97df-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="a97df-116">Jeśli nie chcesz uaktualnić wszystkich przypisanych do jednego planu, Kup licencje dla nowego planu (w tym przypadku Microsoft 365 Business) i [Przypisz te licencje osobno](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) każdemu użytkownikowi, który chcesz uaktualnić.</span><span class="sxs-lookup"><span data-stu-id="a97df-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business), and [assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) to each user that you want to upgrade.</span></span> 
- <span data-ttu-id="a97df-117">**Niektóre dodatki mogą uniemożliwić uaktualnienie** Jeśli próbujesz uruchomić uaktualnienie i masz dodatek, który uniemożliwia kontynuowanie, możesz najpierw usunąć dodatek, a następnie dodać go z powrotem później-Jeśli nadal potrzebujesz.</span><span class="sxs-lookup"><span data-stu-id="a97df-117">**Some add-ons might prevent upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later - if you still need it.</span></span> 
- <span data-ttu-id="a97df-118">**Jeśli przedpłacono plan** Nie ma prostej ścieżki uaktualniania dla planów przedpłaty.</span><span class="sxs-lookup"><span data-stu-id="a97df-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="a97df-119">Będziesz wiedzieć, czy masz plan przedpłaty, ponieważ plan został skonfigurowany przy użyciu identyfikatora produktu zakupionego w sklepie.</span><span class="sxs-lookup"><span data-stu-id="a97df-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="a97df-120">Skontaktuj się z partnerem, przejdź do sklepu Microsoft lub poczekaj, aż plan przedpłaty wygaśnie, aby przełączyć się na nowy plan.</span><span class="sxs-lookup"><span data-stu-id="a97df-120">Contact a partner, go to the Microsoft store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business"></a><span data-ttu-id="a97df-121">Uaktualnienie do Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="a97df-121">Upgrade to Microsoft 365 Business</span></span>
<span data-ttu-id="a97df-122">Kup licencje, wykonując następujące kroki w [nowym centrum administracyjnym](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span><span class="sxs-lookup"><span data-stu-id="a97df-122">Buy your licenses by following these steps in the [new admin center](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span></span>
1. <span data-ttu-id="a97df-123">Zaloguj się do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="a97df-123">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>
2. <span data-ttu-id="a97df-124">Przejdź do okienka nawigacji i wybierz produkty do **rozliczeń** \> **& usługi**.</span><span class="sxs-lookup"><span data-stu-id="a97df-124">Go to the navigation pane and select **Billing** \> **Products & Services**.</span></span> <span data-ttu-id="a97df-125">Znajdź subskrypcję pakietu Office 365 i wybierz ją, aby wyświetlić szczegóły.</span><span class="sxs-lookup"><span data-stu-id="a97df-125">Find your Office 365 subscription and select it to view the details.</span></span> 

    ![Zrzut ekranu pokazuje, jak znaleźć i wybrać subskrypcję w centrum administracyjnym.](media/FindYourSubscription.png)

3. <span data-ttu-id="a97df-127">Na następnej stronie wybierz pozycję **Uaktualnij**.</span><span class="sxs-lookup"><span data-stu-id="a97df-127">On the next page, select **Upgrade**.</span></span> 

      ![Zrzut ekranu pokazuje, gdzie wybrać uaktualnienie w centrum administracyjnym.](media/SelectUpgrade.png)

  > [!NOTE]
  > <span data-ttu-id="a97df-129">Jeśli zostanie wyświetlony komunikat "Uaktualnianie subskrypcji nie jest obsługiwana w przypadku licencjonowania opartego na grupach w usłudze Azure Active Directory", można bezpiecznie zignorować to, chyba że masz bardzo dużą organizację.</span><span class="sxs-lookup"><span data-stu-id="a97df-129">If you see a message that says "Upgrading your subscription is not supported with group-based licensing in Azure Active Directory", you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="a97df-130">Organizacje, które wybrały tę opcję, będą pamiętać, że korzystają z licencjonowania opartego na grupach.</span><span class="sxs-lookup"><span data-stu-id="a97df-130">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="a97df-131">Następnie można wyświetlić listę planów pakietu Office, które można uaktualnić do.</span><span class="sxs-lookup"><span data-stu-id="a97df-131">Next, you can view a list of Office plans that you can upgrade to.</span></span> <span data-ttu-id="a97df-132">W takim przypadku Znajdź Microsoft 365 Business Plan.</span><span class="sxs-lookup"><span data-stu-id="a97df-132">In this case, find the Microsoft 365 Business plan.</span></span> <span data-ttu-id="a97df-133">Można przewijać w dół, jeśli chcesz zobaczyć wszystkie aplikacje pakietu Office i usług, które są dołączone do tego planu.</span><span class="sxs-lookup"><span data-stu-id="a97df-133">You can scroll down if you want to see all the Office apps and services that are included with this plan.</span></span> <span data-ttu-id="a97df-134">W obszarze **microsoft 365 Business**wybierz pozycję **Uaktualnij** , aby dodać firmę Microsoft 365 Business do koszyka.</span><span class="sxs-lookup"><span data-stu-id="a97df-134">Under **Microsoft 365 Business**, select **Upgrade** to add Microsoft 365 Business to your cart.</span></span>
5. <span data-ttu-id="a97df-135">W koszyku:</span><span class="sxs-lookup"><span data-stu-id="a97df-135">In the cart:</span></span>
    1. <span data-ttu-id="a97df-136">Będziemy automatycznie zawierać licencje dla wszystkich Twoich aktualnych użytkowników do koszyka.</span><span class="sxs-lookup"><span data-stu-id="a97df-136">We'll automatically include licenses for all your current users to the cart.</span></span> <span data-ttu-id="a97df-137">Jeśli potrzebujesz więcej lub mniej licencji, musisz [kupić i przypisać te licencje osobno](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="a97df-137">If you need more, or less licenses, you'll need to [buy and assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span></span>  
    2. <span data-ttu-id="a97df-138">Możesz dostosować sposób płatności — miesięczny lub roczny.</span><span class="sxs-lookup"><span data-stu-id="a97df-138">You can adjust how you'd like to pay - monthly or yearly.</span></span> <span data-ttu-id="a97df-139">Wybierz menu rozwijane, aby dokonać wyboru.</span><span class="sxs-lookup"><span data-stu-id="a97df-139">Select the drop-down menu to make your choice.</span></span>
6. <span data-ttu-id="a97df-140">Wybierz pozycję **Przejdź do kasy** , gdzie zobaczysz podsumowanie zakupu, w tym metodę płatności dla tego konta.</span><span class="sxs-lookup"><span data-stu-id="a97df-140">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="a97df-141">Możesz również dodać kod promocyjny tutaj, jeśli masz jeden.</span><span class="sxs-lookup"><span data-stu-id="a97df-141">You can also add a promo code here if you have one.</span></span>
7. <span data-ttu-id="a97df-142">Wybierz opcję **złóż zamówienie** , aby dokończyć zakup.</span><span class="sxs-lookup"><span data-stu-id="a97df-142">Select **Place order** to complete your purchase.</span></span>
<span data-ttu-id="a97df-143">Trwa kilka minut, aby skonfigurować nowe plany usług firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a97df-143">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="a97df-144">Aby sprawdzić postęp, wybierz **Sprawdź stan uaktualnienia**.</span><span class="sxs-lookup"><span data-stu-id="a97df-144">To check on progress, select **Check upgrade status**.</span></span> 
1. <span data-ttu-id="a97df-145">Gdy plan będzie gotowy, może być konieczne ukończenie dodatkowych czynności konfiguracyjnych w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="a97df-145">Once your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="a97df-146">W okienku nawigacji wybierz pozycję **Strona główna** , aby ukończyć dodatkowe kroki konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="a97df-146">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="a97df-147">Otrzymasz proporcjonowaną refundację dla licencji Ofifce 365, których już nie potrzebujesz.</span><span class="sxs-lookup"><span data-stu-id="a97df-147">You'll receive a prorated refund for the Ofifce 365 licenses that you no longer need.</span></span> <span data-ttu-id="a97df-148">Twoje konto bankowe lub karta kredytowa zostaną obciążone około dwa dni po skonfigurowaniu nowego planu.</span><span class="sxs-lookup"><span data-stu-id="a97df-148">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="a97df-149">Chroń urządzenia i pliki użytkownika</span><span class="sxs-lookup"><span data-stu-id="a97df-149">Protect user devices and files</span></span>

<span data-ttu-id="a97df-150">Teraz, gdy zostały przypisane licencje Microsoft 365 Business, wykonaj kroki, aby rozpocząć ochronę urządzeń i plików.</span><span class="sxs-lookup"><span data-stu-id="a97df-150">Now that Microsoft 365 Business licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="a97df-151">Będziesz korzystać z niektórych nowych opcji zawartych w panelu nawigacyjnym centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="a97df-151">You'll be using some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="a97df-152">W centrum administracyjnym, w okienku nawigacji, przejdź do **zasad** **urządzeń** \> .</span><span class="sxs-lookup"><span data-stu-id="a97df-152">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="a97df-153">Na stronie **zasady urządzeń** wybierz pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="a97df-153">On the **Device policies** page, select **Add**.</span></span>
    
3. <span data-ttu-id="a97df-154">W okienku **Dodaj zasady** Nadaj nazwę zasady (na przykład Chroń pliki robocze), a następnie wybierz **Typ zasad** z listy rozwijanej.</span><span class="sxs-lookup"><span data-stu-id="a97df-154">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down.</span></span> 
    
    <span data-ttu-id="a97df-155">Można skonfigurować zasady aplikacji do ochrony plików na urządzeniach z systemem Android i iPhone, a także systemu Windows 10 i można skonfigurować zasady konfiguracji urządzeń dla firmowych urządzeń z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a97df-155">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="a97df-156">Zobacz poniższe łącza, aby uzyskać szczegółowe informacje:</span><span class="sxs-lookup"><span data-stu-id="a97df-156">See the following links for details:</span></span>
    
  - [<span data-ttu-id="a97df-157">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="a97df-157">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="a97df-158">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="a97df-158">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="a97df-159">Ustawianie ustawień ochrony urządzenia dla komputerów z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="a97df-159">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
    
  
4. <span data-ttu-id="a97df-160">Po skonfigurowaniu zasad użytkownik i Twoi pracownicy mogą skonfigurować urządzenia:</span><span class="sxs-lookup"><span data-stu-id="a97df-160">After you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="a97df-161">Jeśli urządzenia z systemem Windows nie są już używane do aktualizacji programu Windows Pro Creator, musisz [uaktualnić je do aktualizacji systemu Windows Pro Creators](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="a97df-161">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
    
  - <span data-ttu-id="a97df-162">Zobacz [Konfigurowanie urządzeń z systemem Windows dla użytkowników Microsoft 365 Business](set-up-windows-devices.md) dla kroków dla urządzeń z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="a97df-162">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="a97df-163">Zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business](set-up-mobile-devices.md) dla kroków dla telefonów z systemem Android i iphone'ów.</span><span class="sxs-lookup"><span data-stu-id="a97df-163">See [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 



