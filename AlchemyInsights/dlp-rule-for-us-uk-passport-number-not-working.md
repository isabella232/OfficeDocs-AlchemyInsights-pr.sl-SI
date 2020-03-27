---
title: Pravilo DLP za številko potnega lista ZDA/UK ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977122"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="ecb79-102">Težave s številkami potnih listov DLP-US/UK</span><span class="sxs-lookup"><span data-stu-id="ecb79-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="ecb79-103">**Pomembno**: med temi neprimerljivo časi, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo-Prosimo, obiščite [SharePoint online začasna prilagoditev funkcij](https://aka.ms/ODSPAdjustments) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="ecb79-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ecb79-104">**DLP vprašanja z ZDA/UK številke potnega lista**</span><span class="sxs-lookup"><span data-stu-id="ecb79-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="ecb79-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko potnega lista ZDA/UK** pri uporabi vrste občutljivih informacij DLP v O365?</span><span class="sxs-lookup"><span data-stu-id="ecb79-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ecb79-106">Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP, ko je ovrednoten.</span><span class="sxs-lookup"><span data-stu-id="ecb79-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="ecb79-107">Na primer, za pravilnik o **številki potnega lista ZDA/UK** , konfigurirani z ravnjo zaupanja 75%, se ocenijo in morajo biti odkrite za pravilo, ki sproži</span><span class="sxs-lookup"><span data-stu-id="ecb79-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="ecb79-108">**[Oblika zapisa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet števk</span><span class="sxs-lookup"><span data-stu-id="ecb79-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="ecb79-109">**[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet zaporednih števk</span><span class="sxs-lookup"><span data-stu-id="ecb79-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="ecb79-110">**[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="ecb79-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="ecb79-111">**[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="ecb79-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ecb79-112">Funkcija Func_usa_uk_passport poišče vsebino, ki se ujema z vzorcem.</span><span class="sxs-lookup"><span data-stu-id="ecb79-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ecb79-113">Najdena je ključna beseda iz Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="ecb79-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="ecb79-114">Na primer, naslednji vzorec bi sprožila za **ZDA/UK številka potnega lista** politike: us passport številka 123456789</span><span class="sxs-lookup"><span data-stu-id="ecb79-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="ecb79-115">Za več informacij o tem, kaj je potrebno za ZDA/UK številka potnega lista, ki se zazna za vašo vsebino, glejte naslednji razdelek v tem članku: [Kaj občutljive vrste informacij IŠČEJO ZDA/UK Passport številka](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="ecb79-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="ecb79-116">Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ecb79-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  