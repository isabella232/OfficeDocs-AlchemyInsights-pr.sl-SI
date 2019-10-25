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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682296"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="6340d-102">Odpravite težave pri dostavi e-pošte za kodo napake 5.7.23</span><span class="sxs-lookup"><span data-stu-id="6340d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="6340d-103">Preverite SPF DNS zapis za vašo domeno na javno voljo SPF ali DNS zapis Checker na spletu.</span><span class="sxs-lookup"><span data-stu-id="6340d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="6340d-104">Preverite, da odhodno sporočilo ni bilo identificirane kot vsiljena pošta s strani Officea 365 in Preusmerjeno prek [bazena za dostavo z visokim tveganjem](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="6340d-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="6340d-105">Sporočila v skupini za dostavo z visokim tveganjem ne bodo uspešno preverila SPF-jev, zato jih organizacija ciljne e-pošte ne bo sprejela.</span><span class="sxs-lookup"><span data-stu-id="6340d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="6340d-106">Če težave ne odpravite, se boste morda morali obrniti na skrbnika poštnega gostitelja, na katerega poskušate poslati e-poštno sporočilo.</span><span class="sxs-lookup"><span data-stu-id="6340d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="6340d-107">Zapišite si podrobno zunanjo napako, ki je na voljo v sporočilu za odklonovanje.</span><span class="sxs-lookup"><span data-stu-id="6340d-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="6340d-108">Podpora za Office 365 morda ne bo mogla dodatno pomagati.</span><span class="sxs-lookup"><span data-stu-id="6340d-108">Office 365 support may not be able to assist further.</span></span>