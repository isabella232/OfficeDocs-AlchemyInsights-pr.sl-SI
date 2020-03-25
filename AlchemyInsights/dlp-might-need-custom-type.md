---
title: DLP bo morda potreboval vrsto po meri
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932674"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="6fdfd-102">DLP bo morda potreboval vrsto po meri</span><span class="sxs-lookup"><span data-stu-id="6fdfd-102">DLP might need a custom type</span></span>

<span data-ttu-id="6fdfd-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6fdfd-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6fdfd-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6fdfd-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6fdfd-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6fdfd-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6fdfd-109">**DLP lahko zahteva vrsto informacij po meri**</span><span class="sxs-lookup"><span data-stu-id="6fdfd-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="6fdfd-110">S pravilnikom za preprečevanje izgub podatkov (DLP) lahko prepoznate in zaščitite občutljive podatke v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="6fdfd-111">V nekaterih primerih boste morda morali ustvariti lastne občutljive vrste podatkov **po meri** za zaščito podatkov organizacije.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="6fdfd-112">Vaša organizacija bo morda morala na primer identificirati in zaščititi ID-je zaposlenih ali druge podatke v neki obliki, ki je specifična za vašo org. Če je tako, si oglejte naslednje članke za več informacij.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="6fdfd-113">**Prilagajanje vgrajene občutljive vrste informacij**</span><span class="sxs-lookup"><span data-stu-id="6fdfd-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="6fdfd-114">Če bi vgrajena vrsta občutljivih informacij zadovoljila vaše potrebe s samo nekaj poteg, lahko [prilagodite vgrajeno vrsto občutljivih podatkov](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6fdfd-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="6fdfd-115">Dodajate ali odstranjujete lahko na primer ključne besede ali dodajate ali odstranjujete dokazila, kot sta datum ali naslov.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="6fdfd-116">**Ustvarjanje vrste občutljivih podatkov po meri**</span><span class="sxs-lookup"><span data-stu-id="6fdfd-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="6fdfd-117">Če pa morate v celoti prepoznati in zaščititi drugačno vrsto občutljivih informacij, lahko [ustvarite vrsto občutljive informacije po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) v uporabniškem vmesniku varnostnega & središča za skladnost.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="6fdfd-118">**Ustvarjanje občutljive vrste podatkov po meri v varnostnem & PowerShell center za skladnost**</span><span class="sxs-lookup"><span data-stu-id="6fdfd-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="6fdfd-119">Končno, če UI ne zagotavlja vseh možnosti, ki jih potrebujete, lahko [ustvarite po meri občutljive informacije vrsto v Security & skladnost center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6fdfd-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="6fdfd-120">Z začetkom z datoteko XML lahko uporabite vse razpoložljive možnosti.</span><span class="sxs-lookup"><span data-stu-id="6fdfd-120">By starting with an XML file, you can use every option available.</span></span>
