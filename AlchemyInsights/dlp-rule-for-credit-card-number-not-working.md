---
title: DLP pravilo za številko kreditne kartice, ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529971"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="755f5-102">DLP teme, številke kreditnih kartic</span><span class="sxs-lookup"><span data-stu-id="755f5-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="755f5-103">Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebino, ki vsebuje **Številko kreditne kartice** , pri uporabi vrsto DLP občutljive informacije v O365?</span><span class="sxs-lookup"><span data-stu-id="755f5-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="755f5-104">Če je tako, se prepričajte, vaše vsebine vsebuje potrebne informacije za sprožitev z DLP politike, ko je ovrednotena.</span><span class="sxs-lookup"><span data-stu-id="755f5-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="755f5-105">Na primer, za **politike kreditne kartice** konfiguriran z 85 % stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži:</span><span class="sxs-lookup"><span data-stu-id="755f5-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="755f5-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 števk, kar lahko oblikovano ali neoblikovano (dddddddddddddddd) in mora prestati preskus Luhn.</span><span class="sxs-lookup"><span data-stu-id="755f5-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="755f5-107">**[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zelo kompleksna in močna vzorec, ki zazna kartice iz vseh večjih blagovnih znamk po vsem svetu, vključno z Visa, MasterCard, odkriti kartico, JCB, American Express, darilne kartice in diner kartice.</span><span class="sxs-lookup"><span data-stu-id="755f5-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="755f5-108">**[Ček:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn ček</span><span class="sxs-lookup"><span data-stu-id="755f5-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="755f5-109">**[Opredelitev:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politiko je 85 % prepričan, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="755f5-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="755f5-110">Vsebina, ki ustreza vzorcu ugotovi, funkcijo Func_credit_card.</span><span class="sxs-lookup"><span data-stu-id="755f5-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="755f5-111">Je izpolnjen eden od naslednjih:</span><span class="sxs-lookup"><span data-stu-id="755f5-111">One of the following is true:</span></span>

  - <span data-ttu-id="755f5-112">Ključno besedo iz Keyword_cc_verification je našel.</span><span class="sxs-lookup"><span data-stu-id="755f5-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="755f5-113">Ključno besedo iz Keyword_cc_name je našel</span><span class="sxs-lookup"><span data-stu-id="755f5-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="755f5-114">Funkcijo Func_expiration_date ugotovi datum v pravi datumski obliki.</span><span class="sxs-lookup"><span data-stu-id="755f5-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="755f5-115">Ček prehaja</span><span class="sxs-lookup"><span data-stu-id="755f5-115">The checksum passes</span></span>

    <span data-ttu-id="755f5-116">Na primer, ta vzorec bi sproži za DLP kreditne kartice številko politike:</span><span class="sxs-lookup"><span data-stu-id="755f5-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="755f5-117">Vizum: 4485 3647 7352 3952</span><span class="sxs-lookup"><span data-stu-id="755f5-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="755f5-118">Poteče: 2/2009</span><span class="sxs-lookup"><span data-stu-id="755f5-118">Expires: 2/2009</span></span>

<span data-ttu-id="755f5-119">Več informacij o tem, kaj je potrebno za **Številko kreditne kartice** za vašo vsebino, je mogoče odkriti, glejte naslednji razdelek v tem članku: [Kaj je občutljive vrste informacij iščejo kreditne kartice #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="755f5-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="755f5-120">Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="755f5-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  