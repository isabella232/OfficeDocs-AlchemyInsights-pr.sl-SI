---
title: DLP pravilo za SSN, ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529886"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d1de4-102">DLP vprašanja s številke socialnega zavarovanja</span><span class="sxs-lookup"><span data-stu-id="d1de4-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d1de4-103">Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebino, ki vsebuje **Številko socialnega zavarovanja (SSN)** , pri uporabi vrsto občutljivih podatkov v Office 365?</span><span class="sxs-lookup"><span data-stu-id="d1de4-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="d1de4-104">Če je tako, preverite, ali vaša vsebina vsebuje potrebne informacije za DLP politike, kaj išče.</span><span class="sxs-lookup"><span data-stu-id="d1de4-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d1de4-105">Na primer, za SSN pravilnik, konfiguriran s 85 % stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži:</span><span class="sxs-lookup"><span data-stu-id="d1de4-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d1de4-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 številk, ki so lahko v vzorec oblikovano ali Neoblikovano</span><span class="sxs-lookup"><span data-stu-id="d1de4-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d1de4-107">**[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije iskati SSNs v štirih različnih vzorcev:</span><span class="sxs-lookup"><span data-stu-id="d1de4-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d1de4-108">Func_ssn najde SSNs s pre-2011 močno oblikovanja, ki so oblikovani s črticami ali prostorov (ddd-dd-dddd ali ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d1de4-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d1de4-109">Func_unformatted_ssn najde SSNs s pre-2011 močno oblikovanja, ki so neoblikovano kot devet zaporednih številk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d1de4-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d1de4-110">Func_randomized_formatted_ssn najde post-2011 SSNs, ki so oblikovani s črticami ali prostorov (ddd-dd-dddd ali ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d1de4-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d1de4-111">Func_randomized_unformatted_ssn najde post-2011 SSNs, ki so neoblikovano kot devet zaporednih številk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d1de4-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d1de4-112">**[Ček:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, ni ne ček</span><span class="sxs-lookup"><span data-stu-id="d1de4-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d1de4-113">**[Opredelitev:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politiko je 85 % prepričan, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="d1de4-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d1de4-114">Vsebina, ki ustreza vzorcu ugotovi, [funkcijo Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) .</span><span class="sxs-lookup"><span data-stu-id="d1de4-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d1de4-115">Ključno besedo iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) je našel.</span><span class="sxs-lookup"><span data-stu-id="d1de4-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="d1de4-116">Primeri ključnih besed vključuje: *socialna varnost, socialno varnost #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="d1de4-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d1de4-117">Na primer, bi ta vzorec sproži za DLP SSN politike: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d1de4-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d1de4-118">Več informacij o tem, kaj je potrebno za SSNs treba odkriti za vašo vsebino, glejte naslednji razdelek v tem članku: [Kaj je občutljive vrste informacij iščejo SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d1de4-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d1de4-119">Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d1de4-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  