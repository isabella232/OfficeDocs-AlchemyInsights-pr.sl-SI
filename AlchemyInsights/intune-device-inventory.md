---
title: InTune inventarja naprave
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667894"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="1fd12-102">InTune inventarja naprave</span><span class="sxs-lookup"><span data-stu-id="1fd12-102">Intune Device Inventory</span></span>

<span data-ttu-id="1fd12-103">Rezilo» Devices «omogoča skrbniku vpogled v naprave v razdelku upravljanje v programu InTune v napravi na osnovi.</span><span class="sxs-lookup"><span data-stu-id="1fd12-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="1fd12-104">Prikazani podatki vključujejo: strojna oprema, odkrite aplikacije, stanje naprave za skladnost s predpisi in stanje konfiguracije naprave.</span><span class="sxs-lookup"><span data-stu-id="1fd12-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="1fd12-105">Podatki o inventarju strojne opreme in odkriti programi so zbrani v sedemdnevnem ciklu.</span><span class="sxs-lookup"><span data-stu-id="1fd12-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="1fd12-106">Aplikacije in določeni elementi strojne opreme se razlikujejo glede na operacijski sistem naprave in ali je naprava osebno ali v lasti podjetja.</span><span class="sxs-lookup"><span data-stu-id="1fd12-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="1fd12-107">Če želite več informacij, glejte [Ogled podrobnosti naprave v programu InTune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="1fd12-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="1fd12-108">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="1fd12-108">**FAQ**</span></span>

<span data-ttu-id="1fd12-109">V: v napravah s sistemom Windows ne prejmem celotnega seznama inventarnih programov, ki so na voljo v razdelku InTune.</span><span class="sxs-lookup"><span data-stu-id="1fd12-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="1fd12-110">zakaj pa ne?</span><span class="sxs-lookup"><span data-stu-id="1fd12-110">Why not?</span></span>

<span data-ttu-id="1fd12-111">A: trenutno so v računalnikih s sistemom Windows 10, ki so prepoznani kot podjetja, navedene le sodobne aplikacije.</span><span class="sxs-lookup"><span data-stu-id="1fd12-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="1fd12-112">InTune ne zbira informacij o aplikacijah Win32, ki so nameščene v teh napravah.</span><span class="sxs-lookup"><span data-stu-id="1fd12-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="1fd12-113">V: zakaj se telefonske številke ne zbirajo v vseh napravah?</span><span class="sxs-lookup"><span data-stu-id="1fd12-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="1fd12-114">A: telefoni, kategorizirani kot podjetja v programu InTune, niso identificirani s polno telefonsko številko, ko na primer zaženete poročilo o inventarju prenosne naprave.</span><span class="sxs-lookup"><span data-stu-id="1fd12-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="1fd12-115">Telefonske številke, ki so na voljo za lastno napravo, so vedno delno prikrite z zvezdicami (\* \* \* \*) in prikazujejo le zadnje štiri števke.</span><span class="sxs-lookup"><span data-stu-id="1fd12-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>