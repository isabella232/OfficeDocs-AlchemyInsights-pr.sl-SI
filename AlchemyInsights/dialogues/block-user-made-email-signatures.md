---
title: Blokiranje uporabniško ustvarjenih e-poštnih podpisov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243635"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="c6ed3-102">Blokiranje uporabniško ustvarjenih e-poštnih podpisov</span><span class="sxs-lookup"><span data-stu-id="c6ed3-102">Block user-made email signatures</span></span>

<span data-ttu-id="c6ed3-103">Ta rešitev velja le za e-poštne podpise, ki so bili ustvarjeni v Outlooku v spletu.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="c6ed3-104">V program Outlook lahko blokirate le podpise, če imate strežnik Exchange Server na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="c6ed3-105">V skrbniškem središču izberite Exchange **skrbniških centrov**  >  .</span><span class="sxs-lookup"><span data-stu-id="c6ed3-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="c6ed3-106">Kliknite **dovoljenja** za  >  **pravilnike programa Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="c6ed3-107">Izberite pravilnik in nato kliknite ikono svinčnika, da jo uredite.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="c6ed3-108">Kliknite **funkcije**  >  **več možnosti**.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="c6ed3-109">V razdelku **Uporabniška izkušnja** počistite potrditveno polje **e-poštni podpis** in kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="c6ed3-110">**Pomembno:** Če je bil podpis dodan, preden počistite to potrditveno polje, ga bo uporabnik še vedno lahko uporabil.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="c6ed3-111">Prosite jih, naj jo odstranijo.</span><span class="sxs-lookup"><span data-stu-id="c6ed3-111">Ask them to remove it.</span></span>
