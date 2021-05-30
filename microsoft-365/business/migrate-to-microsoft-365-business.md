---
title: Uaktualnianie do Microsoft 365 Business Premium z Microsoft 365 Business Standard
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Dowiedz się, jak Microsoft 365 Business Standard i Microsoft 365 Business Premium, oraz jak można uaktualnić system do Microsoft 365 Business Premium.
ms.openlocfilehash: 0968b877820590987f6f3ceca3efbd106b62cbd1
ms.sourcegitcommit: a05f61a291eb4595fa9313757a3815b7f217681d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/29/2021
ms.locfileid: "52705495"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a><span data-ttu-id="76590-103">Uaktualnianie do Microsoft 365 Business Premium z Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="76590-103">Upgrade to Microsoft 365 Business Premium from Microsoft 365 Business Standard</span></span>

<span data-ttu-id="76590-104">Jeśli masz [subskrypcję usługi Microsoft 365](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)dla firm, na przykład Microsoft 365 Business Standard, możesz łatwo uaktualnić do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="76590-104">If you have a [Microsoft 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Microsoft 365 Business Standard, you can easily upgrade to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="76590-105">Uaktualnij Microsoft 365 Business Premium, jeśli chcesz dodać:</span><span class="sxs-lookup"><span data-stu-id="76590-105">Upgrade to Microsoft 365 Business Premium if you want to add:</span></span>

- <span data-ttu-id="76590-106">Windows 10 Pro (na komputery z systemem Windows 8 lub nowszym)</span><span class="sxs-lookup"><span data-stu-id="76590-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>

- <span data-ttu-id="76590-107">Proste kontrolki do zarządzania danymi biznesowymi na urządzeniach</span><span class="sxs-lookup"><span data-stu-id="76590-107">Simple controls that manage business data on devices</span></span>

- <span data-ttu-id="76590-108">Zaawansowane funkcje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="76590-108">Advanced security capabilities.</span></span>
<span data-ttu-id="76590-109">Dowiedz się więcej o Microsoft 365 Business Premium na stronie [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="76590-109">Find out more about Microsoft 365 Business Premium at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a><span data-ttu-id="76590-110">Jaka jest różnica między Microsoft 365 Business Standard a Microsoft 365 Business Premium?</span><span class="sxs-lookup"><span data-stu-id="76590-110">What's the difference between Microsoft 365 Business Standard and Microsoft 365 Business Premium?</span></span>

<span data-ttu-id="76590-111">Dodaliśmy porównanie tych dwóch planów obok Microsoft 365 Business Premium opis [usługi](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="76590-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Premium Service Description](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-begin"></a><span data-ttu-id="76590-112">Przed rozpoczęciem</span><span class="sxs-lookup"><span data-stu-id="76590-112">Before you begin</span></span>

- <span data-ttu-id="76590-113">**Kiedy należy wybrać opcję uaktualnienia?**</span><span class="sxs-lookup"><span data-stu-id="76590-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="76590-114">Uaktualnienie to właściwa możliwość, jeśli chcesz **uaktualnić** wszystkich użytkowników przypisanych do jednego planu.</span><span class="sxs-lookup"><span data-stu-id="76590-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="76590-115">Gdy wybierzesz uaktualnienie, wszyscy użytkownicy planu są równocześnie przełączani do innego planu.</span><span class="sxs-lookup"><span data-stu-id="76590-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="76590-116">Jeśli nie chcesz uaktualnić wszystkich osób przypisanych do jednego planu, kup licencje nowego planu (w [](../admin/manage/assign-licenses-to-users.md) tym przypadku Microsoft 365 Business Premium) i przypisz te licencje poszczególnym użytkownikom, których uaktualnienie chcesz uaktualnić.</span><span class="sxs-lookup"><span data-stu-id="76590-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business Premium), and [assign those licenses individually](../admin/manage/assign-licenses-to-users.md) to each user that you want to upgrade.</span></span>

- <span data-ttu-id="76590-117">**Niektóre dodatki mogą uniemożliwiać uaktualnienie** Jeśli podczas próby rozpoczęcia uaktualnienia masz dodatek uniemożliwiający kontynuowanie pracy, możesz najpierw usunąć dodatek, a następnie dodać go ponownie później, jeśli nadal będzie potrzebny.</span><span class="sxs-lookup"><span data-stu-id="76590-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span>

- <span data-ttu-id="76590-118">**Jeśli plan został opłacony z góry** Nie ma prostej ścieżki uaktualnienia planów przedpłaconych.</span><span class="sxs-lookup"><span data-stu-id="76590-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="76590-119">Dowiesz się, czy masz plan przedpłacony, ponieważ został on ustawiony przy użyciu identyfikatora produktu, który mógł zostać kupiony w sklepie.</span><span class="sxs-lookup"><span data-stu-id="76590-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="76590-120">Skontaktuj się z partnerem, przejdź do Microsoft Store lub poczekaj na wygaśnięcie planu przedpłaconego, aby przełączyć się do nowego planu.</span><span class="sxs-lookup"><span data-stu-id="76590-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business-premium"></a><span data-ttu-id="76590-121">Uaktualnij do Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="76590-121">Upgrade to Microsoft 365 Business Premium</span></span>

1. <span data-ttu-id="76590-122">Zaloguj się do centrum administracyjnego w stronie <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="76590-122">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="76590-123">Przejdź do okienka nawigacji i wybierz pozycję **Rozliczenia** \> **Twoje produkty**.</span><span class="sxs-lookup"><span data-stu-id="76590-123">Go to the navigation pane and select **Billing** \> **Your products**.</span></span> <span data-ttu-id="76590-124">Znajdź bieżącą subskrypcję i wybierz ją, aby wyświetlić szczegóły.</span><span class="sxs-lookup"><span data-stu-id="76590-124">Find your current subscription and select it to view the details.</span></span>

3. <span data-ttu-id="76590-125">Na następnej stronie wybierz pozycję **Uaktualnij**.</span><span class="sxs-lookup"><span data-stu-id="76590-125">On the next page, select **Upgrade**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="76590-126">Jeśli zobaczysz komunikat Uaktualnianie subskrypcji nie jest obsługiwane w przypadku licencjonowania grupowego w programie **Azure Active Directory,** możesz zignorować ten problem, jeśli nie masz bardzo dużej organizacji.</span><span class="sxs-lookup"><span data-stu-id="76590-126">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="76590-127">Organizacje, które wybrały tę opcję, będą wiedzieć, że korzysta z licencjonowania grupowego.</span><span class="sxs-lookup"><span data-stu-id="76590-127">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="76590-128">Następnie możesz wyświetlić listę planów, do których możesz uaktualnić plan.</span><span class="sxs-lookup"><span data-stu-id="76590-128">Next, you can view a list of plans that you can upgrade to.</span></span> <span data-ttu-id="76590-129">W takim przypadku znajdź Microsoft 365 Business Premium projektu.</span><span class="sxs-lookup"><span data-stu-id="76590-129">In this case, find the Microsoft 365 Business Premium plan.</span></span> <span data-ttu-id="76590-130">Jeśli chcesz wyświetlić wszystkie aplikacje i usługi zawarte w tym planie, możesz przewinąć w dół.</span><span class="sxs-lookup"><span data-stu-id="76590-130">You can scroll down if you want to see all the apps and services that are included with this plan.</span></span> <span data-ttu-id="76590-131">W **Microsoft 365 Business Premium** wybierz pozycję **Uaktualnij,** aby dodać Microsoft 365 Business Premium do koszyka.</span><span class="sxs-lookup"><span data-stu-id="76590-131">Under **Microsoft 365 Business Premium**, select **Upgrade** to add Microsoft 365 Business Premium to your cart.</span></span>

5. <span data-ttu-id="76590-132">W koszyku:</span><span class="sxs-lookup"><span data-stu-id="76590-132">In the cart:</span></span>

    1. <span data-ttu-id="76590-133">Automatycznie dołączymy licencje dla wszystkich Twoich bieżących użytkowników.</span><span class="sxs-lookup"><span data-stu-id="76590-133">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="76590-134">Jeśli potrzebujesz większej lub mniejszej liczby licencji, musisz kupić i [przypisać te licencje pojedynczo.](../admin/manage/assign-licenses-to-users.md)</span><span class="sxs-lookup"><span data-stu-id="76590-134">If you need more or fewer licenses, you need to [buy and assign those licenses individually](../admin/manage/assign-licenses-to-users.md).</span></span>  
    2. <span data-ttu-id="76590-135">Możesz dostosować sposób płacenia: miesięcznie lub rocznie.</span><span class="sxs-lookup"><span data-stu-id="76590-135">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="76590-136">Wybierz menu rozwijane, aby dokonać wyboru.</span><span class="sxs-lookup"><span data-stu-id="76590-136">Select the drop-down menu to make your choice.</span></span>

6. <span data-ttu-id="76590-137">Wybierz **pozycję Przejdź do finalizacji** zakupu, gdzie zobaczysz podsumowanie zakupu wraz z metodą płatności dla tego konta.</span><span class="sxs-lookup"><span data-stu-id="76590-137">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="76590-138">W tym miejscu możesz również dodać kod promocyjny, jeśli go masz.</span><span class="sxs-lookup"><span data-stu-id="76590-138">You can also add a promo code here if you have one.</span></span>

7. <span data-ttu-id="76590-139">Wybierz **pozycję Zmów** zamówienie, aby dokończyć zakup.</span><span class="sxs-lookup"><span data-stu-id="76590-139">Select **Place order** to complete your purchase.</span></span>\
<span data-ttu-id="76590-140">Skonfigurowanie nowych planów usług zajmuje firmie Microsoft kilka minut.</span><span class="sxs-lookup"><span data-stu-id="76590-140">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="76590-141">Aby sprawdzić postęp uaktualniania, wybierz **pozycję Sprawdź stan uaktualnienia**.</span><span class="sxs-lookup"><span data-stu-id="76590-141">To check on progress, select **Check upgrade status**.</span></span>

8. <span data-ttu-id="76590-142">Gdy plan będzie gotowy, może być konieczne wykonania pewnych dodatkowych kroków konfiguracji w centrum administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="76590-142">When your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="76590-143">W okienku nawigacji wybierz pozycję **Strona główna,** aby wykonać wszystkie dodatkowe kroki konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="76590-143">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="76590-144">Otrzymasz proporcjonalny zwrot za licencje Microsoft 365, których już nie potrzebujesz.</span><span class="sxs-lookup"><span data-stu-id="76590-144">You'll receive a prorated refund for the Microsoft 365 licenses that you no longer need.</span></span> <span data-ttu-id="76590-145">Opłata za twoje konto bankowe lub kartę kredytową zostanie pobrana po upływie około dwóch dni od skonfigurowania nowego planu.</span><span class="sxs-lookup"><span data-stu-id="76590-145">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="76590-146">Ochrona urządzeń i plików użytkowników</span><span class="sxs-lookup"><span data-stu-id="76590-146">Protect user devices and files</span></span>

<span data-ttu-id="76590-147">Po przypisaniu Microsoft 365 Business Premium wykonaj czynności, aby rozpocząć ochronę urządzeń i plików.</span><span class="sxs-lookup"><span data-stu-id="76590-147">Now that Microsoft 365 Business Premium licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="76590-148">Będziesz używać niektórych nowych opcji dostępnych w okienku nawigacji centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="76590-148">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="76590-149">W centrum administracyjnym w okienku nawigacji przejdź do **pozycji Zasady dotyczące** \> **urządzeń.**</span><span class="sxs-lookup"><span data-stu-id="76590-149">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="76590-150">Na stronie **Zasady dotyczące urządzeń** wybierz pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="76590-150">On the **Device policies** page, select **Add**.</span></span>

3. <span data-ttu-id="76590-151">W **okienku Dodaj** zasady nadaj zasadom nazwę (na przykład Chroń pliki służbowe), **a** następnie wybierz typ zasad z listy rozwijanej.</span><span class="sxs-lookup"><span data-stu-id="76590-151">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span>

    <span data-ttu-id="76590-152">Możesz skonfigurować zasady aplikacji do ochrony plików na urządzeniach z systemami Android i iPhone, a także Windows 10, a także dla firmowych urządzeń Windows 10 urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="76590-152">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="76590-153">Aby uzyskać szczegółowe informacje, zobacz następujące linki:</span><span class="sxs-lookup"><span data-stu-id="76590-153">See the following links for details:</span></span>

    - [<span data-ttu-id="76590-154">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Android lub iOS</span><span class="sxs-lookup"><span data-stu-id="76590-154">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

    - [<span data-ttu-id="76590-155">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="76590-155">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

    - [<span data-ttu-id="76590-156">Konfigurowanie ustawień ochrony urządzeń dla Windows 10 PC</span><span class="sxs-lookup"><span data-stu-id="76590-156">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)

4. <span data-ttu-id="76590-157">Po skonfigurowaniu zasad Ty i Twoi pracownicy możecie skonfigurować urządzenia:</span><span class="sxs-lookup"><span data-stu-id="76590-157">After you set up policies, you and your employees can set up devices:</span></span>

    - <span data-ttu-id="76590-158">Jeśli Twoje Windows nie potrzebują jeszcze aktualizacji Kreatora Windows Pro, musisz uaktualnić je do Windows Pro [dla twórców.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="76590-158">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

    - <span data-ttu-id="76590-159">Zobacz [Konfigurowanie Windows dla Microsoft 365 Business Premium,](set-up-windows-devices.md) aby uzyskać instrukcje dotyczące Windows urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="76590-159">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span>

    - <span data-ttu-id="76590-160">Zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników Microsoft 365 Business Premium,](set-up-mobile-devices.md) aby uzyskać instrukcje dotyczące telefonów iPhone i telefonów z systemem Android.</span><span class="sxs-lookup"><span data-stu-id="76590-160">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span>