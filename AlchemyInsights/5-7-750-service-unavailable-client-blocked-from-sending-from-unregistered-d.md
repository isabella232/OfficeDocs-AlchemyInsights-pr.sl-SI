---
title: 1048 5.7.750 storitev ni na voljo. Odjemalec blokirana za pošiljanje iz Neregistrirana domene
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 06be6babc524ae0d8065355218426c695f49be66
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856636"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="c4e17-103">5.7.750 odjemalca blokirano pošiljanje iz Neregistrirana domene</span><span class="sxs-lookup"><span data-stu-id="c4e17-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="c4e17-104">Napaka se pojavi, ko je velik obseg sporočila so poslana iz domen, ki niso omogočeni v Office 365 (doda kot sprejete domene in potrdil).</span><span class="sxs-lookup"><span data-stu-id="c4e17-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="c4e17-105">Da bi se izognili tej napaki, lahko uporabite priključek tok potrdilo e-pošta, kjer domeno potrdila je omogočena uporaba domene, ali lahko določba vse pošilja domene.</span><span class="sxs-lookup"><span data-stu-id="c4e17-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
