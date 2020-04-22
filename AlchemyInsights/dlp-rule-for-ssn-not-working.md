---
title: Pravilo DLP za SSN ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704101"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="45883-102">Težave DLP s številkami socialnega zavarovanja</span><span class="sxs-lookup"><span data-stu-id="45883-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="45883-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="45883-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="45883-104">**DLP težave s SSNs**</span><span class="sxs-lookup"><span data-stu-id="45883-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="45883-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko socialnega zavarovanja (SSN)** pri uporabi občutljive vrste podatkov v Officeu 365?</span><span class="sxs-lookup"><span data-stu-id="45883-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="45883-106">Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP.</span><span class="sxs-lookup"><span data-stu-id="45883-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="45883-107">Na primer, za pravilnik SSN, konfiguriran z ravnjo zaupanja 85%, se ocenijo in morajo biti zaznani za pravilo, ki sproži:</span><span class="sxs-lookup"><span data-stu-id="45883-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="45883-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 števk, ki so lahko v formatiranem ali neoblikovanem vzorcu</span><span class="sxs-lookup"><span data-stu-id="45883-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="45883-109">**[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije iščejo SSNs v štirih različnih vzorcih:</span><span class="sxs-lookup"><span data-stu-id="45883-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="45883-110">Func_ssn najde SSNs s pre-2011 močno formatiranje, ki so oblikovane s črtice ali presledkov (DDD-DD-dddd ali DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="45883-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="45883-111">Func_unformatted_ssn najde SSNs s pre-2011 močno oblikovanje, ki so neoblikovane kot devet zaporednih števk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="45883-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="45883-112">Func_randomized_formatted_ssn najde post-2011 SSNs, ki so oblikovani s črtice ali presledkov (DDD-DD-dddd ali DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="45883-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="45883-113">Func_randomized_unformatted_ssn najde post-2011 SSNs, ki so neoblikovane kot devet zaporednih števk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="45883-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="45883-114">**[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="45883-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="45883-115">**[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="45883-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="45883-116">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) poišče vsebino, ki se ujema z vzorcem.</span><span class="sxs-lookup"><span data-stu-id="45883-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="45883-117">Najdena je ključna beseda iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="45883-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="45883-118">Primeri ključnih besed vključujejo: *socialna varnost, socialna varnost #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="45883-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="45883-119">Naslednji vzorec bi na primer sprožil pravilnik SSN za DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="45883-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="45883-120">Če želite več informacij o tem, kaj je potrebno za iskanje SSN-ja za vašo vsebino, glejte naslednji razdelek v tem članku: [kaj vrste občutljivih informacij iščejo SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="45883-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="45883-121">Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="45883-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  