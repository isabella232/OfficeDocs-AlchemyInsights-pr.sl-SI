---
title: Kako onemogočiti zunanje skupine
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739509"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="e514a-102">Kako onemogočiti zunanje skupine</span><span class="sxs-lookup"><span data-stu-id="e514a-102">How to disable External Groups</span></span>

<span data-ttu-id="e514a-103">Za zunanje sporočanje yammer veljajo pravila Exchangeevega prenosa (ETRs), niz proaktivnih kontrolnikov, ki preprečujejo skupno rabo podatkov podjetja.</span><span class="sxs-lookup"><span data-stu-id="e514a-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="e514a-104">Če želite uporabnikom omejiti ustvarjanje zunanjih skupin, morate konfigurirati pravilo za Exchangeeva pravila (ETR) in nato konfigurirati storitev Yammer, če želite blokirati zunanje sporočanje s pravilom Exchangevega transporta.</span><span class="sxs-lookup"><span data-stu-id="e514a-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="e514a-105">Ko ustvarite pravilo v skrbniškem središču za Exchange Online, sledite tem korakom, da nastavite ETR za uporabo v storitvi Yammer:</span><span class="sxs-lookup"><span data-stu-id="e514a-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="e514a-106">Prijavite se v storitev Yammer kot preverjen skrbnik in v **skrbniškem središču yammer**pojdite na vsebino C **in varnostne \> varnostne nastavitve.**</span><span class="sxs-lookup"><span data-stu-id="e514a-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="e514a-107">V razdelku **zunanje sporočanje** **v storitvi Yammer izberite uveljavi pravila za prenos Exchange Online Exchange (etrs).**</span><span class="sxs-lookup"><span data-stu-id="e514a-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="e514a-108">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="e514a-108">Choose **Save**.</span></span>

<span data-ttu-id="e514a-109">Če želite več informacij, glejte [Onemogočanje zunanjega sporočanja v omrežju Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="e514a-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  