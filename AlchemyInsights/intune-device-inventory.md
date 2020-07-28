---
title: Inventar naprave Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440477"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="21ef8-102">Inventar naprave Intune</span><span class="sxs-lookup"><span data-stu-id="21ef8-102">Intune Device Inventory</span></span>

<span data-ttu-id="21ef8-103">Rezilo Naprave omogoča skrbniku vpogled v naprave, ki jih upravljali v intunu, na podlagi naprave.</span><span class="sxs-lookup"><span data-stu-id="21ef8-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="21ef8-104">Prikazane informacije vključujejo: Strojna oprema, Odkrite aplikacije, Stanje skladnosti naprave in stanje konfiguracije naprave.</span><span class="sxs-lookup"><span data-stu-id="21ef8-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="21ef8-105">Podatki o zalogah za strojno opremo in odkrite aplikacije se zbirajo v sedemdnevnem ciklu.</span><span class="sxs-lookup"><span data-stu-id="21ef8-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="21ef8-106">Aplikacije in posebni elementi strojne opreme, o katerih so poročali, se razlikujejo glede na operacijski sistem naprave in ali je naprava v zasebni lasti ali v lasti podjetja.</span><span class="sxs-lookup"><span data-stu-id="21ef8-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="21ef8-107">Če želite več informacij, [glejte Ogled podrobnosti o napravi v intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="21ef8-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="21ef8-108">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="21ef8-108">**FAQ**</span></span>

<span data-ttu-id="21ef8-109">V: Ne prejemam celotnega seznama inventarja aplikacij, ki so prisotne v napravah Windows, vpisanih v Intune.</span><span class="sxs-lookup"><span data-stu-id="21ef8-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="21ef8-110">zakaj pa ne?</span><span class="sxs-lookup"><span data-stu-id="21ef8-110">Why not?</span></span>

<span data-ttu-id="21ef8-111">O: Trenutno so za računalnike s sistemom Windows 10, ki so prepoznani kot poslovne naprave, navedene samo sodobne aplikacije.</span><span class="sxs-lookup"><span data-stu-id="21ef8-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="21ef8-112">Intune ne zbira podatkov o aplikacijah Win32, nameščenih v teh napravah.</span><span class="sxs-lookup"><span data-stu-id="21ef8-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="21ef8-113">V: Zakaj telefonske številke niso zbrane iz vseh naprav?</span><span class="sxs-lookup"><span data-stu-id="21ef8-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="21ef8-114">O: Telefoni, ki so v intunu razvrščeni kot poslovne naprave, niso identificirani s polno telefonsko številko, ko na primer zaženete poročilo o inventarju mobilne naprave.</span><span class="sxs-lookup"><span data-stu-id="21ef8-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="21ef8-115">Številke telefonov Bring-you-own-device so vedno delno zakrite z zvezdicami (\*\*\*\*) in prikazujejo samo zadnje štiri števke.</span><span class="sxs-lookup"><span data-stu-id="21ef8-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>