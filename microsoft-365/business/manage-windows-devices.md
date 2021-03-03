---
title: Włączanie zarządzania przez platformę Microsoft 365 dla firm na urządzeniach z systemem Windows 10 przyłączanych do domeny
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
description: Dowiedz się, jak w kilku krokach włączyć na platformie Microsoft 365 ochronę lokalnych urządzeń z systemem Windows 10 przyłącznych do usługi Active Directory.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407083"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="506ec-103">Włączanie zarządzania przez usługę Microsoft 365 Business Premium dla urządzeń przyłączanych do domeny systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="506ec-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="506ec-104">Jeśli Twoja organizacja korzysta z lokalnej usługi Active Directory systemu Windows Server, możesz skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="506ec-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="506ec-105">Aby skonfigurować tę ochronę, możesz zaimplementować urządzenia sprzężenia hybrydowego usługi **Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="506ec-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="506ec-106">Te urządzenia są połączone zarówno z lokalną usługą Active Directory, jak i z usługą Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="506ec-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="506ec-107">W tym klipie wideo opisano czynności, które należy wykonać w celu skonfigurowania tego ustawienia dla najbardziej typowego scenariusza, co opisano również w poniższych krokach.</span><span class="sxs-lookup"><span data-stu-id="506ec-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="506ec-108">Przed rozpoczęciem upewnij się, że wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="506ec-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="506ec-109">Synchronizowanie użytkowników z usługą Azure AD za pomocą programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="506ec-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="506ec-110">Ukończ synchronizację jednostki organizacyjnej programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="506ec-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="506ec-111">Upewnij się, że wszyscy użytkownicy domeny, których synchronizujesz, mają licencje na usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="506ec-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="506ec-112">Aby [uzyskać odpowiednie instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="506ec-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="506ec-113">1. Weryfikowanie uprawnień mdm w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="506ec-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="506ec-114">Przejdź do Menedżera [punktów](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) końcowych i na stronie Usługi  Microsoft Intune wybierz pozycję Rejestracja **urządzeń,** a następnie na stronie Omówienie upewnij się, że zarządzanie **usługą MDM** to **Intune.**</span><span class="sxs-lookup"><span data-stu-id="506ec-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="506ec-115">Jeśli **dla uprawnień mdm**  jest ustawiona wartość **Brak,** kliknij je, aby ustawić dla niego pozycję **Intune.**</span><span class="sxs-lookup"><span data-stu-id="506ec-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="506ec-116">Jeśli zarządzanie **mdm** to usługa Microsoft Office  **365,** przejdź do strony Urządzenia Zarejestruj urządzenia i użyj okna dialogowego Dodawanie urzędu mdm po prawej stronie, aby dodać uprawnienia usługi Intune MDM (okno dialogowe Dodawanie urzędu zarządzania mdm jest dostępne tylko wtedy, gdy dla uprawnienia MDM ustawiono usługę Microsoft Office  >   365).    </span><span class="sxs-lookup"><span data-stu-id="506ec-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="506ec-117">2. Sprawdzanie, czy w usłudze Azure AD włączono dołączanie do komputerów</span><span class="sxs-lookup"><span data-stu-id="506ec-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="506ec-118">Przejdź do centrum administracyjnego i wybierz pozycję Azure Active Directory (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory nie jest widoczna) na liście <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Centra** administracyjne. </span><span class="sxs-lookup"><span data-stu-id="506ec-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="506ec-119">W centrum **administracyjnym usługi Azure Active Directory przejdź** do usługi Azure Active **Directory,** wybierz **pozycję Urządzenia,** a następnie **pozycję Ustawienia urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="506ec-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="506ec-120">Sprawdzanie,**czy użytkownicy mogą dołączać urządzenia do usługi Azure AD**</span><span class="sxs-lookup"><span data-stu-id="506ec-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="506ec-121">Aby włączyć wszystkich użytkowników, ustaw wartość **All (Wszystko).**</span><span class="sxs-lookup"><span data-stu-id="506ec-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="506ec-122">Aby włączyć określonych użytkowników, ustaw opcję **Wybrano** w celu włączenia określonej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="506ec-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="506ec-123">Dodaj odpowiednich użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="506ec-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="506ec-124">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="506ec-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="506ec-125">3. Sprawdzanie, czy w usłudze Azure AD włączono usługę MDM</span><span class="sxs-lookup"><span data-stu-id="506ec-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="506ec-126">Przejdź do centrum administracyjnego i wybierz pozycję Zarządzanie punktami końcowymi (wybierz pozycję Pokaż wszystko, jeśli Menedżer punktów <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> końcowych jest niewidoczny)  </span><span class="sxs-lookup"><span data-stu-id="506ec-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="506ec-127">W centrum **administracyjnym programu Microsoft Endpoint Manager** przejdź do pozycji Urządzenia **z** automatyczną rejestracją systemu  >  **Windows** w systemie  >  **Windows.**  >  </span><span class="sxs-lookup"><span data-stu-id="506ec-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="506ec-128">Sprawdzanie, czy zakres użytkowników usługi MDM jest włączony.</span><span class="sxs-lookup"><span data-stu-id="506ec-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="506ec-129">Aby zarejestrować wszystkie komputery, ustaw wartość Wszystko tak, aby wszystkie komputery użytkowników, które są sprzężeniami z usługą Azure AD, i nowe komputery, gdy użytkownicy dodają konto służbowe w systemie Windows. </span><span class="sxs-lookup"><span data-stu-id="506ec-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="506ec-130">Ustaw wartość **Niektórzy,** aby zarejestrować komputery określonej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="506ec-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="506ec-131">Dodaj odpowiednich użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="506ec-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="506ec-132">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkowników usługi MDM dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="506ec-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="506ec-133">4. Tworzenie wymaganych zasobów</span><span class="sxs-lookup"><span data-stu-id="506ec-133">4. Create the required resources</span></span> 

<span data-ttu-id="506ec-134">Wykonywanie wymaganych zadań w celu skonfigurowania hybrydowego sprzężenia usługi [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) zostało uproszczone dzięki użyciu polecenia cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) które znajduje się w module PowerShell programu [SecMgmt.](https://www.powershellgallery.com/packages/SecMgmt)</span><span class="sxs-lookup"><span data-stu-id="506ec-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="506ec-135">Po wywołaniu tego polecenia cmdlet utworzy ono i skonfiguruje wymagany punkt połączenia usługi oraz zasady grupy.</span><span class="sxs-lookup"><span data-stu-id="506ec-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="506ec-136">Ten moduł można zainstalować, inicjując następujące polecenia z wystąpienia programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="506ec-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="506ec-137">Zalecamy zainstalowanie tego modułu na serwerze Windows Server z uruchomionym programem Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="506ec-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="506ec-138">Aby utworzyć wymagany punkt połączenia usługi i zasady grupy, należy wywołać polecenie cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="506ec-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="506ec-139">Podczas wykonywania tego zadania będziesz potrzebować poświadczeń administratora globalnego usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="506ec-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="506ec-140">Gdy wszystko będzie gotowe do utworzenia zasobów, wywołaj następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="506ec-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="506ec-141">Pierwsze polecenie nawiąze połączenie z chmurą firmy Microsoft, a po wyświetleniu monitu określ poświadczenia administratora globalnego usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="506ec-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="506ec-142">5. Połącz zasady grupy</span><span class="sxs-lookup"><span data-stu-id="506ec-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="506ec-143">W konsoli zasady grupy zarządzania (GPMC) kliknij prawym przyciskiem myszy lokalizację, w której chcesz połączyć zasady, i wybierz z menu kontekstowego pozycję Połącz istniejący element *zasad* grupy.</span><span class="sxs-lookup"><span data-stu-id="506ec-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="506ec-144">Wybierz zasady utworzone w powyższym kroku, a następnie kliknij **przycisk OK.**</span><span class="sxs-lookup"><span data-stu-id="506ec-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="506ec-145">Pobierz najnowsze szablony administracyjne</span><span class="sxs-lookup"><span data-stu-id="506ec-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="506ec-146">Jeśli nie widzisz zasad Włącz automatyczną rejestrację mdm przy użyciu domyślnych poświadczeń usługi **Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego narzędzia ADMX dla systemu Windows 10 w wersji 1803 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="506ec-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="506ec-147">Aby rozwiązać ten problem, wykonaj następujące czynności (Uwaga: najnowsza wersja pliku MDM.admx jest zgodna ze starszymi wersjami):</span><span class="sxs-lookup"><span data-stu-id="506ec-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="506ec-148">Pobierz: [Szablony administracyjne (admx) dla systemu Windows 10 aktualizacja z października 2020 r. (20H2).](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="506ec-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="506ec-149">Zainstaluj pakiet na Kontroler domeny.</span><span class="sxs-lookup"><span data-stu-id="506ec-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="506ec-150">W zależności od wersji szablonów administracyjnych przejdź do folderu: **C:\Program Files (x86)\Microsoft zasady grupy\Windows 10 October 2020 Update (20H2).**</span><span class="sxs-lookup"><span data-stu-id="506ec-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="506ec-151">Zmień nazwę **folderu Definicje** zasad na powyższej ścieżce **na PolicyDefinitions.**</span><span class="sxs-lookup"><span data-stu-id="506ec-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="506ec-152">Skopiuj folder **PolicyDefinitions** do udziału SYSVOL, który domyślnie znajduje się w folderze **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="506ec-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="506ec-153">Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość zasadDefinitions.</span><span class="sxs-lookup"><span data-stu-id="506ec-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="506ec-154">Jeśli masz kilka kontrolerów domen, poczekaj, aż system SYSVOL zreplikuje te zasady, aby były dostępne.</span><span class="sxs-lookup"><span data-stu-id="506ec-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="506ec-155">Ta procedura będzie działać również w przypadku każdej przyszłej wersji szablonów administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="506ec-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="506ec-156">W tym momencie powinno być możliwe wyświetlanie zasad Włącz automatyczną rejestrację mdm przy użyciu domyślnych dostępnych **poświadczeń usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="506ec-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
