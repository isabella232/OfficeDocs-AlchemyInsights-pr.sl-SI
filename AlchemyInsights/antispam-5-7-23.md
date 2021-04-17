---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821427"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="b2ff2-102">Odpravljanje težav za dostavo e-pošte za kodo napake 5.7.23</span><span class="sxs-lookup"><span data-stu-id="b2ff2-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="b2ff2-103">Preverite zapis DNS SPF za svojo domeno pri javno dostopnem SPF-ju ali v spletnem preverjanje zapisov DNS.</span><span class="sxs-lookup"><span data-stu-id="b2ff2-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="b2ff2-104">Prepričajte se, da Microsoft ni identificiral odhodnega sporočila kot neželeno pošto in da je bilo preusmerjeno prek skupine dostav [z visokim tveganjem.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="b2ff2-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="b2ff2-105">Sporočila v poolu za dostavo z visokim tveganjem ne bodo uspešno sprejeta preverjanja SPF, zato ciljna e-poštna organizacija ne bo sprejela.</span><span class="sxs-lookup"><span data-stu-id="b2ff2-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="b2ff2-106">Če težave ne morete odpraviti, se boste morda morali obrnite na skrbnika gostitelja pošte, kateremu poskušate poslati e-pošto.</span><span class="sxs-lookup"><span data-stu-id="b2ff2-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="b2ff2-107">V sporočilu o odklonu si zabeležite podrobno zunanjo napako.</span><span class="sxs-lookup"><span data-stu-id="b2ff2-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="b2ff2-108">Microsoftova podpora morda ne bo mogla dodatno pomagati.</span><span class="sxs-lookup"><span data-stu-id="b2ff2-108">Microsoft support may not be able to assist further.</span></span>
