---
title: 126 za pridobivanje nabiralnika ni mogoče najti napake v programu OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706766"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="9e9c8-102">Ali v Outlooku v spletu ni mogoče najti napake nabiralnika?</span><span class="sxs-lookup"><span data-stu-id="9e9c8-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="9e9c8-103">Če uporabljate Outlook v spletu in prejmete **nabiralnik ni bilo mogoče najti za** napako, račun, s katerim ste vzpostavili povezavo z Outlookom v spletu, nima licence za Exchange Online in zato ni povezan noben nabiralnik z računom.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="9e9c8-104">Skrbnik lahko dodeli licenco za vaš račun tako, da upošteva te korake:</span><span class="sxs-lookup"><span data-stu-id="9e9c8-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="9e9c8-105">Odprite [skrbniško središče za Microsoft 365](https://portal.office.com/adminportal/home#/homepage) in pojdite v razdelek **aktivni uporabniki** v razdelku **Uporabniki** , nato pa izberite uporabnika, ki vidi napako.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="9e9c8-106">Na strani uporabnik, ki se odpre, pojdite v razdelek **licence in programi** , izberite ustrezno vrednost **lokacije** in dodelite licenco, ki vsebuje Exchange Online (razširite licenco, da si ogledate podrobnosti).</span><span class="sxs-lookup"><span data-stu-id="9e9c8-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="9e9c8-107">Ko končate, kliknite **Shrani spremembe**.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-107">When you're finished, click **Save changes**.</span></span>
