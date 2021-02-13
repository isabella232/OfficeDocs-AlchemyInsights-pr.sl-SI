---
title: Uvajanje Microsoftovega roba v sistem iOS, iPadOS in Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194587"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="c97ef-102">Uvajanje Microsoftovega roba v sistem iOS, iPadOS in Android</span><span class="sxs-lookup"><span data-stu-id="c97ef-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="c97ef-103">Spodaj povzeto voden scenarij vam bo pomagal dodeliti Microsoft Edge uporabnikom naprav iOS, iPadOS in Android.</span><span class="sxs-lookup"><span data-stu-id="c97ef-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="c97ef-104">Če ste blokirali uporabnike pred vpisom mobilnih naprav, ta voden scenarij ne deluje in uporabniki bodo morali sami namestiti Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="c97ef-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="c97ef-105">Voden scenarij vključuje te korake:</span><span class="sxs-lookup"><span data-stu-id="c97ef-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="c97ef-106">Predpogoji</span><span class="sxs-lookup"><span data-stu-id="c97ef-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="c97ef-107">Uvod</span><span class="sxs-lookup"><span data-stu-id="c97ef-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="c97ef-108">Osnove</span><span class="sxs-lookup"><span data-stu-id="c97ef-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="c97ef-109">Konfiguracije</span><span class="sxs-lookup"><span data-stu-id="c97ef-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="c97ef-110">Dodelitve</span><span class="sxs-lookup"><span data-stu-id="c97ef-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="c97ef-111">Pregled in ustvarjanje</span><span class="sxs-lookup"><span data-stu-id="c97ef-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="c97ef-112">Ko dokončate korake v vodenem scenariju, bodo pravilniki programa Microsoft InTune omogočili te funkcije Microsoft Edge za podjetja:</span><span class="sxs-lookup"><span data-stu-id="c97ef-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="c97ef-113">Dvojna identiteta</span><span class="sxs-lookup"><span data-stu-id="c97ef-113">Dual identity</span></span>
- <span data-ttu-id="c97ef-114">Integracija s pravilnikom o zaščiti aplikacije Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="c97ef-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="c97ef-115">Integracija s proxyjem programa Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c97ef-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="c97ef-116">Upravljane bližnjice med priljubljenimi in domačo stranjo</span><span class="sxs-lookup"><span data-stu-id="c97ef-116">Managed favorites and home page shortcuts</span></span>
