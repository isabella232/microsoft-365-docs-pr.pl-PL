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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564956"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="a72e7-103">Włączanie zarządzania urządzeniami z systemem Windows 10 przyłączanym do domeny przez usługę Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="a72e7-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a72e7-104">Jeśli twoja organizacja korzysta z usługi Windows Server Active Directory lokalnie, można skonfigurować usługę Microsoft 365 Business Premium w celu ochrony urządzeń z systemem Windows 10, zachowując jednocześnie dostęp do zasobów lokalnych wymagających uwierzytelniania lokalnego.</span><span class="sxs-lookup"><span data-stu-id="a72e7-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="a72e7-105">Aby skonfigurować tę ochronę, można zaimplementować **urządzenia przyłączone do usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="a72e7-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="a72e7-106">Te urządzenia są przyłączane zarówno do lokalnej usługi Active Directory, jak i usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a72e7-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="a72e7-107">W tym klipie wideo opisano kroki dotyczące konfigurowania tego dla najbardziej typowych scenariuszy, który jest również szczegółowo opisany w kolejnych krokach.</span><span class="sxs-lookup"><span data-stu-id="a72e7-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="a72e7-108">Zanim zaczniesz, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a72e7-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="a72e7-109">Synchronizowanie użytkowników z usługą Azure AD z usługą Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a72e7-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="a72e7-110">Pełna synchronizacja jednostki organizacyjnej usługi Azure AD Connect(OU).</span><span class="sxs-lookup"><span data-stu-id="a72e7-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="a72e7-111">Upewnij się, że wszyscy synchronizowani użytkownicy domeny mają licencje na usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a72e7-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a72e7-112">Aby uzyskać [instrukcje,](manage-domain-users.md) zobacz Synchronizowanie użytkowników domeny z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a72e7-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="a72e7-113">1. Sprawdź urząd MDM w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="a72e7-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="a72e7-114">Przejdź do portal.azure.com i w górnej części strony wyszukaj usługę Intune.</span><span class="sxs-lookup"><span data-stu-id="a72e7-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="a72e7-115">Na stronie Usługi Microsoft Intune wybierz pozycję **Rejestracja na urządzenia** i na stronie **Przegląd** upewnij się, że **urzędem MDM** jest **usługa Intune**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="a72e7-116">Jeśli **urząd MDM** to **Brak,** kliknij **urząd MDM,** aby ustawić go na **Intune**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="a72e7-117">Jeśli **urzędem MDM** jest **usługa Microsoft Office 365,** przejdź do urządzenia **Devices**  >  **Rejestruj urządzenia** i użyj okna dialogowego **Dodaj urząd MDM** po prawej stronie, aby dodać uprawnienia **MDM usługi Intune** (okno dialogowe **Dodaj urząd MDM** jest dostępne tylko wtedy, gdy **urząd MDM** jest ustawiony na usługę Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="a72e7-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="a72e7-118">2. Sprawdź, czy usługa Azure AD jest włączona do łączenia komputerów</span><span class="sxs-lookup"><span data-stu-id="a72e7-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="a72e7-119">Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> i wybierz pozycję Usługa Azure Active **Directory** (wybierz pozycję Pokaż wszystko, jeśli usługa Azure Active Directory nie jest widoczna) na liście **Centra administracyjne.**</span><span class="sxs-lookup"><span data-stu-id="a72e7-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="a72e7-120">W **centrum administracyjnym usługi Azure Active Directory**przejdź do **usługi Azure Active Directory** , wybierz pozycję **Urządzenia,** a następnie **ustawienia urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="a72e7-121">Sprawdź, czy**użytkownicy mogą dołączać urządzenia do usługi Azure AD** jest włączona</span><span class="sxs-lookup"><span data-stu-id="a72e7-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="a72e7-122">Aby włączyć wszystkich użytkowników, ustaw opcję **Wszystkie**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="a72e7-123">Aby włączyć określonych użytkowników, ustaw opcję **Wybrane,** aby włączyć określoną grupę użytkowników.</span><span class="sxs-lookup"><span data-stu-id="a72e7-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="a72e7-124">Dodaj żądanych użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="a72e7-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="a72e7-125">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkownika mdm dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="a72e7-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="a72e7-126">3. Sprawdź, czy usługa Azure AD jest włączona dla usługi MDM</span><span class="sxs-lookup"><span data-stu-id="a72e7-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="a72e7-127">Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> i wybierz pozycję **Endpoint Managemen**t (wybierz pozycję **Pokaż wszystko,** jeśli **Menedżer punktów końcowych** nie jest widoczny)</span><span class="sxs-lookup"><span data-stu-id="a72e7-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="a72e7-128">W **centrum administracyjnym programu Microsoft Endpoint Manager**przejdź do **pozycji Urządzenia**Rejestracji systemu  >  **Windows**  >  **Windows Enrollment**  >  **Rejestracja automatyczna rejestracja**systemu .</span><span class="sxs-lookup"><span data-stu-id="a72e7-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="a72e7-129">Sprawdź, czy zakres użytkownika MDM jest włączony.</span><span class="sxs-lookup"><span data-stu-id="a72e7-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="a72e7-130">Aby zarejestrować wszystkie komputery, ustaw opcję **Wszystkie,** aby automatycznie rejestrować wszystkie komputery użytkowników, które są przyłączone do usługi Azure AD i nowe komputery, gdy użytkownicy dodają konto służbowe do systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="a72e7-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="a72e7-131">Ustaw na **Niektóre,** aby zarejestrować komputery określonej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="a72e7-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="a72e7-132">Dodaj żądanych użytkowników domeny zsynchronizowanych w usłudze Azure AD do [grupy zabezpieczeń](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="a72e7-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="a72e7-133">Wybierz **pozycję Wybierz grupy,** aby włączyć zakres użytkownika mdm dla tej grupy zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="a72e7-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="a72e7-134">4. Konfigurowanie punktu połączenia usługi (SCP)</span><span class="sxs-lookup"><span data-stu-id="a72e7-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="a72e7-135">Te kroki są [uproszczone z konfigurowania hybrydowego połączenia usługi Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="a72e7-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="a72e7-136">Aby wykonać kroki, musisz użyć usługi Azure AD Connect i globalnych haseł administratora i administratora usługi Active Directory usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a72e7-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="a72e7-137">Uruchom usługę Azure AD Connect, a następnie wybierz pozycję **Konfiguruj**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="a72e7-138">Na stronie **Zadania dodatkowe** wybierz pozycję **Konfiguruj opcje urządzenia**, a następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="a72e7-139">Na stronie **Przegląd** wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="a72e7-140">Na stronie **Połącz z usługą Azure AD** wprowadź poświadczenia administratora globalnego dla usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a72e7-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="a72e7-141">Na stronie **Opcje urządzenia** wybierz pozycję **Konfiguruj hybrydowe sprzężenie usługi Azure AD,** a następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="a72e7-142">Na stronie **SCP** dla każdego lasu, w którym ma być skonfigurowany protokół SCP usługi Azure AD Connect, wykonaj następujące kroki, a następnie wybierz przycisk **Dalej:**</span><span class="sxs-lookup"><span data-stu-id="a72e7-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="a72e7-143">Zaznacz pole obok nazwy lasu.</span><span class="sxs-lookup"><span data-stu-id="a72e7-143">Check the box beside the forest name.</span></span> <span data-ttu-id="a72e7-144">Las powinien być twoją nazwą domeny usługi AD.</span><span class="sxs-lookup"><span data-stu-id="a72e7-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="a72e7-145">W kolumnie **Usługa uwierzytelniania** otwórz listy rozwijanej i wybierz pasującą nazwę domeny (powinna istnieć tylko jedna opcja).</span><span class="sxs-lookup"><span data-stu-id="a72e7-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="a72e7-146">Wybierz **pozycję Dodaj,** aby wprowadzić poświadczenia administratora domeny.</span><span class="sxs-lookup"><span data-stu-id="a72e7-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="a72e7-147">Na stronie **Systemy operacyjne Urządzenia** wybierz tylko urządzenia z systemem Windows 10 lub nowszym.</span><span class="sxs-lookup"><span data-stu-id="a72e7-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="a72e7-148">Na stronie **Gotowe do skonfigurowania** wybierz pozycję **Konfiguruj**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="a72e7-149">Na stronie **Konfiguracja zakończona** wybierz pozycję **Zakończ**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="a72e7-150">5. Tworzenie obiektu zasad grupy dla rejestracji usługi Intune — metoda ADMX</span><span class="sxs-lookup"><span data-stu-id="a72e7-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="a72e7-151">Używać. admx pliku szablonu.</span><span class="sxs-lookup"><span data-stu-id="a72e7-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="a72e7-152">Zaloguj się do serwera USŁUGI AD, wyszukaj i otwórz **zarządzanie**  >  **Tools**  >  **zasadami grupy**Narzędzia Menedżera serwera .</span><span class="sxs-lookup"><span data-stu-id="a72e7-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="a72e7-153">Wybierz nazwę domeny w obszarze **Domeny** i kliknij prawym przyciskiem myszy **pozycję Obiekty zasad grupy,** aby wybrać pozycję **Nowy**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="a72e7-154">Nadaj nowemu obiektowi obiektu zasad grupy nazwę, na przykład "*Cloud_Enrollment*", a następnie wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="a72e7-155">Kliknij prawym przyciskiem myszy nowy obiekt zasad grupy w obszarze **Obiekty zasad grupy** i wybierz polecenie **Edytuj**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="a72e7-156">W **Edytorze zarządzania zasadami grupy**przejdź do **strony Zasady konfiguracji komputera**  >  **Policies**  >  **Szablony administracyjne składników**systemu  >  **Windows**  >  **MDM**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="a72e7-157">Kliknij prawym przyciskiem myszy **pozycję Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD,** a następnie wybierz pozycję **Włączone**  >  **OK**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="a72e7-158">Zamknij okno edytora.</span><span class="sxs-lookup"><span data-stu-id="a72e7-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a72e7-159">Jeśli zasady nie są widoczne **włącz automatyczne rejestrowanie mdm przy użyciu domyślnych poświadczeń usługi Azure AD,** zobacz [Pobieranie najnowszych szablonów administracyjnych](#get-the-latest-administrative-templates).</span><span class="sxs-lookup"><span data-stu-id="a72e7-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="a72e7-160">6. Wdrażanie zasad grupy</span><span class="sxs-lookup"><span data-stu-id="a72e7-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="a72e7-161">W Menedżerze serwera w obszarze **Domeny** > obiekty zasad grupy wybierz obiekt zasad grupy z kroku 3 powyżej, na przykład "Cloud_Enrollment".</span><span class="sxs-lookup"><span data-stu-id="a72e7-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="a72e7-162">Wybierz kartę **Zakres** dla obiektu zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="a72e7-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="a72e7-163">Na karcie Zakres obiektu zasad grupy kliknij prawym przyciskiem myszy łącze do domeny w obszarze **Łącza**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="a72e7-164">Wybierz **opcję Wymuszone,** aby wdrożyć obiekt zasad grupy, a następnie **przycisk OK** na ekranie potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="a72e7-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="a72e7-165">Pobierz najnowsze szablony administracyjne</span><span class="sxs-lookup"><span data-stu-id="a72e7-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="a72e7-166">Jeśli zasady nie są widoczne **Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD,** może to być spowodowane tym, że nie masz zainstalowanego serwera ADMX dla systemu Windows 10, wersja 1803, wersja 1809 lub wersja 1903.</span><span class="sxs-lookup"><span data-stu-id="a72e7-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="a72e7-167">Aby rozwiązać ten problem, wykonaj następujące kroki (Uwaga: najnowszy plik MDM.admx jest zgodny wstecz:</span><span class="sxs-lookup"><span data-stu-id="a72e7-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="a72e7-168">Pobierz: [Szablony administracyjne (admx) dla systemu Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="a72e7-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="a72e7-169">Zainstaluj pakiet na podstawowym kontrolerze domeny (PDC).</span><span class="sxs-lookup"><span data-stu-id="a72e7-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="a72e7-170">Przejdź, w zależności od wersji do folderu: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="a72e7-171">Zmień nazwę folderu **Definicje zasad** na powyższej ścieżce na **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="a72e7-172">Kopiuj folder **PolicyDefinitions** do **folderu C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="a72e7-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="a72e7-173">Jeśli planujesz używać centralnego magazynu zasad dla całej domeny, dodaj tam zawartość policyDefinitions.</span><span class="sxs-lookup"><span data-stu-id="a72e7-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="a72e7-174">Uruchom ponownie podstawowy kontroler domeny, aby zasady były dostępne.</span><span class="sxs-lookup"><span data-stu-id="a72e7-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="a72e7-175">Ta procedura będzie działać dla każdej przyszłej wersji, jak również.</span><span class="sxs-lookup"><span data-stu-id="a72e7-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="a72e7-176">W tym momencie powinieneś być w stanie zobaczyć zasady **Włącz automatyczną rejestrację MDM przy użyciu domyślnych poświadczeń usługi Azure AD** dostępne.</span><span class="sxs-lookup"><span data-stu-id="a72e7-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

