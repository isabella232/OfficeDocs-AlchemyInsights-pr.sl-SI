---
title: Pravilnik o zaščiti aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423960"
---
# <a name="application-protection-policy"></a><span data-ttu-id="c1013-102">Pravilnik o zaščiti aplikacije</span><span class="sxs-lookup"><span data-stu-id="c1013-102">Application protection policy</span></span>

<span data-ttu-id="c1013-103">Če ste na novo v pravilniku za zaščito aplikacij (APP), si oglejte pregled [pravilnikov za zaščito aplikacij](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="c1013-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="c1013-104">Če želite začeti uporabljati APLIKACIJO, [glejte Ustvarjanje in dodeljevanje pravilnikov o zaščiti aplikacij](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="c1013-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="c1013-105">Zahteve pravilnika o zaščiti aplikacij:</span><span class="sxs-lookup"><span data-stu-id="c1013-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="c1013-106">Uporabnik ima licenco Intune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="c1013-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="c1013-107">Uporabnik pripada skupini, ki so jo ciljali pravilniki za zaščito aplikacij.</span><span class="sxs-lookup"><span data-stu-id="c1013-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="c1013-108">Samo en uporabnik podjetja je vpisan v zaščitene aplikacije v napravi.</span><span class="sxs-lookup"><span data-stu-id="c1013-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="c1013-109">Aplikacija je izvedla [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="c1013-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="c1013-110">Če si želite ogledati seznam aplikacij, ki podpirajo SDK, [glejte Aplikacije, zaščitene z Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="c1013-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="c1013-111">Pravilniki veljajo po tem, ko uporabnik, ki izpolnjuje zgornje zahteve, podpiše v aplikacijo, ki podpira SDK za Intune.</span><span class="sxs-lookup"><span data-stu-id="c1013-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="c1013-112">Najlažji način za ugotavljanje, ali je uporabljen pravilnik, je zahteva, da uporabnik nastavi žebljiček v pravilniku.</span><span class="sxs-lookup"><span data-stu-id="c1013-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="c1013-113">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="c1013-113">For more information, see:</span></span>

[<span data-ttu-id="c1013-114">Pogosta vprašanja o odpravljanju težav z aplikacijami/mam</span><span class="sxs-lookup"><span data-stu-id="c1013-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="c1013-115">Preverjanje veljavnosti nastavitve pravilnika za zaščito aplikacij</span><span class="sxs-lookup"><span data-stu-id="c1013-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="c1013-116">Razumevanje časa izvajanja pravilnika za zaščito aplikacij</span><span class="sxs-lookup"><span data-stu-id="c1013-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="c1013-117">Spremljanje pravilnikov o zaščiti aplikacij</span><span class="sxs-lookup"><span data-stu-id="c1013-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)