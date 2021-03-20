---
title: Włączanie zarządzania przez platformę Microsoft 365 dla firm dla urządzeń przyłącznych do domeny systemu Windows 10
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
description: Dowiedz się, jak w kilku krokach włączyć ochronę lokalnych urządzeń z systemem Windows 10 przyłączanych do usługi Active Directory na platformie Microsoft 365.
ms.openlocfilehash: 82d4ac3f1d6aba9489f9ea153de3a3d2083b47ec
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913199"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="65ded-103">Włączanie zarządzania przez usługę Microsoft 365 Business Premium dla urządzeń przyłączanych do domeny systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="65ded-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="65ded-104">Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="65ded-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="65ded-105">Aby skonfigurować tę ochronę, możesz zaimplementować urządzenia sprzężenia **hybrydowego usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="65ded-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="65ded-106">Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65ded-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="65ded-107">W tym klipie wideo opisano kroki, które należy wykonać w celu skonfigurowania tego najbardziej typowego scenariusza, a także szczegółowo opisano w poniższych krokach.</span><span class="sxs-lookup"><span data-stu-id="65ded-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="65ded-108">Przed rozpoczęciem upewnij się, że wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="65ded-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="65ded-109">Zsynchronizowanie użytkowników z usługą Azure AD za pomocą programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="65ded-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="65ded-110">Ukończ synchronizację jednostek organizacyjnych usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="65ded-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="65ded-111">Upewnij się, że wszyscy użytkownicy domeny, których synchronizujesz, mają licencje na usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="65ded-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="65ded-112">Aby [uzyskać odpowiednie instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="65ded-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="65ded-113">1. Weryfikowanie urzędu zarządzania usługą MDM w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="65ded-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="65ded-114">Przejdź do Menedżera [punktów końcowych](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) i na stronie Microsoft  Intune wybierz pozycję Rejestracja urządzeń **,** a następnie na stronie Omówienie upewnij się, że uprawnienia **MDM** to **Intune.**</span><span class="sxs-lookup"><span data-stu-id="65ded-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="65ded-115">Jeśli **dla uprawnienia MDM jest** ustawiona wartość **Brak,** kliknij uprawnienia **MDM,** aby ustawić dla niego pozycję **Intune.**</span><span class="sxs-lookup"><span data-stu-id="65ded-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="65ded-116">Jeśli uprawnienia **MDM** to usługa Microsoft Office  **365,** przejdź do strony Urządzenia Zarejestruj urządzenia i użyj okna dialogowego Dodawanie urzędu zarządzania mdM po prawej stronie, aby dodać uprawnienia usługi Intune MDM (okno dialogowe Dodawanie urzędu zarządzania mdm jest dostępne tylko wtedy, gdy dla uprawnienia MDM ustawiono usługę Microsoft Office  >   365).    </span><span class="sxs-lookup"><span data-stu-id="65ded-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="65ded-117">2. Sprawdź, czy włączono usługę Azure AD, aby dołączać do komputerów</span><span class="sxs-lookup"><span data-stu-id="65ded-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="65ded-118">Przejdź do centrum administracyjnego w miejscu i wybierz pozycję Azure Active Directory (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory jest niewidoczna) na liście <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Centra** administracyjne. </span><span class="sxs-lookup"><span data-stu-id="65ded-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="65ded-119">W centrum **administracyjnym usługi Azure Active Directory przejdź** do pozycji Azure Active **Directory** , wybierz **pozycję Urządzenia,** a następnie **pozycję Ustawienia urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="65ded-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="65ded-120">Sprawdzanie,**czy użytkownicy mogą dołączać do urządzeń w usłudze Azure AD**</span><span class="sxs-lookup"><span data-stu-id="65ded-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="65ded-121">Aby włączyć wszystkich użytkowników, ustaw wartość **Wszystkie.**</span><span class="sxs-lookup"><span data-stu-id="65ded-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="65ded-122">Aby włączyć określonych użytkowników, ustaw wartość **Wybrani,** aby włączyć konkretną grupę użytkowników.</span><span class="sxs-lookup"><span data-stu-id="65ded-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="65ded-123">Dodaj do grupy zabezpieczeń żądanych użytkowników domeny zsynchronizowanych w [usłudze](../admin/create-groups/create-groups.md)Azure AD.</span><span class="sxs-lookup"><span data-stu-id="65ded-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="65ded-124">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="65ded-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="65ded-125">3. Sprawdzanie, czy usługa Azure AD jest włączona dla usługi MDM</span><span class="sxs-lookup"><span data-stu-id="65ded-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="65ded-126">Przejdź do centrum administracyjnego w i <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> wybierz pozycję Zarządzanie  **punktami** końcowymi t (zaznacz pole wyboru Pokaż **wszystko,** jeśli menedżer punktów końcowych nie jest widoczny)</span><span class="sxs-lookup"><span data-stu-id="65ded-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="65ded-127">W centrum **administracyjnym programu Microsoft Endpoint Manager** przejdź do pozycji Urządzenia **Rejestracja** automatyczna systemu Windows Rejestracja  >    >    >  **automatyczna systemu** Windows.</span><span class="sxs-lookup"><span data-stu-id="65ded-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="65ded-128">Sprawdź, czy jest włączony zakres użytkowników usługi MDM.</span><span class="sxs-lookup"><span data-stu-id="65ded-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="65ded-129">Aby zarejestrować wszystkie komputery, ustaw wartość Wszystkie w celu automatycznego zarejestrowania wszystkich komputerów użytkowników przyłącznych do usługi Azure AD i nowych komputerów, gdy użytkownicy dodają konto służbowe do systemu Windows. </span><span class="sxs-lookup"><span data-stu-id="65ded-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="65ded-130">Ustaw wartość **Some** (Niektóre), aby zarejestrować komputery określonej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="65ded-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="65ded-131">Dodaj do grupy zabezpieczeń żądanych użytkowników domeny zsynchronizowanych w [usłudze](../admin/create-groups/create-groups.md)Azure AD.</span><span class="sxs-lookup"><span data-stu-id="65ded-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="65ded-132">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="65ded-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="65ded-133">4. Tworzenie wymaganych zasobów</span><span class="sxs-lookup"><span data-stu-id="65ded-133">4. Create the required resources</span></span> 

<span data-ttu-id="65ded-134">Wykonywanie wymaganych zadań w celu skonfigurowania hybrydowego sprzężenia usługi [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki użyciu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) w module [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="65ded-134">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="65ded-135">Wywoływanie tego polecenia cmdlet spowoduje utworzenie i skonfigurowanie wymaganego punktu połączenia usługi oraz zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="65ded-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="65ded-136">Ten moduł można zainstalować, odwołując się do następującego wystąpienia programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="65ded-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="65ded-137">Zalecane jest zainstalowanie tego modułu na serwerze Windows Server z uruchomionym programem Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="65ded-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="65ded-138">Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="65ded-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="65ded-139">Podczas wykonywania tego zadania będziesz potrzebować poświadczeń administratora globalnego usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="65ded-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="65ded-140">Gdy wszystko będzie gotowe do utworzenia zasobów, wywołaj następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="65ded-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="65ded-141">Pierwsze polecenie nawiązuje połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="65ded-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="65ded-142">5. Połącz zasady grupy</span><span class="sxs-lookup"><span data-stu-id="65ded-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="65ded-143">W konsoli zasady grupy zarządzania (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, i wybierz z menu kontekstowego pozycję Połącz istniejący element *zasad* grupy.</span><span class="sxs-lookup"><span data-stu-id="65ded-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="65ded-144">Wybierz zasady utworzone w powyższym kroku, a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="65ded-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="65ded-145">Pobierz najnowsze szablony administracyjne</span><span class="sxs-lookup"><span data-stu-id="65ded-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="65ded-146">Jeśli nie widzisz zasad Włącz automatyczną rejestrację mdM przy użyciu domyślnych poświadczeń usługi **Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego narzędzia ADMX dla systemu Windows 10 w wersji 1803 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="65ded-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="65ded-147">Aby rozwiązać ten problem, wykonaj następujące czynności (Uwaga: najnowsza wersja pliku MDM.admx jest zgodna z poprzednimi wersjami):</span><span class="sxs-lookup"><span data-stu-id="65ded-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="65ded-148">Pobierz: Szablony administracyjne (admx) dla systemu Windows 10 z października [2020 r. Aktualizacja (20H2)](https://www.microsoft.com/download/102157).</span><span class="sxs-lookup"><span data-stu-id="65ded-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="65ded-149">Zainstaluj pakiet na Kontroler domeny.</span><span class="sxs-lookup"><span data-stu-id="65ded-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="65ded-150">Przejdź do folderu w zależności od wersji szablonów administracyjnych: **C:\Program Files (x86)\Microsoft zasady grupy\Windows 10 October 2020 Update (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="65ded-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="65ded-151">Zmień nazwę **folderu Definicje** zasad na powyższej ścieżce do **folderu Definicje Zasad.**</span><span class="sxs-lookup"><span data-stu-id="65ded-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="65ded-152">Skopiuj folder **PolicyDefinitions** do udziału SYSVOL, domyślnie znajdujący się w folderze **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="65ded-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="65ded-153">Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość PolaOkreślenia Zasad.</span><span class="sxs-lookup"><span data-stu-id="65ded-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="65ded-154">Jeśli masz kilka kontrolerów domeny, poczekaj, aż narzędzie SYSVOL zreplikuje te zasady, które będą dostępne.</span><span class="sxs-lookup"><span data-stu-id="65ded-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="65ded-155">Ta procedura będzie działać również w przypadku każdej przyszłej wersji szablonów administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="65ded-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="65ded-156">Na tym etapie powinny być dostępne zasady Włącz automatyczną rejestrację **w usłudze MDM przy użyciu domyślnych dostępnych poświadczeń usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="65ded-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>