---
title: Šifriranje s pravili prenosa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915289"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="af587-102">Šifriranje s pravili prenosa</span><span class="sxs-lookup"><span data-stu-id="af587-102">Encryption with transport rules</span></span>

<span data-ttu-id="af587-103">V [skrbniškem središču za Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) lahko uporabite zmogljivosti šifriranja sporočil v Officeu (OME) v pravilih o toku pošte za proženje šifriranja sporočil.</span><span class="sxs-lookup"><span data-stu-id="af587-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="af587-104">V pogoju pravila prenosa izberite možnost **Uporabite šifriranje sporočil v storitvi Office 365 in zaščito pravic**.</span><span class="sxs-lookup"><span data-stu-id="af587-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="af587-105">Več informacij najdete v razdelku [Določite pravilo toka pošte za šifriranje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="af587-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="af587-106">V storitvi Powershell uporabite pripomoček »cmdlet« [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) in vrednost parametra *ApplyOME* nastavite na $true.</span><span class="sxs-lookup"><span data-stu-id="af587-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
