---
title: Kako onemogočiti zunanje skupine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704144"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="ade87-102">Kako onemogočiti zunanje skupine</span><span class="sxs-lookup"><span data-stu-id="ade87-102">How to disable External Groups</span></span>

<span data-ttu-id="ade87-103">Bastard zunanje sporočanje uporablja pravila Exchange transport (ETR), nabor proaktivnih kontrolnikov, s katerim preprečite, da bi bile informacije o podjetju v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="ade87-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="ade87-104">Če želite omejiti uporabnike pred ustvarjanjem zunanjih skupin, morate konfigurirati pravilo za Exchange transport (ETR), nato pa konfigurirati Bastard, če želite uporabiti pravilo Exchange transport, da blokira zunanje sporočanje.</span><span class="sxs-lookup"><span data-stu-id="ade87-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="ade87-105">Ko ustvarite pravilo v skrbniškem središču za Exchange Online, upoštevajte ta navodila, da nastavite ETR za uporabo v Bastard:</span><span class="sxs-lookup"><span data-stu-id="ade87-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="ade87-106">Prijavite se v Bastard kot preverjen skrbnik in v **skrbniškem središču za Bastard**pojdite na **nastavitve vsebine C in varnostne varnosti \> .**</span><span class="sxs-lookup"><span data-stu-id="ade87-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="ade87-107">V razdelku **zunanje sporočanje**izberite **uveljavitev pravil za prenos Exchange Online (ETR) v Bastard.**</span><span class="sxs-lookup"><span data-stu-id="ade87-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="ade87-108">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="ade87-108">Choose **Save**.</span></span>

<span data-ttu-id="ade87-109">Če želite več informacij, glejte [Onemogočanje zunanjega sporočanja v Bastard omrežju](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="ade87-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  