---
title: Outbound relay pool
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381863"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="46ac8-102">Outbound relay pool</span><span class="sxs-lookup"><span data-stu-id="46ac8-102">Outbound relay pool</span></span>

<span data-ttu-id="46ac8-103">Microsoft bo konfiguracijo za posredovanje ali posredovanje e-pošte prek e-pošte Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="46ac8-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="46ac8-104">Sporočila v določenih scenarijih so posredovana ali posredovana prek Microsoft 365 uporabo posebne skupine posredovanja.</span><span class="sxs-lookup"><span data-stu-id="46ac8-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="46ac8-105">Sporočila, poslana s pomočjo skupine prejemnikov, so lahko v mapi z neželeno pošto prejemnika.</span><span class="sxs-lookup"><span data-stu-id="46ac8-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="46ac8-106">Če želite več informacij, glejte [Skupine odhodnih dostav](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="46ac8-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="46ac8-107">Če se želite izogniti scenariju z uporabo skupine posredovanje, se prepričajte, da posredovana/posredovana sporočila izpolnjujejo enega od teh pogojev:</span><span class="sxs-lookup"><span data-stu-id="46ac8-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="46ac8-108">Odhodni pošiljatelj je sprejeta domena najemnika.</span><span class="sxs-lookup"><span data-stu-id="46ac8-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="46ac8-109">Ogrodje SPF (Sender Policy Framework) se poda, ko je sporočilo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="46ac8-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="46ac8-110">DomainKeys Identified Mail (DKIM) v domeni pošiljatelja P2 poda sporočilo, ko se sporočilo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="46ac8-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="46ac8-111">Sporočila, ki ustrezajo zgornjim pogojem, niso posredovala prek skupine posredovanje.</span><span class="sxs-lookup"><span data-stu-id="46ac8-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="46ac8-112">Če je zapis MX za vašo domeno usmerjen v strežnik tretje osebe ali strežnik na mestu uporabe, uporabite izboljšano filtriranje in se prepričajte, da je preverjanje veljavnosti SPF pravilno za dohodno e-pošto in da preprečite pošiljanje e-pošte prek skupine posredovanje.</span><span class="sxs-lookup"><span data-stu-id="46ac8-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="46ac8-113">**Kako lahko vemo, ali je to vplivalo na nas v poolu za posredovanje?**</span><span class="sxs-lookup"><span data-stu-id="46ac8-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="46ac8-114">Če posredovana ali posredovana e-poštna sporočila uporabljajo enega od zgornjih pogojev, sporočila ne bodo posredovana prek skupine posredovanje.</span><span class="sxs-lookup"><span data-stu-id="46ac8-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="46ac8-115">Če pa je sporočilo poslano prek skupine posredovalnih strežnikov, je IP odhodnega strežnika v obsegu 40.95.0.0/16, ime odhodnega strežnika pa je v imenu vključuje **rly.**</span><span class="sxs-lookup"><span data-stu-id="46ac8-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

