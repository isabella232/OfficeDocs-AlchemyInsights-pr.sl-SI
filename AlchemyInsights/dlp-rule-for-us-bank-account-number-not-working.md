---
title: Pravilo DLP za številko bančnega računa ZDA ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704055"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="d92f5-102">DLP težave z ameriški bančnega računa številke</span><span class="sxs-lookup"><span data-stu-id="d92f5-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="d92f5-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d92f5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d92f5-104">**DLP težave z ameriški bančnega računa številke**</span><span class="sxs-lookup"><span data-stu-id="d92f5-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="d92f5-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko bančnega računa ZDA** pri uporabi vrste občutljivih informacij DLP v O365?</span><span class="sxs-lookup"><span data-stu-id="d92f5-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d92f5-106">Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP, ko je ovrednoten.</span><span class="sxs-lookup"><span data-stu-id="d92f5-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d92f5-107">Na primer, za pravilnik o **številki ameriškega bančnega računa** , ki je konfiguriran z ravnjo zaupanja 85%, se ocenijo naslednje in morajo biti odkrite za pravilo, ki sproži:</span><span class="sxs-lookup"><span data-stu-id="d92f5-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d92f5-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 števk</span><span class="sxs-lookup"><span data-stu-id="d92f5-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="d92f5-109">**[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 zaporednih števk.</span><span class="sxs-lookup"><span data-stu-id="d92f5-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="d92f5-110">**[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="d92f5-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d92f5-111">**[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="d92f5-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d92f5-112">Regularni izraz Regex_usa_bank_account_number najde vsebino, ki se ujema z vzorcem</span><span class="sxs-lookup"><span data-stu-id="d92f5-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="d92f5-113">Najdena je ključna beseda iz Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="d92f5-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="d92f5-114">Naslednji vzorec bi na primer sprožil pravilnik o **številki bančnega računa ZDA** : preverjanje računa 78344011</span><span class="sxs-lookup"><span data-stu-id="d92f5-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="d92f5-115">Če želite več informacij o tem, kaj je potrebno za iskanje **številke ameriškega bančnega računa** za vašo vsebino, glejte naslednji razdelek v tem članku: [katere vrste občutljivih informacij so na voljo za ŠTEVILKO bančnega računa ZDA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="d92f5-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="d92f5-116">Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d92f5-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  