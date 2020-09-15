---
title: DLP morda potrebuje vrsto po meri
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712200"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2c9be-102">DLP morda potrebuje vrsto po meri</span><span class="sxs-lookup"><span data-stu-id="2c9be-102">DLP might need a custom type</span></span>

<span data-ttu-id="2c9be-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="2c9be-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2c9be-104">**DLP lahko zahteva vrsto podatkov po meri**</span><span class="sxs-lookup"><span data-stu-id="2c9be-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2c9be-105">S pravilnikom za preprečevanje izgube podatkov (DLP) lahko prepoznate in zaščitite občutljive podatke v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="2c9be-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2c9be-106">V nekaterih primerih boste morda morali ustvariti vrsto občutljivih podatkov **po meri** , da zaščitite podatke organizacije.</span><span class="sxs-lookup"><span data-stu-id="2c9be-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2c9be-107">Vaša organizacija bo morda morala na primer identificirati in varovati ID-je zaposlenih ali druge podatke v neki obliki zapisa, ki je značilna za vaše org. Če je tako, si oglejte te članke za več informacij.</span><span class="sxs-lookup"><span data-stu-id="2c9be-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2c9be-108">**Prilagajanje vgrajene občutljive vrste podatkov**</span><span class="sxs-lookup"><span data-stu-id="2c9be-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2c9be-109">Če bi vgrajena vrsta občutljivega podatka zadovoljila vaše potrebe s samo nekaj potegi, lahko [prilagodite vrsto občutljivega podatka](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2c9be-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2c9be-110">Dodate ali odstranite lahko na primer ključne besede ali pa dodate ali odstranite podporne dokaze, kot je datum ali naslov.</span><span class="sxs-lookup"><span data-stu-id="2c9be-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2c9be-111">**Ustvarjanje vrste občutljivih podatkov po meri**</span><span class="sxs-lookup"><span data-stu-id="2c9be-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2c9be-112">Če pa želite v celoti prepoznati in zaščititi drugačno vrsto občutljivih informacij, lahko [ustvarite vrsto občutljivih podatkov po meri](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) v uporabniškem vmesniku središča za skladnost varnostnega &.</span><span class="sxs-lookup"><span data-stu-id="2c9be-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2c9be-113">**Ustvarjanje vrste občutljivih podatkov po meri v središču za varnost & skladnost z ogrodjem PowerShell**</span><span class="sxs-lookup"><span data-stu-id="2c9be-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2c9be-114">Če uporabniški vmesnik ne ponudi vseh možnosti, ki jih potrebujete, lahko [ustvarite vrsto občutljivih podatkov po meri v središču za varnost & skladnost s predpisi](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2c9be-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2c9be-115">Ko začnete uporabljati datoteko XML, lahko uporabite vse možnosti, ki so na voljo.</span><span class="sxs-lookup"><span data-stu-id="2c9be-115">By starting with an XML file, you can use every option available.</span></span>
