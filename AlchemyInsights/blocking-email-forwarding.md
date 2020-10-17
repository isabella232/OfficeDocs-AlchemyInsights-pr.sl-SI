---
title: 726 blokiranje posredovanja e-pošte
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
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478342"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="0efb8-102">Blokiranje ali odblokiranje posredovanja e-pošte</span><span class="sxs-lookup"><span data-stu-id="0efb8-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="0efb8-103">Če želite omogočiti ali onemogočiti posredovanje e-pošte za določen nabiralnik, glejte [Konfiguracija posredovanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="0efb8-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="0efb8-104">Na ravni najemnika se nadzor zunanjega posredovanja izvaja s pravilnikom odhodne neželene pošte.</span><span class="sxs-lookup"><span data-stu-id="0efb8-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="0efb8-105">Pravilnik za filtriranje neželene pošte lahko preverite [v središču za](https://protection.office.com/antispam) varnost in skladnost s predpisi ali pa uporabite [ukaz» Get-HostedOutboundSpamFilterPolicy «](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="0efb8-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="0efb8-106">Če se prikaže to sporočilo o napaki: **» 550 5.7.520 Access je zavrnjen, vaša organizacija ne dovoli zunanje posredovanosti «**, preverite, ali je pravilnik konfiguriran tako, da omogoča zunanjo samodejno posredovanje.</span><span class="sxs-lookup"><span data-stu-id="0efb8-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="0efb8-107">**Opomba:** Priporočljivo je, da zunanje samodejno posredovanje onemogočite na privzeti pravilnik za filtriranje neželene pošte in ga omogočite le za uporabnike, ki potrebujejo zunanjo preusmeritev, tako da ustvarijo pravilnik po meri za te uporabnike.</span><span class="sxs-lookup"><span data-stu-id="0efb8-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="0efb8-108">Več informacij najdete v članku [Konfiguriranje posredovanja zunanjih e-poštnih sporočil v sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="0efb8-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>