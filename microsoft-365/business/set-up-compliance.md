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
ms.custom:
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
description: Konfigurowanie pakietu Office 365 Zaawansowana ochrona przed zagrożeniami i ochrony poufnych danych.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086370"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="81130-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="81130-103">Set up compliance features</span></span>

<span data-ttu-id="81130-104">365 firmy Microsoft zawiera funkcje do ochrony Twoich danych i urządzeń i pomagają zabezpieczyć Twoje i poufne informacje klientów.</span><span class="sxs-lookup"><span data-stu-id="81130-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="81130-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="81130-105">Set up DLP features</span></span>

<span data-ttu-id="81130-106">Zobacz [Tworzenie zasad DLP z szablonu](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) , na przykład dotyczące sposobu definiowania zasad ochrony przed identyfikowalne dane osobowe.</span><span class="sxs-lookup"><span data-stu-id="81130-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="81130-107">DLP zawiera wiele szablonów zasad gotowe do użycia dla wielu różnych ustawień regionalnych.</span><span class="sxs-lookup"><span data-stu-id="81130-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="81130-108">Na przykład, danych finansowych Australia, Kanada ustawy informacji osobowych, danych finansowych USA, itp. Aby uzyskać pełną listę, zobacz [Szablony zasad DLP co zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) .</span><span class="sxs-lookup"><span data-stu-id="81130-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="81130-109">Wszystkie te szablony można włączyć podobne do przykładu PII szablonu.</span><span class="sxs-lookup"><span data-stu-id="81130-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="81130-110">Konfigurowanie przechowywanie wiadomości e-mail z programu Exchange Online — archiwum</span><span class="sxs-lookup"><span data-stu-id="81130-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="81130-111">Funkcje licencji **Exchange Online — archiwum** pomóc w zachowaniu zgodności i normami zachowując e-mail zawartości dla zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="81130-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="81130-112">Również pomaga zmniejszyć ryzyko w przypadku pozwu i daje możliwość odzyskania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy.</span><span class="sxs-lookup"><span data-stu-id="81130-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="81130-113">Możesz użyć sądowym, aby zachować całą zawartość użytkownika lub umożliwia dostosowywanie, mają być zachowane zasady przechowywania.</span><span class="sxs-lookup"><span data-stu-id="81130-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="81130-114">**Sądowym:** Można zachować całą zawartość skrzynki pocztowej przytrzymaj tym elementów usuniętych przez umieszczenie całej skrzynki pocztowej użytkownika na postępowania sądowego.</span><span class="sxs-lookup"><span data-stu-id="81130-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="81130-115">Aby umieścić skrzynkę pocztową z postępowaniem sądowym, w Centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="81130-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="81130-116">W nawigacji z lewej strony, przejdź do **użytkowników** \> **aktywnych użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="81130-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="81130-117">Wybierz użytkownika, której skrzynkę pocztową chcesz umieścić na spory sądowe przytrzymaj i w okienku użytkownika rozwiń **Ustawienia poczty** i obok **Więcej ustawień** , wybierz polecenie **Właściwości, edytowanie programu Exchange**.</span><span class="sxs-lookup"><span data-stu-id="81130-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="81130-118">Na stronie skrzynki pocztowej użytkownika, wybierz opcję \*\* Funkcje skrzynki pocztowej \*\* na nawigacji z lewej strony, a następnie wybierz **Włącz** łącze w obszarze **sądowym**.</span><span class="sxs-lookup"><span data-stu-id="81130-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="81130-119">W **sądowym** okno dialogowe można określić postępowania sądowego przytrzymaj czasu trwania w polu **czas trwania sądowym** , pozostaw pole puste, jeśli chcesz umieścić nieskończone blokady.</span><span class="sxs-lookup"><span data-stu-id="81130-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="81130-120">Można również dodawać notatki i bezpośrednie właściciela pola korespondencji do witryny, może zajść potrzeba wyjaśnienia, więcej informacji na temat postępowania sądowego przytrzymaj \> **zapisać**.</span><span class="sxs-lookup"><span data-stu-id="81130-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="81130-121">**Retencji:** Zasady przechowywania niestandardowe, na przykład, można włączyć w celu zachowania przez określoną ilość czasu lub trwale usunąć zawartość z końcem okresu przetrzymania.</span><span class="sxs-lookup"><span data-stu-id="81130-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="81130-122">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="81130-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="81130-123">Konfigurowanie funkcji ochrony informacji Azure</span><span class="sxs-lookup"><span data-stu-id="81130-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="81130-124">Ochrona informacji Azure (AIP) pomaga klasyfikowania i opcjonalnie chronić Twoje dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="81130-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="81130-125">Etykiety można automatycznie zastosowane przez administratorów, którzy definiują zasady i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, gdzie użytkownicy są podane zalecenia.</span><span class="sxs-lookup"><span data-stu-id="81130-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="81130-126">W programie Outlook w sieci web do wiadomości e-mail można zastosować następujące etykiety wbudowanych i ograniczenia:</span><span class="sxs-lookup"><span data-stu-id="81130-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="81130-127">**Nie przesyłaj dalej**: Adresaci mogą czytać wiadomości, ale one nie można przesłać dalej, wydrukować ani skopiować zawartości</span><span class="sxs-lookup"><span data-stu-id="81130-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="81130-128">**Szyfruj**: całą wiadomość jest zaszyfrowana.</span><span class="sxs-lookup"><span data-stu-id="81130-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="81130-129">Adresaci muszą potwierdzić swoją tożsamość przed uzyskaniem dostępu do zaszyfrowanej zawartości i nie można usunąć szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="81130-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="81130-130">**Poufne**: daje pracowników w firmie pełne uprawnienia w odniesieniu do treści wiadomości e-mail i załączniki, ale nie do osób spoza organizacji.</span><span class="sxs-lookup"><span data-stu-id="81130-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="81130-131">Właścicieli danych można śledzić i odwołać zawartości w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="81130-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="81130-132">**Ściśle tajne**: tego ograniczenia mogą być stosowane do ściśle poufne dane, dzięki czemu pracownicy wyświetlić, edytować i odpowiedzieć, ale nie do przodu, drukowania lub kopiowania danych.</span><span class="sxs-lookup"><span data-stu-id="81130-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="81130-133">Właścicieli danych można śledzić i odwołać zawartości w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="81130-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="81130-134">Upewnij się, że włączono ochronę informacji Azure</span><span class="sxs-lookup"><span data-stu-id="81130-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="81130-135">Aby zweryfikować, że AIP jest włączona:</span><span class="sxs-lookup"><span data-stu-id="81130-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="81130-136">Zalogować się do [portalu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="81130-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="81130-137">Wybierz **wszystkie usługi** i typ w *Ochronie informacji Azure* w **Pole wyszukiwania**.</span><span class="sxs-lookup"><span data-stu-id="81130-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="81130-138">Gdy wyniki są wyświetlane, kliknij przycisk start, dalej do **Ochrony informacji Azure** , aby dodać ją do ulubionych i łatwo później odnaleźć.</span><span class="sxs-lookup"><span data-stu-id="81130-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="81130-139">Wybierz opcję **Ochrony informacji Azure** \> **aktywacji ochrony** i upewnij się, że stan jest ustawiony do aktywowany.</span><span class="sxs-lookup"><span data-stu-id="81130-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="81130-140">Wyświetlanie etykiety zasad i domyślną ochronę informacji Azure</span><span class="sxs-lookup"><span data-stu-id="81130-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="81130-141">Aby przeglądać i modyfikować, istniejące etykiety:</span><span class="sxs-lookup"><span data-stu-id="81130-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="81130-142">Na pulpicie nawigacyjnym Azure ochrony informacji, wybierz **Klasyfikacje** \> **etykiety**.</span><span class="sxs-lookup"><span data-stu-id="81130-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="81130-143">![Standardowe etykiety dla ochrony informacji Azure.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="81130-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="81130-144">Wszelkie etykiety, aby wyświetlić opcje można wybrać, można zmienić nazwę wyświetlaną, kolory itd.</span><span class="sxs-lookup"><span data-stu-id="81130-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="81130-145">Zobacz [Modyfikuj i Utwórz nowe etykiety](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Jeśli chcesz tworzyć swoje własne.</span><span class="sxs-lookup"><span data-stu-id="81130-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="81130-146">Ręcznie zainstaluj klienta ochrony informacji Azure</span><span class="sxs-lookup"><span data-stu-id="81130-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="81130-147">Aby ręcznie zainstalować klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="81130-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="81130-148">**AzInfoProtection.exe** pobrać z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="81130-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="81130-149">Można sprawdzić, czy instalacja zadziałała wyświetlając dokument programu Word i upewniając się, że opcja **Ochrona** jest dostępna na karcie **Narzędzia główne** .</span><span class="sxs-lookup"><span data-stu-id="81130-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="81130-150">![Kartę Ochrona listy rozwijanej w dokumencie programu Word.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="81130-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="81130-151">Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="81130-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
