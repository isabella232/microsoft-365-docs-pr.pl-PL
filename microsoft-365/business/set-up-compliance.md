---
title: Zwiększ ochronę przed zagrożeniami dla firmy Microsoft 365 Business
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i oznaczać poufne dane.
ms.openlocfilehash: 09619de03aafde37106fb3942890b457c488ad43
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593410"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="b7397-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="b7397-103">Set up compliance features</span></span>

<span data-ttu-id="b7397-104">Firma Microsoft 365 Business jest wyposażona w funkcje chroniące dane i urządzenia oraz ułatwiające bezpieczeństwo poufnych informacji użytkownika i klientów.</span><span class="sxs-lookup"><span data-stu-id="b7397-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="b7397-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="b7397-105">Set up DLP features</span></span>

<span data-ttu-id="b7397-106">Zobacz [Tworzenie zasad DLP z szablonu,](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) aby uzyskać przykład konfigurowania zasad chroniących przed danymi osobowymi (PII).</span><span class="sxs-lookup"><span data-stu-id="b7397-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="b7397-107">DLP jest wyposażony w wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych.</span><span class="sxs-lookup"><span data-stu-id="b7397-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="b7397-108">Na przykład Australia Financial Data, Canada Personal Information Act, U.S. Financial Data itd.</span><span class="sxs-lookup"><span data-stu-id="b7397-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="b7397-109">Zobacz, [jakie szablony zasad DLP zawierają,](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) aby uzyskać pełną listę.</span><span class="sxs-lookup"><span data-stu-id="b7397-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="b7397-110">Wszystkie te szablony można włączyć podobnie do przykładu szablonu interfejsu ii.</span><span class="sxs-lookup"><span data-stu-id="b7397-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="b7397-111">Konfigurowanie przechowywania wiadomości e-mail za pomocą archiwizacji online programu Exchange</span><span class="sxs-lookup"><span data-stu-id="b7397-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="b7397-112">Funkcje licencji **usługi Exchange Online Archiving** pomagają zachować zgodność i standardy regulacyjne, zachowując zawartość wiadomości e-mail w celu zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="b7397-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="b7397-113">Pomaga również zmniejszyć ryzyko, jeśli istnieje pozew, i zapewnia sposób odzyskiwania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy.</span><span class="sxs-lookup"><span data-stu-id="b7397-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="b7397-114">Możesz użyć blokady sporów, aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować.</span><span class="sxs-lookup"><span data-stu-id="b7397-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="b7397-115">**Wstrzymanie postępowania sądowego:** Możesz zachować całą zawartość skrzynki pocztowej, w tym usunięte elementy, wstrzymując całą skrzynkę pocztową użytkownika.</span><span class="sxs-lookup"><span data-stu-id="b7397-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="b7397-116">Aby zawiesić skrzynkę pocztową w sporze sądowym, w centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="b7397-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="b7397-117">W lewej nav przejdź do **użytkowników** \> **aktywnych użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="b7397-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="b7397-118">Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić w sporze sądowym.</span><span class="sxs-lookup"><span data-stu-id="b7397-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="b7397-119">W okienku użytkownika rozwiń **pozycję Ustawienia poczty,** a następnie pozycję **Więcej ustawień**wybierz pozycję Edytuj właściwości **programu Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b7397-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="b7397-120">Na stronie skrzynki pocztowej użytkownika wybierz \*\* funkcje skrzynki pocztowej \*\* po lewej stronie naw, a następnie wybierz łącze **Włącz** w obszarze **Wstrzymaj postępowanie sądowe**.</span><span class="sxs-lookup"><span data-stu-id="b7397-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="b7397-121">W oknie dialogowym **wstrzymanie sporu** można określić czas trwania blokady sporu w polu Czas **trwania blokady sporu.**</span><span class="sxs-lookup"><span data-stu-id="b7397-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="b7397-122">Pozostaw pole puste, jeśli chcesz umieścić nieskończone przytrzymanie.</span><span class="sxs-lookup"><span data-stu-id="b7397-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="b7397-123">Możesz również dodawać notatki i kierować właściciela skrzynki pocztowej do witryny sieci Web, którą może być trudniej wyjaśnić na temat blokady sporów.</span><span class="sxs-lookup"><span data-stu-id="b7397-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="b7397-124">\>**Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="b7397-124">\> **Save**.</span></span>
    
<span data-ttu-id="b7397-125">**Retencja:** Można włączyć dostosowane zasady przechowywania, na przykład, aby zachować przez określony czas lub trwale usunąć zawartość na koniec okresu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="b7397-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="b7397-126">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="b7397-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="b7397-127">Konfigurowanie etykiet czułości</span><span class="sxs-lookup"><span data-stu-id="b7397-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="b7397-128">Etykiety czułości są wyposażone w plan 1 usługi Azure Information Protection (AIP) i pomagają klasyfikować i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="b7397-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="b7397-129">Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, w której użytkownicy otrzymują rekomendacje.</span><span class="sxs-lookup"><span data-stu-id="b7397-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="b7397-130">Aby skonfigurować etykiety czułości, [wyświetlaj tworzenie i zarządzanie klipem wideo etykiet czułości.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="b7397-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="b7397-131">Ręczne instalowanie klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b7397-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="b7397-132">Aby ręcznie zainstalować klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="b7397-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="b7397-133">Pobierz **AzinfoProtection_UL.exe** z [Centrum pobierania firmy Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="b7397-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="b7397-134">Instalację można sprawdzić, czy instalacja działała, wyświetlając dokument programu Word i upewniając się, że opcja **Czułość** jest dostępna na karcie **Narzędzia główne.**</span><span class="sxs-lookup"><span data-stu-id="b7397-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="b7397-135">![Rozwijanie listy rozwijanej karty Ochrona w dokumencie programu Word.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="b7397-135">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="b7397-136">Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="b7397-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
