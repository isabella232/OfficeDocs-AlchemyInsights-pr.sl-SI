---
title: DLP pravilo za številko kreditne kartice ne deluje
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932459"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b2dbb-102">Težave z DLP s številkami kreditnih kartic</span><span class="sxs-lookup"><span data-stu-id="b2dbb-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="b2dbb-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b2dbb-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b2dbb-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b2dbb-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b2dbb-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b2dbb-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b2dbb-109">**Težave z DLP s številkami kreditnih kartic**</span><span class="sxs-lookup"><span data-stu-id="b2dbb-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="b2dbb-110">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko kreditne kartice** pri uporabi vrste občutljivih informacij DLP v O365?</span><span class="sxs-lookup"><span data-stu-id="b2dbb-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b2dbb-111">Če je tako, preverite, ali vsebina vsebuje potrebne informacije, da sproži pravilnik DLP, ko je ovrednoten.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b2dbb-112">Na primer, za **pravilnik o kreditni kartici** , konfigurirani z ravnjo zaupanja 85%, so ovrednotene naslednje in morajo biti odkrite za pravilo, ki sproži:</span><span class="sxs-lookup"><span data-stu-id="b2dbb-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b2dbb-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 številk, ki jih je mogoče formatirati ali neoblikovano (dddddddddddddddd) in mora opraviti test Luhn.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b2dbb-114">**[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zelo zapleten in robusten vzorec, ki zazna kartice iz vseh večjih blagovnih znamk po vsem svetu, vključno z Visa, MasterCard, Odkrijte Card, JCB, American Express, darilne kartice, in Diner kartice.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b2dbb-115">**[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, Luhn ček</span><span class="sxs-lookup"><span data-stu-id="b2dbb-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b2dbb-116">**[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="b2dbb-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b2dbb-117">Funkcija Func_credit_card poišče vsebino, ki se ujema z vzorcem.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b2dbb-118">Nekaj od tega je res:</span><span class="sxs-lookup"><span data-stu-id="b2dbb-118">One of the following is true:</span></span>

  - <span data-ttu-id="b2dbb-119">Najdena je ključna beseda iz Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b2dbb-120">Na voljo je ključna beseda iz Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="b2dbb-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b2dbb-121">Funkcija Func_expiration_date najde datum v pravem datumski obliki.</span><span class="sxs-lookup"><span data-stu-id="b2dbb-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b2dbb-122">Kontrolna vsota prehaja</span><span class="sxs-lookup"><span data-stu-id="b2dbb-122">The checksum passes</span></span>

    <span data-ttu-id="b2dbb-123">Naslednji vzorec bi na primer sprožil pravilnik o številki kreditne kartice DLP:</span><span class="sxs-lookup"><span data-stu-id="b2dbb-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b2dbb-124">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="b2dbb-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b2dbb-125">Poteče: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b2dbb-125">Expires: 2/2009</span></span>

<span data-ttu-id="b2dbb-126">Če želite več informacij o tem, kaj se zahteva za **številko kreditne kartice** , ki jo želite odkriti za vašo vsebino, glejte naslednji razdelek v tem članku: [katere vrste občutljivih informacij so na voljo za kreditno kartico #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b2dbb-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b2dbb-127">Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b2dbb-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  