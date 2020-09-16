---
title: Pošiljanje obvestil po meri z InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720662"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="9b4f1-102">Pošiljanje obvestil po meri uporabnikom upravljanih naprav s sistemom iOS in naprave s sistemom Android</span><span class="sxs-lookup"><span data-stu-id="9b4f1-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="9b4f1-103">Obvestila po meri za InTune obdeluje program portal podjetja v napravi uporabnika.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="9b4f1-104">Aplikacija nato ustvari obvestilo potisni v tej napravi.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="9b4f1-105">V nadaljevanju so pogoji za naprave, ki podpirajo prejemanje obvestil po meri, in za aplikacijo, da nato ustvarite obvestilo o potiskanju:</span><span class="sxs-lookup"><span data-stu-id="9b4f1-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="9b4f1-106">Naprava mora imeti nameščeno aplikacijo portal podjetja.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="9b4f1-107">Naprava mora omogočati aplikacijo portala za podjetja, če želite poslati potisna obvestila.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="9b4f1-108">Ko je aplikacija nameščena ali posodobljena, bo pozval uporabnika, da dovoli obvestila.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="9b4f1-109">Naprave s sistemom Android morajo imeti nameščene storitve Google Play.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="9b4f1-110">Naprava mora biti včlanjena v sozvočju.</span><span class="sxs-lookup"><span data-stu-id="9b4f1-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="9b4f1-111">Če želite več informacij o tem, kako poslati sporočilo, si oglejte [dokumentacijo funkcije](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="9b4f1-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
