---
title: Pošlji obvestila po meri z InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886873"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="92ebd-102">Kako poslati obvestila po meri uporabnikom upravljanih naprav iOS in Android</span><span class="sxs-lookup"><span data-stu-id="92ebd-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="92ebd-103">Obvestila po meri za InTune obdelujejo aplikacija portal podjetja v uporabnikovi napravi.</span><span class="sxs-lookup"><span data-stu-id="92ebd-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="92ebd-104">Aplikacija nato ustvari potisno obvestilo v tej napravi.</span><span class="sxs-lookup"><span data-stu-id="92ebd-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="92ebd-105">V nadaljevanju so predpogoji naprave za podporo prejemu obvestil po meri in za aplikacijo, ki nato Ustvari sporočilo za potiskanje:</span><span class="sxs-lookup"><span data-stu-id="92ebd-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="92ebd-106">Naprava mora imeti nameščeno aplikacijo portal za podjetja.</span><span class="sxs-lookup"><span data-stu-id="92ebd-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="92ebd-107">Naprava mora dovoliti, da aplikacija portal za podjetja pošilja potisna obvestila.</span><span class="sxs-lookup"><span data-stu-id="92ebd-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="92ebd-108">Ko je aplikacija nameščena ali posodobljena, bo pozvala uporabnika, da dovoli obvestila.</span><span class="sxs-lookup"><span data-stu-id="92ebd-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="92ebd-109">Naprave Android morajo imeti nameščene storitve Google Play.</span><span class="sxs-lookup"><span data-stu-id="92ebd-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="92ebd-110">Napravo morate vpisati z InTune.</span><span class="sxs-lookup"><span data-stu-id="92ebd-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="92ebd-111">Če želite več informacij, vključno s pošiljanjem sporočila, si oglejte [dokumentacijo funkcije](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="92ebd-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
