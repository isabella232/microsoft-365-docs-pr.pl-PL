---
title: Zwiększanie ochrony przed zagrożeniami dla programu Microsoft 365 Business Premium
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
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i zapewnić bezpieczeństwo informacji poufnych przez klientów.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841178"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="e520a-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="e520a-103">Set up compliance features</span></span>

<span data-ttu-id="e520a-104">Program Microsoft 365 Business Premium zawiera funkcje chroniące dane i urządzenia, a ponadto ułatwia ochronę danych poufnych przez klientów.</span><span class="sxs-lookup"><span data-stu-id="e520a-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="e520a-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="e520a-105">Set up DLP features</span></span>

<span data-ttu-id="e520a-106">Zobacz [Tworzenie zasad DLP na podstawie szablonu](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) , aby zapoznać się z przykładem konfigurowania zasad w celu ochrony przed utratą danych osobowych.</span><span class="sxs-lookup"><span data-stu-id="e520a-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="e520a-107">W ramach DLP jest dostępnych wiele gotowych szablonów zasad dla wielu różnych ustawień regionalnych.</span><span class="sxs-lookup"><span data-stu-id="e520a-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="e520a-108">Na przykład dane finansowe Australii, stan danych osobowych w Kanadzie, dane finansowe USA itd.</span><span class="sxs-lookup"><span data-stu-id="e520a-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="e520a-109">Zobacz [, co zawiera szablon zasady DLP,](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) Aby uzyskać pełną listę.</span><span class="sxs-lookup"><span data-stu-id="e520a-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="e520a-110">Wszystkie te szablony można włączyć podobnie jak w przypadku szablonu dane OSOBowe.</span><span class="sxs-lookup"><span data-stu-id="e520a-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="e520a-111">Konfigurowanie przechowywania poczty e-mail przy użyciu aplikacji Exchange Online Archiwizuj</span><span class="sxs-lookup"><span data-stu-id="e520a-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="e520a-112">Funkcje licencji **usługi Exchange Online do archiwizacji** ułatwiają zachowanie zgodności i standardów normatywnych przez zachowywanie zawartości wiadomości E-mail dla zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="e520a-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="e520a-113">Pomaga to w ograniczeniu ryzyka, jeśli istnieje sprawność, a także umożliwia odzyskanie danych po naruszeniu zabezpieczeń lub w przypadku konieczności odzyskania elementów usuniętych.</span><span class="sxs-lookup"><span data-stu-id="e520a-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="e520a-114">W celu zachowania całej zawartości użytkownika lub użycia zasad przechowywania w celu dostosowania tego, co chcesz zachować, można użyć funkcji wstrzymania płatności sądowych.</span><span class="sxs-lookup"><span data-stu-id="e520a-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="e520a-115">**Przechowywanie sporów sądowych:** Całą zawartość skrzynki pocztowej, w tym usunięte elementy, można zachować, umieszczając całą skrzynkę pocztową użytkownika w ramach blokady sądowej.</span><span class="sxs-lookup"><span data-stu-id="e520a-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="e520a-116">Aby umieścić skrzynkę pocztową w ramach blokady sądowej, w centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="e520a-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="e520a-117">W lewym okienku nawigacji przejdź do obszaru **Użytkownicy** \> **aktywni** użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="e520a-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="e520a-118">Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić w ramach blokady sądowej.</span><span class="sxs-lookup"><span data-stu-id="e520a-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="e520a-119">W okienku użytkownika rozwiń pozycję **Ustawienia poczty** i obok pozycji **więcej ustawień** wybierz pozycję **Edytuj właściwości serwera Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e520a-119">In the user pane, expand **Mail settings** , and next to **More settings** , choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="e520a-120">Na stronie Skrzynka pocztowa użytkownika wybierz pozycję \* \* Funkcje skrzynki pocztowej \* \* w lewym obszarze nawigacyjnym, a następnie wybierz link **Włącz** w obszarze **powstrzymywania sporu**.</span><span class="sxs-lookup"><span data-stu-id="e520a-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="e520a-121">W oknie dialogowym **zawieszanie sporu** możesz określić czas trwania zadania sądowego w polu **czas trwania blokady sądowej** .</span><span class="sxs-lookup"><span data-stu-id="e520a-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="e520a-122">Pozostaw pole puste, jeśli chcesz zawiesić blokadę.</span><span class="sxs-lookup"><span data-stu-id="e520a-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="e520a-123">Możesz również dodać notatki i skierować właściciela skrzynki pocztowej do witryny sieci Web, aby dowiedzieć się więcej o zawieszeniu sporu.</span><span class="sxs-lookup"><span data-stu-id="e520a-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="e520a-124">\>**Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="e520a-124">\> **Save**.</span></span>
    
<span data-ttu-id="e520a-125">**Zachowanie:** Możesz włączyć niestandardowe zasady przechowywania, na przykład w celu zachowania określonej ilości czasu lub trwałego usunięcia zawartości na końcu okresu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="e520a-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="e520a-126">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="e520a-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="e520a-127">Konfigurowanie etykiet czułości</span><span class="sxs-lookup"><span data-stu-id="e520a-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="e520a-128">Etykiety wrażliwości są dostarczane z planem (dla Europy) usługi Azure Information Protection (dla Europy) i pomagają w klasyfikowaniu, a opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="e520a-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="e520a-129">Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, w której użytkownicy otrzymują rekomendacje.</span><span class="sxs-lookup"><span data-stu-id="e520a-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="e520a-130">Aby skonfigurować etykiety czułości, zobacz [Tworzenie i zarządzanie etykietami czułości](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .</span><span class="sxs-lookup"><span data-stu-id="e520a-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="e520a-131">Ręczne instalowanie klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="e520a-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="e520a-132">Aby ręcznie zainstalować klienta w instalacji:</span><span class="sxs-lookup"><span data-stu-id="e520a-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="e520a-133">Pobierz **AzinfoProtection_UL.exe** z [Centrum pobierania Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="e520a-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="e520a-134">Możesz sprawdzić, czy instalacja działała, wyświetlając dokument programu Word i upewniając się, że opcja **czułość** jest dostępna na karcie **Narzędzia główne** .</span><span class="sxs-lookup"><span data-stu-id="e520a-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="e520a-135">![Lista rozwijana karty Ochrona w dokumencie programu Word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="e520a-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="e520a-136">Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="e520a-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
