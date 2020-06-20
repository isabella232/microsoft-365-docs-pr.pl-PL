---
title: Zwiększenie ochrony przed zagrożeniami dla usługi Microsoft 365 Business Premium
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i zapewnić bezpieczeństwo poufnych informacji twoich i klientów.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785837"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="13e15-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="13e15-103">Set up compliance features</span></span>

<span data-ttu-id="13e15-104">Usługa Microsoft 365 Business Premium jest wyposażona w funkcje ochrony danych i urządzeń oraz pomagają chronić poufne informacje użytkownika i klientów.</span><span class="sxs-lookup"><span data-stu-id="13e15-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="13e15-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="13e15-105">Set up DLP features</span></span>

<span data-ttu-id="13e15-106">Zobacz [Tworzenie zasad DLP na podstawie szablonu,](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) aby uzyskać przykład na temat konfigurowania zasad w celu ochrony przed danymi umożliwiającymi identyfikację użytkownika.</span><span class="sxs-lookup"><span data-stu-id="13e15-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="13e15-107">DLP jest wyposażony w wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych.</span><span class="sxs-lookup"><span data-stu-id="13e15-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="13e15-108">Na przykład Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, itd.</span><span class="sxs-lookup"><span data-stu-id="13e15-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="13e15-109">Zobacz, [co zawierają szablony zasad DLP,](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) aby uzyskać pełną listę.</span><span class="sxs-lookup"><span data-stu-id="13e15-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="13e15-110">Wszystkie te szablony można włączyć podobnie jak przykład szablonu pii.</span><span class="sxs-lookup"><span data-stu-id="13e15-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="13e15-111">Konfigurowanie przechowywania poczty e-mail za pomocą archiwizacji usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="13e15-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="13e15-112">Funkcje licencji **Exchange Online Archiving** pomagają utrzymać zgodność i standardy regulacyjne, zachowując zawartość wiadomości e-mail do elektronicznego zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="13e15-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="13e15-113">Pomaga również zmniejszyć ryzyko, jeśli istnieje pozew, i zapewnia sposób odzyskiwania danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy.</span><span class="sxs-lookup"><span data-stu-id="13e15-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="13e15-114">Za pomocą blokady postępowania sądowego można zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować.</span><span class="sxs-lookup"><span data-stu-id="13e15-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="13e15-115">**Wstrzymanie postępowania sądowego:** Można zachować całą zawartość skrzynki pocztowej, w tym usunięte elementy, umieszczając całą skrzynkę pocztową użytkownika w zawieszeniu w postępowaniu sądowym.</span><span class="sxs-lookup"><span data-stu-id="13e15-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="13e15-116">Aby zawiesić skrzynkę pocztową w postępowaniu sądowym, w Centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="13e15-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="13e15-117">W lewej stronie nawigacyjnej przejdź do **strony Użytkownicy** \> **aktywni użytkownicy**.</span><span class="sxs-lookup"><span data-stu-id="13e15-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="13e15-118">Wybierz użytkownika, którego skrzynkę pocztową chcesz zawiesić w postępowaniu sądowym.</span><span class="sxs-lookup"><span data-stu-id="13e15-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="13e15-119">W okienku użytkownika rozwiń pozycję **Ustawienia poczty**, a obok pozycji **Więcej ustawień**wybierz pozycję Edytuj właściwości **programu Exchange**.</span><span class="sxs-lookup"><span data-stu-id="13e15-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="13e15-120">Na stronie skrzynki pocztowej dla użytkownika wybierz \*\* funkcje skrzynki pocztowej \*\* na lewym polu nawigacyjnym, a następnie wybierz **łącze Włącz** w obszarze **Wstrzymanie postępowania sądowego**.</span><span class="sxs-lookup"><span data-stu-id="13e15-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="13e15-121">W oknie dialogowym **wstrzymanie postępowania sądowego** można określić czas trwania wstrzymania postępowania sądowego w polu **Czas trwania wstrzymania postępowania sądowego.**</span><span class="sxs-lookup"><span data-stu-id="13e15-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="13e15-122">Pozostaw pole puste, jeśli chcesz umieścić nieskończone przytrzymanie.</span><span class="sxs-lookup"><span data-stu-id="13e15-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="13e15-123">Możesz również dodać notatki i skierować właściciela skrzynki pocztowej do witryny sieci Web, która może być bardziej wyjaśniona na temat wstrzymania postępowania sądowego.</span><span class="sxs-lookup"><span data-stu-id="13e15-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="13e15-124">\>**Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="13e15-124">\> **Save**.</span></span>
    
<span data-ttu-id="13e15-125">**Retencja:** Można włączyć dostosowane zasady przechowywania, na przykład, aby zachować przez określony czas lub usunąć zawartość trwale na koniec okresu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="13e15-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="13e15-126">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="13e15-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="13e15-127">Konfigurowanie etykiet czułości</span><span class="sxs-lookup"><span data-stu-id="13e15-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="13e15-128">Etykiety czułości są wyposażone w plan 1 usługi Azure Information Protection (AIP) i ułatwiają klasyfikowanie i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="13e15-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="13e15-129">Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki ręcznie przez użytkowników lub przy użyciu kombinacji, w której użytkownicy otrzymują rekomendacje.</span><span class="sxs-lookup"><span data-stu-id="13e15-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="13e15-130">Aby skonfigurować etykiety czułości, wyświetl [wideo tworzenie etykiet czułości i zarządzanie nimi.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="13e15-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="13e15-131">Ręczne instalowanie klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="13e15-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="13e15-132">Aby ręcznie zainstalować klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="13e15-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="13e15-133">Pobierz **AzinfoProtection_UL.exe** z [centrum pobierania Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="13e15-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="13e15-134">Można sprawdzić, czy instalacja zadziałała, przeglądając dokument programu Word i upewniając się, że opcja **Czułość** jest dostępna na karcie **Narzędzia** główne.</span><span class="sxs-lookup"><span data-stu-id="13e15-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="13e15-135">![Karta Ochrony rozwijana w dokumencie programu Word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="13e15-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="13e15-136">Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="13e15-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
