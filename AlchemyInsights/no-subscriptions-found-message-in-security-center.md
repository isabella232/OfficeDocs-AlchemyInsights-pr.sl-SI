---
title: V Varnostnem središču ni bilo mogoče najti sporočila o naročninah
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544124"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="8ad43-102">V Varnostnem središču ni bilo mogoče najti sporočila o naročninah</span><span class="sxs-lookup"><span data-stu-id="8ad43-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="8ad43-103">Če med dostopom do storitve Microsoft Defender Security Center prikaže sporočilo »Nobene naročnine ni bilo mogoče najti«, to pomeni, da storitev Azure Active Directory (AAD), ki se uporablja za prijavo uporabnika v portal, nima licence za Microsoft Defender ATP licence.</span><span class="sxs-lookup"><span data-stu-id="8ad43-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="8ad43-104">Licenci Windows E5 in Office E5 sta ločeni licenci.</span><span class="sxs-lookup"><span data-stu-id="8ad43-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="8ad43-105">Odprite primer podpore, če ste licenco kupili, vendar ni bila omogočena za ta primerek storitve AAD.</span><span class="sxs-lookup"><span data-stu-id="8ad43-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="8ad43-106">Imate:</span><span class="sxs-lookup"><span data-stu-id="8ad43-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="8ad43-107">Morebitne težave z omogočanjem uporabe licenc.</span><span class="sxs-lookup"><span data-stu-id="8ad43-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="8ad43-108">Ne glede na to, ali ste licenco nenamerno omogočali za Microsoftovo storitev AAD, kot je bila ta, uporabljena za preverjanje pristnosti, v storitev.</span><span class="sxs-lookup"><span data-stu-id="8ad43-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>