---
title: DLP pravilo za nas številka bančnega računa ne deluje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489598"
---
<span data-ttu-id="4e9ca-p101">Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebino, ki vsebuje **Številko bančnega računa ZDA** pri uporabi vrsto DLP občutljive informacije v O365? Če je tako, poskrbite, da vaša vsebina vsebuje potrebne informacije za kaj je politika DLP iščejo, ko je ovrednotena.</span><span class="sxs-lookup"><span data-stu-id="4e9ca-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="4e9ca-104">Na primer, za politike **ZDA številka bančnega računa** , konfiguriran s 85 % stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži:</span><span class="sxs-lookup"><span data-stu-id="4e9ca-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="4e9ca-105">**[Oblika:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 številk</span><span class="sxs-lookup"><span data-stu-id="4e9ca-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="4e9ca-106">**[Vzorec:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 zaporednih številk.</span><span class="sxs-lookup"><span data-stu-id="4e9ca-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="4e9ca-107">**[Ček:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni ne ček</span><span class="sxs-lookup"><span data-stu-id="4e9ca-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="4e9ca-108">**[Opredelitev:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika je 75 % prepričana, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="4e9ca-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="4e9ca-109">Regularni izraz Regex_usa_bank_account_number najde vsebine, ki se ujema z vzorcem</span><span class="sxs-lookup"><span data-stu-id="4e9ca-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="4e9ca-110">Ključno besedo iz Keyword_usa_Bank_Account je našel.</span><span class="sxs-lookup"><span data-stu-id="4e9ca-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="4e9ca-111">Na primer, ta vzorec bi sprožila politike **ZDA številka bančnega računa** : tekoči račun 78344011</span><span class="sxs-lookup"><span data-stu-id="4e9ca-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="4e9ca-112">Več informacij o tem, kaj je potrebno za **ZDA številka bančnega računa** za vašo vsebino, je mogoče odkriti, glejte naslednji razdelek v tem članku: [Kaj je občutljive vrste informacij poiščite ZDA številka bančnega računa](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="4e9ca-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="4e9ca-113">Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4e9ca-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

