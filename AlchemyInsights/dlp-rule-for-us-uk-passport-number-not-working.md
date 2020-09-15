---
title: Pravilo DLP za številko potnega lista US/UK ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679240"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="13424-102">Težave s številkami potnega lista za DLP – US/UK</span><span class="sxs-lookup"><span data-stu-id="13424-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="13424-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="13424-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="13424-104">**Težave z DLP s številkami potnega lista ZDA/UK**</span><span class="sxs-lookup"><span data-stu-id="13424-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="13424-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko potnega lista ZDA/UK** , ko uporabljate vrsto občutljivih podatkov DLP v O365?</span><span class="sxs-lookup"><span data-stu-id="13424-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="13424-106">Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije o tem, kaj išče pravilnik DLP, ko ga ocenite.</span><span class="sxs-lookup"><span data-stu-id="13424-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="13424-107">Na primer, za pravilnik **številka potnega lista ZDA/UK** , konfiguriran z ravnjo zaupanja 75%, je treba ovrednotiti te in jih je treba zaznati, da bo pravilo sprožilo</span><span class="sxs-lookup"><span data-stu-id="13424-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="13424-108">**[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet števk</span><span class="sxs-lookup"><span data-stu-id="13424-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="13424-109">**[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet zaporednih števk</span><span class="sxs-lookup"><span data-stu-id="13424-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="13424-110">**[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="13424-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="13424-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="13424-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="13424-112">Funkcija Func_usa_uk_passport najde vsebino, ki se ujema z vzorcem.</span><span class="sxs-lookup"><span data-stu-id="13424-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="13424-113">Najde se ključna beseda iz Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="13424-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="13424-114">Na primer, naslednji vzorec bi sprožilo za pravilnik **številka potnega lista ZDA/UK** : us Passportova številka 123456789</span><span class="sxs-lookup"><span data-stu-id="13424-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="13424-115">Če želite več informacij o tem, kaj je potrebno za številko Passporta ZDA/UK, ki jo želite zaznati za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste informacij za US/UK številka potnega lista](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="13424-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="13424-116">Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="13424-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  