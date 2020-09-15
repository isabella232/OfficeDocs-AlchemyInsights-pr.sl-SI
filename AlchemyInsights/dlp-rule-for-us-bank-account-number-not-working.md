---
title: Pravilo DLP za številko AMERIŠKEGA bančnega računa ne deluje
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679312"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="cf66f-102">Težave z DLP s številkami AMERIŠKEGA bančnega računa</span><span class="sxs-lookup"><span data-stu-id="cf66f-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="cf66f-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="cf66f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="cf66f-104">**Težave z DLP s številkami AMERIŠKEGA bančnega računa**</span><span class="sxs-lookup"><span data-stu-id="cf66f-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="cf66f-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko ameriškega bančnega računa** , ko uporabljate vrsto občutljivih podatkov DLP v O365?</span><span class="sxs-lookup"><span data-stu-id="cf66f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="cf66f-106">Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije o tem, kaj išče pravilnik DLP, ko ga ocenite.</span><span class="sxs-lookup"><span data-stu-id="cf66f-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="cf66f-107">Na primer, za pravilnik **številka ameriškega bančnega računa** , konfiguriran z ravnjo zaupanja 85%, se ocenijo in jih je treba zaznati, da sproži pravilo:</span><span class="sxs-lookup"><span data-stu-id="cf66f-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="cf66f-108">**[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 števk</span><span class="sxs-lookup"><span data-stu-id="cf66f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="cf66f-109">**[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 zaporednih števk.</span><span class="sxs-lookup"><span data-stu-id="cf66f-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="cf66f-110">**[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="cf66f-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="cf66f-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="cf66f-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="cf66f-112">Regularni izraz Regex_usa_bank_account_number najde vsebino, ki se ujema z vzorcem</span><span class="sxs-lookup"><span data-stu-id="cf66f-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="cf66f-113">Najde se ključna beseda iz Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="cf66f-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="cf66f-114">Na primer, naslednji vzorec bi sprožilo za pravilnik o **številu bančnih računov v ZDA** : preverjanje računa 78344011</span><span class="sxs-lookup"><span data-stu-id="cf66f-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="cf66f-115">Če želite več informacij o tem, kaj je potrebno za **številko bančnega računa v ZDA** , ki jo želite zaznati za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste informacij za ameriško številko bančnega računa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="cf66f-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="cf66f-116">Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="cf66f-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  