---
title: V Varnostnem središču ni bilo mogoče najti sporočila» naročnine «
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "50714388"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="91a59-102">V Varnostnem središču ni bilo mogoče najti sporočila» naročnine «</span><span class="sxs-lookup"><span data-stu-id="91a59-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="91a59-103">Če se pri dostopu do varnostnega središča Microsoft Defender prikaže sporočilo» brez naročnine «, to pomeni, da je imenik Azure Active Directory (ZVOČNa datoteka), ki se uporablja za prijavo uporabnika v portal, nima licence za Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="91a59-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="91a59-104">Licence sistema Windows E5 in Office E5 sta ločeni licenci.</span><span class="sxs-lookup"><span data-stu-id="91a59-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="91a59-105">Odprite primer podpore, če je bila licenca kupljena, vendar ni bila omogočena za ta primerek.</span><span class="sxs-lookup"><span data-stu-id="91a59-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="91a59-106">Ali imate:</span><span class="sxs-lookup"><span data-stu-id="91a59-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="91a59-107">Možna izdaja za omogočanje uporabe licence.</span><span class="sxs-lookup"><span data-stu-id="91a59-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="91a59-108">Licenco ste pomotoma omogočili za drugo Microsoftovo ZVOČNO polje, kot je bila uporabljena za preverjanje pristnosti v storitvi.</span><span class="sxs-lookup"><span data-stu-id="91a59-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>