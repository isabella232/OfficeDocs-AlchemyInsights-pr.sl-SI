---
title: 1554 Winsock napaka 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766185"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="127e8-102">Winsock napaka 10061</span><span class="sxs-lookup"><span data-stu-id="127e8-102">Winsock error 10061</span></span>

<span data-ttu-id="127e8-103">Ta koda napake pomeni, da Microsoft ni mogel vzpostaviti TCP vtičnice (povezave) s ciljnim gostiteljem.</span><span class="sxs-lookup"><span data-stu-id="127e8-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="127e8-104">Najverjetnejši vzrok za to napako je težava s konfiguracijo požarnega zidu.</span><span class="sxs-lookup"><span data-stu-id="127e8-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="127e8-105">Težavo odpravite tako, da preverite te nastavitve:</span><span class="sxs-lookup"><span data-stu-id="127e8-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="127e8-106">Preverite konfiguracijo požarnega zidu z informacijami v [Microsoft 365 URL-jev in obsegih IP naslovov](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="127e8-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="127e8-107">Če je napaka specifična za spletno zaščito Exchange Online (EOP), bi morali biti prej obveščeni o spremembi [naslovov IP za zaščito Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="127e8-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="127e8-108">Preverite, ali ponudnik internetnih storitev (ISP) ne blokira vrat.</span><span class="sxs-lookup"><span data-stu-id="127e8-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="127e8-109">Preverite nastavitve pametnega gostitelja in ciljnega strežnika v konektorjih.</span><span class="sxs-lookup"><span data-stu-id="127e8-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="127e8-110">Upoštevajte, da Microsoft 365 ne blokira *dohodnih* povezav na ta način.</span><span class="sxs-lookup"><span data-stu-id="127e8-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
