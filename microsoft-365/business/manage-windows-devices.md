---
title: Włączanie zarządzania przez Windows 10 przyłączone do domeny Microsoft 365 dla firm
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Dowiedz się, jak Microsoft 365 chronić lokalne urządzenia Windows 10 przyłączone do usługi Active-Directory w kilku krokach.
ms.openlocfilehash: ec80159bdceffd8a13d09a297a2acc1b78c9b1b3
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52636091"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="084dc-103">Włączanie zarządzania przez Windows 10 przyłączone do domeny Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="084dc-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="084dc-104">Jeśli Twoja organizacja korzysta z lokalnej usługi Windows Server Active Directory, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych, które wymagają uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="084dc-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="084dc-105">Aby skonfigurować tę ochronę, możesz zaimplementować urządzenia sprzężenia **hybrydowego usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="084dc-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="084dc-106">Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i Twoją Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="084dc-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

## <a name="watch-configure-hybrid-azure-active-directory-join"></a><span data-ttu-id="084dc-107">Obejrzyj: Konfigurowanie dołączania do Azure Active Directory hybrydowego</span><span class="sxs-lookup"><span data-stu-id="084dc-107">Watch: Configure Hybrid Azure Active Directory join</span></span>

<span data-ttu-id="084dc-108">W tym klipie wideo opisano kroki, które należy wykonać w celu skonfigurowania tego najbardziej typowego scenariusza, a także szczegółowo opisano w poniższych krokach.</span><span class="sxs-lookup"><span data-stu-id="084dc-108">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a><span data-ttu-id="084dc-109">Przed rozpoczęciem</span><span class="sxs-lookup"><span data-stu-id="084dc-109">Before you begin</span></span>

- <span data-ttu-id="084dc-110">Zsynchronizowanie użytkowników z usługą Azure AD z usługą Azure AD Połączenie.</span><span class="sxs-lookup"><span data-stu-id="084dc-110">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="084dc-111">Ukończ synchronizację Połączenie organizacyjnej usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="084dc-111">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="084dc-112">Upewnij się, że wszyscy użytkownicy domeny, których synchronizujesz, mają licencje Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="084dc-112">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="084dc-113">Aby [uzyskać odpowiednie instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="084dc-113">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="084dc-114">1. Weryfikowanie urzędu zarządzania usługą MDM w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="084dc-114">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="084dc-115">Przejdź do [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) i na stronie Microsoft Intune rejestracja **urządzeń ,** a  następnie na stronie Omówienie upewnij się, że uprawnienia **mdM** to **Intune.**</span><span class="sxs-lookup"><span data-stu-id="084dc-115">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="084dc-116">Jeśli **dla uprawnienia MDM jest** ustawiona wartość **Brak,** kliknij uprawnienia **MDM,** aby ustawić dla niego pozycję **Intune.**</span><span class="sxs-lookup"><span data-stu-id="084dc-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="084dc-117">Jeśli uprawnienia **MDM** Microsoft Office 365, przejdź **do** strony Urządzenia Zarejestruj urządzenia i użyj okna dialogowego Dodawanie urzędu zarządzania urządzeniami przenośnymi po prawej stronie, aby dodać uprawnienia usługi   >   **Intune MDM** (okno dialogowe Dodawanie uprawnień **MDM** jest dostępne tylko wtedy, gdy dla uprawnienia **MDM** jest ustawiona wartość Microsoft Office 365). </span><span class="sxs-lookup"><span data-stu-id="084dc-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="084dc-118">2. Sprawdź, czy włączono usługę Azure AD, aby dołączać do komputerów</span><span class="sxs-lookup"><span data-stu-id="084dc-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="084dc-119">Przejdź do centrum administracyjnego w miejscu i wybierz pozycję Azure Active Directory (wybierz pozycję Pokaż wszystko, Azure Active Directory nie jest widoczna) na liście <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Centra** administracyjne. </span><span class="sxs-lookup"><span data-stu-id="084dc-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="084dc-120">W centrum **administracyjnym Azure Active Directory przejdź** do pozycji Azure Active Directory **,** wybierz **pozycję Urządzenia,** a następnie **pozycję Ustawienia urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="084dc-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="084dc-121">Sprawdzanie,**czy użytkownicy mogą dołączać do urządzeń w usłudze Azure AD**</span><span class="sxs-lookup"><span data-stu-id="084dc-121">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="084dc-122">Aby włączyć wszystkich użytkowników, ustaw wartość **Wszystkie.**</span><span class="sxs-lookup"><span data-stu-id="084dc-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="084dc-123">Aby włączyć określonych użytkowników, ustaw wartość **Wybrani,** aby włączyć konkretną grupę użytkowników.</span><span class="sxs-lookup"><span data-stu-id="084dc-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="084dc-124">Dodaj do grupy zabezpieczeń żądanych użytkowników domeny zsynchronizowanych w [usłudze](../admin/create-groups/create-groups.md)Azure AD.</span><span class="sxs-lookup"><span data-stu-id="084dc-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="084dc-125">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="084dc-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="084dc-126">3. Sprawdzanie, czy usługa Azure AD jest włączona dla usługi MDM</span><span class="sxs-lookup"><span data-stu-id="084dc-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="084dc-127">Przejdź do centrum administracyjnego w i wybierz pozycję Zarządzanie punktami końcowymi t (zaznacz pole wyboru Pokaż wszystko, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Manager** nie jest widoczne)  </span><span class="sxs-lookup"><span data-stu-id="084dc-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="084dc-128">W centrum **Microsoft Endpoint Manager przejdź** do pozycji Urządzenia  >  **Windows** Windows  >  **rejestracja**  >  **automatyczna.**</span><span class="sxs-lookup"><span data-stu-id="084dc-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="084dc-129">Sprawdź, czy jest włączony zakres użytkowników usługi MDM.</span><span class="sxs-lookup"><span data-stu-id="084dc-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="084dc-130">Aby zarejestrować wszystkie komputery, ustaw wartość Wszystkie w celu automatycznego zarejestrowania wszystkich komputerów użytkowników, które są połączone z usługą Azure AD, i nowych komputerów, gdy użytkownicy dodają konto służbowe do usługi Windows. </span><span class="sxs-lookup"><span data-stu-id="084dc-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="084dc-131">Ustaw wartość **Some** (Niektóre), aby zarejestrować komputery określonej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="084dc-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="084dc-132">Dodaj do grupy zabezpieczeń żądanych użytkowników domeny zsynchronizowanych w [usłudze](../admin/create-groups/create-groups.md)Azure AD.</span><span class="sxs-lookup"><span data-stu-id="084dc-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="084dc-133">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="084dc-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="084dc-134">4. Tworzenie wymaganych zasobów</span><span class="sxs-lookup"><span data-stu-id="084dc-134">4. Create the required resources</span></span> 

<span data-ttu-id="084dc-135">Wykonywanie wymaganych zadań w celu skonfigurowania hybrydowego sprzężenia usługi [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki użyciu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) w module [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="084dc-135">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="084dc-136">Wywoływanie tego polecenia cmdlet spowoduje utworzenie i skonfigurowanie wymaganego punktu połączenia usługi oraz zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="084dc-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="084dc-137">Ten moduł można zainstalować, odwołując się do następującego wystąpienia programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="084dc-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="084dc-138">Zalecane jest zainstalowanie tego modułu na serwerze usługi Windows z uruchomionym programem Azure AD Połączenie.</span><span class="sxs-lookup"><span data-stu-id="084dc-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="084dc-139">Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="084dc-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="084dc-140">Podczas wykonywania tego Microsoft 365 Business Premium będziesz potrzebować poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="084dc-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="084dc-141">Gdy wszystko będzie gotowe do utworzenia zasobów, wywołaj następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="084dc-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="084dc-142">Pierwsze polecenie nawiązuje połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ swoje Microsoft 365 Business Premium poświadczenia administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="084dc-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="084dc-143">5. Połącz zasady grupy</span><span class="sxs-lookup"><span data-stu-id="084dc-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="084dc-144">W konsoli zasady grupy zarządzania (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, i wybierz z menu kontekstowego pozycję Połącz istniejący element *zasad* grupy.</span><span class="sxs-lookup"><span data-stu-id="084dc-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="084dc-145">Wybierz zasady utworzone w powyższym kroku, a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="084dc-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="084dc-146">Pobierz najnowsze szablony administracyjne</span><span class="sxs-lookup"><span data-stu-id="084dc-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="084dc-147">Jeśli nie widzisz zasad Włącz automatyczną rejestrację mdM przy użyciu domyślnych poświadczeń usługi **Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego narzędzia ADMX dla programu Windows 10 w wersji 1803 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="084dc-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="084dc-148">Aby rozwiązać ten problem, wykonaj następujące czynności (Uwaga: najnowsza wersja pliku MDM.admx jest zgodna z poprzednimi wersjami):</span><span class="sxs-lookup"><span data-stu-id="084dc-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="084dc-149">Pobierz: [Szablony administracyjne (admx) dla systemu Windows 10 października 2020 r. (20h2)](https://www.microsoft.com/download/102157).</span><span class="sxs-lookup"><span data-stu-id="084dc-149">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="084dc-150">Zainstaluj pakiet na Kontroler domeny.</span><span class="sxs-lookup"><span data-stu-id="084dc-150">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="084dc-151">Przejdź do folderu w zależności od wersji szablonów **administracyjnych: C:\Program Files (x86)\Microsoft zasady grupy\Windows 10 aktualizacja z października 2020 r. (20h2)**.</span><span class="sxs-lookup"><span data-stu-id="084dc-151">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="084dc-152">Zmień nazwę **folderu Definicje** zasad na powyższej ścieżce do **folderu Definicje Zasad.**</span><span class="sxs-lookup"><span data-stu-id="084dc-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="084dc-153">Skopiuj folder **PolicyDefinitions** do udziału SYSVOL, domyślnie znajdujący się w folderze **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="084dc-153">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="084dc-154">Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość PolaOkreślenia Zasad.</span><span class="sxs-lookup"><span data-stu-id="084dc-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="084dc-155">Jeśli masz kilka kontrolerów domeny, poczekaj, aż narzędzie SYSVOL zreplikuje te zasady, które będą dostępne.</span><span class="sxs-lookup"><span data-stu-id="084dc-155">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="084dc-156">Ta procedura będzie działać również w przypadku każdej przyszłej wersji szablonów administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="084dc-156">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="084dc-157">Na tym etapie powinny być dostępne zasady Włącz automatyczną rejestrację **w usłudze MDM przy użyciu domyślnych dostępnych poświadczeń usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="084dc-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="084dc-158">Zawartość pokrewna</span><span class="sxs-lookup"><span data-stu-id="084dc-158">Related content</span></span>

<span data-ttu-id="084dc-159">[Synchronizowanie użytkowników domeny z Microsoft 365](manage-domain-users.md) (artykuł)</span><span class="sxs-lookup"><span data-stu-id="084dc-159">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>\
<span data-ttu-id="084dc-160">[Tworzenie grupy w centrum administracyjnym](../admin/create-groups/create-groups.md) (artykuł)</span><span class="sxs-lookup"><span data-stu-id="084dc-160">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>\
<span data-ttu-id="084dc-161">[Samouczek: konfigurowanie dołączania Azure Active Directory hybrydowego dla domen zarządzanych](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (artykuł)</span><span class="sxs-lookup"><span data-stu-id="084dc-161">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>