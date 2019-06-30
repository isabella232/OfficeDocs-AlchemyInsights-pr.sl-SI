---
title: Kako v onesposobiti zunanjih skupin
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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384841"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="4b22f-102">Kako v onesposobiti zunanjih skupin</span><span class="sxs-lookup"><span data-stu-id="4b22f-102">How to disable External Groups</span></span>

<span data-ttu-id="4b22f-103">Kukati, zunanjih sporočil uporablja pravila izmenjave prevoza (ETRs), niz proaktivne ukrepe, da preprečijo podatki podjetja skupne rabe.</span><span class="sxs-lookup"><span data-stu-id="4b22f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="4b22f-104">Da bi določim ustvarjanje zunanjih skupin, boste morali oblikovati pravilo za izmenjavo prometa ("ETR"), ter torej oblikovati Bastard rabiti Exchangeev prenos pravilo v tnalo zunanja sporočila.</span><span class="sxs-lookup"><span data-stu-id="4b22f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="4b22f-105">Ko ustvarite pravilo v Exchange Online admin center, sledite tem korakom nastaviti ETR v Bastard:</span><span class="sxs-lookup"><span data-stu-id="4b22f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="4b22f-106">Prijaviti Bastard kot preverjene admin in **Kukati skrbniško središče**, pojdite na C **vsebino in varnost \> varnostne nastavitve.**</span><span class="sxs-lookup"><span data-stu-id="4b22f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="4b22f-107">Pod, **Zunanjih sporočil**, izberite **vsili Exchange Online izmenjavo prometa pravila (ETRs) v Bastard.**</span><span class="sxs-lookup"><span data-stu-id="4b22f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="4b22f-108">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="4b22f-108">Choose **Save**.</span></span>

<span data-ttu-id="4b22f-109">Če želite več informacij, glejte [nadzor zunanjih sporočil v mrežo Bastard pravilom Exchangeev prenos](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="4b22f-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  