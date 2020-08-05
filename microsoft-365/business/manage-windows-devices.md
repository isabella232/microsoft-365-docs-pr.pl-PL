---
title: Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączonych do domeny przez usługę Microsoft 365 dla firm
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
description: Dowiedz się, jak w kilku krokach umożliwić programowi Microsoft 365 ochronę lokalnych urządzeń z systemem Windows 10 połączonych z usługą Active Directory.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560848"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="c8626-103">Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączanym do domeny przez usługę Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c8626-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="c8626-104">Jeśli twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, można skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="c8626-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="c8626-105">Aby skonfigurować tę ochronę, można zaimplementować **urządzenia przyłączone do usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="c8626-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="c8626-106">Te urządzenia są przyłączane zarówno do lokalnej usługi Active Directory, jak i usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8626-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="c8626-107">W tym klipie wideo opisano kroki dotyczące konfigurowania tego dla najbardziej typowych scenariuszy, który jest również szczegółowo opisany w kolejnych krokach.</span><span class="sxs-lookup"><span data-stu-id="c8626-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="c8626-108">Zanim zaczniesz, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="c8626-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="c8626-109">Synchronizowanie użytkowników z usługą Azure AD z usługą Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c8626-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="c8626-110">Pełna synchronizacja jednostki organizacyjnej usługi Azure AD Connect(OU).</span><span class="sxs-lookup"><span data-stu-id="c8626-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="c8626-111">Upewnij się, że wszyscy synchronizowani użytkownicy domeny mają licencje na usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c8626-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="c8626-112">Aby uzyskać [instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8626-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="c8626-113">1. Sprawdź urząd MDM w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="c8626-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="c8626-114">Przejdź do [Menedżera punktów końcowych](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) i na stronie Microsoft Intune wybierz pozycję **Rejestracja urządzenia**, a następnie na stronie **Przegląd** upewnij się, że **urzędem MDM** jest **usługa Intune**.</span><span class="sxs-lookup"><span data-stu-id="c8626-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="c8626-115">Jeśli **urząd MDM** to **Brak,** kliknij **urząd MDM,** aby ustawić go na **Intune**.</span><span class="sxs-lookup"><span data-stu-id="c8626-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="c8626-116">Jeśli **urzędem MDM** jest **usługa Microsoft Office 365,** przejdź do urządzenia **Devices**  >  **Rejestruj urządzenia** i użyj okna dialogowego **Dodaj urząd MDM** po prawej stronie, aby dodać uprawnienia **MDM usługi Intune** (okno dialogowe **Dodaj urząd MDM** jest dostępne tylko wtedy, gdy **urząd MDM** jest ustawiony na usługę Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="c8626-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="c8626-117">2. Sprawdź, czy usługa Azure AD jest włączona do łączenia komputerów</span><span class="sxs-lookup"><span data-stu-id="c8626-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="c8626-118">Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> i wybierz pozycję Usługa Azure Active **Directory** (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory nie jest widoczna) na liście **Centra administracyjne.**</span><span class="sxs-lookup"><span data-stu-id="c8626-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="c8626-119">W **centrum administracyjnym usługi Azure Active Directory**przejdź do **usługi Azure Active Directory** , wybierz pozycję **Urządzenia,** a następnie **ustawienia urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="c8626-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="c8626-120">Sprawdź, czy**użytkownicy mogą dołączać urządzenia do usługi Azure AD** jest włączona</span><span class="sxs-lookup"><span data-stu-id="c8626-120">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="c8626-121">Aby włączyć wszystkich użytkowników, ustaw opcję **Wszystkie**.</span><span class="sxs-lookup"><span data-stu-id="c8626-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="c8626-122">Aby włączyć określonych użytkowników, ustaw opcję **Wybrane,** aby włączyć określoną grupę użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c8626-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="c8626-123">Dodaj żądanych użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="c8626-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="c8626-124">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkownika mdm dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="c8626-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="c8626-125">3. Sprawdź, czy usługa Azure AD jest włączona dla usługi MDM</span><span class="sxs-lookup"><span data-stu-id="c8626-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="c8626-126">Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> i wybierz pozycję **Endpoint Managemen**t (wybierz pozycję **Pokaż wszystko,** jeśli **Menedżer punktów końcowych** nie jest widoczny)</span><span class="sxs-lookup"><span data-stu-id="c8626-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="c8626-127">W **centrum administracyjnym programu Microsoft Endpoint Manager**przejdź do **pozycji Urządzenia**Rejestracji systemu  >  **Windows**  >  **Windows Enrollment**  >  **Rejestracja automatyczna rejestracja**systemu .</span><span class="sxs-lookup"><span data-stu-id="c8626-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="c8626-128">Sprawdź, czy zakres użytkownika MDM jest włączony.</span><span class="sxs-lookup"><span data-stu-id="c8626-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="c8626-129">Aby zarejestrować wszystkie komputery, ustaw opcję **Wszystkie,** aby automatycznie rejestrować wszystkie komputery użytkowników, które są przyłączone do usługi Azure AD i nowe komputery, gdy użytkownicy dodają konto służbowe do systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="c8626-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="c8626-130">Ustaw na **Niektóre,** aby zarejestrować komputery określonej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c8626-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="c8626-131">Dodaj żądanych użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="c8626-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="c8626-132">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkownika mdm dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="c8626-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="c8626-133">4. Tworzenie wymaganych zasobów</span><span class="sxs-lookup"><span data-stu-id="c8626-133">4. Create the required resources</span></span> 

<span data-ttu-id="c8626-134">Wykonywanie zadań wymaganych do [konfigurowania hybrydowego sprzężenia usługi Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki zastosowaniu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) znalezionego w module [Programu SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c8626-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="c8626-135">Po wywołaniu tego polecenia cmdlet utworzy i skonfiguruje wymagany punkt połączenia usługi i zasady grupy.</span><span class="sxs-lookup"><span data-stu-id="c8626-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="c8626-136">Ten moduł można zainstalować, wywołując następujące z wystąpienia programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c8626-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="c8626-137">Zaleca się zainstalowanie tego modułu w systemie Windows Server z systemem Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c8626-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="c8626-138">Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="c8626-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="c8626-139">Podczas wykonywania tego zadania potrzebne będą poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c8626-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="c8626-140">Gdy chcesz utworzyć zasoby, należy wywołać następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="c8626-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="c8626-141">Pierwsze polecenie nawiąza połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c8626-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="c8626-142">5. Połącz zasady grupy</span><span class="sxs-lookup"><span data-stu-id="c8626-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="c8626-143">W konsoli zarządzania zasadami grupy (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, a następnie wybierz polecenie *Połącz istniejący obiekt zasad grupy...* z menu kontekstowego.</span><span class="sxs-lookup"><span data-stu-id="c8626-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="c8626-144">Wybierz zasady utworzone w powyższym kroku, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="c8626-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="c8626-145">Pobierz najnowsze szablony administracyjne</span><span class="sxs-lookup"><span data-stu-id="c8626-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="c8626-146">Jeśli zasady nie są widoczne **Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego serwera ADMX dla systemu Windows 10, wersja 1803, wersja 1809 lub wersja 1903.</span><span class="sxs-lookup"><span data-stu-id="c8626-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="c8626-147">Aby rozwiązać ten problem, wykonaj następujące kroki (Uwaga: najnowszy plik MDM.admx jest zgodny wstecz:</span><span class="sxs-lookup"><span data-stu-id="c8626-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="c8626-148">Pobierz: [Szablony administracyjne (admx) dla systemu Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="c8626-148">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="c8626-149">Zainstaluj pakiet na podstawowym kontrolerze domeny (PDC).</span><span class="sxs-lookup"><span data-stu-id="c8626-149">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="c8626-150">Przejdź, w zależności od wersji do folderu: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="c8626-150">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="c8626-151">Zmień nazwę folderu **Definicje zasad** na powyższej ścieżce na **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="c8626-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="c8626-152">Kopiuj folder **PolicyDefinitions** do **folderu C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="c8626-152">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="c8626-153">Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość policyDefinitions.</span><span class="sxs-lookup"><span data-stu-id="c8626-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="c8626-154">Uruchom ponownie podstawowy kontroler domeny, aby zasady były dostępne.</span><span class="sxs-lookup"><span data-stu-id="c8626-154">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="c8626-155">Ta procedura będzie działać dla każdej przyszłej wersji, jak również.</span><span class="sxs-lookup"><span data-stu-id="c8626-155">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="c8626-156">W tym momencie powinieneś być w stanie zobaczyć zasady **Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD** dostępne.</span><span class="sxs-lookup"><span data-stu-id="c8626-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
