---
title: DLP bo morda potreboval vrsto po meri
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704505"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="1f4d8-102">DLP bo morda potreboval vrsto po meri</span><span class="sxs-lookup"><span data-stu-id="1f4d8-102">DLP might need a custom type</span></span>

<span data-ttu-id="1f4d8-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="1f4d8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1f4d8-104">**DLP lahko zahteva vrsto informacij po meri**</span><span class="sxs-lookup"><span data-stu-id="1f4d8-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="1f4d8-105">S pravilnikom za preprečevanje izgub podatkov (DLP) lahko prepoznate in zaščitite občutljive podatke v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="1f4d8-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="1f4d8-106">V nekaterih primerih boste morda morali ustvariti lastne občutljive vrste podatkov **po meri** za zaščito podatkov organizacije.</span><span class="sxs-lookup"><span data-stu-id="1f4d8-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="1f4d8-107">Vaša organizacija bo morda morala na primer identificirati in zaščititi ID-je zaposlenih ali druge podatke v neki obliki, ki je specifična za vašo org. Če je tako, si oglejte naslednje članke za več informacij.</span><span class="sxs-lookup"><span data-stu-id="1f4d8-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="1f4d8-108">**Prilagajanje vgrajene občutljive vrste informacij**</span><span class="sxs-lookup"><span data-stu-id="1f4d8-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="1f4d8-109">Če bi vgrajena vrsta občutljivih informacij zadovoljila vaše potrebe s samo nekaj poteg, lahko [prilagodite vgrajeno vrsto občutljivih podatkov](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1f4d8-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="1f4d8-110">Dodajate ali odstranjujete lahko na primer ključne besede ali dodajate ali odstranjujete dokazila, kot sta datum ali naslov.</span><span class="sxs-lookup"><span data-stu-id="1f4d8-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="1f4d8-111">**Ustvarjanje vrste občutljivih podatkov po meri**</span><span class="sxs-lookup"><span data-stu-id="1f4d8-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="1f4d8-112">Če pa morate v celoti prepoznati in zaščititi drugačno vrsto občutljivih informacij, lahko [ustvarite vrsto občutljive informacije po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) v uporabniškem vmesniku varnostnega & središča za skladnost.</span><span class="sxs-lookup"><span data-stu-id="1f4d8-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="1f4d8-113">**Ustvarjanje občutljive vrste podatkov po meri v varnostnem & PowerShell center za skladnost**</span><span class="sxs-lookup"><span data-stu-id="1f4d8-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="1f4d8-114">Končno, če UI ne zagotavlja vseh možnosti, ki jih potrebujete, lahko [ustvarite po meri občutljive informacije vrsto v Security & skladnost center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1f4d8-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="1f4d8-115">Z začetkom z datoteko XML lahko uporabite vse razpoložljive možnosti.</span><span class="sxs-lookup"><span data-stu-id="1f4d8-115">By starting with an XML file, you can use every option available.</span></span>
