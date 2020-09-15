---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717341"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="862a4-102">Odpravljanje težav z dostavo e-pošte za kodo napake 5.7.23</span><span class="sxs-lookup"><span data-stu-id="862a4-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="862a4-103">Preverite zapis SPF DNS za svojo domeno na javno razpoložljivem pregledovalniku SPF ali DNS v spletu.</span><span class="sxs-lookup"><span data-stu-id="862a4-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="862a4-104">Preverite, ali je Microsoft in preusmerjeni prek [paketa z visokim tveganjem](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages), ki ga je navedla neželena sporočila.</span><span class="sxs-lookup"><span data-stu-id="862a4-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="862a4-105">Sporočila v skupini z visokim tveganjem ne bodo posredovala preverjanja SPF, zato je ne bo sprejela ciljna e-poštna organizacija.</span><span class="sxs-lookup"><span data-stu-id="862a4-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="862a4-106">Če težave ne morete odpraviti, se boste morda morali obrniti na skrbnika poštnega gostitelja, v katerega želite poslati e-pošto.</span><span class="sxs-lookup"><span data-stu-id="862a4-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="862a4-107">Seznanite se s podrobno zunanjo napako, ki je na voljo v sporočilu Bounce.</span><span class="sxs-lookup"><span data-stu-id="862a4-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="862a4-108">Microsoftova podpora morda ne bo mogla več pomagati.</span><span class="sxs-lookup"><span data-stu-id="862a4-108">Microsoft support may not be able to assist further.</span></span>
