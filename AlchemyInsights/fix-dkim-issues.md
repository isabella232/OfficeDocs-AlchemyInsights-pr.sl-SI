---
title: Odpravljanje težav z nastavitvijo DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717578"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="8d446-102">Odpravljanje težav z nastavitvijo DKIM</span><span class="sxs-lookup"><span data-stu-id="8d446-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="8d446-103">Če naletite na težave, ki omogočajo DKIM za vašo domeno po meri, uporabite naslednje korake:</span><span class="sxs-lookup"><span data-stu-id="8d446-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="8d446-104">Večina težav z nastavitvijo DKIM je povezanih z nepravilnimi zapisi DNS.</span><span class="sxs-lookup"><span data-stu-id="8d446-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="8d446-105">Preverite, ali je zapis DKIM CNAME (**ne** zapis txt) pravilno formatiran.</span><span class="sxs-lookup"><span data-stu-id="8d446-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="8d446-106">Če želite več informacij, glejte to [temo](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="8d446-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="8d446-107">Ko ustvarite ali posodobite zapise DKIM DNS v storitvi gostovanja DNS za vašo domeno (običajno je to registrar domene), počakajte, da se zapisi DNS razširijo.</span><span class="sxs-lookup"><span data-stu-id="8d446-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="8d446-108">Če ne morete ustvariti zapisov DKIM DNS v skrbniškem središču, lahko \<zamenjate customdomain\> s svojo domeno po meri (na primer contoso.com) in zaženete ta ukaz v [PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`</span><span class="sxs-lookup"><span data-stu-id="8d446-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
