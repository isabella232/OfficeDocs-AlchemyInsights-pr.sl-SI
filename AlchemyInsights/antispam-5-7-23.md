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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506459"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="44845-102">Odpravite težave pri dostavi e-pošte za kodo napake 5.7.23</span><span class="sxs-lookup"><span data-stu-id="44845-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="44845-103">Preverite SPF DNS zapis za vašo domeno na javno voljo SPF ali DNS zapis Checker na spletu.</span><span class="sxs-lookup"><span data-stu-id="44845-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="44845-104">Prepričajte se, da Microsoft odhodno sporočilo ni bilo identificiran kot vsiljena pošta in preusmerjen prek [paketa za dostavo z visokim tveganjem](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="44845-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="44845-105">Sporočila v skupini za dostavo z visokim tveganjem ne bodo uspešno preverila SPF-jev, zato jih organizacija ciljne e-pošte ne bo sprejela.</span><span class="sxs-lookup"><span data-stu-id="44845-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="44845-106">Če težave ne odpravite, se boste morda morali obrniti na skrbnika poštnega gostitelja, na katerega poskušate poslati e-poštno sporočilo.</span><span class="sxs-lookup"><span data-stu-id="44845-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="44845-107">Zapišite si podrobno zunanjo napako, ki je na voljo v sporočilu za odklonovanje.</span><span class="sxs-lookup"><span data-stu-id="44845-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="44845-108">Microsoftova podpora morda ne bo mogla dodatno pomagati.</span><span class="sxs-lookup"><span data-stu-id="44845-108">Microsoft support may not be able to assist further.</span></span>
