---
title: Pošlji obvestila po meri z InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992328"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="cb61e-102">Kako poslati obvestila po meri uporabnikom upravljanih naprav iOS in Android</span><span class="sxs-lookup"><span data-stu-id="cb61e-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="cb61e-103">Obvestila po meri za InTune obdelujejo aplikacija portal podjetja v uporabnikovi napravi.</span><span class="sxs-lookup"><span data-stu-id="cb61e-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="cb61e-104">Aplikacija nato ustvari potisno obvestilo v tej napravi.</span><span class="sxs-lookup"><span data-stu-id="cb61e-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="cb61e-105">V nadaljevanju so predpogoji naprave za podporo prejemu obvestil po meri in za aplikacijo, ki nato Ustvari sporočilo za potiskanje:</span><span class="sxs-lookup"><span data-stu-id="cb61e-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="cb61e-106">Naprava mora imeti nameščeno aplikacijo portal za podjetja.</span><span class="sxs-lookup"><span data-stu-id="cb61e-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="cb61e-107">Naprava mora dovoliti, da aplikacija portal za podjetja pošilja potisna obvestila.</span><span class="sxs-lookup"><span data-stu-id="cb61e-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="cb61e-108">Ko je aplikacija nameščena ali posodobljena, bo pozvala uporabnika, da dovoli obvestila.</span><span class="sxs-lookup"><span data-stu-id="cb61e-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="cb61e-109">Naprave Android morajo imeti nameščene storitve Google Play.</span><span class="sxs-lookup"><span data-stu-id="cb61e-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="cb61e-110">Napravo morate vpisati z InTune.</span><span class="sxs-lookup"><span data-stu-id="cb61e-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="cb61e-111">Če želite več informacij, vključno s pošiljanjem sporočila, si oglejte [dokumentacijo funkcije](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="cb61e-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
