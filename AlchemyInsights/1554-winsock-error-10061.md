---
title: Napaka Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903128"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="25167-102">Napaka Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="25167-102">Winsock error 10061</span></span>

<span data-ttu-id="25167-p101">Pomeni ta koda napake, da Office 365 ni mogel vzpostaviti vtičnico TCP (povezava) s ciljnega gostitelja. Najverjetnejši vzrok te napake je problem s konfiguracijo požarnega zidu. Težavo, preverite te nastavitve:</span><span class="sxs-lookup"><span data-stu-id="25167-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="25167-106">Preverite konfiguracijo požarnega zidu z informacijami v [Office 365 URL in IP naslov razponi](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="25167-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="25167-107">Če napaka je specifična za Exchange Online varstvo (EOP), si mora prej vročenega spremembo v [Exchange Online zaščite IP naslove](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="25167-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="25167-108">Preverite, da vaš Internet storitev ponudnik (ISP) ni blokira vrata.</span><span class="sxs-lookup"><span data-stu-id="25167-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="25167-109">Preverjanje pametnih in gostiteljskim ter ciljnim nastavitve strežnika v vaš priključki.</span><span class="sxs-lookup"><span data-stu-id="25167-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="25167-110">Upoštevajte, da Office 365 ne blokira *dohodne* povezave na ta način.</span><span class="sxs-lookup"><span data-stu-id="25167-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

