---
title: DLP pravilo za ZDA / UK številka potnega lista, ne deluje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28313134"
---
<span data-ttu-id="62c1f-p101">Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebine, ki vsebuje a **ZDA / UK številka potnega lista** čas using DLP tip zelo občutljliv sporočilo v O365? Če je tako, poskrbite, da vaša vsebina vsebuje potrebne informacije za kaj je politika DLP iščejo, ko je ovrednotena.</span><span class="sxs-lookup"><span data-stu-id="62c1f-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="62c1f-104">Na primer na **US / UK številka potnega lista** pravilnik, konfiguriran s 75 odstotno stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži</span><span class="sxs-lookup"><span data-stu-id="62c1f-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="62c1f-105">**[Oblika:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet števk</span><span class="sxs-lookup"><span data-stu-id="62c1f-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="62c1f-106">**[Vzorec:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet zaporednih številk</span><span class="sxs-lookup"><span data-stu-id="62c1f-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="62c1f-107">**[Ček:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni ne ček</span><span class="sxs-lookup"><span data-stu-id="62c1f-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="62c1f-108">**[Opredelitev:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika je 75 % prepričana, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="62c1f-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="62c1f-109">Vsebina, ki ustreza vzorcu ugotovi, funkcijo Func_usa_uk_passport.</span><span class="sxs-lookup"><span data-stu-id="62c1f-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="62c1f-110">Ključno besedo iz Keyword_passport je našel.</span><span class="sxs-lookup"><span data-stu-id="62c1f-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="62c1f-111">Na primer, bi ta vzorec sproži za v **ZDA / UK številka potnega lista** politike: številka potnega lista ZDA 123456789</span><span class="sxs-lookup"><span data-stu-id="62c1f-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="62c1f-112">Za več informacij o tem, kaj je potrebno za ZDA / UK številka potnega lista z zazna za vašo vsebino, glejte razdelek naslednje v tem članku: [Kaj je občutljive vrste informacij iščejo ZDA / UK številka potnega lista](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="62c1f-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="62c1f-113">Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="62c1f-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

