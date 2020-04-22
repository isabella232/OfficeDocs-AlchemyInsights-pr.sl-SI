---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676513"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="85e64-102">Odpravite težave pri dostavi e-pošte za kodo napake 5.7.23</span><span class="sxs-lookup"><span data-stu-id="85e64-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="85e64-103">Preverite SPF DNS zapis za vašo domeno na javno voljo SPF ali DNS zapis Checker na spletu.</span><span class="sxs-lookup"><span data-stu-id="85e64-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="85e64-104">Prepričajte se, da Microsoft odhodno sporočilo ni bilo identificiran kot vsiljena pošta in preusmerjen prek [paketa za dostavo z visokim tveganjem](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="85e64-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="85e64-105">Sporočila v skupini za dostavo z visokim tveganjem ne bodo uspešno preverila SPF-jev, zato jih organizacija ciljne e-pošte ne bo sprejela.</span><span class="sxs-lookup"><span data-stu-id="85e64-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="85e64-106">Če težave ne odpravite, se boste morda morali obrniti na skrbnika poštnega gostitelja, na katerega poskušate poslati e-poštno sporočilo.</span><span class="sxs-lookup"><span data-stu-id="85e64-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="85e64-107">Zapišite si podrobno zunanjo napako, ki je na voljo v sporočilu za odklonovanje.</span><span class="sxs-lookup"><span data-stu-id="85e64-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="85e64-108">Microsoftova podpora morda ne bo mogla dodatno pomagati.</span><span class="sxs-lookup"><span data-stu-id="85e64-108">Microsoft support may not be able to assist further.</span></span>
