---
title: Odpravljanje težav pri preverjanjih, povezanih z zaznavanjem prevar, v varnostnem namigu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834747"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c35b4-102">Odpravljanje težav pri preverjanjih, povezanih z zaznavanjem prevar, v varnostnem namigu</span><span class="sxs-lookup"><span data-stu-id="c35b4-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c35b4-103">Če se vam prikaže varnostni nasvet »Pošiljatelj ni uspel pri zaznavanju prevar in morda ni to, za koga je bil«, pošiljatelj ni uspešno uspešno opravil preverjanja pristnosti DKIM ali SPF.</span><span class="sxs-lookup"><span data-stu-id="c35b4-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c35b4-104">Najboljši način, da to razrešite, je, da se pošiljatelj pooblasti sam.</span><span class="sxs-lookup"><span data-stu-id="c35b4-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c35b4-105">Če pošiljatelj pošilja sporočila v vašem imenu, jih morate pooblastiti tako, da dodate naslov IP pošiljatelja v zapis SPF.</span><span class="sxs-lookup"><span data-stu-id="c35b4-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c35b4-106">Če [želite več informacij, glejte Odpravljanje težav z rdečim (sumljivim) varnostnim](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) nasvetom za zaznavanje prevar.</span><span class="sxs-lookup"><span data-stu-id="c35b4-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c35b4-107">Tukaj je še nekaj drugih povezav, ki so vam lahko v pomoč:</span><span class="sxs-lookup"><span data-stu-id="c35b4-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c35b4-108">Kako Microsoft uporablja ogrodje SPF (sender policy framework) za preprečevanje sporočila o ponarejenem pošiljatelju</span><span class="sxs-lookup"><span data-stu-id="c35b4-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c35b4-109">Nastavitev SPF-a za preprečevanje zlorabe</span><span class="sxs-lookup"><span data-stu-id="c35b4-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
