---
title: Niz uporabnikovega posrednika za Microsoft Edge (namizni)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679333"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="f559b-102">Niz uporabnikovega posrednika za Microsoft Edge (namizni)</span><span class="sxs-lookup"><span data-stu-id="f559b-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="f559b-103">Nize uporabniških posrednikov (UA) lahko uporabite za odkrivanje, katero različico določenega brskalnika uporabljamo za določen operacijski sistem.</span><span class="sxs-lookup"><span data-stu-id="f559b-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="f559b-104">Tako kot drugi brskalniki Microsoft Edge vključuje te informacije v glavi» user-agent «HTTP, kadar koli zaprosi za mesto.</span><span class="sxs-lookup"><span data-stu-id="f559b-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="f559b-105">Informacije o različici brskalnika lahko dostopate tudi prek JavaScripta, tako da poizveduje po vrednosti» Navigator. userAgent «.</span><span class="sxs-lookup"><span data-stu-id="f559b-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="f559b-106">Priporočamo, da spletni razvijalci uporabijo zaznavanje funkcije, kadar koli je to mogoče, za izboljšanje vzdrževanja kode, zmanjšanje ranljivosti kode in odpravljanje tveganja preloma kode v primeru prihodnjih posodobitev niza za UA.</span><span class="sxs-lookup"><span data-stu-id="f559b-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="f559b-107">Če želite več informacij, glejte [niz uporabnikovega posrednika za Microsoft Edge (namizje)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="f559b-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>