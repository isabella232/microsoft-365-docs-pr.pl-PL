---
title: Zwiększanie ochrony przed zagrożeniami dla Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Skonfiguruj funkcje zgodności, aby zapobiec utracie danych i zapewnić bezpieczeństwo poufnych informacji Twoich i Twoich klientów.
ms.openlocfilehash: 945f8a283b90b89da2fbe67a073e0807b80d198f
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245089"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="7d88a-103">Konfigurowanie funkcji zgodności</span><span class="sxs-lookup"><span data-stu-id="7d88a-103">Set up compliance features</span></span>

<span data-ttu-id="7d88a-104">Twój Microsoft 365 Business Premium oferuje funkcje ochrony danych i urządzeń oraz pomaga zabezpieczyć poufne informacje Twoich i klientów.</span><span class="sxs-lookup"><span data-stu-id="7d88a-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="7d88a-105">Konfigurowanie funkcji DLP</span><span class="sxs-lookup"><span data-stu-id="7d88a-105">Set up DLP features</span></span>

<span data-ttu-id="7d88a-106">Zobacz [Tworzenie zasad DLP](../compliance/create-a-dlp-policy-from-a-template.md) na podstawie szablonu, aby uzyskać przykład sposobu skonfigurowania zasad w celu ochrony przed utratą danych osobowych.</span><span class="sxs-lookup"><span data-stu-id="7d88a-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="7d88a-107">Zasady DLP są dostępne z wieloma gotowymi do użycia szablonami zasad dla wielu różnych lokalizacji regionalnych.</span><span class="sxs-lookup"><span data-stu-id="7d88a-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="7d88a-108">Na przykład Australia Financial Data, Canada Personal Information Act, Us.S. Financial Data i tak dalej.</span><span class="sxs-lookup"><span data-stu-id="7d88a-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="7d88a-109">Zobacz [Co zawierają szablony zasad DLP,](../compliance/what-the-dlp-policy-templates-include.md) aby uzyskać pełną listę.</span><span class="sxs-lookup"><span data-stu-id="7d88a-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="7d88a-110">Wszystkie te szablony można włączyć podobnie jak w przykładzie szablonu piI.</span><span class="sxs-lookup"><span data-stu-id="7d88a-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="7d88a-111">Konfigurowanie przechowywania poczty e-mail przy użyciu Exchange Online — archiwum</span><span class="sxs-lookup"><span data-stu-id="7d88a-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="7d88a-112">**Exchange Online — archiwum** funkcji licencji pomagają w zachowaniu zgodności z normami i przepisami prawa, zachowując zawartość wiadomości e-mail na rzecz zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="7d88a-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="7d88a-113">Pomaga to również zmniejszyć ryzyko w przypadku wystąpienia do sądu i umożliwia odzyskanie danych po naruszeniu zabezpieczeń lub potrzebie odzyskania usuniętych elementów.</span><span class="sxs-lookup"><span data-stu-id="7d88a-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="7d88a-114">Aby zachować całą zawartość użytkownika, możesz użyć funkcji postępowania sądowego lub zasad przechowywania, aby dostosować to, co chcesz zachować.</span><span class="sxs-lookup"><span data-stu-id="7d88a-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="7d88a-115">**Zawieszenie w postępowaniem sądowym:** Całą zawartość skrzynki pocztowej, w tym elementy usunięte, można zachować, umieszczając całą skrzynkę pocztową użytkownika na postępowaniem sądowym.</span><span class="sxs-lookup"><span data-stu-id="7d88a-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="7d88a-116">Aby umieścić skrzynkę pocztową w związku z postępowaniem sądowym, w centrum administracyjnym:</span><span class="sxs-lookup"><span data-stu-id="7d88a-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="7d88a-117">W lewym okienku narracji przejdź do **strony** \> **Aktywni użytkownicy użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="7d88a-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="7d88a-118">Wybierz użytkownika, którego skrzynkę pocztową chcesz umieścić w postępowaniem sądowym.</span><span class="sxs-lookup"><span data-stu-id="7d88a-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="7d88a-119">W okienku użytkownika rozwiń **pozycję Ustawienia poczty**, a następnie obok **przycisku Więcej** ustawień wybierz pozycję Edytuj Exchange **właściwości**.</span><span class="sxs-lookup"><span data-stu-id="7d88a-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="7d88a-120">Na stronie skrzynki pocztowej dla użytkownika wybierz \*\* funkcje skrzynki pocztowej \*\* w lewym obszarze wyszukiwania, a następnie wybierz **link** Włącz w obszarze Zawieszenie w związku z **postępowaniem sądowym.**</span><span class="sxs-lookup"><span data-stu-id="7d88a-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="7d88a-121">W **oknie dialogowym Zawieszenie** w związku z postępowaniem sądowym w polu Czas trwania trwania w związku z postępowaniem sądowym możesz określić czas trwania trwania w związku z postępowaniem **sądowym.**</span><span class="sxs-lookup"><span data-stu-id="7d88a-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="7d88a-122">Pozostaw to pole puste, jeśli chcesz umieścić nieskończoną przestrzeń.</span><span class="sxs-lookup"><span data-stu-id="7d88a-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="7d88a-123">Możesz również dodawać notatki i kierować właściciela skrzynki pocztowej do witryny internetowej, w przypadku których może być konieczne dodatkowe wyjaśnienie dotyczące postępowania sądowego.</span><span class="sxs-lookup"><span data-stu-id="7d88a-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="7d88a-124">\>**Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="7d88a-124">\> **Save**.</span></span>
    
<span data-ttu-id="7d88a-125">**Przechowywanie:** Można włączyć niestandardowe zasady przechowywania, na przykład w celu zachowania określonego czasu lub trwałego usuwania zawartości na koniec okresu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="7d88a-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="7d88a-126">Aby dowiedzieć się więcej, zobacz [Omówienie zasad przechowywania.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="7d88a-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="7d88a-127">Konfigurowanie etykiet wrażliwości</span><span class="sxs-lookup"><span data-stu-id="7d88a-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="7d88a-128">Etykiety wrażliwości są dostępne w ramach usługi Azure Information Protection (AIP, Azure Information Protection) (plan 1) i pomagają klasyfikować oraz opcjonalnie chronić dokumenty i wiadomości e-mail, stosując etykiety.</span><span class="sxs-lookup"><span data-stu-id="7d88a-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="7d88a-129">Etykiety mogą być stosowane automatycznie przez administratorów definiujących reguły i warunki, ręcznie przez użytkowników lub za pomocą kombinacji, w której użytkownicy mają zalecenia.</span><span class="sxs-lookup"><span data-stu-id="7d88a-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="7d88a-130">Aby skonfigurować etykiety wrażliwości, wyświetl [klip wideo o tworzeniu etykiet wrażliwości i zarządzaniu nimi.](../business-video/create-sensitivity-labels.md)</span><span class="sxs-lookup"><span data-stu-id="7d88a-130">To set up Sensitivity labels, view [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="7d88a-131">Ręczne instalowanie klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7d88a-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="7d88a-132">Aby ręcznie zainstalować klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="7d88a-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="7d88a-133">Pobierz **AzinfoProtection_UL.exe** z [Centrum pobierania Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="7d88a-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="7d88a-134">Możesz sprawdzić, czy instalacja się działała, wyświetlając  dokument programu Word i upewnijąc się, że opcja Charakter jest dostępna na **karcie Narzędzia** główne.</span><span class="sxs-lookup"><span data-stu-id="7d88a-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="7d88a-135">![Lista rozwijana na karcie Ochrona w dokumencie programu Word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="7d88a-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="7d88a-136">Aby uzyskać więcej informacji, [zobacz Instalowanie klienta.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="7d88a-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>