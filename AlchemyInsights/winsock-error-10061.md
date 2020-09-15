---
title: Napaka 1554 Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698878"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="2c348-102">Napaka Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="2c348-102">Winsock error 10061</span></span>

<span data-ttu-id="2c348-103">Ta koda napake pomeni, da Microsoft ni mogel vzpostaviti TCP vtičnice (povezave) s ciljnim gostiteljem.</span><span class="sxs-lookup"><span data-stu-id="2c348-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="2c348-104">Najverjetnejši vzrok te napake je težava pri konfiguraciji požarnega zidu.</span><span class="sxs-lookup"><span data-stu-id="2c348-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="2c348-105">Težavo odpravite tako, da preverite te nastavitve:</span><span class="sxs-lookup"><span data-stu-id="2c348-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="2c348-106">Preverjanje konfiguracije požarnega zidu s podatki v [URL-jih naslovov Microsoft 365 in obsegi naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2c348-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="2c348-107">Če je prišlo do napake v storitvi Exchange Online Protection (EOP), bi morali biti predhodno obveščeni na spremembo [naslovov IP za Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2c348-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="2c348-108">Preverite, ali vaš ponudnik internetnih storitev (ISP) ne blokira vrat.</span><span class="sxs-lookup"><span data-stu-id="2c348-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="2c348-109">Preverite nastavitve pametnega gostitelja in ciljnega strežnika v povezovalnikih.</span><span class="sxs-lookup"><span data-stu-id="2c348-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="2c348-110">Upoštevajte, da Microsoft 365 ne blokira *dohodnih* povezav na ta način.</span><span class="sxs-lookup"><span data-stu-id="2c348-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
