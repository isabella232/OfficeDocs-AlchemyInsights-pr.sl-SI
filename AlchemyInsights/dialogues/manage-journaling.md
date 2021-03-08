---
title: Upravljanje dnevnika
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526146"
---
# <a name="manage-journaling"></a><span data-ttu-id="512ad-102">Upravljanje dnevnika</span><span class="sxs-lookup"><span data-stu-id="512ad-102">Manage journaling</span></span>

<span data-ttu-id="512ad-103">Journaling omogoča, da se vaša organizacija odzove na zahteve za pravno, regulativno in organizacijsko skladnost s snemanjem dohodnih in odhodnih e-poštnih sporočil.</span><span class="sxs-lookup"><span data-stu-id="512ad-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="512ad-104">Imejte v mislih:</span><span class="sxs-lookup"><span data-stu-id="512ad-104">Keep in mind:</span></span>

* <span data-ttu-id="512ad-105">Preden lahko upravljate dnevnike, morate imeti dovoljenja za upravljanje [organizacije](https://go.microsoft.com/fwlink/?linkid=2115259) in [zapise](https://go.microsoft.com/fwlink/?linkid=2115469) .</span><span class="sxs-lookup"><span data-stu-id="512ad-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="512ad-106">Imeti morate nabiralnik dnevnika in (po želji) konfiguriran nadomestni nabiralnik dnevnika.</span><span class="sxs-lookup"><span data-stu-id="512ad-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="512ad-107">Če želite izvedeti več, glejte [Konfiguracija dnevnika v storitvi Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="512ad-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="512ad-108">V storitvi Exchange Online je na voljo omejitev števila pravil temeljnice, ki jih lahko ustvarite.</span><span class="sxs-lookup"><span data-stu-id="512ad-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="512ad-109">Če želite več informacij, glejte [omejitve pravil za dnevnik, prenos in mapo» Prejeto «](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="512ad-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="512ad-110">Exchange Online ne podpira dostavljanja poročil v programu Exchange Online v nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="512ad-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="512ad-111">Določiti morate e-poštni naslov sistema za arhiviranje na mestu uporabe ali storitev za arhiviranje neodvisnih ponudnikov kot nabiralnik v dnevniku.</span><span class="sxs-lookup"><span data-stu-id="512ad-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
