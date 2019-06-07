---
title: 1065 Negodovanje EOP odhodne IP naslov rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752971"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="26c4d-102">Negodovanje EOP odhodne IP naslov razponi</span><span class="sxs-lookup"><span data-stu-id="26c4d-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="26c4d-103">Smo odkrili do morebitnega vprašanje z organizacijo, ki (če ni popravljen s oktober 26, 2018) morda prekinil tok pošte krajevne ali zunanjih ciljev.</span><span class="sxs-lookup"><span data-stu-id="26c4d-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="26c4d-104">Kot prej sporočiti, poenostaviti upravljanje IP naslov obsega, smo si utrditev Exchange Online varstvo (EOP) IP naslov območja, ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj Office 365.</span><span class="sxs-lookup"><span data-stu-id="26c4d-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="26c4d-105">Naše analize kažejo, da eden ali več zunanjih email virov ali ciljev, ki ste jih konfigurirali v poštni tok priključki niso sprejemanje povezav iz je IP naslov razponi prikazano [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="26c4d-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="26c4d-106">Delovala pred 26 oktobra za zagotovitev teh virov in destinacij bo sprejemanje povezav in iz vseh [objavljenih EOP IP naslove](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="26c4d-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="26c4d-107">Če želite več informacij o tej spremembi, si oglejte sporočilo Center delovnih mest, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="26c4d-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="26c4d-108">**Opomba**: Če ste prej uporabljali IP ali URL objavljanje preko HTML, XML in RSS za posodobitve končna točka, tudi naj preselite v novih spletnih storitev za avtomatizacijo tovrstnih posodobitve.</span><span class="sxs-lookup"><span data-stu-id="26c4d-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="26c4d-109">Če želite več informacij, glejte [Office 365 končne točke kategorije in Office 365 IP naslov in spletni naslov spletne storitve](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="26c4d-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
