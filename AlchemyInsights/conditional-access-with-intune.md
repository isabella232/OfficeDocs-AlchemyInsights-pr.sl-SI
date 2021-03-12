---
title: Pogojni dostop z InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704802"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="3edb7-102">Pogojni dostop z InTune</span><span class="sxs-lookup"><span data-stu-id="3edb7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="3edb7-103">Uporaba  **pogojnega dostopa**  s funkcijo InTune zahteva 3 korake:</span><span class="sxs-lookup"><span data-stu-id="3edb7-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="3edb7-104">Ustvarite  **pravilnik o skladnosti**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), da določite nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za skladno.</span><span class="sxs-lookup"><span data-stu-id="3edb7-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="3edb7-105">Na primer, mora imeti naprava PIN vsaj 6 števk, preden se šteje za združljivo.</span><span class="sxs-lookup"><span data-stu-id="3edb7-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="3edb7-106">Ustvarjanje **pravilnika za pogojni dostop**  , ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolnjevati za dostop do teh virov.</span><span class="sxs-lookup"><span data-stu-id="3edb7-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="3edb7-107">Naprava mora biti na [primer](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) združljiva pred dostopom do e-pošte podjetja.</span><span class="sxs-lookup"><span data-stu-id="3edb7-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="3edb7-108">Zagotovite, da bodo **Pravilniki o skladnosti**  in  **Pravilniki pogojnega dostopa**  usmerjeni na želene skupine uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="3edb7-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="3edb7-109">S tem boste morda morali ustvariti določene skupine uporabnikov v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3edb7-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="3edb7-110">**Uporabne povezave:**</span><span class="sxs-lookup"><span data-stu-id="3edb7-110">**Helpful links:**</span></span>

[<span data-ttu-id="3edb7-111">Pregled skladnosti naprave</span><span class="sxs-lookup"><span data-stu-id="3edb7-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="3edb7-112">Odpravljanje težav CA</span><span class="sxs-lookup"><span data-stu-id="3edb7-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="3edb7-113">Pravilnik za odpravljanje težav</span><span class="sxs-lookup"><span data-stu-id="3edb7-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="3edb7-114">Za zaščito e-pošte (Exchange Online) iz Accessa z nezdružljivimi napravami je treba upoštevati oba dokumenta:</span><span class="sxs-lookup"><span data-stu-id="3edb7-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="3edb7-115">Zaščita e-poštnega dostopa v napravah s storitvijo EAS</span><span class="sxs-lookup"><span data-stu-id="3edb7-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="3edb7-116">Zaščita e-pošte v napravah s sodobnimi strankami za preverjanje pristnosti, kot je Outlook</span><span class="sxs-lookup"><span data-stu-id="3edb7-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)