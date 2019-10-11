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
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i etykietach poufnych danych.
ms.openlocfilehash: a0ba2fa6dbe7c786d577ad7098c1790f569f5acc
ms.sourcegitcommit: 255e8194bb5767a9983d54d16e79d628732a1d97
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/11/2019
ms.locfileid: "37453926"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="c3bac-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="c3bac-103">Set up compliance features</span></span>

<span data-ttu-id="c3bac-104">Twoja firma Microsoft 365 Business zawiera funkcje chroniące dane i urządzenia oraz pomagające w zabezpieczeniu poufnych informacji Twoich i Twoich klientów.</span><span class="sxs-lookup"><span data-stu-id="c3bac-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="c3bac-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="c3bac-105">Set up DLP features</span></span>

<span data-ttu-id="c3bac-106">Zobacz [Tworzenie zasad DLP z szablonu](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) , aby zapoznać się z przykładem sposobu konfigurowania zasad w celu ochrony przed danymi osobowymi (PII).</span><span class="sxs-lookup"><span data-stu-id="c3bac-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="c3bac-107">DLP zawiera wiele gotowych do użycia szablonów zasad dla wielu różnych ustawień regionalnych.</span><span class="sxs-lookup"><span data-stu-id="c3bac-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="c3bac-108">Na przykład, Australia dane finansowe, Kanada informacje osobiste Act, dane finansowe USA, itp. Zobacz [, jakie szablony zasad DLP zawierają](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pełną listę.</span><span class="sxs-lookup"><span data-stu-id="c3bac-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="c3bac-109">Wszystkie te szablony można włączyć podobne do przykładu szablonu PII.</span><span class="sxs-lookup"><span data-stu-id="c3bac-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="c3bac-110">Konfigurowanie przechowywania poczty e-mail przy użyciu usługi Exchange Online archiwizacji</span><span class="sxs-lookup"><span data-stu-id="c3bac-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="c3bac-111">Funkcje **programu Exchange Online archiwizowanie** licencji ułatwiają zachowanie zgodności i standardów regulacyjnych przez zachowanie zawartości poczty elektronicznej na potrzeby zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="c3bac-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="c3bac-112">Pomaga również zmniejszyć ryzyko w przypadku pozew i umożliwia odzyskanie danych po naruszeniu zabezpieczeń lub gdy trzeba odzyskać usunięte elementy.</span><span class="sxs-lookup"><span data-stu-id="c3bac-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="c3bac-113">Aby zachować całą zawartość użytkownika lub użyć zasad przechowywania, aby dostosować to, co chcesz zachować, możesz użyć wstrzymania w postępowaniu sądowym.</span><span class="sxs-lookup"><span data-stu-id="c3bac-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="c3bac-114">**Sądowym:** Możesz zachować całą zawartość skrzynki pocztowej, w tym elementy usunięte, umieszczając całą skrzynkę pocztową użytkownika w postępowaniu sądowym.</span><span class="sxs-lookup"><span data-stu-id="c3bac-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="c3bac-115">Aby umieścić skrzynkę pocztową w postępowaniu sądowym, w centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="c3bac-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="c3bac-116">W lewym NAV przejdź do **użytkowników** \> **aktywnych**użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c3bac-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="c3bac-117">Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić na sądowym i w okienku użytkownika rozwiń **Ustawienia poczty** i obok **więcej ustawień** wybierz **Edytuj właściwości programu Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c3bac-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="c3bac-118">Na stronie skrzynki pocztowej dla użytkownika wybierz \* \* funkcje skrzynki pocztowej \* \* na lewej NAV, a następnie wybierz **Włącz** łącze w związku z **postępowaniem sądowym**.</span><span class="sxs-lookup"><span data-stu-id="c3bac-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="c3bac-119">W oknie dialogowym wstrzymanie w postępowaniu **sądowym** można określić czas trwania wstrzymania w trakcie postępowania sądowego w polu **czas trwania wstrzymania** , pozostawić pole puste, jeśli chcesz umieścić nieskończoną wstrzymania.</span><span class="sxs-lookup"><span data-stu-id="c3bac-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="c3bac-120">Można również dodawać notatki i kierować właścicielem skrzynki pocztowej do witryny sieci Web może być trzeba wyjaśnić więcej o sądowym wstrzymanie \> **zapisywania**.</span><span class="sxs-lookup"><span data-stu-id="c3bac-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="c3bac-121">**Zatrzymanie:** Można włączyć niestandardowe zasady przechowywania, na przykład, aby zachować określoną ilość czasu lub trwale usunąć zawartość na końcu okresu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="c3bac-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="c3bac-122">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="c3bac-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="c3bac-123">Ustawianie etykiet czułości</span><span class="sxs-lookup"><span data-stu-id="c3bac-123">Set up Sensitivity labels</span></span>

<span data-ttu-id="c3bac-124">Etykiety czułości są objęte planem 1 usługi Azure Information Protection (AIP) i ułatwiają klasyfikować i opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="c3bac-124">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="c3bac-125">Etykiety mogą być stosowane automatycznie przez administratorów, którzy definiują reguły i warunki, ręcznie przez użytkowników lub przy użyciu kombinacji, gdzie użytkownicy są podane zalecenia.</span><span class="sxs-lookup"><span data-stu-id="c3bac-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="c3bac-126">Aby skonfigurować etykiety czułości, zobacz [Tworzenie i zarządzanie etykietami czułości](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) wideo.</span><span class="sxs-lookup"><span data-stu-id="c3bac-126">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="c3bac-127">Ręczne instalowanie klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c3bac-127">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="c3bac-128">Aby ręcznie zainstalować klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="c3bac-128">To manually install the AIP client:</span></span>

1. <span data-ttu-id="c3bac-129">Pobierz **AzinfoProtection_UL. exe** z [Centrum pobierania Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="c3bac-129">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="c3bac-130">Można sprawdzić, czy instalacja zadziałało, przeglądając dokument programu Word i upewniając się, że opcja **czułość** jest dostępna na karcie **Narzędzia główne** .</span><span class="sxs-lookup"><span data-stu-id="c3bac-130">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="c3bac-131">![Karta ochrona listy rozwijanej w dokumencie programu Word.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="c3bac-131">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="c3bac-132">Aby uzyskać więcej informacji, zobacz [Instalowanie klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="c3bac-132">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
