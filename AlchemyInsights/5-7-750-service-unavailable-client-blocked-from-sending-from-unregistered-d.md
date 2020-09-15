---
title: 1048 5.7.750 storitev ni na voljo. Odjemalec je blokiral pošiljanje iz neregistriranih domen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664258"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="23c3b-103">5.7.750 odjemalec je blokiral pošiljanje iz neregistrirane domene</span><span class="sxs-lookup"><span data-stu-id="23c3b-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="23c3b-104">Do napake pride, ko se v domenah, ki niso omogočene v vašem najemniku, pošiljajo velike količine sporočil (dodane kot sprejete domene in preverjene).</span><span class="sxs-lookup"><span data-stu-id="23c3b-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="23c3b-105">Če se želite izogniti tej napaki, lahko uporabite povezovalnik toka pošte, ki temelji na potrdilu, kjer je domena potrdila omogočena domena, lahko pa omogočite vse domene za pošiljanje.</span><span class="sxs-lookup"><span data-stu-id="23c3b-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
