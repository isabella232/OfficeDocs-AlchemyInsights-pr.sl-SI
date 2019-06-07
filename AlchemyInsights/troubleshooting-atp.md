---
title: Odpravljanje težav z Office 365 napreden grožnja varstvo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765427"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="c0ff5-102">Odpravljanje težav z Office 365 napreden grožnja varstvo</span><span class="sxs-lookup"><span data-stu-id="c0ff5-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="c0ff5-103">Ali ste opazili zamude pri dostavi sporočilo?</span><span class="sxs-lookup"><span data-stu-id="c0ff5-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="c0ff5-104">Uporabite možnost [Dinamičnega prikazovanja](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) v ATP varno Priloge pravilnika.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="c0ff5-105">To bo pomagalo izogniti sporočilo zamude, hkrati pa ščiti prejemniki zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="c0ff5-106">Ali želite Microsoftu poročati napačen ali lažno negativen?</span><span class="sxs-lookup"><span data-stu-id="c0ff5-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="c0ff5-107">Uporabite to [povezavo](https://www.microsoft.com/wdsi/filesubmission/) za oddajo datoteke za analizo.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="c0ff5-108">Ali ste vedeli, da lahko omogočite zaščito varne povezave za interne elektronske pošte poslal med prejemnike znotraj vaše organizacije?</span><span class="sxs-lookup"><span data-stu-id="c0ff5-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="c0ff5-109">Sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="c0ff5-109">Follow these steps:</span></span>

  1. <span data-ttu-id="c0ff5-110">Pojdi na [https://protection.office.com](https://protection.office.com) in se prijavite z globalno skrbnik ali skrbniški račun varnosti.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="c0ff5-111">V levem navigacijskem pod **grožnjo upravljanje**, izberite **pravilnik** \> **Varne povezave**.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="c0ff5-112">V razdelku **pravila, ki veljajo za celotno organizacijo** , izbrati pravilnik in kliknite **Urejanje**.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="c0ff5-113">Pod **Nastavitve**omogočajo **uporabi varne povezave na sporočila, poslana v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="c0ff5-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
