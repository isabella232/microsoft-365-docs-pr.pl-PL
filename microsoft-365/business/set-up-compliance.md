---
title: Zwiększ ochronę przed zagrożeniami dla Microsoft 365 Business
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Skonfiguruj zaawansowaną ochronę przed zagrożeniami w pakiecie Office 365 i Chroń poufne dane.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288750"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="9b01f-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="9b01f-103">Set up compliance features</span></span>

<span data-ttu-id="9b01f-104">Twoja firma Microsoft 365 Business zawiera funkcje chroniące dane i urządzenia oraz pomagające w zabezpieczeniu poufnych informacji Twoich i Twoich klientów.</span><span class="sxs-lookup"><span data-stu-id="9b01f-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="9b01f-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="9b01f-105">Set up DLP features</span></span>

<span data-ttu-id="9b01f-106">Zobacz [Tworzenie zasad DLP z szablonu](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) , aby zapoznać się z przykładem sposobu konfigurowania zasad w celu ochrony przed danymi osobowymi (PII).</span><span class="sxs-lookup"><span data-stu-id="9b01f-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="9b01f-107">DLP zawiera wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych.</span><span class="sxs-lookup"><span data-stu-id="9b01f-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="9b01f-108">Na przykład, Australia dane finansowe, Kanada informacje osobiste Act, dane finansowe USA, itp. Zobacz [, jakie szablony zasad DLP zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pełną listę.</span><span class="sxs-lookup"><span data-stu-id="9b01f-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="9b01f-109">Wszystkie te szablony można włączyć podobne do przykładu szablonu PII.</span><span class="sxs-lookup"><span data-stu-id="9b01f-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="9b01f-110">Konfigurowanie przechowywania poczty e-mail przy użyciu usługi Exchange Online archiwizacji</span><span class="sxs-lookup"><span data-stu-id="9b01f-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="9b01f-111">Funkcje **programu Exchange Online archiwizowanie** licencji ułatwiają zachowanie zgodności i standardów regulacyjnych przez zachowanie zawartości poczty elektronicznej na potrzeby zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="9b01f-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="9b01f-112">Pomaga również zmniejszyć ryzyko w przypadku pozew i umożliwia odzyskanie danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy.</span><span class="sxs-lookup"><span data-stu-id="9b01f-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="9b01f-113">Aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować, możesz użyć wstrzymania w postępowaniu sądowym.</span><span class="sxs-lookup"><span data-stu-id="9b01f-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="9b01f-114">**Sądowym:** Możesz zachować całą zawartość skrzynki pocztowej, w tym elementy usunięte, umieszczając całą skrzynkę pocztową użytkownika w postępowaniu sądowym.</span><span class="sxs-lookup"><span data-stu-id="9b01f-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="9b01f-115">Aby umieścić skrzynkę pocztową w postępowaniu sądowym, w centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="9b01f-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="9b01f-116">W lewym NAV przejdź do **użytkowników** \> **aktywnych**użytkowników.</span><span class="sxs-lookup"><span data-stu-id="9b01f-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="9b01f-117">Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić na sądowym i w okienku użytkownika rozwiń **Ustawienia poczty** i obok **więcej ustawień** wybierz **Edytuj właściwości programu Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9b01f-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="9b01f-118">Na stronie skrzynki pocztowej dla użytkownika wybierz \* \* funkcje skrzynki pocztowej \* \* na lewej NAV, a następnie wybierz **Włącz** łącze w związku z **postępowaniem sądowym**.</span><span class="sxs-lookup"><span data-stu-id="9b01f-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="9b01f-119">W oknie dialogowym wstrzymanie w postępowaniu **sądowym** można określić czas trwania wstrzymania w trakcie postępowania sądowego w polu **czas trwania wstrzymania** , pozostawić pole puste, jeśli chcesz umieścić nieskończoną wstrzymania.</span><span class="sxs-lookup"><span data-stu-id="9b01f-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="9b01f-120">Można również dodawać notatki i kierować właścicielem skrzynki pocztowej do witryny sieci Web może być trzeba wyjaśnić więcej o sądowym wstrzymanie \> **zapisywania**.</span><span class="sxs-lookup"><span data-stu-id="9b01f-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="9b01f-121">**Zatrzymanie:** Można włączyć niestandardowe zasady przechowywania, na przykład, aby zachować określoną ilość czasu lub trwale usunąć zawartość na końcu okresu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="9b01f-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="9b01f-122">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="9b01f-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="9b01f-123">Konfigurowanie funkcji usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9b01f-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="9b01f-124">Usługa Azure Information Protection (AIP) pomaga klasyfikować i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="9b01f-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="9b01f-125">Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub przy użyciu kombinacji, gdzie użytkownicy są podane zalecenia.</span><span class="sxs-lookup"><span data-stu-id="9b01f-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="9b01f-126">W programie Outlook w sieci Web można zastosować następujące wbudowane etykiety i ograniczenia do wiadomości e-mail:</span><span class="sxs-lookup"><span data-stu-id="9b01f-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="9b01f-127">**Nie przesyłają dalej**: odbiorcy mogą odczytać wiadomość, ale nie mogą przekazywać, drukować ani kopiować zawartości</span><span class="sxs-lookup"><span data-stu-id="9b01f-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="9b01f-128">**Encrypt**: cała wiadomość jest szyfrowana.</span><span class="sxs-lookup"><span data-stu-id="9b01f-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="9b01f-129">Odbiorcy muszą potwierdzić swoją tożsamość przed uzyskaniem dostępu do zaszyfrowanej zawartości i nie mogą usunąć szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="9b01f-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="9b01f-130">**Poufne**: zapewnia pracownikom w organizacji pełne uprawnienia do zawartości wiadomości e-mail i załączników, ale nie do osób spoza organizacji.</span><span class="sxs-lookup"><span data-stu-id="9b01f-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="9b01f-131">Właściciele danych mogą śledzić i odwoływać zawartość w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="9b01f-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="9b01f-132">**Wysoce poufne**: to ograniczenie można zastosować do wysoce poufnych danych, umożliwiając pracownikom wyświetlanie, edytowanie i odpowiadanie, ale nie przekazywanie, drukowanie lub kopiowanie danych.</span><span class="sxs-lookup"><span data-stu-id="9b01f-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="9b01f-133">Właściciele danych mogą śledzić i odwoływać zawartość w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="9b01f-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="9b01f-134">Upewnij się, że usługa Azure Information Protection jest aktywna</span><span class="sxs-lookup"><span data-stu-id="9b01f-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="9b01f-135">Aby sprawdzić, czy włączono AIP:</span><span class="sxs-lookup"><span data-stu-id="9b01f-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="9b01f-136">Zaloguj się do [witryny Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="9b01f-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="9b01f-137">Wybierz **wszystkie usługi** i wpisz w *usłudze Azure Information Protection* w **polu wyszukiwania**.</span><span class="sxs-lookup"><span data-stu-id="9b01f-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="9b01f-138">Po wyświetleniu wyników kliknij przycisk Start obok **usługi Azure Information Protection** , aby uczynić go ulubionym i łatwo znaleźć później.</span><span class="sxs-lookup"><span data-stu-id="9b01f-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="9b01f-139">Wybierz \> **aktywacji ochrony** **informacji Azure** i upewnij się, że stan jest ustawiony na aktywowany.</span><span class="sxs-lookup"><span data-stu-id="9b01f-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="9b01f-140">Wyświetlanie zasad usługi Azure Information Protection i etykiet domyślnych</span><span class="sxs-lookup"><span data-stu-id="9b01f-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="9b01f-141">Aby wyświetlić i zmodyfikować istniejące etykiety:</span><span class="sxs-lookup"><span data-stu-id="9b01f-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="9b01f-142">Na pulpicie nawigacyjnym usługi Azure Information Protection wybierz pozycję **klasyfikacje** \> **etykiet**.</span><span class="sxs-lookup"><span data-stu-id="9b01f-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="9b01f-143">![Standardowe etykiety dla usługi Azure Information Protection.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="9b01f-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="9b01f-144">Można wybrać dowolną etykietę, aby wyświetlić opcje, można zmienić nazwę wyświetlaną, kolory, itp.</span><span class="sxs-lookup"><span data-stu-id="9b01f-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="9b01f-145">Zobacz [modyfikowanie i tworzenie nowych etykiet](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) , jeśli chcesz tworzyć własne.</span><span class="sxs-lookup"><span data-stu-id="9b01f-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="9b01f-146">Ręczne instalowanie klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9b01f-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="9b01f-147">Aby ręcznie zainstalować klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="9b01f-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="9b01f-148">Pobierz **Azinfoprotection. exe** z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="9b01f-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="9b01f-149">Można sprawdzić, czy instalacja zadziałało, przeglądając dokument programu Word i upewniając się, że opcja **Chroń** jest dostępna na karcie **Narzędzia główne** .</span><span class="sxs-lookup"><span data-stu-id="9b01f-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="9b01f-150">![Karta ochrona listy rozwijanej w dokumencie programu Word.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="9b01f-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="9b01f-151">Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="9b01f-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
