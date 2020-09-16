---
title: Odpravljanje težav z nastavitvijo DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744966"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="3a977-102">Odpravljanje težav z nastavitvijo DKIM</span><span class="sxs-lookup"><span data-stu-id="3a977-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="3a977-103">Če se pojavijo težave, ki omogočajo DKIM za vašo domeno po meri, uporabite te korake:</span><span class="sxs-lookup"><span data-stu-id="3a977-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="3a977-104">Večina težav z nastavitvijo DKIM je povezana z nepravilnimi zapisi DNS.</span><span class="sxs-lookup"><span data-stu-id="3a977-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="3a977-105">Preverite zapis CNAME DKIM (**ne** zapis txt), ki je pravilno oblikovan.</span><span class="sxs-lookup"><span data-stu-id="3a977-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="3a977-106">Če želite več informacij, glejte to [temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="3a977-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="3a977-107">Ko ustvarite ali posodobite zapise DNS DKIM pri ponudniku storitev gostovanja DNS za svojo domeno (po navadi je to vaš Registrator domene), počakajte, da se zapisi DNS širijo.</span><span class="sxs-lookup"><span data-stu-id="3a977-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="3a977-108">Če ne morete ustvariti zapisov DNS DKIM v skrbniškem središču, lahko zamenjate \<CustomDomain\> z domeno po meri (na primer contoso.com) in zaženete ta ukaz v [storitvi Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="3a977-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
