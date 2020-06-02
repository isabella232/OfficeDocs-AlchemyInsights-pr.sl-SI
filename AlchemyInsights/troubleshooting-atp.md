---
title: Odpravljanje težav pri uradu 365 napredna zaščita pred grožnjami
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512606"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="7b228-102">Odpravljanje težav pri uradu 365 napredna zaščita pred grožnjami</span><span class="sxs-lookup"><span data-stu-id="7b228-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="7b228-103">Ali opazite zamude pri dostavi sporočila?</span><span class="sxs-lookup"><span data-stu-id="7b228-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="7b228-104">Uporabite [dinamično možnost dostave](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v pravilniku o VARNIH prilogah ATP.</span><span class="sxs-lookup"><span data-stu-id="7b228-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="7b228-105">To bo pripomoglo k preprečevanju zamud pri sporočilih, ko boste zaščitili prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="7b228-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="7b228-106">Ali želite Microsoftu sporočiti lažne pozitivne ali lažne negative?</span><span class="sxs-lookup"><span data-stu-id="7b228-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="7b228-107">Uporabite to [povezavo](https://www.microsoft.com/wdsi/filesubmission/) za pošiljanje datotek za analizo.</span><span class="sxs-lookup"><span data-stu-id="7b228-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="7b228-108">Ali ste vedeli, da lahko omogočite zaščito varnih povezav za interno e-poštno sporočilo, poslano med prejemniki v vaši organizaciji?</span><span class="sxs-lookup"><span data-stu-id="7b228-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="7b228-109">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="7b228-109">Follow these steps:</span></span>

  1. <span data-ttu-id="7b228-110">Pojdite [https://protection.office.com](https://protection.office.com) in se vpišite z globalnim skrbnikom ali računom varnostnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="7b228-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="7b228-111">V levem podoknu za krmarjenje pod **upravljanjem groženj**izberite **Policy** \> **varne povezave**pravilnika.</span><span class="sxs-lookup"><span data-stu-id="7b228-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="7b228-112">V **pravilnikih, ki veljajo za celotno organizacijo** , izberite pravilnik in kliknite **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="7b228-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="7b228-113">Pod možnostjo **Nastavitve**omogočite **uporabo varnih povezav za sporočila, poslana v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="7b228-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
