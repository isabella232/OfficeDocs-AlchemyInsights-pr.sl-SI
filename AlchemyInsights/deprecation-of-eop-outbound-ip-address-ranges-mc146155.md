---
title: 1065 zastaranje EOP odhodnega IP naslova rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806811"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="c941f-102">Zastaranje EOP odhodnih naslovov IP</span><span class="sxs-lookup"><span data-stu-id="c941f-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="c941f-103">Zaznali smo potencialno težavo z vašo organizacijo, ki (če ni popravljena do oktobra 26. oktober 2018), lahko prelom pošte prekine s storitvijo na mestu uporabe ali zunanjimi cilji.</span><span class="sxs-lookup"><span data-stu-id="c941f-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="c941f-104">Kot je bilo predhodno sporočeno, da poenostavite upravljanje obsega naslovov IP, združujemo obsege naslovov IP za Exchange Online (EOP), ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj programa Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c941f-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="c941f-105">Naša analiza kaže, da je eden ali več zunanjih virov e-pošte ali ciljev, ki ste jih konfigurirali v povezovalnikih toka pošte, ne sprejema povezav z [prikazanih](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)obsegov naslovov IP.</span><span class="sxs-lookup"><span data-stu-id="c941f-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c941f-106">Ukrepajte pred oktobrom 26, da zagotovite, da bodo ti viri in cilji sprejeli povezave do vseh [objavljenih EOP naslovov IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)in iz njih.</span><span class="sxs-lookup"><span data-stu-id="c941f-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c941f-107">Če želite več informacij o tej spremembi, glejte sporočila središča za pošto [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="c941f-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="c941f-108">**Opomba**: Če ste že uporabljali IP ali URL za objavljanje prek storitev HTML, XML in RSS za končne točke, morate preseliti tudi v nove spletne storitve za avtomatizacijo teh vrst posodobitev.</span><span class="sxs-lookup"><span data-stu-id="c941f-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="c941f-109">Če želite več informacij, glejte [kategorije končnih točk za microsoft 365 in microsoft 365 naslov IP ter spletna storitev URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="c941f-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
