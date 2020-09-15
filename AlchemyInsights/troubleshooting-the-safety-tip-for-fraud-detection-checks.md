---
title: Odpravljanje težav z varnostnim namigom za preverjanje goljufij
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658426"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ab669-102">Odpravljanje težav z varnostnim namigom za preverjanje goljufij</span><span class="sxs-lookup"><span data-stu-id="ab669-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ab669-103">Če ste dobili varnostni namig, v katerem je navedeno, da» pošiljatelj ni uspel zaznati preverjanja prevare in morda ni tak, kot je videti «, pošiljatelj ni uspel izvesti preverjanja pristnosti v DKIM ali SPF.</span><span class="sxs-lookup"><span data-stu-id="ab669-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ab669-104">Najboljši način za rešitev tega je, da se pošiljatelj pooblasti.</span><span class="sxs-lookup"><span data-stu-id="ab669-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ab669-105">Če pošiljatelj pošilja v vašem imenu, ga morate pooblastiti tako, da dodate naslov IP pošiljatelja v zapis SPF.</span><span class="sxs-lookup"><span data-stu-id="ab669-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ab669-106">Če želite več informacij, glejte [Odpravljanje težav z rdečim (sumljivim) varnostnim namigom za odkrivanje goljufij](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="ab669-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="ab669-107">Tukaj je nekaj drugih povezav, ki vam lahko pomagajo:</span><span class="sxs-lookup"><span data-stu-id="ab669-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ab669-108">Kako Microsoft uporablja okvir pravilnika pošiljatelja (SPF) za preprečevanje lažnega predstavljanja</span><span class="sxs-lookup"><span data-stu-id="ab669-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="ab669-109">Nastavitev SPF za preprečevanje lažnega predstavljanja</span><span class="sxs-lookup"><span data-stu-id="ab669-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
