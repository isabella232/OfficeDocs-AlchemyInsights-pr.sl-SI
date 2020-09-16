---
title: Odhodna e-pošta v mapo z neželeno e-pošto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769199"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="ecd2f-102">Odhodna e-pošta v mapo z neželeno e-pošto</span><span class="sxs-lookup"><span data-stu-id="ecd2f-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="ecd2f-103">Če vidite, da je odhodna sporočila označena kot neželena, naredite to:</span><span class="sxs-lookup"><span data-stu-id="ecd2f-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="ecd2f-104">Če tega še niste storili, razmislite o [konfiguriranju odhodnih obvestil pravilnika za neželeno pošto](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="ecd2f-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="ecd2f-105">Uporabite [sledenje sporočil](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) , če želite preveriti, ali je odhodno sporočilo **nezaželena** vrednost dogodka z dodatnimi podrobnostmi: **uporabite skupino za dostavo tveganja**.</span><span class="sxs-lookup"><span data-stu-id="ecd2f-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="ecd2f-106">Za ta sporočila potrdite vsebino sporočila, da si ogledate, kaj bi lahko veljalo za neželeno pošto.</span><span class="sxs-lookup"><span data-stu-id="ecd2f-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="ecd2f-107">Podpisi lahko na primer včasih povzročijo težave za številne uporabnike.</span><span class="sxs-lookup"><span data-stu-id="ecd2f-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="ecd2f-108">Če imate več primerov legitimnih odhodnih sporočil, ki so označena kot neželena, odprite vstopnico za podporo in prosite posrednika za podporo, da pošljete vaša sporočila kot lažne pozitivne podatke našim analitikom neželene pošte.</span><span class="sxs-lookup"><span data-stu-id="ecd2f-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="ecd2f-109">Bodite pripravljeni, da zagotovite vzorčna sporočila, ki vključujejo vse glave sporočil.</span><span class="sxs-lookup"><span data-stu-id="ecd2f-109">Be prepared to provide sample messages that include all message headers.</span></span>
