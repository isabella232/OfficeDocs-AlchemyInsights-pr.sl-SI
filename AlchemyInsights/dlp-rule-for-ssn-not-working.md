---
title: Pravilo DLP za SSN ne deluje
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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932551"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="500b2-102">Težave DLP s številkami socialnega zavarovanja</span><span class="sxs-lookup"><span data-stu-id="500b2-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="500b2-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="500b2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="500b2-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="500b2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="500b2-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="500b2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="500b2-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="500b2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="500b2-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="500b2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="500b2-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="500b2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="500b2-109">**DLP težave s SSNs**</span><span class="sxs-lookup"><span data-stu-id="500b2-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="500b2-110">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko socialnega zavarovanja (SSN)** pri uporabi občutljive vrste podatkov v Officeu 365?</span><span class="sxs-lookup"><span data-stu-id="500b2-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="500b2-111">Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP.</span><span class="sxs-lookup"><span data-stu-id="500b2-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="500b2-112">Na primer, za pravilnik SSN, konfiguriran z ravnjo zaupanja 85%, se ocenijo in morajo biti zaznani za pravilo, ki sproži:</span><span class="sxs-lookup"><span data-stu-id="500b2-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="500b2-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 števk, ki so lahko v formatiranem ali neoblikovanem vzorcu</span><span class="sxs-lookup"><span data-stu-id="500b2-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="500b2-114">**[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije iščejo SSNs v štirih različnih vzorcih:</span><span class="sxs-lookup"><span data-stu-id="500b2-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="500b2-115">Func_ssn najde SSNs s pre-2011 močno formatiranje, ki so oblikovane s črtice ali presledkov (DDD-DD-dddd ali DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="500b2-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="500b2-116">Func_unformatted_ssn najde SSNs s pre-2011 močno oblikovanje, ki so neoblikovane kot devet zaporednih števk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="500b2-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="500b2-117">Func_randomized_formatted_ssn najde post-2011 SSNs, ki so oblikovani s črtice ali presledkov (DDD-DD-dddd ali DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="500b2-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="500b2-118">Func_randomized_unformatted_ssn najde post-2011 SSNs, ki so neoblikovane kot devet zaporednih števk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="500b2-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="500b2-119">**[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="500b2-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="500b2-120">**[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="500b2-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="500b2-121">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) poišče vsebino, ki se ujema z vzorcem.</span><span class="sxs-lookup"><span data-stu-id="500b2-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="500b2-122">Najdena je ključna beseda iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="500b2-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="500b2-123">Primeri ključnih besed vključujejo: *socialna varnost, socialna varnost #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="500b2-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="500b2-124">Naslednji vzorec bi na primer sprožil pravilnik SSN za DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="500b2-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="500b2-125">Če želite več informacij o tem, kaj je potrebno za iskanje SSN-ja za vašo vsebino, glejte naslednji razdelek v tem članku: [kaj vrste občutljivih informacij iščejo SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="500b2-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="500b2-126">Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="500b2-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  